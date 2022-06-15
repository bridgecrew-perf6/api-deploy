---
title: 'Historical Currency'
date: 2019-02-11T19:27:37+10:00
weight: 4
---

Provides currency exchange rate on the specific day.

#### Endpoint:
```
GET: /currency/historical/{YYYY-MM-DD}?from={from}&amp;to={to}&amp;amount={amount}&amp;format={format} 
```
#### Parameters:
* YYYY-MM-DD: required date in the format YYYY-MM-DD
* from: the code of the base currency.The default base currency is EUR.
* to: the code of the currency to convert to. If the value is not provided then the list of all supported currencies will be returned. You can provide several currencies using comma (to=GBP,EUR,AUD)
* amount: amount that needs to be converted
* Format: JSON or XML

#### Example Response:

```json
{
    "status":"success",
    "updated_date":"2018-10-12",
    "base_currency_code":"EUR",
    "amount":10,"
    "base_currency_name":"Euro",
    rates":{
        "GBP":{
            "currency_name":"Pound Sterling",
            "rate":"0.8764",
            "rate_for_amount":"8.7640"
        }
    }
}
```