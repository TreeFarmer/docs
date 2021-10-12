---
description: This endpoint provides information about trees.
---

# Trees

{% swagger baseUrl="https://api.treefarmer.xyz" path="/trees" method="get" summary="Tree Information" %}
{% swagger-description %}
This endpoint will provide an array of trees by level with their name, planting region, fun fact, growth time, log count, log value, sapling cost and upgrade cost.
{% endswagger-description %}

{% swagger-parameter in="header" name="Authorization" type="string" %}
Your Tree Farmer API token
{% endswagger-parameter %}

{% swagger-parameter in="query" name="search" type="string" %}
Find a specific tree by its name or level (e.g. American Arborvitae or 5)
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
```javascript
{
  "error": false,
  "message": "The requested tree data successfully found.",
  "data": [
    {
      "name": "African Juniper",
      "funfact": "It is the only juniper to occur south of the equator.",
      "plantingRegion": "Africa",
      "level": 1,
      "growthTime": 60,
      "logCount": 119,
      "logValue": 6,
      "saplingCost": 69,
      "upgradeCost": 0
    },
    {
      "name": "American Arborvitae",
      "funfact": "The specific name, 'Occidentalis', means 'west,' the direction from Sweden where this tree was discovered.",
      "plantingRegion": "North America",
      "level": 2,
      "growthTime": 61,
      "logCount": 124,
      "logValue": 8,
      "saplingCost": 79,
      "upgradeCost": 11500
    }
    
    ...
    
  ]
}
```
{% endswagger-response %}

{% swagger-response status="404" description="The value of the query was invalid." %}
```javascript
{
  "error": true,
  "message": "The requested tree could not be found with the provided query. Please check the name or ID and try again."
}
```
{% endswagger-response %}
{% endswagger %}
