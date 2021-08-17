# Experiments



{% api-method method="get" host="https://api.plantgenie.org" path="/experiment/get\_all" %}
{% api-method-summary %}
Get experiments
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get all the experiments belongs to given database.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="experiment" type="string" required=true %}
experiments
{% endapi-method-parameter %}

{% api-method-parameter name="get\_all" type="string" required=true %}
get everything
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-query-parameters %}
{% api-method-parameter name="name" type="string" required=true %}
by given database name
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Get all the experiments by given database
{% endapi-method-response-example-description %}

```
[{"experiment_id":"2","experiment_name":"AspWood","experiment_value":"aspwood","experiment_table":"expression","visibility":"true","default selection":"0","tool_category":"expression","tools":"exheatmap,explot,eximage","method":"TPM"},{"experiment_id":"3","experiment_name":"P. tremula exatlas","experiment_value":"exatlas","experiment_table":"expression","visibility":"true","default selection":"0","tool_category":"expression","tools":"exheatmap,explot,eximage","method":"TPM"},{"experiment_id":"4","experiment_name":"Robinson et al 2014 (Sex)","experiment_value":"sex","experiment_table":"expression","visibility":"true","default selection":"0","tool_category":"expression","tools":"exheatmap,explot,eximage","method":"TPM"},{"experiment_id":"5","experiment_name":"P. trichocarpa Tissues","experiment_value":"log","experiment_table":"expression","visibility":"false","default selection":"0","tool_category":"expression","tools":"exheatmap,explot,eximage","method":"TPM"},{"experiment_id":"10","experiment_name":"SwAsp population (buds)","experiment_value":"swasp","experiment_table":"expression","visibility":"true","default selection":"0","tool_category":"expression","tools":"exheatmap,explot","method":"TPM"},{"experiment_id":"11","experiment_name":"AspLeaf","experiment_value":"leaf_development","experiment_table":"expression","visibility":"true","default selection":"0","tool_category":"expression","tools":"exheatmap,explot,eximage","method":"TPM"},{"experiment_id":"12","experiment_name":"Xylem and Leaf","experiment_value":"xylem_leaf","experiment_table":"expression","visibility":"true","default selection":"0","tool_category":"expression","tools":"exheatmap,explot,eximage","method":"TPM"},{"experiment_id":"13","experiment_name":"Senescence 1","experiment_value":"senescence1","experiment_table":"expression","visibility":"true","default selection":"0","tool_category":"expression","tools":"exheatmap,explot,eximage","method":"TPM"},{"experiment_id":"14","experiment_name":"Senescence 2","experiment_value":"senescence2","experiment_table":"expression","visibility":"true","default selection":"0","tool_category":"expression","tools":"exheatmap,explot","method":"TPM"}]
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



