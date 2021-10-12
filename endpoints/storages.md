---
description: This endpoint provides information about storages.
---

# Storages

{% swagger baseUrl="https://api.treefarmer.xyz" path="/storages" method="get" summary="Storage Information" %}
{% swagger-description %}
This endpoint will provide an array of storages by level with their cost, capacity and name.
{% endswagger-description %}

{% swagger-parameter in="header" name="Authorization" type="string" %}
Your Tree Farmer API token
{% endswagger-parameter %}

{% swagger-parameter in="query" name="search" type="string" %}
Find a specific storage by its name or level (e.g. American Arborvitae or 5)
{% endswagger-parameter %}

{% swagger-response status="200" description="An array of storages" %}
```javascript
{
  "error": false,
  "message": "The requested storage data successfully found.",
  "data": [
    {
      "capacity": 79,
      "cost": 159,
      "level": 1,
      "name": "Chest"
    },
    {
      "capacity": 197,
      "cost": 1192,
      "level": 2,
      "name": "Crate"
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
   "message": "The requested storage could not be found with the provided query. Please check the name or ID and try again."
}
```
{% endswagger-response %}
{% endswagger %}

