---
title: 'Currencies List'
date: 2019-02-11T19:27:37+10:00
weight: 2
---

This returns the list of available currencies

#### Endpoint:
```
GET: /currency/list?format={format}
```
#### Parameters:
* Format: JSON or XML

####     Example Response:

```json
{
    "status":"success",
    "currencies":[
        "AUD":"Australian Dollar",
        "BGN":"Bulgarian Lev",
        [ ... ]
    ]
}
```