# API for PlantGenIE

Here we will discuss main API end points that we used in PlantGenIE. There are some important input parameters that we need to feed into the API.

#### User ID:

This is an important parameter to uniquely identify users and their previous actions. For example: GeneList and ExperimentList. Current version of API uses random ID as user ID and it will be stored as cookie in the web browser . 

{% hint style="warning" %}
Cookie baed User ID is domain dependent which means we can not expect the same user id when we change domain names.
{% endhint %}

#### Database Name:

We have to pass the database name 

{% embed url="https://api.plantgenie.org" %}





