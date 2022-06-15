---
title: 'Errors'
date: 2019-02-11T19:27:37+10:00
weight: 6
---

If the request fails or the resource is unavailable, an error message in JSON or XML format will be returned.

#### Error Response:

```json
{
    "status":"failed",
    "error":{
        "message":"Invalid key.",
        "code":"403"
    }
}

```

#### Parameters:
* 400 : Bad request.
* 403 : Authentication failed
* 404 : Resource is not found or requested format is incorrect
* 405 : Method is not allowed.
* 500 : Server error. We hope you never see this error.