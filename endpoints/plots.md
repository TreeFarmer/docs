---
description: This endpoint provides information about plots.
---

# Plots

{% swagger baseUrl="https://api.treefarmer.xyz" path="/plots" method="get" summary="Plot Information" %}
{% swagger-description %}
This endpoint will provide an array of plots by level with their cost and growth speed.
{% endswagger-description %}

{% swagger-parameter in="header" name="Authorization" type="string" %}
Your Tree Farmer API token
{% endswagger-parameter %}

{% swagger-parameter in="query" name="search" type="string" %}
Find a specific plot by its level (e.g. 5)
{% endswagger-parameter %}

{% swagger-response status="200" description="An array of plots" %}
```javascript
{
  "error": false,
  "message": "The requested plot data successfully found.",
  "data": [
    {
      "cost": 479,
      "level": 1,
      "growthSpeed": 100
    },
    {
      "cost": 1197,
      "level": 2,
      "growthSpeed": 102
    }
        
    ...
      
  ]
}
```
{% endswagger-response %}

{% swagger-response status="404" description="The value of the query was invalid" %}
```javascript
{
  "error": true,
  "message": "The requested plot could not be found with the provided query. Please check the name or ID and try again."
}
```
{% endswagger-response %}
{% endswagger %}

