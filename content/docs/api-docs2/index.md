---
title: 'Currency Conversion'
date: 2019-02-11T19:27:37+10:00
weight: 3
---

Currency Conversion Lookup converts once currency to another.

#### Endpoint:
```
GET: /currency/convert?&amp;from={from}&amp;to={to}&amp;amount={amount}&amp;format={format}
```
#### Parameters:
* from: the code of the base currency.The default base currency is EUR.
* to: the code of the currency to convert to. If the value is not provided then the list of all supported currencies will be returned. You can provide several currencies using comma (to=GBP,EUR,AUD)
* amount: amount that needs to be converted
* Format: JSON or XML

#### Example Response:

```json
{
    "status":"success",
    "updated_date":"2018-12-27",
    "base_currency_code":"EUR",
    "amount":10,"
    "base_currency_name":"Euro",
    rates":{
        "GBP":{
            "currency_name":"Pound Sterling",
            "rate":"0.9007",
            "rate_for_amount":"9.0070"
        }
    }
}
```