---
description: >-
  Tree Farmer offers an easy to use RESTful API that can gather data of the game
  and of a user. Start by getting an API token from the community server.
---

# Welcome

## Authentication

To use any endpoint of the API, you must generate an API token. To generate a token you must:

* Own a tree farm (create one with `/start`)
* Be in our Discord server (join at [**treefarmer.xyz/discord**](https://treefarmer.xyz/discord))

Then, you can run `/api` to generate your token. Please make sure to store it somewhere safe because it will not be accessible again from the bot. The token must be used in the authorization header of every request. API wrappers will be available soon. Here are some examples of authentication.

## JavaScript / TypeScript

```javascript
import req from 'petitio';

const init = req('https://api.treefarmer.xyz/cutters', 'GET').header('Authorization', 'your API token');
const res = await init.send();

console.log(res)
```

