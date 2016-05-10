# General API

API development URL : [api-sandbox.tiket.com](http://api-sandbox.tiket.com) 
API production URL : [api.tiket.com](https://api.tiket.com)

NOTE :

* Data that is provided for testing is different from the actual

These are the API command for general configurations

## Get Token

```http
GET /apiv1/payexpress HTTP/1.1
Host: api-sandbox.tiket.com
User-Agent: twh:123456789;Partner Name;
```

```xml
<tiket>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.0586</elapsetime>
    <memoryusage>4.49MB</memoryusage>
    <unix_timestamp>1399524305</unix_timestamp>
    <confirm>success</confirm>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <output_type>xml</output_type>
  <login_status>false</login_status>
  <token>712402a7c363b12d87f6b02749f6f0c91b64c47e</token>
</tiket>
```

```json
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.0555",
    "memoryusage": "4.48MB",
    "unix_timestamp": 1399524662,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "login_status": "false",
  "token": "712402a7c363b12d87f6b02749f6f0c91b64c47e"
}
```

```matlab
a: 4: {
  s: 10: "diagnostic";a: 7: {
    s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.1005";s: 11: "memoryusage";s: 14: "4.48MB";s: 14: "unix_timestamp";i: 1399524810;s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "id";s: 8: "currency";s: 3: "IDR";
  }
  s: 11: "output_type";s: 9: "serialize";s: 12: "login_status";s: 5: "false";s: 5: "token";s: 40: "712402a7c363b12d87f6b02749f6f0c91b64c47e";
}
```

Use to access the API, active until checkout payment.

Important Info:

* Secret key only used for this link when you get token. For the other link you only need to use token.

### HTTP Request

`GET https://api-sandbox.tiket.com/apiv1/payexpress?method=getToken&secretkey=56c8624d6a62e1ab22f0d9915ff2d43c`

### Parameters

Name | Description | Format    | Default   | Mandatory
--------- | ------- | ----------- | ----------- | -----------
method | Request Method | CONST | getToken | TRUE
secretkey | API secret key given by Tiket.com | CHAR(128) |  | TRUE


