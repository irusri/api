# Network

{% api-method method="get" host="https://api.plantgenie.org" path="/network/get\_all" %}
{% api-method-summary %}
Get experiments
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get all the available networks for the given database.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="network" type="string" required=true %}
networks
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
JSON object of available networks
{% endapi-method-response-example-description %}

```
[{"experiment_id":"6","experiment_name":"AspLeaf - Terminal","experiment_value":"aspleaf","experiment_table":"network","visibility":"true","default selection":"1","tool_category":"network","tools":"exnet","method":"Seidr"},{"experiment_id":"7","experiment_name":"AspWood","experiment_value":"aspwood","experiment_table":"network","visibility":"true","default selection":"0","tool_category":"network","tools":"exnet","method":"Seidr"},{"experiment_id":"8","experiment_name":"exAtlas","experiment_value":"exatlas","experiment_table":"network","visibility":"true","default selection":"0","tool_category":"network","tools":"exnet","method":"Seidr"},{"experiment_id":"9","experiment_name":"AspMetaNet","experiment_value":"full","experiment_table":"network","visibility":"true","default selection":"0","tool_category":"network","tools":"exnet","method":"Seidr"},{"experiment_id":"15","experiment_name":"SwAsp population (buds)","experiment_value":"Bud","experiment_table":"network","visibility":"true","default selection":"0","tool_category":"network","tools":"exnet","method":"Seidr"}]
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=302 %}
{% api-method-response-example-description %}
An empty array
{% endapi-method-response-example-description %}

```
[]
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

