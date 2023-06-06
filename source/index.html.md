---
title: API Reference

language_tabs: # must be one of https://github.com/rouge-ruby/rouge/wiki/List-of-supported-languages-and-lexers
  - javascript

toc_footers:
  - <a href='#'>Sign Up **for** a Developer Key</a>
  - <a href='https://github.com/slatedocs/slate'>Documentation Powered by Slate</a>

includes:
  # - errors

search: true

code_clipboard: true

meta:
  - name: description
    content: Documentation for the Music Social App API
---

# Introduction

Welcome to the Music Social API! You can use our API to access Music Social API endpoints, which can get information on various posts, user profiles, and music files in our database.

You can view code examples in the dark area to the right.

<!-- # Authentication -->

# Music Social App API

## Get All Posts

This endpoint retrieves all posts

```javascript
import axios from "axios";

const response = await axios.get("http://localhost:5000/api/posts", {
  params: {
    page: 1,
  },
});

console.log(response.data);
```

> The above command returns JSON structured like this:

```json
{
  "message": "Success",
  "posts": [
    {
      "id": 1,
      "mediaUrl": "https://images.unsplash.com/photo-1520496938502-73e942d08cc3?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w0NTc0NzZ8MHwxfHJhbmRvbXx8fHx8fHx8fDE2ODU5NzQ3NDB8&ixlib=rb-4.0.3&q=80&w=1080",
      "createdAt": "2023-06-05T14:19:10.000Z",
      "updatedAt": "2023-06-05T14:19:10.000Z",
      "userId": 10
    },
    {
      "id": 2,
      "mediaUrl": "https://images.unsplash.com/photo-1621542866289-21a3d62c91d3?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w0NTc0NzZ8MHwxfHJhbmRvbXx8fHx8fHx8fDE2ODU5NzQ3NDB8&ixlib=rb-4.0.3&q=80&w=1080",
      "createdAt": "2023-06-05T14:19:10.000Z",
      "updatedAt": "2023-06-05T14:19:10.000Z",
      "userId": 22
    },
    {
      "id": 3,
      "mediaUrl": "https://images.unsplash.com/photo-1655875356554-3da38f0bb3e3?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w0NTc0NzZ8MHwxfHJhbmRvbXx8fHx8fHx8fDE2ODU5NzQ3NDB8&ixlib=rb-4.0.3&q=80&w=1080",
      "createdAt": "2023-06-05T14:19:10.000Z",
      "updatedAt": "2023-06-05T14:19:10.000Z",
      "userId": 71
    }
  ]
}
```

### HTTP Request

<code>GET http://localhost:5000/api/posts?<var>parameters</var></code>

### URL Parameters

| Parameter | Description                                                                                          |
| --------- | ---------------------------------------------------------------------------------------------------- |
| page      | Page with posts. By default, there are 20 posts per page. The page parameter is set to 1 by default. |

<!--
## Get a Specific Post

```javascript
const kittn = require("kittn");

let api = kittn.authorize("meowmeowmeow");
let max = api.kittens.get(2);
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "name": "Max",
  "breed": "unknown",
  "fluffiness": 5,
  "cuteness": 10
}
```

This endpoint retrieves a specific post by id.

### HTTP Request

`GET http://localhost:5000/api/posts/<ID>`

### URL Parameters

| Parameter | Description                    |
| --------- | ------------------------------ |
| ID        | The ID of the post to retrieve |

## Delete a Specific Post

```javascript
const kittn = require("kittn");

let api = kittn.authorize("meowmeowmeow");
let max = api.kittens.delete(2);
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "deleted": ":("
}
```

This endpoint deletes a specific post.

### HTTP Request

`DELETE http://localhost:5000/api/posts/<ID>`

### URL Parameters

| Parameter | Description                  |
| --------- | ---------------------------- |
| ID        | The ID of the post to delete | -->
