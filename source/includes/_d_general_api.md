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

#### HTTP Request

`GET https://api-sandbox.tiket.com/apiv1/payexpress?method=getToken&secretkey=56c8624d6a62e1ab22f0d9915ff2d43c`

#### Parameters

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


#### HTTP Request

`GET https://api-sandbox.tiket.com/apiv1/payexpress?method=getToken&secretkey=56c8624d6a62e1ab22f0d9915ff2d43c&token=712402a7c363b12d87f6b02749f6f0c91b64c47e`

#### Parameters

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

#### HTTP Request

`GET https://api-sandbox.tiket.com/order?token=c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f&output=xml`

#### Parameter

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
<?xml version="1.0" encoding="utf-8"?>
<tiket>
    <diagnostic>
        <status>200</status>
        <elapsetime>0.0762</elapsetime>
        <memoryusage>4.65MB</memoryusage>
        <unix_timestamp>1470208326</unix_timestamp>
        <confirm>success</confirm>
        <lang>id</lang>
        <currency>IDR</currency>
    </diagnostic>
    <output_type>xml</output_type>
    <result>
        <id>au</id>
        <lang>en-au</lang>
        <code>AUD</code>
        <name>AUD - Dolar Australia</name>
    </result>
    <result>
        <id>bn</id>
        <lang>ms</lang>
        <code>BND</code>
        <name>BND - Dolar Brunei</name>
    </result>
    <result>
        <id>ca</id>
        <lang>en-ca</lang>
        <code>CAD</code>
        <name>CAD - Dolar Kanada</name>
    </result>
    <result>
        <id>ch</id>
        <lang>fr-ch</lang>
        <code>CHF</code>
        <name>CHF - Swiss Franc</name>
    </result>
    <result>
        <id>cn</id>
        <lang>zh-cn</lang>
        <code>CNY</code>
        <name>CNY - Yuan China</name>
    </result>
    <result>
        <id>dk</id>
        <lang>da</lang>
        <code>DKK</code>
        <name>DKK - Danish Krone</name>
    </result>
    <result>
        <id>eu</id>
        <lang>en-gb</lang>
        <code>EUR</code>
        <name>EUR - Euro</name>
    </result>
    <result>
        <id>gb</id>
        <lang>en-gb</lang>
        <code>GBP</code>
        <name>GBP - British Pound</name>
    </result>
    <result>
        <id>hk</id>
        <lang>zh-hk</lang>
        <code>HKD</code>
        <name>HKD - Dolar Hongkong</name>
    </result>
    <result>
        <id>id</id>
        <lang>id</lang>
        <code>IDR</code>
        <name>IDR - Rupiah Indonesia</name>
    </result>
    <result>
        <id>in</id>
        <lang>hi</lang>
        <code>INR</code>
        <name>INR - Rupee India</name>
    </result>
    <result>
        <id>jp</id>
        <lang>ja</lang>
        <code>JPY</code>
        <name>JPY - Yen Jepang</name>
    </result>
    <result>
        <id>kr</id>
        <lang>ko</lang>
        <code>KRW</code>
        <name>KRW - Won Korea</name>
    </result>
    <result>
        <id>kw</id>
        <lang>ar-kw</lang>
        <code>KWD</code>
        <name>KWD - Kuwaiti Dinar</name>
    </result>
    <result>
        <id>lb</id>
        <lang>ar-lb</lang>
        <code>LBP</code>
        <name>LBP - Lebanese Pound</name>
    </result>
    <result>
        <id>mo</id>
        <lang>pt</lang>
        <code>MOP</code>
        <name>MOP - Macau Pataca</name>
    </result>
    <result>
        <id>my</id>
        <lang>my</lang>
        <code>MYR</code>
        <name>MYR - Ringgit Malaysia</name>
    </result>
    <result>
        <id>no</id>
        <lang>no</lang>
        <code>NOK</code>
        <name>NOK - Norwegian Krone</name>
    </result>
    <result>
        <id>np</id>
        <lang>ne</lang>
        <code>NPR</code>
        <name>NPR - Nepal Rupee</name>
    </result>
    <result>
        <id>nz</id>
        <lang>en-gb</lang>
        <code>NZD</code>
        <name>NZD - Dolar Selandia Baru</name>
    </result>
    <result>
        <id>pg</id>
        <lang>ngf</lang>
        <code>PGK</code>
        <name>PGK - Papua New Guinean Kina</name>
    </result>
    <result>
        <id>ph</id>
        <lang>phi</lang>
        <code>PHP</code>
        <name>PHP - Peso Filipina</name>
    </result>
    <result>
        <id>pl</id>
        <lang>pl</lang>
        <code>PLN</code>
        <name>PLN - Polish Zloty</name>
    </result>
    <result>
        <id>ru</id>
        <lang>fa</lang>
        <code>RUB</code>
        <name>RUB - Rubel Rusia</name>
    </result>
    <result>
        <id>sa</id>
        <lang>ar</lang>
        <code>SAR</code>
        <name>SAR - Saudi Riyal</name>
    </result>
    <result>
        <id>se</id>
        <lang>sv</lang>
        <code>SEK</code>
        <name>SEK - Swedish Krona</name>
    </result>
    <result>
        <id>sg</id>
        <lang>zh-sg</lang>
        <code>SGD</code>
        <name>SGD - Dolar Singapura</name>
    </result>
    <result>
        <id>th</id>
        <lang>th</lang>
        <code>THB</code>
        <name>THB - Baht Thailand</name>
    </result>
    <result>
        <id>tw</id>
        <lang>zh-tw</lang>
        <code>TWD</code>
        <name>TWD - Dolar Taiwan</name>
    </result>
    <result>
        <id>us</id>
        <lang>en-us</lang>
        <code>USD</code>
        <name>USD - Dolar Amerika</name>
    </result>
    <result>
        <id>vn</id>
        <lang>vi</lang>
        <code>VND</code>
        <name>VND - Dong Vietnam</name>
    </result>
    <login_status>false</login_status>
    <token>f9b29ac359ca5d77755e7588751c089bf96f0dc9</token>
</tiket>
```

```json
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.0790",
    "memoryusage": "4.64MB",
    "unix_timestamp": 1470207787,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "result": [
    {
      "id": "au",
      "lang": "en-au",
      "code": "AUD",
      "name": "AUD - Dolar Australia"
    },
    {
      "id": "bn",
      "lang": "ms",
      "code": "BND",
      "name": "BND - Dolar Brunei"
    },
    {
      "id": "ca",
      "lang": "en-ca",
      "code": "CAD",
      "name": "CAD - Dolar Kanada"
    },
    {
      "id": "ch",
      "lang": "fr-ch",
      "code": "CHF",
      "name": "CHF - Swiss Franc"
    },
    {
      "id": "cn",
      "lang": "zh-cn",
      "code": "CNY",
      "name": "CNY - Yuan China"
    },
    {
      "id": "dk",
      "lang": "da",
      "code": "DKK",
      "name": "DKK - Danish Krone"
    },
    {
      "id": "eu",
      "lang": "en-gb",
      "code": "EUR",
      "name": "EUR - Euro"
    },
    {
      "id": "gb",
      "lang": "en-gb",
      "code": "GBP",
      "name": "GBP - British Pound"
    },
    {
      "id": "hk",
      "lang": "zh-hk",
      "code": "HKD",
      "name": "HKD - Dolar Hongkong"
    },
    {
      "id": "id",
      "lang": "id",
      "code": "IDR",
      "name": "IDR - Rupiah Indonesia"
    },
    {
      "id": "in",
      "lang": "hi",
      "code": "INR",
      "name": "INR - Rupee India"
    },
    {
      "id": "jp",
      "lang": "ja",
      "code": "JPY",
      "name": "JPY - Yen Jepang"
    },
    {
      "id": "kr",
      "lang": "ko",
      "code": "KRW",
      "name": "KRW - Won Korea"
    },
    {
      "id": "kw",
      "lang": "ar-kw",
      "code": "KWD",
      "name": "KWD - Kuwaiti Dinar"
    },
    {
      "id": "lb",
      "lang": "ar-lb",
      "code": "LBP",
      "name": "LBP - Lebanese Pound"
    },
    {
      "id": "mo",
      "lang": "pt",
      "code": "MOP",
      "name": "MOP - Macau Pataca"
    },
    {
      "id": "my",
      "lang": "my",
      "code": "MYR",
      "name": "MYR - Ringgit Malaysia"
    },
    {
      "id": "no",
      "lang": "no",
      "code": "NOK",
      "name": "NOK - Norwegian Krone"
    },
    {
      "id": "np",
      "lang": "ne",
      "code": "NPR",
      "name": "NPR - Nepal Rupee"
    },
    {
      "id": "nz",
      "lang": "en-gb",
      "code": "NZD",
      "name": "NZD - Dolar Selandia Baru"
    },
    {
      "id": "pg",
      "lang": "ngf",
      "code": "PGK",
      "name": "PGK - Papua New Guinean Kina"
    },
    {
      "id": "ph",
      "lang": "phi",
      "code": "PHP",
      "name": "PHP - Peso Filipina"
    },
    {
      "id": "pl",
      "lang": "pl",
      "code": "PLN",
      "name": "PLN - Polish Zloty"
    },
    {
      "id": "ru",
      "lang": "fa",
      "code": "RUB",
      "name": "RUB - Rubel Rusia"
    },
    {
      "id": "sa",
      "lang": "ar",
      "code": "SAR",
      "name": "SAR - Saudi Riyal"
    },
    {
      "id": "se",
      "lang": "sv",
      "code": "SEK",
      "name": "SEK - Swedish Krona"
    },
    {
      "id": "sg",
      "lang": "zh-sg",
      "code": "SGD",
      "name": "SGD - Dolar Singapura"
    },
    {
      "id": "th",
      "lang": "th",
      "code": "THB",
      "name": "THB - Baht Thailand"
    },
    {
      "id": "tw",
      "lang": "zh-tw",
      "code": "TWD",
      "name": "TWD - Dolar Taiwan"
    },
    {
      "id": "us",
      "lang": "en-us",
      "code": "USD",
      "name": "USD - Dolar Amerika"
    },
    {
      "id": "vn",
      "lang": "vi",
      "code": "VND",
      "name": "VND - Dong Vietnam"
    }
  ],
  "login_status": "false",
  "token": "f9b29ac359ca5d77755e7588751c089bf96f0dc9"
}
```

```matlab
a:5:{s:10:"diagnostic";a:7:{s:6:"status";i:200;s:10:"elapsetime";s:14:"0.0736";s:11:"memoryusage";s:14:"4.64MB";s:14:"unix_timestamp";i:1470208487;s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:11:"output_type";s:9:"serialize";s:6:"result";a:31:{i:0;a:4:{s:2:"id";s:2:"au";s:4:"lang";s:5:"en-au";s:4:"code";s:3:"AUD";s:4:"name";s:22:"AUD - Dolar Australia";}i:1;a:4:{s:2:"id";s:2:"bn";s:4:"lang";s:2:"ms";s:4:"code";s:3:"BND";s:4:"name";s:22:"BND - Dolar Brunei";}i:2;a:4:{s:2:"id";s:2:"ca";s:4:"lang";s:5:"en-ca";s:4:"code";s:3:"CAD";s:4:"name";s:22:"CAD - Dolar Kanada";}i:3;a:4:{s:2:"id";s:2:"ch";s:4:"lang";s:5:"fr-ch";s:4:"code";s:3:"CHF";s:4:"name";s:22:"CHF - Swiss Franc";}i:4;a:4:{s:2:"id";s:2:"cn";s:4:"lang";s:5:"zh-cn";s:4:"code";s:3:"CNY";s:4:"name";s:22:"CNY - Yuan China";}i:5;a:4:{s:2:"id";s:2:"dk";s:4:"lang";s:2:"da";s:4:"code";s:3:"DKK";s:4:"name";s:22:"DKK - Danish Krone";}i:6;a:4:{s:2:"id";s:2:"eu";s:4:"lang";s:5:"en-gb";s:4:"code";s:3:"EUR";s:4:"name";s:22:"EUR - Euro";}i:7;a:4:{s:2:"id";s:2:"gb";s:4:"lang";s:5:"en-gb";s:4:"code";s:3:"GBP";s:4:"name";s:22:"GBP - British Pound";}i:8;a:4:{s:2:"id";s:2:"hk";s:4:"lang";s:5:"zh-hk";s:4:"code";s:3:"HKD";s:4:"name";s:22:"HKD - Dolar Hongkong";}i:9;a:4:{s:2:"id";s:2:"id";s:4:"lang";s:2:"id";s:4:"code";s:3:"IDR";s:4:"name";s:22:"IDR - Rupiah Indonesia";}i:10;a:4:{s:2:"id";s:2:"in";s:4:"lang";s:2:"hi";s:4:"code";s:3:"INR";s:4:"name";s:22:"INR - Rupee India";}i:11;a:4:{s:2:"id";s:2:"jp";s:4:"lang";s:2:"ja";s:4:"code";s:3:"JPY";s:4:"name";s:22:"JPY - Yen Jepang";}i:12;a:4:{s:2:"id";s:2:"kr";s:4:"lang";s:2:"ko";s:4:"code";s:3:"KRW";s:4:"name";s:22:"KRW - Won Korea";}i:13;a:4:{s:2:"id";s:2:"kw";s:4:"lang";s:5:"ar-kw";s:4:"code";s:3:"KWD";s:4:"name";s:22:"KWD - Kuwaiti Dinar";}i:14;a:4:{s:2:"id";s:2:"lb";s:4:"lang";s:5:"ar-lb";s:4:"code";s:3:"LBP";s:4:"name";s:22:"LBP - Lebanese Pound";}i:15;a:4:{s:2:"id";s:2:"mo";s:4:"lang";s:2:"pt";s:4:"code";s:3:"MOP";s:4:"name";s:22:"MOP - Macau Pataca";}i:16;a:4:{s:2:"id";s:2:"my";s:4:"lang";s:2:"my";s:4:"code";s:3:"MYR";s:4:"name";s:22:"MYR - Ringgit Malaysia";}i:17;a:4:{s:2:"id";s:2:"no";s:4:"lang";s:2:"no";s:4:"code";s:3:"NOK";s:4:"name";s:22:"NOK - Norwegian Krone";}i:18;a:4:{s:2:"id";s:2:"np";s:4:"lang";s:2:"ne";s:4:"code";s:3:"NPR";s:4:"name";s:22:"NPR - Nepal Rupee";}i:19;a:4:{s:2:"id";s:2:"nz";s:4:"lang";s:5:"en-gb";s:4:"code";s:3:"NZD";s:4:"name";s:22:"NZD - Dolar Selandia Baru";}i:20;a:4:{s:2:"id";s:2:"pg";s:4:"lang";s:3:"ngf";s:4:"code";s:3:"PGK";s:4:"name";s:22:"PGK - Papua New Guinean Kina";}i:21;a:4:{s:2:"id";s:2:"ph";s:4:"lang";s:3:"phi";s:4:"code";s:3:"PHP";s:4:"name";s:22:"PHP - Peso Filipina";}i:22;a:4:{s:2:"id";s:2:"pl";s:4:"lang";s:2:"pl";s:4:"code";s:3:"PLN";s:4:"name";s:22:"PLN - Polish Zloty";}i:23;a:4:{s:2:"id";s:2:"ru";s:4:"lang";s:2:"fa";s:4:"code";s:3:"RUB";s:4:"name";s:22:"RUB - Rubel Rusia";}i:24;a:4:{s:2:"id";s:2:"sa";s:4:"lang";s:2:"ar";s:4:"code";s:3:"SAR";s:4:"name";s:22:"SAR - Saudi Riyal";}i:25;a:4:{s:2:"id";s:2:"se";s:4:"lang";s:2:"sv";s:4:"code";s:3:"SEK";s:4:"name";s:22:"SEK - Swedish Krona";}i:26;a:4:{s:2:"id";s:2:"sg";s:4:"lang";s:5:"zh-sg";s:4:"code";s:3:"SGD";s:4:"name";s:22:"SGD - Dolar Singapura";}i:27;a:4:{s:2:"id";s:2:"th";s:4:"lang";s:2:"th";s:4:"code";s:3:"THB";s:4:"name";s:22:"THB - Baht Thailand";}i:28;a:4:{s:2:"id";s:2:"tw";s:4:"lang";s:5:"zh-tw";s:4:"code";s:3:"TWD";s:4:"name";s:22:"TWD - Dolar Taiwan";}i:29;a:4:{s:2:"id";s:2:"us";s:4:"lang";s:5:"en-us";s:4:"code";s:3:"USD";s:4:"name";s:22:"USD - Dolar Amerika";}i:30;a:4:{s:2:"id";s:2:"vn";s:4:"lang";s:2:"vi";s:4:"code";s:3:"VND";s:4:"name";s:22:"VND - Dong Vietnam";}}s:12:"login_status";s:5:"false";s:5:"token";s:40:"f9b29ac359ca5d77755e7588751c089bf96f0dc9";}
```

List of all the currency available at Tiket.com

#### HTTP Request

`GET https://api-sandbox.tiket.com/general_api/listCurrency?token=c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f`

#### Parameter

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

```matlab
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

#### HTTP Request

`GET https://api-sandbox.tiket.com/general_api/listLanguage?token=c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f`

#### Parameter

Name | Description | Format    | Default   | Mandatory
--------- | ------- | ----------- | ----------- | -----------
token | Token acquired from gettoken | CHAR(128) |  | TRUE

## List Country

```http
GET /general_api/listCountry?token=c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f HTTP/1.1
Host: api-sandbox.tiket.com
User-Agent: twh:123456789;Partner Name;
Content-Type: text/plain
```

```xml
<tiket>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.0754</elapsetime>
    <memoryusage>5.05MB</memoryusage>
    <unix_timestamp>1399538816</unix_timestamp>
    <confirm>success</confirm>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <output_type>xml</output_type>
  <listCountry>
    <country_id>id</country_id>
    <country_name>Indonesia</country_name>
    <country_areacode>+62</country_areacode>
  </listCountry>
  <listCountry>
    <country_id>sg</country_id>
    <country_name>Singapore</country_name>
    <country_areacode>+65</country_areacode>
  </listCountry>
  <listCountry>
    <country_id>gb</country_id>
    <country_name>United Kingdom</country_name>
    <country_areacode>+44</country_areacode>
  </listCountry>
  <listCountry>
    <country_id>us</country_id>
    <country_name>United States</country_name>
    <country_areacode>+1</country_areacode>
  </listCountry>
  <login_status>false</login_status>
  <token>c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f</token>
</tiket>
```

```json
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.0574",
    "memoryusage": "5.02MB",
    "unix_timestamp": 1399538966,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "listCountry": [{
    "country_id": "id",
    "country_name": "Indonesia",
    "country_areacode": "+62"
  }, {
    "country_id": "sg",
    "country_name": "Singapore ",
    "country_areacode": "+65"
  }, {
    "country_id": "gb",
    "country_name": "United Kingdom ",
    "country_areacode": "+44"
  }, {
    "country_id": "us",
    "country_name": "United States ",
    "country_areacode": "+1"
  }],
  "login_status": "false",
  "token": "c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f"
}
```

```matlib
a: 5: {
  s: 10: "diagnostic";a: 7: {
    s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.0617";s: 11: "memoryusage";s: 14: "5.03MB";s: 14: "unix_timestamp";i: 1399539028;s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "id";s: 8: "currency";s: 3: "IDR";
  }
  s: 11: "output_type";s: 9: "serialize";s: 11: "listCountry";a: 4: {
    i: 0;a: 3: {
      s: 10: "country_id";s: 2: "id";s: 12: "country_name";s: 9: "Indonesia";s: 16: "country_areacode";s: 3: "+62";
    }
    i: 1;a: 3: {
      s: 10: "country_id";s: 2: "sg";s: 12: "country_name";s: 10: "Singapore ";s: 16: "country_areacode";s: 3: "+65";
    }
    i: 2;a: 3: {
      s: 10: "country_id";s: 2: "gb";s: 12: "country_name";s: 15: "United Kingdom ";s: 16: "country_areacode";s: 3: "+44";
    }
    i: 3;a: 3: {
      s: 10: "country_id";s: 2: "us";s: 12: "country_name";s: 14: "United States ";s: 16: "country_areacode";s: 2: "+1";
    }
  }
  s: 12: "login_status";s: 5: "false";s: 5: "token";s: 40: "c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f";
}
```

List all available countries.

#### HTTP Request

`GET https://api-sandbox.tiket.com/general_api/listCountry?token=c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f`

#### Parameter

Name | Description | Format    | Default   | Mandatory
--------- | ------- | ----------- | ----------- | -----------
token | Token acquired from gettoken | CHAR(128) |  | TRUE

## Get Transaction Policies


```http
GET /general_api/getPolicies?token=c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f&lang=id HTTP/1.1
Host: api-sandbox.tiket.com
User-Agent: twh:123456789;Partner Name;
Content-Type: text/plain
```

```xml
<?xml version="1.0" encoding="UTF-8"?>
<diagnostic>
  <status>200</status>
  <elapsetime>0.0664</elapsetime>
  <memoryusage>4.6MB</memoryusage>
  <unix_timestamp>1399539657</unix_timestamp>
  <confirm>success</confirm>
  <lang>id</lang>
  <currency>IDR</currency>
</diagnostic>
<output_type>xml</output_type>
<policies>
  <klikbca>
    <name>KlikBCA</name>
    <before>
      Jika setelah transaksi anda menerima pesan gagal seperti \"Transaction Failed, Please Call Tiket.com Call Center\", umumnya dana telah di debet dan transaksi diproses. Mohon periksa email anda untuk voucher booking anda. Jika setelah 15 menit and belum
      menerima voucher booking anda, mohon print screen dan email ke cs@tiket.com atau menghubungi customer service kami di +62 21 2963 3600
    </before>
    <before>
      User ID KlikBCA yang dimasukkan adalah User ID yang telah terdaftar pada KlikBCA.
    </before>
    <before>
      Pembayaran harus dilakukan dalam 60 menit setelah pemesanan.
    </before>
    <before>
      Transaksi akan dibatalkan (berakhir) jika anda tidak melakukan pembayaran pada periode waktu yang telah ditentukan.
    </before>
    <before>
      Untuk konfirmasi dan pencetakan bukti pembayaran, anda perlu melakukan login kembali ke Tiket.com
    </before>
    <before>
      Setelah menyelesaikan pembayaran, dalam 5 menit anda akan menerima email berisi Voucher Hotel / Event / Pesawat untuk pembelian Hotel / Tiket Event / Tiket Pesawat atau kode pemesanan
    </before>
  </klikbca>
  <jatis>
    <name>ATM Transfer</name>
    <before>
      Hanya transfer ATM via jaringan Bersama atau jaringan Prima yang bisa diproses oleh metode pembayaran ini. Untuk Internet Banking/Mobile Banking/Transfer melalui Teller/Non ATM , harap gunakan metode pembayaran transfer lewat bank
    </before>
    <before>
      Akan dikenakan biaya IDR 5.000/transaksi (tidak termasuk di total transaksi) untuk pembayaran melalui jaringan ATM bersama, Prima atau Alto. Biaya yang dikenakan sesuai dengan ketetapan ATM Bersama, Prima dan Alto.
    </before>
    <before>
      Untuk pengguna ATM Mandiri, minimum transaksi adalah IDR 50.000
    </before>
    <before>
      Hanya transfer ATM via jaringan Bersama atau jaringan Prima yang bisa diproses oleh metode pembayaran ini. Untuk Internet Banking/Mobile Banking/Transfer melalui Teller/Non ATM , harap gunakan metode pembayaran transfer lewat bank
    </before>
    <before>
      Transaksi akan dibatalkan (berakhir) jika anda tidak melakukan pembayaran pada periode waktu yang telah ditentukan.
    </before>
    <before>
      Untuk konfirmasi dan pencetakan bukti pembayaran, anda perlu melakukan login kembali ke Tiket.com
    </before>
    <before>
      Setelah menyelesaikan pembayaran, dalam 5 menit anda akan menerima email berisi Voucher Hotel / Event / Pesawat untuk pembelian Hotel / Tiket Event / Tiket Pesawat atau kode pemesanan
    </before>
    <after>
      Hanya transfer ATM via jaringan Bersama atau jaringan Prima yang bisa diproses oleh metode pembayaran ini. Untuk Internet Banking/Mobile Banking/Transfer melalui Teller/Non ATM , harap gunakan metode pembayaran transfer lewat bank
    </after>
    <after>
      10 Digit terakhir nomor Virtual Account adalah order id anda
    </after>
    <after>
      Akan dikenakan biaya IDR 5.000/transaksi (tidak termasuk di total transaksi) untuk pembayaran melalui jaringan ATM bersama, Prima atau Alto. Biaya yang dikenakan sesuai dengan ketetapan ATM Bersama, Prima dan Alto.
    </after>
    <after>
      Untuk pengguna ATM Mandiri, minimum transaksi adalah IDR 50.000
    </after>
  </jatis>
</policies>
<login_status>false</login_status>
<token>c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f</token>
</tiket>
```

```json
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.0630",
    "memoryusage": "4.59MB",
    "unix_timestamp": 1399539790,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "policies": {
    "klikbca": {
      "name": "KlikBCA",
      "before": ["Jika setelah transaksi anda menerima pesan gagal seperti \"Transaction Failed, Please Call Tiket.com Call Center\", umumnya dana telah di debet dan transaksi diproses. Mohon periksa email anda untuk voucher booking anda. Jika setelah 15 menit and belum menerima voucher booking anda, mohon print screen dan email ke cs@tiket.com atau menghubungi customer service kami di +62 21 2963 3600", "User ID KlikBCA yang dimasukkan adalah User ID yang telah terdaftar pada KlikBCA.", "Pembayaran harus dilakukan dalam 60 menit setelah pemesanan.", "Transaksi akan dibatalkan (berakhir) jika anda tidak melakukan pembayaran pada periode waktu yang telah ditentukan.", "Untuk konfirmasi dan pencetakan bukti pembayaran, anda perlu melakukan login kembali ke Tiket.com", "Setelah menyelesaikan pembayaran, dalam 5 menit anda akan menerima email berisi  Voucher Hotel / Event / Pesawat untuk pembelian Hotel / Tiket Event / Tiket Pesawat atau kode pemesanan"],
      "after": []
    },
    "jatis": {
      "name": "ATM Transfer",
      "before": ["Hanya transfer ATM via jaringan Bersama atau jaringan Prima yang bisa diproses oleh metode pembayaran ini. Untuk Internet Banking/Mobile Banking/Transfer melalui Teller/Non ATM , harap gunakan metode pembayaran transfer lewat bank", "Akan dikenakan biaya IDR 5.000/transaksi (tidak termasuk di total transaksi) untuk pembayaran melalui jaringan ATM bersama, Prima atau Alto. Biaya yang dikenakan sesuai dengan ketetapan ATM Bersama, Prima dan Alto. ", "Untuk pengguna ATM Mandiri, minimum transaksi adalah IDR 50.000", "Hanya transfer ATM via jaringan Bersama atau jaringan Prima yang bisa diproses oleh metode pembayaran ini. Untuk Internet Banking/Mobile Banking/Transfer melalui Teller/Non ATM , harap gunakan metode pembayaran transfer lewat bank", "Transaksi akan dibatalkan (berakhir) jika anda tidak melakukan pembayaran pada periode waktu yang telah ditentukan.", "Untuk konfirmasi dan pencetakan bukti pembayaran, anda perlu melakukan login kembali ke Tiket.com", "Setelah menyelesaikan pembayaran, dalam 5 menit anda akan menerima email berisi  Voucher Hotel / Event / Pesawat untuk pembelian Hotel / Tiket Event / Tiket Pesawat atau kode pemesanan"],
      "after": ["Hanya transfer ATM via jaringan Bersama atau jaringan Prima yang bisa diproses oleh metode pembayaran ini. Untuk Internet Banking/Mobile Banking/Transfer melalui Teller/Non ATM , harap gunakan metode pembayaran transfer lewat bank", "10 Digit terakhir nomor Virtual Account adalah order id anda", "Akan dikenakan biaya IDR 5.000/transaksi (tidak termasuk di total transaksi) untuk pembayaran melalui jaringan ATM bersama, Prima atau Alto. Biaya yang dikenakan sesuai dengan ketetapan ATM Bersama, Prima dan Alto. ", "Untuk pengguna ATM Mandiri, minimum transaksi adalah IDR 50.000"]
    }
  },
  "login_status": "false",
  "token": "c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f"
}
```

```matlab
a: 5: {
  s: 10: "diagnostic";a: 7: {
    s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.0704";s: 11: "memoryusage";s: 14: "4.59MB";s: 14: "unix_timestamp";i: 1399539812;s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "id";s: 8: "currency";s: 3: "IDR";
  }
  s: 11: "output_type";s: 9: "serialize";s: 8: "policies";a: 2: {
    s: 7: "klikbca";a: 3: {
      s: 4: "name";s: 7: "KlikBCA";s: 6: "before";a: 6: {
        i: 0;s: 46: "Jika setelah transaksi anda menerima pesan gagal seperti \"Transaction Failed, Please Call Tiket.com Call Center\", umumnya dana telah di debet dan transaksi diproses. Mohon periksa email anda untuk voucher booking anda. Jika setelah 15 menit and belum menerima voucher booking anda, mohon print screen dan email ke cs@tiket.com atau menghubungi customer service kami di +62 21 2963 3600";i: 1;s: 36: "User ID KlikBCA yang dimasukkan adalah User ID yang telah terdaftar pada KlikBCA.";i: 2;s: 36: "Pembayaran harus dilakukan dalam 60 menit setelah pemesanan.";i: 3;s: 32: "Transaksi akan dibatalkan (berakhir) jika anda tidak melakukan pembayaran pada periode waktu yang telah ditentukan.";i: 4;s: 36: "Untuk konfirmasi dan pencetakan bukti pembayaran, anda perlu melakukan login kembali ke Tiket.com";i: 5;s: 34: "Setelah menyelesaikan pembayaran, dalam 5 menit anda akan menerima email berisi Voucher Hotel / Event / Pesawat untuk pembelian Hotel / Tiket Event / Tiket Pesawat atau kode pemesanan";
      }
      s: 5: "after";a: 0: {}
    }
    s: 5: "jatis";a: 3: {
      s: 4: "name";s: 12: "ATM Transfer";s: 6: "before";a: 7: {
        i: 0;s: 36: "Hanya transfer ATM via jaringan Bersama atau jaringan Prima yang bisa diproses oleh metode pembayaran ini. Untuk Internet Banking/Mobile Banking/Transfer melalui Teller/Non ATM , harap gunakan metode pembayaran transfer lewat bank";i: 1;s: 35: "Akan dikenakan biaya IDR 5.000/transaksi (tidak termasuk di total transaksi) untuk pembayaran melalui jaringan ATM bersama, Prima atau Alto. Biaya yang dikenakan sesuai dengan ketetapan ATM Bersama, Prima dan Alto. ";i: 2;s: 26: "Untuk pengguna ATM Mandiri, minimum transaksi adalah IDR 50.000";i: 3;s: 36: "Hanya transfer ATM via jaringan Bersama atau jaringan Prima yang bisa diproses oleh metode pembayaran ini. Untuk Internet Banking/Mobile Banking/Transfer melalui Teller/Non ATM , harap gunakan metode pembayaran transfer lewat bank";i: 4;s: 32: "Transaksi akan dibatalkan (berakhir) jika anda tidak melakukan pembayaran pada periode waktu yang telah ditentukan.";i: 5;s: 36: "Untuk konfirmasi dan pencetakan bukti pembayaran, anda perlu melakukan login kembali ke Tiket.com";i: 6;s: 34: "Setelah menyelesaikan pembayaran, dalam 5 menit anda akan menerima email berisi Voucher Hotel / Event / Pesawat untuk pembelian Hotel / Tiket Event / Tiket Pesawat atau kode pemesanan";
      }
      s: 5: "after";a: 4: {
        i: 0;s: 36: "Hanya transfer ATM via jaringan Bersama atau jaringan Prima yang bisa diproses oleh metode pembayaran ini. Untuk Internet Banking/Mobile Banking/Transfer melalui Teller/Non ATM , harap gunakan metode pembayaran transfer lewat bank";i: 1;s: 19: "10 Digit terakhir nomor Virtual Account adalah order id anda";i: 2;s: 35: "Akan dikenakan biaya IDR 5.000/transaksi (tidak termasuk di total transaksi) untuk pembayaran melalui jaringan ATM bersama, Prima atau Alto. Biaya yang dikenakan sesuai dengan ketetapan ATM Bersama, Prima dan Alto. ";i: 3;s: 26: "Untuk pengguna ATM Mandiri, minimum transaksi adalah IDR 50.000";
      }
    }
  }
  s: 12: "login_status";s: 5: "false";s: 5: "token";s: 40: "c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f";
}
```

Text to be used on you checkout process. <code>before</code> means the text is placed before customer finalize payment. <code>after</code> means the text is placed right after customer finish checking out.

#### HTTP Request

`GET https://api-sandbox.tiket.com/general_api/getPolicies?token=c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f&lang=id`

#### Parameter

Name | Description | Format    | Default   | Mandatory
--------- | ------- | ----------- | ----------- | -----------
token | Token acquired from gettoken | CHAR(128) |  | TRUE
lang  | The [language](#list-language) used | CHAR(2) | id | FALSE





