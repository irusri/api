# GeneList

```text
HTML CSS JSResult Skip Results Iframe
EDIT ON
// Debug parameters
GenIE_userID =document.getElementById("user_id").innerText;
GenIE_selectedspeciesAbbreviation= document.getElementById("abbreviation").innerText;
GenIE_genelistDatabase="plantgenie_genelist";

// Initialize GenIE object
GenIE =({
  allGenelists: {},
  activeGenelist: {},
  allExperiments: {},
  activeExperiment: {},
  allDatabases: {},
  userID: GenIE_userID,
  selectedspeciesAbbreviation: GenIE_selectedspeciesAbbreviation,
  genelistDatabase: GenIE_genelistDatabase,
  databaseURL : "https://api.plantgenie.org/db",
  genelistURL : "https://api.plantgenie.org/genelist/get_active_list",
  experimentURL : "https://api.plantgenie.org/experiment",
  expressionURL : "https://api.plantgenie.org/experiment/expression",
  networkURL : "https://api.plantgenie.org/network"
});

// Common promise request
const plantgenieRequest = (url) => {  
     return new Promise((resolve, reject) => {
        const xhr = new XMLHttpRequest();
        xhr.open('GET', url, true);
        xhr.send();
        xhr.onreadystatechange = () => {
            if (xhr.readyState !== 4) {
                return;
            }
            if (xhr.status === 200) {
                resolve(JSON.parse(xhr.responseText));
            } else {
                const error = xhr.statusText || 'Something went wrong!';
                reject(error);
            }
        };
    });
}

//onload function
onLoad= async () => {
  let database_name = await plantgenieRequest(GenIE.databaseURL + "/" + GenIE.selectedspeciesAbbreviation);
  if (database_name) {
    GenIE.selectedspeciesDatabase = database_name[0].db;
  }
  let genelist = null;
    genelist = await plantgenieRequest(GenIE.genelistURL + "?name=" + GenIE.genelistDatabase + "&fingerprint=" + GenIE.userID + "&table=" + GenIE.selectedspeciesDatabase)
  if (genelist) {
    GenIE.activeGenelist = genelist;
  }
  let experiments = null;
  experiments = await plantgenieRequest(GenIE.experimentURL + "/get_all?name=" + GenIE.selectedspeciesDatabase);
  if(experiments){
    GenIE.allExperiments = experiments;
  }
  console.log(GenIE)
};
onLoad();

```

