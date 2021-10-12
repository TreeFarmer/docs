---
description: This endpoint provides information about vehicles.
---

# Vehicles

{% swagger baseUrl="https://api.treefarmer.xyz" path="/vehicles" method="get" summary="Vehicle Information" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="header" name="Authorization" type="string" %}
Your Tree Farmer API token
{% endswagger-parameter %}

{% swagger-parameter in="query" name="search" type="string" %}
Find a specific vehicle by its name or level (e.g. wagon or 5)
{% endswagger-parameter %}

{% swagger-response status="200" description="An array of vehicles" %}
```javascript
{
  "error": false,
  "message": "The requested vehicle data successfully found.",
  "data": [
    {
      "capacity": 16,
      "cooldown": 60,
      "cost": 389,
      "level": 1,
      "name": "Wagon"
    },
    {
      "capacity": 56,
      "cooldown": 69,
      "cost": 1750,
      "level": 2,
      "name": "Cargo Bike"
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
  "message": "The requested vehicle could not be found with the provided query. Please check the name or ID and try again."
}
```
{% endswagger-response %}
{% endswagger %}
