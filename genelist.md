# GeneList
***********
{% api-method method="get" host="https://api.plantgenie.org/genelist" path="/get_all" %}
{% api-method-summary %}
Get all genelists 
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get all PlantGenIE databases.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}

{% api-method-parameter name="name" type="string" required=true %}
database name to represent databases
{% endapi-method-parameter %}

{% api-method-parameter name="table" type="string" required=true %}
database name to represent databases
{% endapi-method-parameter %}


{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Display information from all databases
{% endapi-method-response-example-description %}

```
[{"db":"beta_plantgenie_amtri_v10","species":"Amborella trichopoda","abbreviation":"amtri","version":"v1.0","pubmed_id":"24357323","tax_id":"13333","source":"Phytozome","url":"https:\/\/phytozome.jgi.doe.gov\/pz\/portal.html#!info?alias=Org_Atrichopoda"},{"db":"beta_plantgenie_aqcoe_v31","species":"Aquilegia coerulea","abbreviation":"aqcoe","version":"v3.1","pubmed_id":"30325307","tax_id":"218851","source":"Phytozome","url":"https:\/\/phytozome.jgi.doe.gov\/pz\/portal.html#!info?alias=Org_Acoerulea"},{"db":"beta_plantgenie_artha_v11","species":"Arabidopsis thaliana","abbreviation":"artha","version":"v11","pubmed_id":"11130711","tax_id":"3702","source":"Araport11","url":"https:\/\/www.araport.org\/"},{"db":"beta_plantgenie_arann_v10","species":"Artemisia annua","abbreviation":"arann","version":"v1","pubmed_id":"29703587","tax_id":"35608","source":"NCBI","url":"ftp:\/\/ftp.ncbi.nlm.nih.gov\/genomes\/all\/GCA\/003\/112\/345\/GCA_003112345.1_ASM311234v1"},{"db":"beta_plantgenie_bevul_v12","species":"Beta vulgaris","abbreviation":"bevul","version":"v1.2","pubmed_id":"24352233","tax_id":"161934","source":"ensemblgenome","url":"ftp:\/\/ftp.ensemblgenomes.org\/pub\/release-44\/plants\/"},{"db":"beta_plantgenie_bepen_v14","species":"Betula pendula","abbreviation":"bepen","version":"1.4c","pubmed_id":"31197270","tax_id":"3505","source":"CoGe","url":"https:\/\/genomevolution.org\/CoGe\/GenomeInfo.pl?gid=35080"},{"db":"beta_plantgenie_casin_v20","species":"Camellia sinensis","abbreviation":"casin","version":"AHAU_CSS_2","pubmed_id":"29678829","tax_id":"4442","source":"NCBI","url":"ftp:\/\/ftp.ncbi.nlm.nih.gov\/genomes\/all\/GCA\/004\/153\/795\/GCA_004153795.2_AHAU_CSS_2"},{"db":"beta_plantgenie_cikan_v10","species":"Cinnamomum kanehirae","abbreviation":"cikan","version":"v1.0","pubmed_id":"30626928","tax_id":"337451","source":"NCBI","url":"ftp:\/\/ftp.ncbi.nlm.nih.gov\/genomes\/all\/GCA\/003\/546\/025\/GCA_003546025.1_ASBRC_Ckan_1.0"},{"db":"beta_plantgenie_cusat_v10","species":"Cucumis sativus L.","abbreviation":"cusat","version":"v1.0","pubmed_id":"0","tax_id":"3659","source":"Phytozome","url":"https:\/\/phytozome.jgi.doe.gov\/pz\/portal.html#!info?alias=Org_Csativus"},{"db":"beta_plantgenie_eugra_v20","species":"Eucalyptus grandis","abbreviation":"eugra","version":"v2.0","pubmed_id":"24919147","tax_id":"71139","source":"Phytozome","url":"https:\/\/phytozome.jgi.doe.gov\/pz\/portal.html#!info?alias=Org_Egrandis"},{"db":"beta_plantgenie_gibil_2016","species":"Ginkgo biloba","abbreviation":"gibil","version":"2016","pubmed_id":"27871309","tax_id":"3311","source":"GigaScience","url":"ftp:\/\/parrot.genomics.cn\/gigadb\/pub\/10.5524\/100001_101000\/100209\/"},{"db":"beta_plantgenie_gnmon","species":"Gnetum montanum","abbreviation":"gnmon","version":"NA","pubmed_id":"29379155","tax_id":"3381","source":"DRAYD","url":"https:\/\/datadryad.org\/stash\/landing\/show?big=showme&id=doi%3A10.5061%2Fdryad.0vm37"},{"db":"beta_plantgenie_haimp","species":"Handroanthus impetiginosus","abbreviation":"haimp","version":"NA","pubmed_id":"29253216","tax_id":"429701","source":"GigaScience","url":"ftp:\/\/parrot.genomics.cn\/gigadb\/pub\/10.5524\/100001_101000\/100379\/"},{"db":"beta_plantgenie_maole","species":"Malania oleifera","abbreviation":"maole","version":"NA","pubmed_id":"30689848","tax_id":"397392","source":"GigaScience","url":"ftp:\/\/parrot.genomics.cn\/gigadb\/pub\/10.5524\/100001_101000\/100549\/"},{"db":"beta_plantgenie_madom_v20","species":"Malus domestica","abbreviation":"madom","version":"v2.0","pubmed_id":"27503335","tax_id":"3750","source":"GigaScience","url":"https:\/\/phytozome.jgi.doe.gov\/pz\/portal.html#!info?alias=Org_Mdomestica"},{"db":"beta_plantgenie_metru_v10","species":"Medicago truncatula","abbreviation":"metru","version":"mt4.0v1","pubmed_id":"24767513","tax_id":"3880","source":"Phytozome","url":"https:\/\/phytozome.jgi.doe.gov\/pz\/portal.html#!info?alias=Org_Mtruncatula"},{"db":"beta_plantgenie_migut_v20","species":"Mimulus guttatus","abbreviation":"migut","version":"v2.0","pubmed_id":"24225854","tax_id":"4155","source":"Phytozome","url":"https:\/\/phytozome.jgi.doe.gov\/pz\/portal.html#!info?alias=Org_Mguttatus"},{"db":"beta_plantgenie_nitab_v45","species":"Nicotiana tabacum","abbreviation":"nitab","version":"v4.5 (Edwards 2017)","pubmed_id":"28625162","tax_id":"4097","source":"Sol Genomics Network","url":"ftp:\/\/ftp.solgenomics.net\/genomes\/Nicotiana_tabacum\/edwards_et_al_2017"},{"db":"parasponia","species":"parasponia andersonii","abbreviation":"paand","version":null,"pubmed_id":null,"tax_id":null,"source":null,"url":null},{"db":"beta_plantgenie_phpat_v33","species":"Physcomitrella patens","abbreviation":"phpat","version":"v3.3","pubmed_id":"18079367","tax_id":"3218","source":"Phytozome","url":"https:\/\/phytozome.jgi.doe.gov\/pz\/portal.html#!info?alias=Org_Ppatens"},{"db":"beta_plantgenie_piabi_v10","species":"Picea abies","abbreviation":"piabi","version":"congenie_v1","pubmed_id":"23698360","tax_id":"3329","source":"PlantGenIE","url":"https:\/\/plantgenie.org\/"},{"db":"beta_plantgenie_pilam_v10","species":"Pinus lambertiana","abbreviation":"pilam","version":"v1.0","pubmed_id":"27794028","tax_id":"3343","source":"TreegenesDB","url":"https:\/\/treegenesdb.org\/FTP\/Genomes\/Pila\/v1.0\/"},{"db":"beta_plantgenie_pitae_v20","species":"Pinus taeda","abbreviation":"pitae","version":"v2.01","pubmed_id":"24647006","tax_id":"3352","source":"TreegenesDB","url":"https:\/\/treegenesdb.org\/FTP\/Genomes\/Pita\/v2.01\/"},{"db":"beta_plantgenie_poeup_v20","species":"Populus euphratica","abbreviation":"poeup","version":"v2.0","pubmed_id":"32034885","tax_id":"75702","source":"NCBI","url":"https:\/\/bigd.big.ac.cn\/gwh\/Assembly\/649\/show"},{"db":"beta_plantgenie_potra_v22","species":"Populus tremula","abbreviation":"potra","version":"v2.2","pubmed_id":"0","tax_id":"113636","source":"PlantGenIE","url":"https:\/\/plantgenie.org\/"},{"db":"explorer_aspleaf_potra_v11","species":"Populus tremula","abbreviation":"potrav1","version":"v1.0","pubmed_id":"0","tax_id":"113636","source":"PlantGenIE","url":"https:\/\/plantgenie.org\/"},{"db":"beta_plantgenie_potrx_v10","species":"Populus tremula x Populus tremuloides","abbreviation":"potrx","version":"v1.0","pubmed_id":"22871142","tax_id":"47664","source":"PlantGenIE","url":"https:\/\/plantgenie.org\/"},{"db":"beta_plantgenie_potrs_v11","species":"Populus tremuloides","abbreviation":"potrs","version":"v1.1","pubmed_id":"30373829","tax_id":"3693","source":"PlantGenIE","url":"https:\/\/plantgenie.org\/"},{"db":"beta_plantgenie_potri_v31","species":"Populus trichocarpa","abbreviation":"potri","version":"v3.1","pubmed_id":"16973872","tax_id":"3694","source":"Phytozome","url":"https:\/\/phytozome.jgi.doe.gov\/pz\/portal.html#!info?alias=Org_Ptrichocarpa_er"},{"db":"beta_plantgenie_psmen_v10","species":"Pseudotsuga menziesii","abbreviation":"psmen","version":"v1.0","pubmed_id":"28751502","tax_id":"3357","source":"TreegenesDB","url":"https:\/\/treegenesdb.org\/FTP\/Genomes\/Psme\/v1.0\/"},{"db":"beta_plantgenie_sapur_v10","species":"Salix purpurea","abbreviation":"sapur","version":"v1.0","pubmed_id":"0","tax_id":"77065","source":"Phytozome","url":"https:\/\/phytozome.jgi.doe.gov\/pz\/portal.html#!info?alias=Org_Spurpurea"},{"db":"salix","species":"salix viminalis","abbreviation":"savim","version":null,"pubmed_id":null,"tax_id":null,"source":null,"url":null},{"db":"beta_plantgenie_vivin_genoscope12x","species":"Vitis vinifera","abbreviation":"vivin","version":"genoscope12x","pubmed_id":"17721507","tax_id":"29760","source":"Phytozome","url":"https:\/\/phytozome.jgi.doe.gov\/pz\/portal.html#!info?alias=Org_Vvinifera"},{"db":"beta_plantgenie_yellowhorn_xasor_v2f","species":"Xanthoceras sorbifolium","abbreviation":"xasor","version":"v2f","pubmed_id":"0","tax_id":"99658","source":"BFU","url":"https:\/\/plantgenie.org\/"},{"db":"beta_plantgenie_zomar_v22","species":"Zostera marina","abbreviation":"zomar","version":"v2.2","pubmed_id":"26814964","tax_id":"29655","source":"Phytozome","url":"https:\/\/phytozome.jgi.doe.gov\/pz\/portal.html#!info?alias=Org_Zmarina"}]
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=302 %}
{% api-method-response-example-description %}
Empty array
{% endapi-method-response-example-description %}

```
[]
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}
***********

{% api-method method="get" host="https://api.plantgenie.org" path="/db" %}
{% api-method-summary %}
Get all databases
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get all PlantGenIE databases .
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="db" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% embed url="https://codepen.io/irusri/pen/GRNYpPR" %}



