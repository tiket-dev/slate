# General API

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

Use this to access the API, the token will be active  until checkout payment. Once you finish checkout, this token will expire. If you want to keep logged in user from getting logout, kindly use Renew Token.


<aside class="notice">Secretkey is only used to generate token. For every other activity, you are only required to use token.</aside>

### HTTP Request

`GET https://api-sandbox.tiket.com/apiv1/payexpress?method=getToken&secretkey=56c8624d6a62e1ab22f0d9915ff2d43c`

### Parameters

Name | Description | Format    | Default   | Mandatory
--------- | ------- | ----------- | ----------- | -----------
method | Request Method | CONST | getToken | TRUE
secretkey | API secret key given by Tiket.com | CHAR(128) |  | TRUE

## Renew Token

```http
GET /apiv1/payexpress?method=getToken&secretkey=56c8624d6a62e1ab22f0d9915ff2d43c&token=712402a7c363b12d87f6b02749f6f0c91b64c47e HTTP/1.1
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
  <token>c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f</token>
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
  "token": "c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f"
}
```

```matlab
: 4: {
  s: 10: "diagnostic";a: 7: {
    s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.1005";s: 11: "memoryusage";s: 14: "4.48MB";s: 14: "unix_timestamp";i: 1399524810;s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "id";s: 8: "currency";s: 3: "IDR";
  }
  s: 11: "output_type";s: 9: "serialize";s: 12: "login_status";s: 5: "false";s: 5: "token";s: 40: "712402a7c363b12d87f6b02749f6f0c91b64c47e";
}
```
Similar to getToken, but once the token expire, you have to call getToken again. If you want to keep logged in users from logged out, use this function instead.


### HTTP Request

`GET https://api-sandbox.tiket.com/apiv1/payexpress?method=getToken&secretkey=56c8624d6a62e1ab22f0d9915ff2d43c&token=712402a7c363b12d87f6b02749f6f0c91b64c47e`

### Parameters

Name | Description | Format    | Default   | Mandatory
--------- | ------- | ----------- | ----------- | -----------
method | Request Method | CONST | getToken | TRUE
secretkey | API secret key given by Tiket.com | CHAR(128) |  | TRUE
token  | The expired token you wish to keep the login information | CHAR(128) |  | FALSE





## Change Output Format

To change output, you can add parameter output in URL format.
Type of parameter output :

* **array**
* xml
* json
* serialize

### HTTP Request

`GET https://api-sandbox.tiket.com/order?token=c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f&output=xml`

### Parameter

Name | Description | Format    | Default   | Mandatory
--------- | ------- | ----------- | ----------- | -----------
output | Output format | CONST | array | FALSE


## List Currencies

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
    <code>AUD</code>
    <name>Dolar Australia (AUD)</name>
  </result>
  <result>
    <code>BND</code>
    <name>Dolar Brunei (BND)</name>
  </result>
  <result>
    <code>CAD</code>
    <name>Dolar Kanada (CAD)</name>
  </result>
  <result>
    <code>CHF</code>
    <name>Swiss Franc (CHF)</name>
  </result>
  <result>
    <code>CNY</code>
    <name>Yuan China (CNY)</name>
  </result>
  <result>
    <code>DKK</code>
    <name>Danish Krone (DKK)</name>
  </result>
  <result>
    <code>EUR</code>
    <name>Euro (EUR)</name>
  </result>
  <result>
    <code>GBP</code>
    <name>British Pound (GBP)</name>
  </result>
  <result>
    <code>HKD</code>
    <name>Dolar Hongkong (HKD)</name>
  </result>
  <result>
    <code>IDR</code>
    <name>Rupiah Indonesia (IDR)</name>
  </result>
  <result>
    <code>JPY</code>
    <name>Yen Jepang (JPY)</name>
  </result>
  <result>
    <code>KRW</code>
    <name>Won Korea (KRW)</name>
  </result>
  <result>
    <code>KWD</code>
    <name>Kuwaiti Dinar (KWD)</name>
  </result>
  <result>
    <code>MOP</code>
    <name>Macau Pataca (MOP)</name>
  </result>
  <result>
    <code>MYR</code>
    <name>Ringgit Malaysia (MYR)</name>
  </result>
  <result>
    <code>NOK</code>
    <name>Norwegian Krone (NOK)</name>
  </result>
  <result>
    <code>NPR</code>
    <name>Nepal Rupee (NPR)</name>
  </result>
  <result>
    <code>NZD</code>
    <name>Dolar Selandia Baru (NZD)</name>
  </result>
  <result>
    <code>PGK</code>
    <name>Papua New Guinean Kina (PGK)</name>
  </result>
  <result>
    <code>PHP</code>
    <name>Peso Filipina (PHP)</name>
  </result>
  <result>
    <code>RUB</code>
    <name>Rubel Rusia (RUB)</name>
  </result>
  <result>
    <code>SAR</code>
    <name>Saudi Riyal (SAR)</name>
  </result>
  <result>
    <code>SEK</code>
    <name>Swedish Krona (SEK)</name>
  </result>
  <result>
    <code>SGD</code>
    <name>Dolar Singapura (SGD)</name>
  </result>
  <result>
    <code>THB</code>
    <name>Baht Thailand (THB)</name>
  </result>
  <result>
    <code>TWD</code>
    <name>Dolar Taiwan (TWD)</name>
  </result>
  <result>
    <code>USD</code>
    <name>Dolar Amerika (USD)</name>
  </result>
  <result>
    <code>VND</code>
    <name>Dong Vietnam (VND)</name>
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
    "code": "AUD",
    "name": "Dolar Australia (AUD)"
  }, {
    "code": "BND",
    "name": "Dolar Brunei (BND)"
  }, {
    "code": "CAD",
    "name": "Dolar Kanada (CAD)"
  }, {
    "code": "CHF",
    "name": "Swiss Franc (CHF)"
  }, {
    "code": "CNY",
    "name": "Yuan China (CNY)"
  }, {
    "code": "DKK",
    "name": "Danish Krone (DKK)"
  }, {
    "code": "EUR",
    "name": "Euro (EUR)"
  }, {
    "code": "GBP",
    "name": "British Pound (GBP)"
  }, {
    "code": "HKD",
    "name": "Dolar Hongkong (HKD)"
  }, {
    "code": "IDR",
    "name": "Rupiah Indonesia (IDR)"
  }, {
    "code": "JPY",
    "name": "Yen Jepang (JPY)"
  }, {
    "code": "KRW",
    "name": "Won Korea (KRW)"
  }, {
    "code": "KWD",
    "name": "Kuwaiti Dinar (KWD)"
  }, {
    "code": "MOP",
    "name": "Macau Pataca (MOP)"
  }, {
    "code": "MYR",
    "name": "Ringgit Malaysia (MYR)"
  }, {
    "code": "NOK",
    "name": "Norwegian Krone (NOK)"
  }, {
    "code": "NPR",
    "name": "Nepal Rupee (NPR)"
  }, {
    "code": "NZD",
    "name": "Dolar Selandia Baru (NZD)"
  }, {
    "code": "PGK",
    "name": "Papua New Guinean Kina (PGK)"
  }, {
    "code": "PHP",
    "name": "Peso Filipina (PHP)"
  }, {
    "code": "RUB",
    "name": "Rubel Rusia (RUB)"
  }, {
    "code": "SAR",
    "name": "Saudi Riyal (SAR)"
  }, {
    "code": "SEK",
    "name": "Swedish Krona (SEK)"
  }, {
    "code": "SGD",
    "name": "Dolar Singapura (SGD)"
  }, {
    "code": "THB",
    "name": "Baht Thailand (THB)"
  }, {
    "code": "TWD",
    "name": "Dolar Taiwan (TWD)"
  }, {
    "code": "USD",
    "name": "Dolar Amerika (USD)"
  }, {
    "code": "VND",
    "name": "Dong Vietnam (VND)"
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
  s: 11: "output_type";s: 9: "serialize";s: 6: "result";a: 28: {
    i: 0;a: 2: {
      s: 4: "code";s: 3: "AUD";s: 4: "name";s: 22: "Dolar Australia (AUD)";
    }
    i: 1;a: 2: {
      s: 4: "code";s: 3: "BND";s: 4: "name";s: 22: "Dolar Brunei (BND)";
    }
    i: 2;a: 2: {
      s: 4: "code";s: 3: "CAD";s: 4: "name";s: 22: "Dolar Kanada (CAD)";
    }
    i: 3;a: 2: {
      s: 4: "code";s: 3: "CHF";s: 4: "name";s: 22: "Swiss Franc (CHF)";
    }
    i: 4;a: 2: {
      s: 4: "code";s: 3: "CNY";s: 4: "name";s: 22: "Yuan China (CNY)";
    }
    i: 5;a: 2: {
      s: 4: "code";s: 3: "DKK";s: 4: "name";s: 22: "Danish Krone (DKK)";
    }
    i: 6;a: 2: {
      s: 4: "code";s: 3: "EUR";s: 4: "name";s: 22: "Euro (EUR)";
    }
    i: 7;a: 2: {
      s: 4: "code";s: 3: "GBP";s: 4: "name";s: 22: "British Pound (GBP)";
    }
    i: 8;a: 2: {
      s: 4: "code";s: 3: "HKD";s: 4: "name";s: 22: "Dolar Hongkong (HKD)";
    }
    i: 9;a: 2: {
      s: 4: "code";s: 3: "IDR";s: 4: "name";s: 22: "Rupiah Indonesia (IDR)";
    }
    i: 10;a: 2: {
      s: 4: "code";s: 3: "JPY";s: 4: "name";s: 22: "Yen Jepang (JPY)";
    }
    i: 11;a: 2: {
      s: 4: "code";s: 3: "KRW";s: 4: "name";s: 22: "Won Korea (KRW)";
    }
    i: 12;a: 2: {
      s: 4: "code";s: 3: "KWD";s: 4: "name";s: 22: "Kuwaiti Dinar (KWD)";
    }
    i: 13;a: 2: {
      s: 4: "code";s: 3: "MOP";s: 4: "name";s: 22: "Macau Pataca (MOP)";
    }
    i: 14;a: 2: {
      s: 4: "code";s: 3: "MYR";s: 4: "name";s: 22: "Ringgit Malaysia (MYR)";
    }
    i: 15;a: 2: {
      s: 4: "code";s: 3: "NOK";s: 4: "name";s: 22: "Norwegian Krone (NOK)";
    }
    i: 16;a: 2: {
      s: 4: "code";s: 3: "NPR";s: 4: "name";s: 22: "Nepal Rupee (NPR)";
    }
    i: 17;a: 2: {
      s: 4: "code";s: 3: "NZD";s: 4: "name";s: 22: "Dolar Selandia Baru (NZD)";
    }
    i: 18;a: 2: {
      s: 4: "code";s: 3: "PGK";s: 4: "name";s: 22: "Papua New Guinean Kina (PGK)";
    }
    i: 19;a: 2: {
      s: 4: "code";s: 3: "PHP";s: 4: "name";s: 22: "Peso Filipina (PHP)";
    }
    i: 20;a: 2: {
      s: 4: "code";s: 3: "RUB";s: 4: "name";s: 22: "Rubel Rusia (RUB)";
    }
    i: 21;a: 2: {
      s: 4: "code";s: 3: "SAR";s: 4: "name";s: 22: "Saudi Riyal (SAR)";
    }
    i: 22;a: 2: {
      s: 4: "code";s: 3: "SEK";s: 4: "name";s: 22: "Swedish Krona (SEK)";
    }
    i: 23;a: 2: {
      s: 4: "code";s: 3: "SGD";s: 4: "name";s: 22: "Dolar Singapura (SGD)";
    }
    i: 24;a: 2: {
      s: 4: "code";s: 3: "THB";s: 4: "name";s: 22: "Baht Thailand (THB)";
    }
    i: 25;a: 2: {
      s: 4: "code";s: 3: "TWD";s: 4: "name";s: 22: "Dolar Taiwan (TWD)";
    }
    i: 26;a: 2: {
      s: 4: "code";s: 3: "USD";s: 4: "name";s: 22: "Dolar Amerika (USD)";
    }
    i: 27;a: 2: {
      s: 4: "code";s: 3: "VND";s: 4: "name";s: 22: "Dong Vietnam (VND)";
    }
  }
  s: 12: "login_status";s: 5: "false";s: 5: "token";s: 40: "c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f";
}
```

List of all the currency available at Tiket.com

### HTTP Request

`GET https://api-sandbox.tiket.com/general_api/listCurrency?token=c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f`

### Parameter

Name | Description | Format    | Default   | Mandatory
--------- | ------- | ----------- | ----------- | -----------
token | Token acquired from gettoken | CHAR(128) |  | TRUE


## List Language

```http
GET /general_api/listLanguage?token=c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f HTTP/1.1
Host: api-sandbox.tiket.com
User-Agent: twh:123456789;Partner Name;
Content-Type: text/plain
```

```xml
<tiket>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.0606</elapsetime>
    <memoryusage>4.48MB</memoryusage>
    <unix_timestamp>1399539230</unix_timestamp>
    <confirm>success</confirm>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <output_type>xml</output_type>
  <result>
    <code>en</code>
    <name_long>English</name_long>
    <name_short>ENG</name_short>
  </result>
  <result>
    <code>id</code>
    <name_long>Indonesian</name_long>
    <name_short>IND</name_short>
  </result>
  <login_status>false</login_status>
  <token>c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f</token>
</tiket>
```

```json
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.0579",
    "memoryusage": "4.47MB",
    "unix_timestamp": 1399539322,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "result": [{
    "code": "en",
    "name_long": "English",
    "name_short": "ENG"
  }, {
    "code": "id",
    "name_long": "Indonesian",
    "name_short": "IND"
  }],
  "login_status": "false",
  "token": "c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f"
}
```

```matlib
a: 5: {
  s: 10: ”diagnostic”;a: 7: {
    s: 6: ”status”;i: 200;s: 10: ”elapsetime”;s: 14: ”0.3551″;s: 11: ”memoryusage”;s: 14: ”4.47 MB”;s: 14: ”unix_timestamp”;i: 1399539348;s: 7: ”confirm”;s: 7: ”success”;s: 4: ”lang”;s: 2: ”id”;s: 8: ”currency”;s: 3: ”IDR”;
  }
  s: 11: ”output_type”;s: 9: ”serialize”;s: 6: ”result”;a: 2: {
    i: 0;a: 3: {
      s: 4: ”code”;s: 2: ”en”;s: 9: ”name_long”;s: 7: ”English”;s: 10: ”name_short”;s: 3: ”ENG”;
    }
    i: 1;a: 3: {
      s: 4: ”code”;s: 2: ”id”;s: 9: ”name_long”;s: 10: ”Indonesian”;s: 10: ”name_short”;s: 3: ”IND”;
    }
  }
  s: 12: ”login_status”;s: 5: ”false”;s: 5: ”token”;s: 40: ”c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f”;
}
```

List all available languages.

To change the languages, just add parameter <code>lang=&lt;code&gt;</code>. For example:

`GET https://api-sandox.tiket.com/order?lang=id&token=c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f`

### HTTP Request

`GET https://api-sandbox.tiket.com/general_api/listLanguage?token=c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f`

### Parameter

Name | Description | Format    | Default   | Mandatory
--------- | ------- | ----------- | ----------- | -----------
token | Token acquired from gettoken | CHAR(128) |  | TRUE










