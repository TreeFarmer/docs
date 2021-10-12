---
description: This endpoint provides information about cutters.
---

# Cutters

{% swagger baseUrl="https://api.treefarmer.xyz" path="/cutters" method="get" summary="Cutter Information" %}
{% swagger-description %}
This endpoint will provide an array of cutters by level with their cooldown, cost, efficiency and name.
{% endswagger-description %}

{% swagger-parameter in="header" name="Authorization" type="string" %}
Your Tree Farmer API token
{% endswagger-parameter %}

{% swagger-parameter in="query" name="search" type="string" %}
Find a specific cutter by its name or level (e.g. breadknife or 3)
{% endswagger-parameter %}

{% swagger-response status="200" description="An array of cutters " %}
```javascript
{
  "error": false,
  "message": "The requested cutter data was successfully found.",
  "data": [
    {
      "cooldown": 60,
      "cost": 249,
      "efficiency": [10, 20],
      "level": 1,
      "name": "Fist"
    }, 
    {
      "cooldown": 69,
      "cost": 1120,
      "efficiency": [20, 30],
      "level": 2,
      "name": "Bread Knife"
    },
  
    ...
      
  ]
}
```
{% endswagger-response %}

{% swagger-response status="404" description="The search query was invalid." %}
```javascript
{
  "error": true,
  "message": "The requested cutter could not be found with the provided query. Please check the name or ID and try again."
}
```
{% endswagger-response %}
{% endswagger %}
