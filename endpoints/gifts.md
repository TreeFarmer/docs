---
description: This endpoint provides information about gifts.
---

# Gifts

{% swagger baseUrl="https://api.treefarmer.xyz" path="/gifts" method="get" summary="Gift Information" %}
{% swagger-description %}
This endpoint will provide an array of gifts by level with all their rewards.
{% endswagger-description %}

{% swagger-parameter in="header" name="Authorization" type="string" %}

{% endswagger-parameter %}

{% swagger-parameter in="query" name="search" type="string" %}
Find a specific gift by its name or level (e.g. small or 1)
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
```javascript
{
  "error": false,
  "message": "The requested gift data was successfully found.",
  "data": [
    {
      "level": 1,
      "name": "small",
      "money": [100, 200],
      "logs": [7, 16],
      "saplings": [1, 2],
      "cutters": [0, 1],
      "plots": [0, 1],
      "vehicles": [0, 1]
    }, 
    {
      "level": 1,
      "name": "medium",
      "money": [300, 600],
      "logs": [15, 24],
      "saplings": [2, 4],
      "cutters": [1, 2],
      "plots": [1, 2],
      "vehicles": [1, 2]
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
