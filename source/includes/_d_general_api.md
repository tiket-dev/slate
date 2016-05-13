# General API

API development URL : [api-sandbox.tiket.com](http://api-sandbox.tiket.com) 
API production URL : [api.tiket.com](https://api.tiket.com)

NOTE :

* Data that is provided for testing is different from the actual

These are the API command for general configurations

## Get Token

```http
GET /apiv1/payexpress?method=getToken&secretkey=56c8624d6a62e1ab22f0d9915ff2d43c&output=[json|xml|serialize|array] HTTP/1.1
Host: api-sandbox.tiket.com
User-Agent: twh:123456789;Partner Name;
Content-Type: text/plain
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

## Change Output Format

To change output, you can add parameter output in URL format.
Type of parameter output :

* **array**
* xml
* json
* serialize

### HTTP Request

`https://api-sandbox.tiket.com/order?token=c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f&output=xml`

### Parameter

 Name | Description | Format    | Default   | Mandatory
 --------- | ------- | ----------- | ----------- | -----------
 output | Output format | CONST | array | FALSE


 ## List Currency

```http
GET /general_api/listCurrency?token=c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f HTTP/1.1
Host: api-sandbox.tiket.com
User-Agent: twh:123456789;Partner Name;
Content-Type: text/plain
```

```xml
<tiket>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.0591</elapsetime>
    <memoryusage>4.49MB</memoryusage>
    <unix_timestamp>1399537382</unix_timestamp>
    <confirm>success</confirm>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <output_type>xml</output_type>
  <result>
    <code>EUR</code>
    <name>Euro (EUR)</name>
  </result>
  <result>
    <code>IDR</code>
    <name>Rupiah Indonesia (IDR)</name>
  </result>
  <result>
    <code>SGD</code>
    <name>Dolar Singapura (SGD)</name>
  </result>
  <result>
    <code>USD</code>
    <name>Dolar Amerika (USD)</name>
  </result>
  <login_status>false</login_status>
  <token>c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f</token>
</tiket>
```

```json
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.0564",
    "memoryusage": "4.48MB",
    "unix_timestamp": 1399537660,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "result": [{
    "code": "EUR",
    "name": "Euro (EUR)"
  }, {
    "code": "IDR",
    "name": "Rupiah Indonesia (IDR)"
  }, {
    "code": "SGD",
    "name": "Dolar Singapura (SGD)"
  }, {
    "code": "USD",
    "name": "Dolar Amerika (USD)"
  }],
  "login_status": "false",
  "token": "c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f"
}
```

```matlab
a: 5: {
  s: 10: "diagnostic";a: 7: {
    s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.0633";s: 11: "memoryusage";s: 14: "4.49MB";s: 14: "unix_timestamp";i: 1399538021;s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "id";s: 8: "currency";s: 3: "IDR";
  }
  s: 11: "output_type";s: 9: "serialize";s: 6: "result";a: 4: {
    i: 0;a: 2: {
      s: 4: "code";s: 3: "EUR";s: 4: "name";s: 22: "Euro (EUR)";
    }
    i: 1;a: 2: {
      s: 4: "code";s: 3: "IDR";s: 4: "name";s: 22: "Rupiah Indonesia (IDR)";
    }
    i: 2;a: 2: {
      s: 4: "code";s: 3: "SGD";s: 4: "name";s: 22: "Dolar Singapura (SGD)";
    }
    i: 3;a: 2: {
      s: 4: "code";s: 3: "USD";s: 4: "name";s: 22: "Dolar Amerika (USD)";
    }
  }
  s: 12: "login_status";s: 5: "false";s: 5: "token";s: 40: "c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f";
}
```

List of all the currency available at Tiket.com

### HTTP Request

 `http://api-sandbox.tiket.com/general_api/listCurrency?token=c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f`

### Parameter

Name | Description | Format    | Default   | Mandatory
--------- | ------- | ----------- | ----------- | -----------
output | Output format | CONST | array | FALSE

