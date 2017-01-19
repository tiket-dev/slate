# General API

These are the API command for general configurations

## Get Token

```http
GET /apiv1/payexpress?method=getToken&secretkey=[your-secret-key-here]&output=[json|xml|serialize|array] HTTP/1.1
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

`GET https://api-sandbox.tiket.com/apiv1/payexpress?method=getToken&secretkey=[your-secret-key-here]`

#### Parameters

Name | Description | Format    | Default   | Mandatory
--------- | ------- | ----------- | ----------- | -----------
method | Request Method | CONST | getToken | TRUE
secretkey | API secret key given by Tiket.com | CHAR(128) |  | TRUE

## Renew Token

```http
GET /apiv1/payexpress?method=getToken&secretkey=[your-secret-key-here]&token=712402a7c363b12d87f6b02749f6f0c91b64c47e HTTP/1.1
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

`GET https://api-sandbox.tiket.com/apiv1/payexpress?method=getToken&secretkey=[your-secret-key-here]&token=712402a7c363b12d87f6b02749f6f0c91b64c47e`

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
<?xml version="1.0" encoding="utf-8"?>
<tiket>
    <diagnostic>
        <status>200</status>
        <elapsetime>0.0912</elapsetime>
        <memoryusage>5.24MB</memoryusage>
        <unix_timestamp>1470210705</unix_timestamp>
        <confirm>success</confirm>
        <lang>id</lang>
        <currency>IDR</currency>
    </diagnostic>
    <output_type>xml</output_type>
    <listCountry>
        <country_id>af</country_id>
        <country_name>Afghanistan </country_name>
        <country_areacode>+93</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ax</country_id>
        <country_name>land Islands </country_name>
        <country_areacode>+358</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>al</country_id>
        <country_name>Albania </country_name>
        <country_areacode>+355</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>dz</country_id>
        <country_name>Algeria </country_name>
        <country_areacode>+213</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>as</country_id>
        <country_name>American Samoa </country_name>
        <country_areacode>+684</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ad</country_id>
        <country_name>Andorra </country_name>
        <country_areacode>+376</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ao</country_id>
        <country_name>Angola </country_name>
        <country_areacode>+244</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ai</country_id>
        <country_name>Anguilla </country_name>
        <country_areacode>+126</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>aq</country_id>
        <country_name>Antarctica </country_name>
        <country_areacode>+672</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ag</country_id>
        <country_name>Antigua And Barbuda </country_name>
        <country_areacode>+126</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ar</country_id>
        <country_name>Argentina </country_name>
        <country_areacode>+54</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>am</country_id>
        <country_name>Armenia </country_name>
        <country_areacode>+374</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>aw</country_id>
        <country_name>Aruba </country_name>
        <country_areacode>+297</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>au</country_id>
        <country_name>Australia </country_name>
        <country_areacode>+61</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>at</country_id>
        <country_name>Austria </country_name>
        <country_areacode>+43</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>az</country_id>
        <country_name>Azerbaijan </country_name>
        <country_areacode>+994</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>bs</country_id>
        <country_name>Bahamas </country_name>
        <country_areacode>+124</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>bh</country_id>
        <country_name>Bahrain </country_name>
        <country_areacode>+973</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>bd</country_id>
        <country_name>Bangladesh </country_name>
        <country_areacode>+880</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>bb</country_id>
        <country_name>Barbados </country_name>
        <country_areacode>+124</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>by</country_id>
        <country_name>Belarus </country_name>
        <country_areacode>+375</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>be</country_id>
        <country_name>Belgium </country_name>
        <country_areacode>+32</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>bz</country_id>
        <country_name>Belize </country_name>
        <country_areacode>+501</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>bj</country_id>
        <country_name>Benin </country_name>
        <country_areacode>+229</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>bm</country_id>
        <country_name>Bermuda </country_name>
        <country_areacode>+144</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>bt</country_id>
        <country_name>Bhutan </country_name>
        <country_areacode>+975</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>bo</country_id>
        <country_name>Bolivia </country_name>
        <country_areacode>+591</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ba</country_id>
        <country_name>Bosnia And Herzegovina </country_name>
        <country_areacode>+387</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>bw</country_id>
        <country_name>Botswana </country_name>
        <country_areacode>+267</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>bv</country_id>
        <country_name>Bouvet Island </country_name>
        <country_areacode>+47</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>br</country_id>
        <country_name>Brazil </country_name>
        <country_areacode>+55</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>io</country_id>
        <country_name>British Indian Ocean Territory </country_name>
        <country_areacode>+246</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>bn</country_id>
        <country_name>Brunei Darussalam </country_name>
        <country_areacode>+673</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>bg</country_id>
        <country_name>Bulgaria </country_name>
        <country_areacode>+359</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>bf</country_id>
        <country_name>Burkina Faso </country_name>
        <country_areacode>+226</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>bi</country_id>
        <country_name>Burundi </country_name>
        <country_areacode>+257</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>kh</country_id>
        <country_name>Cambodia </country_name>
        <country_areacode>+855</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>cm</country_id>
        <country_name>Cameroon </country_name>
        <country_areacode>+237</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ca</country_id>
        <country_name>Canada </country_name>
        <country_areacode>+1</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>cv</country_id>
        <country_name>Cape Verde </country_name>
        <country_areacode>+238</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ky</country_id>
        <country_name>Cayman Islands </country_name>
        <country_areacode>+345</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>cf</country_id>
        <country_name>Central African Republic </country_name>
        <country_areacode>+236</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>td</country_id>
        <country_name>Chad </country_name>
        <country_areacode>+235</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>cl</country_id>
        <country_name>Chile </country_name>
        <country_areacode>+56</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>cn</country_id>
        <country_name>China </country_name>
        <country_areacode>+86</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>cx</country_id>
        <country_name>Christmas Island </country_name>
        <country_areacode>+61</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>cc</country_id>
        <country_name>Cocos Keeling Islands </country_name>
        <country_areacode>+61</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>co</country_id>
        <country_name>Colombia </country_name>
        <country_areacode>+57</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>km</country_id>
        <country_name>Comoros </country_name>
        <country_areacode>+269</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>cg</country_id>
        <country_name>Congo </country_name>
        <country_areacode>+242</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>cd</country_id>
        <country_name>Congo The Democratic Republic Of The </country_name>
        <country_areacode>+243</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ck</country_id>
        <country_name>Cook Islands </country_name>
        <country_areacode>+682</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>cr</country_id>
        <country_name>Costa Rica </country_name>
        <country_areacode>+506</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ci</country_id>
        <country_name>Cte DIvoire </country_name>
        <country_areacode>+225</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>hr</country_id>
        <country_name>Croatia </country_name>
        <country_areacode>+385</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>cu</country_id>
        <country_name>Cuba </country_name>
        <country_areacode>+53</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>cy</country_id>
        <country_name>Cyprus </country_name>
        <country_areacode>+357</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>cz</country_id>
        <country_name>Czech Republic </country_name>
        <country_areacode>+420</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>dk</country_id>
        <country_name>Denmark </country_name>
        <country_areacode>+45</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>dj</country_id>
        <country_name>Djibouti </country_name>
        <country_areacode>+253</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>dm</country_id>
        <country_name>Dominica </country_name>
        <country_areacode>+767</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>do</country_id>
        <country_name>Dominican Republic </country_name>
        <country_areacode>+809</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ec</country_id>
        <country_name>Ecuador </country_name>
        <country_areacode>+593</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>eg</country_id>
        <country_name>Egypt</country_name>
        <country_areacode>+20</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>sv</country_id>
        <country_name>El Salvador </country_name>
        <country_areacode>+503</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>gq</country_id>
        <country_name>Equatorial Guinea </country_name>
        <country_areacode>+240</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>er</country_id>
        <country_name>Eritrea </country_name>
        <country_areacode>+291</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ee</country_id>
        <country_name>Estonia </country_name>
        <country_areacode>+372</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>et</country_id>
        <country_name>Ethiopia </country_name>
        <country_areacode>+251</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>fk</country_id>
        <country_name>Falkland Islands Malvinas </country_name>
        <country_areacode>+500</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>fo</country_id>
        <country_name>Faroe Islands </country_name>
        <country_areacode>+298</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>fj</country_id>
        <country_name>Fiji </country_name>
        <country_areacode>+679</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>fi</country_id>
        <country_name>Finland </country_name>
        <country_areacode>+358</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>fr</country_id>
        <country_name>France </country_name>
        <country_areacode>+33</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>gf</country_id>
        <country_name>French Guiana </country_name>
        <country_areacode>+594</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>pf</country_id>
        <country_name>French Polynesia </country_name>
        <country_areacode>+689</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>tf</country_id>
        <country_name>French Southern Territories </country_name>
        <country_areacode>+596</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ga</country_id>
        <country_name>Gabon </country_name>
        <country_areacode>+241</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>gm</country_id>
        <country_name>Gambia </country_name>
        <country_areacode>+220</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ge</country_id>
        <country_name>Georgia </country_name>
        <country_areacode>+995</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>de</country_id>
        <country_name>Germany </country_name>
        <country_areacode>+49</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>gh</country_id>
        <country_name>Ghana </country_name>
        <country_areacode>+233</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>gi</country_id>
        <country_name>Gibraltar </country_name>
        <country_areacode>+350</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>gr</country_id>
        <country_name>Greece </country_name>
        <country_areacode>+30</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>gl</country_id>
        <country_name>Greenland </country_name>
        <country_areacode>+299</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>gd</country_id>
        <country_name>Grenada </country_name>
        <country_areacode>+147</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>gp</country_id>
        <country_name>Guadeloupe </country_name>
        <country_areacode>+590</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>gu</country_id>
        <country_name>Guam </country_name>
        <country_areacode>+167</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>gt</country_id>
        <country_name>Guatemala </country_name>
        <country_areacode>+502</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>gg</country_id>
        <country_name>Guernsey </country_name>
        <country_areacode>+44</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>gn</country_id>
        <country_name>Guinea </country_name>
        <country_areacode>+224</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>gw</country_id>
        <country_name>GuineaBissau </country_name>
        <country_areacode>+245</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>gy</country_id>
        <country_name>Guyana </country_name>
        <country_areacode>+592</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ht</country_id>
        <country_name>Haiti </country_name>
        <country_areacode>+509</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>hm</country_id>
        <country_name>Heard Island And Mcdonald Islands </country_name>
        <country_areacode>+672</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>hn</country_id>
        <country_name>Honduras </country_name>
        <country_areacode>+504</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>hk</country_id>
        <country_name>Hong Kong </country_name>
        <country_areacode>+852</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>hu</country_id>
        <country_name>Hungary </country_name>
        <country_areacode>+36</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>is</country_id>
        <country_name>Iceland </country_name>
        <country_areacode>+354</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>in</country_id>
        <country_name>India </country_name>
        <country_areacode>+91</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>id</country_id>
        <country_name>Indonesia</country_name>
        <country_areacode>+62</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ir</country_id>
        <country_name>Iran Islamic Republic Of </country_name>
        <country_areacode>+98</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>iq</country_id>
        <country_name>Iraq </country_name>
        <country_areacode>+964</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ie</country_id>
        <country_name>Ireland </country_name>
        <country_areacode>+353</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>im</country_id>
        <country_name>Isle Of Man </country_name>
        <country_areacode>+44</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>il</country_id>
        <country_name>Israel </country_name>
        <country_areacode>+972</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>it</country_id>
        <country_name>Italy </country_name>
        <country_areacode>+39</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>jm</country_id>
        <country_name>Jamaica </country_name>
        <country_areacode>+876</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>jp</country_id>
        <country_name>Japan </country_name>
        <country_areacode>+81</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>je</country_id>
        <country_name>Jersey </country_name>
        <country_areacode>+44</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>jo</country_id>
        <country_name>Jordan </country_name>
        <country_areacode>+962</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>kz</country_id>
        <country_name>Kazakhstan </country_name>
        <country_areacode>+7</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ke</country_id>
        <country_name>Kenya </country_name>
        <country_areacode>+254</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ki</country_id>
        <country_name>Kiribati </country_name>
        <country_areacode>+686</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>kw</country_id>
        <country_name>Kuwait </country_name>
        <country_areacode>+965</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>kg</country_id>
        <country_name>Kyrgyzstan </country_name>
        <country_areacode>+996</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>la</country_id>
        <country_name>Laos</country_name>
        <country_areacode>+856</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>lv</country_id>
        <country_name>Latvia </country_name>
        <country_areacode>+371</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>lb</country_id>
        <country_name>Lebanon </country_name>
        <country_areacode>+961</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ls</country_id>
        <country_name>Lesotho </country_name>
        <country_areacode>+266</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>lr</country_id>
        <country_name>Liberia </country_name>
        <country_areacode>+231</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ly</country_id>
        <country_name>Libyan Arab Jamahiriya </country_name>
        <country_areacode>+218</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>li</country_id>
        <country_name>Liechtenstein </country_name>
        <country_areacode>+423</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>lt</country_id>
        <country_name>Lithuania </country_name>
        <country_areacode>+370</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>lu</country_id>
        <country_name>Luxembourg </country_name>
        <country_areacode>+352</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>mo</country_id>
        <country_name>Macau </country_name>
        <country_areacode>+853</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>mk</country_id>
        <country_name>Macedonia The Former Yugoslav Republic Of </country_name>
        <country_areacode>+389</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>mg</country_id>
        <country_name>Madagascar </country_name>
        <country_areacode>+261</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>mw</country_id>
        <country_name>Malawi </country_name>
        <country_areacode>+265</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>my</country_id>
        <country_name>Malaysia </country_name>
        <country_areacode>+60</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>mv</country_id>
        <country_name>Maldives </country_name>
        <country_areacode>+960</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ml</country_id>
        <country_name>Mali </country_name>
        <country_areacode>+223</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>mt</country_id>
        <country_name>Malta </country_name>
        <country_areacode>+356</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>mh</country_id>
        <country_name>Marshall Islands </country_name>
        <country_areacode>+692</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>mq</country_id>
        <country_name>Martinique </country_name>
        <country_areacode>+596</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>mr</country_id>
        <country_name>Mauritania </country_name>
        <country_areacode>+222</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>mu</country_id>
        <country_name>Mauritius </country_name>
        <country_areacode>+230</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>yt</country_id>
        <country_name>Mayotte </country_name>
        <country_areacode>+269</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>mx</country_id>
        <country_name>Mexico </country_name>
        <country_areacode>+52</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>fm</country_id>
        <country_name>Micronesia Federated States Of </country_name>
        <country_areacode>+691</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>md</country_id>
        <country_name>Moldova </country_name>
        <country_areacode>+373</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>mc</country_id>
        <country_name>Monaco </country_name>
        <country_areacode>+377</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>mn</country_id>
        <country_name>Mongolia </country_name>
        <country_areacode>+976</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>me</country_id>
        <country_name>Montenegro </country_name>
        <country_areacode>+382</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ms</country_id>
        <country_name>Montserrat </country_name>
        <country_areacode>+166</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ma</country_id>
        <country_name>Morocco </country_name>
        <country_areacode>+212</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>mz</country_id>
        <country_name>Mozambique </country_name>
        <country_areacode>+258</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>mm</country_id>
        <country_name>Myanmar </country_name>
        <country_areacode>+95</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>na</country_id>
        <country_name>Namibia </country_name>
        <country_areacode>+264</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>nr</country_id>
        <country_name>Nauru </country_name>
        <country_areacode>+674</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>np</country_id>
        <country_name>Nepal </country_name>
        <country_areacode>+977</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>nl</country_id>
        <country_name>Netherlands </country_name>
        <country_areacode>+31</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>an</country_id>
        <country_name>Netherlands Antilles </country_name>
        <country_areacode>+599</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>nc</country_id>
        <country_name>New Caledonia </country_name>
        <country_areacode>+687</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>nz</country_id>
        <country_name>New Zealand </country_name>
        <country_areacode>+64</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ni</country_id>
        <country_name>Nicaragua </country_name>
        <country_areacode>+505</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ne</country_id>
        <country_name>Niger </country_name>
        <country_areacode>+227</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ng</country_id>
        <country_name>Nigeria </country_name>
        <country_areacode>+234</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>nu</country_id>
        <country_name>Niue </country_name>
        <country_areacode>+683</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>nf</country_id>
        <country_name>Norfolk Island </country_name>
        <country_areacode>+672</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>kp</country_id>
        <country_name>North Korea</country_name>
        <country_areacode>+850</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>mp</country_id>
        <country_name>Northern Mariana Islands </country_name>
        <country_areacode>+670</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>no</country_id>
        <country_name>Norway </country_name>
        <country_areacode>+47</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>om</country_id>
        <country_name>Oman </country_name>
        <country_areacode>+968</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>pk</country_id>
        <country_name>Pakistan </country_name>
        <country_areacode>+92</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>pw</country_id>
        <country_name>Palau </country_name>
        <country_areacode>+680</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ps</country_id>
        <country_name>Palestinian Territory Occupied </country_name>
        <country_areacode>+970</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>pa</country_id>
        <country_name>Panama </country_name>
        <country_areacode>+507</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>pg</country_id>
        <country_name>Papua New Guinea </country_name>
        <country_areacode>+675</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>py</country_id>
        <country_name>Paraguay </country_name>
        <country_areacode>+595</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>pe</country_id>
        <country_name>Peru </country_name>
        <country_areacode>+51</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ph</country_id>
        <country_name>Philippines </country_name>
        <country_areacode>+63</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>pn</country_id>
        <country_name>Pitcairn </country_name>
        <country_areacode>+870</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>pl</country_id>
        <country_name>Poland </country_name>
        <country_areacode>+48</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>pt</country_id>
        <country_name>Portugal </country_name>
        <country_areacode>+351</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>pr</country_id>
        <country_name>Puerto Rico </country_name>
        <country_areacode>+787</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>qa</country_id>
        <country_name>Qatar </country_name>
        <country_areacode>+974</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>re</country_id>
        <country_name>Runion </country_name>
        <country_areacode>+262</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ro</country_id>
        <country_name>Romania </country_name>
        <country_areacode>+40</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ru</country_id>
        <country_name>Russia</country_name>
        <country_areacode>+7</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>rw</country_id>
        <country_name>Rwanda </country_name>
        <country_areacode>+250</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>bl</country_id>
        <country_name>Saint Barthlemy </country_name>
        <country_areacode>+590</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>sh</country_id>
        <country_name>Saint Helena </country_name>
        <country_areacode>+290</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>kn</country_id>
        <country_name>Saint Kitts And Nevis </country_name>
        <country_areacode>+186</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>lc</country_id>
        <country_name>Saint Lucia </country_name>
        <country_areacode>+175</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>mf</country_id>
        <country_name>Saint Martin </country_name>
        <country_areacode>+159</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>pm</country_id>
        <country_name>Saint Pierre And Miquelon </country_name>
        <country_areacode>+508</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>vc</country_id>
        <country_name>Saint Vincent And The Grenadines </country_name>
        <country_areacode>+178</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ws</country_id>
        <country_name>Samoa </country_name>
        <country_areacode>+685</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>sm</country_id>
        <country_name>San Marino </country_name>
        <country_areacode>+378</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>st</country_id>
        <country_name>Sao Tome And Principe </country_name>
        <country_areacode>+239</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>sa</country_id>
        <country_name>Saudi Arabia </country_name>
        <country_areacode>+966</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>sn</country_id>
        <country_name>Senegal </country_name>
        <country_areacode>+221</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>rs</country_id>
        <country_name>Serbia </country_name>
        <country_areacode>+381</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>sc</country_id>
        <country_name>Seychelles </country_name>
        <country_areacode>+248</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>sl</country_id>
        <country_name>Sierra Leone </country_name>
        <country_areacode>+232</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>sg</country_id>
        <country_name>Singapore </country_name>
        <country_areacode>+65</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>sk</country_id>
        <country_name>Slovakia </country_name>
        <country_areacode>+421</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>si</country_id>
        <country_name>Slovenia </country_name>
        <country_areacode>+386</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>sb</country_id>
        <country_name>Solomon Islands </country_name>
        <country_areacode>+677</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>so</country_id>
        <country_name>Somalia </country_name>
        <country_areacode>+252</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>za</country_id>
        <country_name>South Africa </country_name>
        <country_areacode>+27</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>gs</country_id>
        <country_name>South Georgia And The South Sandwich Islands </country_name>
        <country_areacode>+500</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>kr</country_id>
        <country_name>South Korea</country_name>
        <country_areacode>+82</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>es</country_id>
        <country_name>Spain </country_name>
        <country_areacode>+34</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>lk</country_id>
        <country_name>Sri Lanka </country_name>
        <country_areacode>+94</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>sd</country_id>
        <country_name>Sudan </country_name>
        <country_areacode>+249</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>sr</country_id>
        <country_name>Suriname </country_name>
        <country_areacode>+597</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>sj</country_id>
        <country_name>Svalbard And Jan Mayen </country_name>
        <country_areacode>+47</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>sz</country_id>
        <country_name>Swaziland </country_name>
        <country_areacode>+268</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>se</country_id>
        <country_name>Sweden </country_name>
        <country_areacode>+46</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ch</country_id>
        <country_name>Switzerland </country_name>
        <country_areacode>+41</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>sy</country_id>
        <country_name>Syrian Arab Republic </country_name>
        <country_areacode>+963</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>tw</country_id>
        <country_name>Taiwan</country_name>
        <country_areacode>+886</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>tj</country_id>
        <country_name>Tajikistan </country_name>
        <country_areacode>+992</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>tz</country_id>
        <country_name>Tanzania</country_name>
        <country_areacode>+255</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>th</country_id>
        <country_name>Thailand </country_name>
        <country_areacode>+66</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>tl</country_id>
        <country_name>TimorLeste </country_name>
        <country_areacode>+670</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>tg</country_id>
        <country_name>Togo </country_name>
        <country_areacode>+228</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>tk</country_id>
        <country_name>Tokelau </country_name>
        <country_areacode>+690</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>to</country_id>
        <country_name>Tonga </country_name>
        <country_areacode>+676</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>tt</country_id>
        <country_name>Trinidad And Tobago </country_name>
        <country_areacode>+868</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>tn</country_id>
        <country_name>Tunisia </country_name>
        <country_areacode>+216</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>tr</country_id>
        <country_name>Turkey </country_name>
        <country_areacode>+90</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>tm</country_id>
        <country_name>Turkmenistan </country_name>
        <country_areacode>+993</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>tc</country_id>
        <country_name>Turks And Caicos Islands </country_name>
        <country_areacode>+649</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>tv</country_id>
        <country_name>Tuvalu </country_name>
        <country_areacode>+688</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ug</country_id>
        <country_name>Uganda </country_name>
        <country_areacode>+256</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ua</country_id>
        <country_name>Ukraine </country_name>
        <country_areacode>+380</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ae</country_id>
        <country_name>United Arab Emirates </country_name>
        <country_areacode>+971</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>gb</country_id>
        <country_name>United Kingdom </country_name>
        <country_areacode>+44</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>us</country_id>
        <country_name>United States </country_name>
        <country_areacode>+1</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>um</country_id>
        <country_name>United States Minor Outlying Islands </country_name>
        <country_areacode>+1</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>uy</country_id>
        <country_name>Uruguay </country_name>
        <country_areacode>+598</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>uz</country_id>
        <country_name>Uzbekistan </country_name>
        <country_areacode>+998</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>vu</country_id>
        <country_name>Vanuatu </country_name>
        <country_areacode>+678</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>va</country_id>
        <country_name>Vatican City State </country_name>
        <country_areacode>+379</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ve</country_id>
        <country_name>Venezuela </country_name>
        <country_areacode>+58</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>vn</country_id>
        <country_name>Vietnam </country_name>
        <country_areacode>+84</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>vg</country_id>
        <country_name>Virgin Islands British </country_name>
        <country_areacode>+128</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>vi</country_id>
        <country_name>Virgin Islands US </country_name>
        <country_areacode>+134</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>wf</country_id>
        <country_name>Wallis And Futuna </country_name>
        <country_areacode>+681</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>eh</country_id>
        <country_name>Western Sahara </country_name>
        <country_areacode>+212</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>ye</country_id>
        <country_name>Yemen </country_name>
        <country_areacode>+967</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>zm</country_id>
        <country_name>Zambia </country_name>
        <country_areacode>+260</country_areacode>
    </listCountry>
    <listCountry>
        <country_id>zw</country_id>
        <country_name>Zimbabwe</country_name>
        <country_areacode>+263</country_areacode>
    </listCountry>
    <login_status>false</login_status>
    <token>f9b29ac359ca5d77755e7588751c089bf96f0dc9</token>
</tiket>
```

```json
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.1179",
    "memoryusage": "5.21MB",
    "unix_timestamp": 1470211079,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "listCountry": [
    {
      "country_id": "af",
      "country_name": "Afghanistan ",
      "country_areacode": "+93"
    },
    {
      "country_id": "ax",
      "country_name": "land Islands ",
      "country_areacode": "+358"
    },
    {
      "country_id": "al",
      "country_name": "Albania ",
      "country_areacode": "+355"
    },
    {
      "country_id": "dz",
      "country_name": "Algeria ",
      "country_areacode": "+213"
    },
    {
      "country_id": "as",
      "country_name": "American Samoa ",
      "country_areacode": "+684"
    },
    {
      "country_id": "ad",
      "country_name": "Andorra ",
      "country_areacode": "+376"
    },
    {
      "country_id": "ao",
      "country_name": "Angola ",
      "country_areacode": "+244"
    },
    {
      "country_id": "ai",
      "country_name": "Anguilla ",
      "country_areacode": "+126"
    },
    {
      "country_id": "aq",
      "country_name": "Antarctica ",
      "country_areacode": "+672"
    },
    {
      "country_id": "ag",
      "country_name": "Antigua And Barbuda ",
      "country_areacode": "+126"
    },
    {
      "country_id": "ar",
      "country_name": "Argentina ",
      "country_areacode": "+54"
    },
    {
      "country_id": "am",
      "country_name": "Armenia ",
      "country_areacode": "+374"
    },
    {
      "country_id": "aw",
      "country_name": "Aruba ",
      "country_areacode": "+297"
    },
    {
      "country_id": "au",
      "country_name": "Australia ",
      "country_areacode": "+61"
    },
    {
      "country_id": "at",
      "country_name": "Austria ",
      "country_areacode": "+43"
    },
    {
      "country_id": "az",
      "country_name": "Azerbaijan ",
      "country_areacode": "+994"
    },
    {
      "country_id": "bs",
      "country_name": "Bahamas ",
      "country_areacode": "+124"
    },
    {
      "country_id": "bh",
      "country_name": "Bahrain ",
      "country_areacode": "+973"
    },
    {
      "country_id": "bd",
      "country_name": "Bangladesh ",
      "country_areacode": "+880"
    },
    {
      "country_id": "bb",
      "country_name": "Barbados ",
      "country_areacode": "+124"
    },
    {
      "country_id": "by",
      "country_name": "Belarus ",
      "country_areacode": "+375"
    },
    {
      "country_id": "be",
      "country_name": "Belgium ",
      "country_areacode": "+32"
    },
    {
      "country_id": "bz",
      "country_name": "Belize ",
      "country_areacode": "+501"
    },
    {
      "country_id": "bj",
      "country_name": "Benin ",
      "country_areacode": "+229"
    },
    {
      "country_id": "bm",
      "country_name": "Bermuda ",
      "country_areacode": "+144"
    },
    {
      "country_id": "bt",
      "country_name": "Bhutan ",
      "country_areacode": "+975"
    },
    {
      "country_id": "bo",
      "country_name": "Bolivia ",
      "country_areacode": "+591"
    },
    {
      "country_id": "ba",
      "country_name": "Bosnia And Herzegovina ",
      "country_areacode": "+387"
    },
    {
      "country_id": "bw",
      "country_name": "Botswana ",
      "country_areacode": "+267"
    },
    {
      "country_id": "bv",
      "country_name": "Bouvet Island ",
      "country_areacode": "+47"
    },
    {
      "country_id": "br",
      "country_name": "Brazil ",
      "country_areacode": "+55"
    },
    {
      "country_id": "io",
      "country_name": "British Indian Ocean Territory ",
      "country_areacode": "+246"
    },
    {
      "country_id": "bn",
      "country_name": "Brunei Darussalam ",
      "country_areacode": "+673"
    },
    {
      "country_id": "bg",
      "country_name": "Bulgaria ",
      "country_areacode": "+359"
    },
    {
      "country_id": "bf",
      "country_name": "Burkina Faso ",
      "country_areacode": "+226"
    },
    {
      "country_id": "bi",
      "country_name": "Burundi ",
      "country_areacode": "+257"
    },
    {
      "country_id": "kh",
      "country_name": "Cambodia ",
      "country_areacode": "+855"
    },
    {
      "country_id": "cm",
      "country_name": "Cameroon ",
      "country_areacode": "+237"
    },
    {
      "country_id": "ca",
      "country_name": "Canada ",
      "country_areacode": "+1"
    },
    {
      "country_id": "cv",
      "country_name": "Cape Verde ",
      "country_areacode": "+238"
    },
    {
      "country_id": "ky",
      "country_name": "Cayman Islands ",
      "country_areacode": "+345"
    },
    {
      "country_id": "cf",
      "country_name": "Central African Republic ",
      "country_areacode": "+236"
    },
    {
      "country_id": "td",
      "country_name": "Chad ",
      "country_areacode": "+235"
    },
    {
      "country_id": "cl",
      "country_name": "Chile ",
      "country_areacode": "+56"
    },
    {
      "country_id": "cn",
      "country_name": "China ",
      "country_areacode": "+86"
    },
    {
      "country_id": "cx",
      "country_name": "Christmas Island ",
      "country_areacode": "+61"
    },
    {
      "country_id": "cc",
      "country_name": "Cocos Keeling Islands ",
      "country_areacode": "+61"
    },
    {
      "country_id": "co",
      "country_name": "Colombia ",
      "country_areacode": "+57"
    },
    {
      "country_id": "km",
      "country_name": "Comoros ",
      "country_areacode": "+269"
    },
    {
      "country_id": "cg",
      "country_name": "Congo ",
      "country_areacode": "+242"
    },
    {
      "country_id": "cd",
      "country_name": "Congo The Democratic Republic Of The ",
      "country_areacode": "+243"
    },
    {
      "country_id": "ck",
      "country_name": "Cook Islands ",
      "country_areacode": "+682"
    },
    {
      "country_id": "cr",
      "country_name": "Costa Rica ",
      "country_areacode": "+506"
    },
    {
      "country_id": "ci",
      "country_name": "Cte DIvoire ",
      "country_areacode": "+225"
    },
    {
      "country_id": "hr",
      "country_name": "Croatia ",
      "country_areacode": "+385"
    },
    {
      "country_id": "cu",
      "country_name": "Cuba ",
      "country_areacode": "+53"
    },
    {
      "country_id": "cy",
      "country_name": "Cyprus ",
      "country_areacode": "+357"
    },
    {
      "country_id": "cz",
      "country_name": "Czech Republic ",
      "country_areacode": "+420"
    },
    {
      "country_id": "dk",
      "country_name": "Denmark ",
      "country_areacode": "+45"
    },
    {
      "country_id": "dj",
      "country_name": "Djibouti ",
      "country_areacode": "+253"
    },
    {
      "country_id": "dm",
      "country_name": "Dominica ",
      "country_areacode": "+767"
    },
    {
      "country_id": "do",
      "country_name": "Dominican Republic ",
      "country_areacode": "+809"
    },
    {
      "country_id": "ec",
      "country_name": "Ecuador ",
      "country_areacode": "+593"
    },
    {
      "country_id": "eg",
      "country_name": "Egypt",
      "country_areacode": "+20"
    },
    {
      "country_id": "sv",
      "country_name": "El Salvador ",
      "country_areacode": "+503"
    },
    {
      "country_id": "gq",
      "country_name": "Equatorial Guinea ",
      "country_areacode": "+240"
    },
    {
      "country_id": "er",
      "country_name": "Eritrea ",
      "country_areacode": "+291"
    },
    {
      "country_id": "ee",
      "country_name": "Estonia ",
      "country_areacode": "+372"
    },
    {
      "country_id": "et",
      "country_name": "Ethiopia ",
      "country_areacode": "+251"
    },
    {
      "country_id": "fk",
      "country_name": "Falkland Islands Malvinas ",
      "country_areacode": "+500"
    },
    {
      "country_id": "fo",
      "country_name": "Faroe Islands ",
      "country_areacode": "+298"
    },
    {
      "country_id": "fj",
      "country_name": "Fiji ",
      "country_areacode": "+679"
    },
    {
      "country_id": "fi",
      "country_name": "Finland ",
      "country_areacode": "+358"
    },
    {
      "country_id": "fr",
      "country_name": "France ",
      "country_areacode": "+33"
    },
    {
      "country_id": "gf",
      "country_name": "French Guiana ",
      "country_areacode": "+594"
    },
    {
      "country_id": "pf",
      "country_name": "French Polynesia ",
      "country_areacode": "+689"
    },
    {
      "country_id": "tf",
      "country_name": "French Southern Territories ",
      "country_areacode": "+596"
    },
    {
      "country_id": "ga",
      "country_name": "Gabon ",
      "country_areacode": "+241"
    },
    {
      "country_id": "gm",
      "country_name": "Gambia ",
      "country_areacode": "+220"
    },
    {
      "country_id": "ge",
      "country_name": "Georgia ",
      "country_areacode": "+995"
    },
    {
      "country_id": "de",
      "country_name": "Germany ",
      "country_areacode": "+49"
    },
    {
      "country_id": "gh",
      "country_name": "Ghana ",
      "country_areacode": "+233"
    },
    {
      "country_id": "gi",
      "country_name": "Gibraltar ",
      "country_areacode": "+350"
    },
    {
      "country_id": "gr",
      "country_name": "Greece ",
      "country_areacode": "+30"
    },
    {
      "country_id": "gl",
      "country_name": "Greenland ",
      "country_areacode": "+299"
    },
    {
      "country_id": "gd",
      "country_name": "Grenada ",
      "country_areacode": "+147"
    },
    {
      "country_id": "gp",
      "country_name": "Guadeloupe ",
      "country_areacode": "+590"
    },
    {
      "country_id": "gu",
      "country_name": "Guam ",
      "country_areacode": "+167"
    },
    {
      "country_id": "gt",
      "country_name": "Guatemala ",
      "country_areacode": "+502"
    },
    {
      "country_id": "gg",
      "country_name": "Guernsey ",
      "country_areacode": "+44"
    },
    {
      "country_id": "gn",
      "country_name": "Guinea ",
      "country_areacode": "+224"
    },
    {
      "country_id": "gw",
      "country_name": "GuineaBissau ",
      "country_areacode": "+245"
    },
    {
      "country_id": "gy",
      "country_name": "Guyana ",
      "country_areacode": "+592"
    },
    {
      "country_id": "ht",
      "country_name": "Haiti ",
      "country_areacode": "+509"
    },
    {
      "country_id": "hm",
      "country_name": "Heard Island And Mcdonald Islands ",
      "country_areacode": "+672"
    },
    {
      "country_id": "hn",
      "country_name": "Honduras ",
      "country_areacode": "+504"
    },
    {
      "country_id": "hk",
      "country_name": "Hong Kong ",
      "country_areacode": "+852"
    },
    {
      "country_id": "hu",
      "country_name": "Hungary ",
      "country_areacode": "+36"
    },
    {
      "country_id": "is",
      "country_name": "Iceland ",
      "country_areacode": "+354"
    },
    {
      "country_id": "in",
      "country_name": "India ",
      "country_areacode": "+91"
    },
    {
      "country_id": "id",
      "country_name": "Indonesia",
      "country_areacode": "+62"
    },
    {
      "country_id": "ir",
      "country_name": "Iran Islamic Republic Of ",
      "country_areacode": "+98"
    },
    {
      "country_id": "iq",
      "country_name": "Iraq ",
      "country_areacode": "+964"
    },
    {
      "country_id": "ie",
      "country_name": "Ireland ",
      "country_areacode": "+353"
    },
    {
      "country_id": "im",
      "country_name": "Isle Of Man ",
      "country_areacode": "+44"
    },
    {
      "country_id": "il",
      "country_name": "Israel ",
      "country_areacode": "+972"
    },
    {
      "country_id": "it",
      "country_name": "Italy ",
      "country_areacode": "+39"
    },
    {
      "country_id": "jm",
      "country_name": "Jamaica ",
      "country_areacode": "+876"
    },
    {
      "country_id": "jp",
      "country_name": "Japan ",
      "country_areacode": "+81"
    },
    {
      "country_id": "je",
      "country_name": "Jersey ",
      "country_areacode": "+44"
    },
    {
      "country_id": "jo",
      "country_name": "Jordan ",
      "country_areacode": "+962"
    },
    {
      "country_id": "kz",
      "country_name": "Kazakhstan ",
      "country_areacode": "+7"
    },
    {
      "country_id": "ke",
      "country_name": "Kenya ",
      "country_areacode": "+254"
    },
    {
      "country_id": "ki",
      "country_name": "Kiribati ",
      "country_areacode": "+686"
    },
    {
      "country_id": "kw",
      "country_name": "Kuwait ",
      "country_areacode": "+965"
    },
    {
      "country_id": "kg",
      "country_name": "Kyrgyzstan ",
      "country_areacode": "+996"
    },
    {
      "country_id": "la",
      "country_name": "Laos",
      "country_areacode": "+856"
    },
    {
      "country_id": "lv",
      "country_name": "Latvia ",
      "country_areacode": "+371"
    },
    {
      "country_id": "lb",
      "country_name": "Lebanon ",
      "country_areacode": "+961"
    },
    {
      "country_id": "ls",
      "country_name": "Lesotho ",
      "country_areacode": "+266"
    },
    {
      "country_id": "lr",
      "country_name": "Liberia ",
      "country_areacode": "+231"
    },
    {
      "country_id": "ly",
      "country_name": "Libyan Arab Jamahiriya ",
      "country_areacode": "+218"
    },
    {
      "country_id": "li",
      "country_name": "Liechtenstein ",
      "country_areacode": "+423"
    },
    {
      "country_id": "lt",
      "country_name": "Lithuania ",
      "country_areacode": "+370"
    },
    {
      "country_id": "lu",
      "country_name": "Luxembourg ",
      "country_areacode": "+352"
    },
    {
      "country_id": "mo",
      "country_name": "Macau ",
      "country_areacode": "+853"
    },
    {
      "country_id": "mk",
      "country_name": "Macedonia The Former Yugoslav Republic Of ",
      "country_areacode": "+389"
    },
    {
      "country_id": "mg",
      "country_name": "Madagascar ",
      "country_areacode": "+261"
    },
    {
      "country_id": "mw",
      "country_name": "Malawi ",
      "country_areacode": "+265"
    },
    {
      "country_id": "my",
      "country_name": "Malaysia ",
      "country_areacode": "+60"
    },
    {
      "country_id": "mv",
      "country_name": "Maldives ",
      "country_areacode": "+960"
    },
    {
      "country_id": "ml",
      "country_name": "Mali ",
      "country_areacode": "+223"
    },
    {
      "country_id": "mt",
      "country_name": "Malta ",
      "country_areacode": "+356"
    },
    {
      "country_id": "mh",
      "country_name": "Marshall Islands ",
      "country_areacode": "+692"
    },
    {
      "country_id": "mq",
      "country_name": "Martinique ",
      "country_areacode": "+596"
    },
    {
      "country_id": "mr",
      "country_name": "Mauritania ",
      "country_areacode": "+222"
    },
    {
      "country_id": "mu",
      "country_name": "Mauritius ",
      "country_areacode": "+230"
    },
    {
      "country_id": "yt",
      "country_name": "Mayotte ",
      "country_areacode": "+269"
    },
    {
      "country_id": "mx",
      "country_name": "Mexico ",
      "country_areacode": "+52"
    },
    {
      "country_id": "fm",
      "country_name": "Micronesia Federated States Of ",
      "country_areacode": "+691"
    },
    {
      "country_id": "md",
      "country_name": "Moldova ",
      "country_areacode": "+373"
    },
    {
      "country_id": "mc",
      "country_name": "Monaco ",
      "country_areacode": "+377"
    },
    {
      "country_id": "mn",
      "country_name": "Mongolia ",
      "country_areacode": "+976"
    },
    {
      "country_id": "me",
      "country_name": "Montenegro ",
      "country_areacode": "+382"
    },
    {
      "country_id": "ms",
      "country_name": "Montserrat ",
      "country_areacode": "+166"
    },
    {
      "country_id": "ma",
      "country_name": "Morocco ",
      "country_areacode": "+212"
    },
    {
      "country_id": "mz",
      "country_name": "Mozambique ",
      "country_areacode": "+258"
    },
    {
      "country_id": "mm",
      "country_name": "Myanmar ",
      "country_areacode": "+95"
    },
    {
      "country_id": "na",
      "country_name": "Namibia ",
      "country_areacode": "+264"
    },
    {
      "country_id": "nr",
      "country_name": "Nauru ",
      "country_areacode": "+674"
    },
    {
      "country_id": "np",
      "country_name": "Nepal ",
      "country_areacode": "+977"
    },
    {
      "country_id": "nl",
      "country_name": "Netherlands ",
      "country_areacode": "+31"
    },
    {
      "country_id": "an",
      "country_name": "Netherlands Antilles ",
      "country_areacode": "+599"
    },
    {
      "country_id": "nc",
      "country_name": "New Caledonia ",
      "country_areacode": "+687"
    },
    {
      "country_id": "nz",
      "country_name": "New Zealand ",
      "country_areacode": "+64"
    },
    {
      "country_id": "ni",
      "country_name": "Nicaragua ",
      "country_areacode": "+505"
    },
    {
      "country_id": "ne",
      "country_name": "Niger ",
      "country_areacode": "+227"
    },
    {
      "country_id": "ng",
      "country_name": "Nigeria ",
      "country_areacode": "+234"
    },
    {
      "country_id": "nu",
      "country_name": "Niue ",
      "country_areacode": "+683"
    },
    {
      "country_id": "nf",
      "country_name": "Norfolk Island ",
      "country_areacode": "+672"
    },
    {
      "country_id": "kp",
      "country_name": "North Korea",
      "country_areacode": "+850"
    },
    {
      "country_id": "mp",
      "country_name": "Northern Mariana Islands ",
      "country_areacode": "+670"
    },
    {
      "country_id": "no",
      "country_name": "Norway ",
      "country_areacode": "+47"
    },
    {
      "country_id": "om",
      "country_name": "Oman ",
      "country_areacode": "+968"
    },
    {
      "country_id": "pk",
      "country_name": "Pakistan ",
      "country_areacode": "+92"
    },
    {
      "country_id": "pw",
      "country_name": "Palau ",
      "country_areacode": "+680"
    },
    {
      "country_id": "ps",
      "country_name": "Palestinian Territory Occupied ",
      "country_areacode": "+970"
    },
    {
      "country_id": "pa",
      "country_name": "Panama ",
      "country_areacode": "+507"
    },
    {
      "country_id": "pg",
      "country_name": "Papua New Guinea ",
      "country_areacode": "+675"
    },
    {
      "country_id": "py",
      "country_name": "Paraguay ",
      "country_areacode": "+595"
    },
    {
      "country_id": "pe",
      "country_name": "Peru ",
      "country_areacode": "+51"
    },
    {
      "country_id": "ph",
      "country_name": "Philippines ",
      "country_areacode": "+63"
    },
    {
      "country_id": "pn",
      "country_name": "Pitcairn ",
      "country_areacode": "+870"
    },
    {
      "country_id": "pl",
      "country_name": "Poland ",
      "country_areacode": "+48"
    },
    {
      "country_id": "pt",
      "country_name": "Portugal ",
      "country_areacode": "+351"
    },
    {
      "country_id": "pr",
      "country_name": "Puerto Rico ",
      "country_areacode": "+787"
    },
    {
      "country_id": "qa",
      "country_name": "Qatar ",
      "country_areacode": "+974"
    },
    {
      "country_id": "re",
      "country_name": "Runion ",
      "country_areacode": "+262"
    },
    {
      "country_id": "ro",
      "country_name": "Romania ",
      "country_areacode": "+40"
    },
    {
      "country_id": "ru",
      "country_name": "Russia",
      "country_areacode": "+7"
    },
    {
      "country_id": "rw",
      "country_name": "Rwanda ",
      "country_areacode": "+250"
    },
    {
      "country_id": "bl",
      "country_name": "Saint Barthlemy ",
      "country_areacode": "+590"
    },
    {
      "country_id": "sh",
      "country_name": "Saint Helena ",
      "country_areacode": "+290"
    },
    {
      "country_id": "kn",
      "country_name": "Saint Kitts And Nevis ",
      "country_areacode": "+186"
    },
    {
      "country_id": "lc",
      "country_name": "Saint Lucia ",
      "country_areacode": "+175"
    },
    {
      "country_id": "mf",
      "country_name": "Saint Martin ",
      "country_areacode": "+159"
    },
    {
      "country_id": "pm",
      "country_name": "Saint Pierre And Miquelon ",
      "country_areacode": "+508"
    },
    {
      "country_id": "vc",
      "country_name": "Saint Vincent And The Grenadines ",
      "country_areacode": "+178"
    },
    {
      "country_id": "ws",
      "country_name": "Samoa ",
      "country_areacode": "+685"
    },
    {
      "country_id": "sm",
      "country_name": "San Marino ",
      "country_areacode": "+378"
    },
    {
      "country_id": "st",
      "country_name": "Sao Tome And Principe ",
      "country_areacode": "+239"
    },
    {
      "country_id": "sa",
      "country_name": "Saudi Arabia ",
      "country_areacode": "+966"
    },
    {
      "country_id": "sn",
      "country_name": "Senegal ",
      "country_areacode": "+221"
    },
    {
      "country_id": "rs",
      "country_name": "Serbia ",
      "country_areacode": "+381"
    },
    {
      "country_id": "sc",
      "country_name": "Seychelles ",
      "country_areacode": "+248"
    },
    {
      "country_id": "sl",
      "country_name": "Sierra Leone ",
      "country_areacode": "+232"
    },
    {
      "country_id": "sg",
      "country_name": "Singapore ",
      "country_areacode": "+65"
    },
    {
      "country_id": "sk",
      "country_name": "Slovakia ",
      "country_areacode": "+421"
    },
    {
      "country_id": "si",
      "country_name": "Slovenia ",
      "country_areacode": "+386"
    },
    {
      "country_id": "sb",
      "country_name": "Solomon Islands ",
      "country_areacode": "+677"
    },
    {
      "country_id": "so",
      "country_name": "Somalia ",
      "country_areacode": "+252"
    },
    {
      "country_id": "za",
      "country_name": "South Africa ",
      "country_areacode": "+27"
    },
    {
      "country_id": "gs",
      "country_name": "South Georgia And The South Sandwich Islands ",
      "country_areacode": "+500"
    },
    {
      "country_id": "kr",
      "country_name": "South Korea",
      "country_areacode": "+82"
    },
    {
      "country_id": "es",
      "country_name": "Spain ",
      "country_areacode": "+34"
    },
    {
      "country_id": "lk",
      "country_name": "Sri Lanka ",
      "country_areacode": "+94"
    },
    {
      "country_id": "sd",
      "country_name": "Sudan ",
      "country_areacode": "+249"
    },
    {
      "country_id": "sr",
      "country_name": "Suriname ",
      "country_areacode": "+597"
    },
    {
      "country_id": "sj",
      "country_name": "Svalbard And Jan Mayen ",
      "country_areacode": "+47"
    },
    {
      "country_id": "sz",
      "country_name": "Swaziland ",
      "country_areacode": "+268"
    },
    {
      "country_id": "se",
      "country_name": "Sweden ",
      "country_areacode": "+46"
    },
    {
      "country_id": "ch",
      "country_name": "Switzerland ",
      "country_areacode": "+41"
    },
    {
      "country_id": "sy",
      "country_name": "Syrian Arab Republic ",
      "country_areacode": "+963"
    },
    {
      "country_id": "tw",
      "country_name": "Taiwan",
      "country_areacode": "+886"
    },
    {
      "country_id": "tj",
      "country_name": "Tajikistan ",
      "country_areacode": "+992"
    },
    {
      "country_id": "tz",
      "country_name": "Tanzania",
      "country_areacode": "+255"
    },
    {
      "country_id": "th",
      "country_name": "Thailand ",
      "country_areacode": "+66"
    },
    {
      "country_id": "tl",
      "country_name": "TimorLeste ",
      "country_areacode": "+670"
    },
    {
      "country_id": "tg",
      "country_name": "Togo ",
      "country_areacode": "+228"
    },
    {
      "country_id": "tk",
      "country_name": "Tokelau ",
      "country_areacode": "+690"
    },
    {
      "country_id": "to",
      "country_name": "Tonga ",
      "country_areacode": "+676"
    },
    {
      "country_id": "tt",
      "country_name": "Trinidad And Tobago ",
      "country_areacode": "+868"
    },
    {
      "country_id": "tn",
      "country_name": "Tunisia ",
      "country_areacode": "+216"
    },
    {
      "country_id": "tr",
      "country_name": "Turkey ",
      "country_areacode": "+90"
    },
    {
      "country_id": "tm",
      "country_name": "Turkmenistan ",
      "country_areacode": "+993"
    },
    {
      "country_id": "tc",
      "country_name": "Turks And Caicos Islands ",
      "country_areacode": "+649"
    },
    {
      "country_id": "tv",
      "country_name": "Tuvalu ",
      "country_areacode": "+688"
    },
    {
      "country_id": "ug",
      "country_name": "Uganda ",
      "country_areacode": "+256"
    },
    {
      "country_id": "ua",
      "country_name": "Ukraine ",
      "country_areacode": "+380"
    },
    {
      "country_id": "ae",
      "country_name": "United Arab Emirates ",
      "country_areacode": "+971"
    },
    {
      "country_id": "gb",
      "country_name": "United Kingdom ",
      "country_areacode": "+44"
    },
    {
      "country_id": "us",
      "country_name": "United States ",
      "country_areacode": "+1"
    },
    {
      "country_id": "um",
      "country_name": "United States Minor Outlying Islands ",
      "country_areacode": "+1"
    },
    {
      "country_id": "uy",
      "country_name": "Uruguay ",
      "country_areacode": "+598"
    },
    {
      "country_id": "uz",
      "country_name": "Uzbekistan ",
      "country_areacode": "+998"
    },
    {
      "country_id": "vu",
      "country_name": "Vanuatu ",
      "country_areacode": "+678"
    },
    {
      "country_id": "va",
      "country_name": "Vatican City State ",
      "country_areacode": "+379"
    },
    {
      "country_id": "ve",
      "country_name": "Venezuela ",
      "country_areacode": "+58"
    },
    {
      "country_id": "vn",
      "country_name": "Vietnam ",
      "country_areacode": "+84"
    },
    {
      "country_id": "vg",
      "country_name": "Virgin Islands British ",
      "country_areacode": "+128"
    },
    {
      "country_id": "vi",
      "country_name": "Virgin Islands US ",
      "country_areacode": "+134"
    },
    {
      "country_id": "wf",
      "country_name": "Wallis And Futuna ",
      "country_areacode": "+681"
    },
    {
      "country_id": "eh",
      "country_name": "Western Sahara ",
      "country_areacode": "+212"
    },
    {
      "country_id": "ye",
      "country_name": "Yemen ",
      "country_areacode": "+967"
    },
    {
      "country_id": "zm",
      "country_name": "Zambia ",
      "country_areacode": "+260"
    },
    {
      "country_id": "zw",
      "country_name": "Zimbabwe",
      "country_areacode": "+263"
    }
  ],
  "login_status": "false",
  "token": "f9b29ac359ca5d77755e7588751c089bf96f0dc9"
}
```

```matlab
a:5:{s:10:"diagnostic";a:7:{s:6:"status";i:200;s:10:"elapsetime";s:14:"0.0854";s:11:"memoryusage";s:14:"5.22MB";s:14:"unix_timestamp";i:1470211117;s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:11:"output_type";s:9:"serialize";s:11:"listCountry";a:246:{i:0;a:3:{s:10:"country_id";s:2:"af";s:12:"country_name";s:12:"Afghanistan ";s:16:"country_areacode";s:3:"+93";}i:1;a:3:{s:10:"country_id";s:2:"ax";s:12:"country_name";s:13:"land Islands ";s:16:"country_areacode";s:4:"+358";}i:2;a:3:{s:10:"country_id";s:2:"al";s:12:"country_name";s:8:"Albania ";s:16:"country_areacode";s:4:"+355";}i:3;a:3:{s:10:"country_id";s:2:"dz";s:12:"country_name";s:8:"Algeria ";s:16:"country_areacode";s:4:"+213";}i:4;a:3:{s:10:"country_id";s:2:"as";s:12:"country_name";s:15:"American Samoa ";s:16:"country_areacode";s:4:"+684";}i:5;a:3:{s:10:"country_id";s:2:"ad";s:12:"country_name";s:8:"Andorra ";s:16:"country_areacode";s:4:"+376";}i:6;a:3:{s:10:"country_id";s:2:"ao";s:12:"country_name";s:7:"Angola ";s:16:"country_areacode";s:4:"+244";}i:7;a:3:{s:10:"country_id";s:2:"ai";s:12:"country_name";s:9:"Anguilla ";s:16:"country_areacode";s:4:"+126";}i:8;a:3:{s:10:"country_id";s:2:"aq";s:12:"country_name";s:11:"Antarctica ";s:16:"country_areacode";s:4:"+672";}i:9;a:3:{s:10:"country_id";s:2:"ag";s:12:"country_name";s:20:"Antigua And Barbuda ";s:16:"country_areacode";s:4:"+126";}i:10;a:3:{s:10:"country_id";s:2:"ar";s:12:"country_name";s:10:"Argentina ";s:16:"country_areacode";s:3:"+54";}i:11;a:3:{s:10:"country_id";s:2:"am";s:12:"country_name";s:8:"Armenia ";s:16:"country_areacode";s:4:"+374";}i:12;a:3:{s:10:"country_id";s:2:"aw";s:12:"country_name";s:6:"Aruba ";s:16:"country_areacode";s:4:"+297";}i:13;a:3:{s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";s:16:"country_areacode";s:3:"+61";}i:14;a:3:{s:10:"country_id";s:2:"at";s:12:"country_name";s:8:"Austria ";s:16:"country_areacode";s:3:"+43";}i:15;a:3:{s:10:"country_id";s:2:"az";s:12:"country_name";s:11:"Azerbaijan ";s:16:"country_areacode";s:4:"+994";}i:16;a:3:{s:10:"country_id";s:2:"bs";s:12:"country_name";s:8:"Bahamas ";s:16:"country_areacode";s:4:"+124";}i:17;a:3:{s:10:"country_id";s:2:"bh";s:12:"country_name";s:8:"Bahrain ";s:16:"country_areacode";s:4:"+973";}i:18;a:3:{s:10:"country_id";s:2:"bd";s:12:"country_name";s:11:"Bangladesh ";s:16:"country_areacode";s:4:"+880";}i:19;a:3:{s:10:"country_id";s:2:"bb";s:12:"country_name";s:9:"Barbados ";s:16:"country_areacode";s:4:"+124";}i:20;a:3:{s:10:"country_id";s:2:"by";s:12:"country_name";s:8:"Belarus ";s:16:"country_areacode";s:4:"+375";}i:21;a:3:{s:10:"country_id";s:2:"be";s:12:"country_name";s:8:"Belgium ";s:16:"country_areacode";s:3:"+32";}i:22;a:3:{s:10:"country_id";s:2:"bz";s:12:"country_name";s:7:"Belize ";s:16:"country_areacode";s:4:"+501";}i:23;a:3:{s:10:"country_id";s:2:"bj";s:12:"country_name";s:6:"Benin ";s:16:"country_areacode";s:4:"+229";}i:24;a:3:{s:10:"country_id";s:2:"bm";s:12:"country_name";s:8:"Bermuda ";s:16:"country_areacode";s:4:"+144";}i:25;a:3:{s:10:"country_id";s:2:"bt";s:12:"country_name";s:7:"Bhutan ";s:16:"country_areacode";s:4:"+975";}i:26;a:3:{s:10:"country_id";s:2:"bo";s:12:"country_name";s:8:"Bolivia ";s:16:"country_areacode";s:4:"+591";}i:27;a:3:{s:10:"country_id";s:2:"ba";s:12:"country_name";s:23:"Bosnia And Herzegovina ";s:16:"country_areacode";s:4:"+387";}i:28;a:3:{s:10:"country_id";s:2:"bw";s:12:"country_name";s:9:"Botswana ";s:16:"country_areacode";s:4:"+267";}i:29;a:3:{s:10:"country_id";s:2:"bv";s:12:"country_name";s:14:"Bouvet Island ";s:16:"country_areacode";s:3:"+47";}i:30;a:3:{s:10:"country_id";s:2:"br";s:12:"country_name";s:7:"Brazil ";s:16:"country_areacode";s:3:"+55";}i:31;a:3:{s:10:"country_id";s:2:"io";s:12:"country_name";s:31:"British Indian Ocean Territory ";s:16:"country_areacode";s:4:"+246";}i:32;a:3:{s:10:"country_id";s:2:"bn";s:12:"country_name";s:18:"Brunei Darussalam ";s:16:"country_areacode";s:4:"+673";}i:33;a:3:{s:10:"country_id";s:2:"bg";s:12:"country_name";s:9:"Bulgaria ";s:16:"country_areacode";s:4:"+359";}i:34;a:3:{s:10:"country_id";s:2:"bf";s:12:"country_name";s:13:"Burkina Faso ";s:16:"country_areacode";s:4:"+226";}i:35;a:3:{s:10:"country_id";s:2:"bi";s:12:"country_name";s:8:"Burundi ";s:16:"country_areacode";s:4:"+257";}i:36;a:3:{s:10:"country_id";s:2:"kh";s:12:"country_name";s:9:"Cambodia ";s:16:"country_areacode";s:4:"+855";}i:37;a:3:{s:10:"country_id";s:2:"cm";s:12:"country_name";s:9:"Cameroon ";s:16:"country_areacode";s:4:"+237";}i:38;a:3:{s:10:"country_id";s:2:"ca";s:12:"country_name";s:7:"Canada ";s:16:"country_areacode";s:2:"+1";}i:39;a:3:{s:10:"country_id";s:2:"cv";s:12:"country_name";s:11:"Cape Verde ";s:16:"country_areacode";s:4:"+238";}i:40;a:3:{s:10:"country_id";s:2:"ky";s:12:"country_name";s:15:"Cayman Islands ";s:16:"country_areacode";s:4:"+345";}i:41;a:3:{s:10:"country_id";s:2:"cf";s:12:"country_name";s:25:"Central African Republic ";s:16:"country_areacode";s:4:"+236";}i:42;a:3:{s:10:"country_id";s:2:"td";s:12:"country_name";s:5:"Chad ";s:16:"country_areacode";s:4:"+235";}i:43;a:3:{s:10:"country_id";s:2:"cl";s:12:"country_name";s:6:"Chile ";s:16:"country_areacode";s:3:"+56";}i:44;a:3:{s:10:"country_id";s:2:"cn";s:12:"country_name";s:6:"China ";s:16:"country_areacode";s:3:"+86";}i:45;a:3:{s:10:"country_id";s:2:"cx";s:12:"country_name";s:17:"Christmas Island ";s:16:"country_areacode";s:3:"+61";}i:46;a:3:{s:10:"country_id";s:2:"cc";s:12:"country_name";s:22:"Cocos Keeling Islands ";s:16:"country_areacode";s:3:"+61";}i:47;a:3:{s:10:"country_id";s:2:"co";s:12:"country_name";s:9:"Colombia ";s:16:"country_areacode";s:3:"+57";}i:48;a:3:{s:10:"country_id";s:2:"km";s:12:"country_name";s:8:"Comoros ";s:16:"country_areacode";s:4:"+269";}i:49;a:3:{s:10:"country_id";s:2:"cg";s:12:"country_name";s:6:"Congo ";s:16:"country_areacode";s:4:"+242";}i:50;a:3:{s:10:"country_id";s:2:"cd";s:12:"country_name";s:37:"Congo The Democratic Republic Of The ";s:16:"country_areacode";s:4:"+243";}i:51;a:3:{s:10:"country_id";s:2:"ck";s:12:"country_name";s:13:"Cook Islands ";s:16:"country_areacode";s:4:"+682";}i:52;a:3:{s:10:"country_id";s:2:"cr";s:12:"country_name";s:11:"Costa Rica ";s:16:"country_areacode";s:4:"+506";}i:53;a:3:{s:10:"country_id";s:2:"ci";s:12:"country_name";s:12:"Cte DIvoire ";s:16:"country_areacode";s:4:"+225";}i:54;a:3:{s:10:"country_id";s:2:"hr";s:12:"country_name";s:8:"Croatia ";s:16:"country_areacode";s:4:"+385";}i:55;a:3:{s:10:"country_id";s:2:"cu";s:12:"country_name";s:5:"Cuba ";s:16:"country_areacode";s:3:"+53";}i:56;a:3:{s:10:"country_id";s:2:"cy";s:12:"country_name";s:7:"Cyprus ";s:16:"country_areacode";s:4:"+357";}i:57;a:3:{s:10:"country_id";s:2:"cz";s:12:"country_name";s:15:"Czech Republic ";s:16:"country_areacode";s:4:"+420";}i:58;a:3:{s:10:"country_id";s:2:"dk";s:12:"country_name";s:8:"Denmark ";s:16:"country_areacode";s:3:"+45";}i:59;a:3:{s:10:"country_id";s:2:"dj";s:12:"country_name";s:9:"Djibouti ";s:16:"country_areacode";s:4:"+253";}i:60;a:3:{s:10:"country_id";s:2:"dm";s:12:"country_name";s:9:"Dominica ";s:16:"country_areacode";s:4:"+767";}i:61;a:3:{s:10:"country_id";s:2:"do";s:12:"country_name";s:19:"Dominican Republic ";s:16:"country_areacode";s:4:"+809";}i:62;a:3:{s:10:"country_id";s:2:"ec";s:12:"country_name";s:8:"Ecuador ";s:16:"country_areacode";s:4:"+593";}i:63;a:3:{s:10:"country_id";s:2:"eg";s:12:"country_name";s:5:"Egypt";s:16:"country_areacode";s:3:"+20";}i:64;a:3:{s:10:"country_id";s:2:"sv";s:12:"country_name";s:12:"El Salvador ";s:16:"country_areacode";s:4:"+503";}i:65;a:3:{s:10:"country_id";s:2:"gq";s:12:"country_name";s:18:"Equatorial Guinea ";s:16:"country_areacode";s:4:"+240";}i:66;a:3:{s:10:"country_id";s:2:"er";s:12:"country_name";s:8:"Eritrea ";s:16:"country_areacode";s:4:"+291";}i:67;a:3:{s:10:"country_id";s:2:"ee";s:12:"country_name";s:8:"Estonia ";s:16:"country_areacode";s:4:"+372";}i:68;a:3:{s:10:"country_id";s:2:"et";s:12:"country_name";s:9:"Ethiopia ";s:16:"country_areacode";s:4:"+251";}i:69;a:3:{s:10:"country_id";s:2:"fk";s:12:"country_name";s:26:"Falkland Islands Malvinas ";s:16:"country_areacode";s:4:"+500";}i:70;a:3:{s:10:"country_id";s:2:"fo";s:12:"country_name";s:14:"Faroe Islands ";s:16:"country_areacode";s:4:"+298";}i:71;a:3:{s:10:"country_id";s:2:"fj";s:12:"country_name";s:5:"Fiji ";s:16:"country_areacode";s:4:"+679";}i:72;a:3:{s:10:"country_id";s:2:"fi";s:12:"country_name";s:8:"Finland ";s:16:"country_areacode";s:4:"+358";}i:73;a:3:{s:10:"country_id";s:2:"fr";s:12:"country_name";s:7:"France ";s:16:"country_areacode";s:3:"+33";}i:74;a:3:{s:10:"country_id";s:2:"gf";s:12:"country_name";s:14:"French Guiana ";s:16:"country_areacode";s:4:"+594";}i:75;a:3:{s:10:"country_id";s:2:"pf";s:12:"country_name";s:17:"French Polynesia ";s:16:"country_areacode";s:4:"+689";}i:76;a:3:{s:10:"country_id";s:2:"tf";s:12:"country_name";s:28:"French Southern Territories ";s:16:"country_areacode";s:4:"+596";}i:77;a:3:{s:10:"country_id";s:2:"ga";s:12:"country_name";s:6:"Gabon ";s:16:"country_areacode";s:4:"+241";}i:78;a:3:{s:10:"country_id";s:2:"gm";s:12:"country_name";s:7:"Gambia ";s:16:"country_areacode";s:4:"+220";}i:79;a:3:{s:10:"country_id";s:2:"ge";s:12:"country_name";s:8:"Georgia ";s:16:"country_areacode";s:4:"+995";}i:80;a:3:{s:10:"country_id";s:2:"de";s:12:"country_name";s:8:"Germany ";s:16:"country_areacode";s:3:"+49";}i:81;a:3:{s:10:"country_id";s:2:"gh";s:12:"country_name";s:6:"Ghana ";s:16:"country_areacode";s:4:"+233";}i:82;a:3:{s:10:"country_id";s:2:"gi";s:12:"country_name";s:10:"Gibraltar ";s:16:"country_areacode";s:4:"+350";}i:83;a:3:{s:10:"country_id";s:2:"gr";s:12:"country_name";s:7:"Greece ";s:16:"country_areacode";s:3:"+30";}i:84;a:3:{s:10:"country_id";s:2:"gl";s:12:"country_name";s:10:"Greenland ";s:16:"country_areacode";s:4:"+299";}i:85;a:3:{s:10:"country_id";s:2:"gd";s:12:"country_name";s:8:"Grenada ";s:16:"country_areacode";s:4:"+147";}i:86;a:3:{s:10:"country_id";s:2:"gp";s:12:"country_name";s:11:"Guadeloupe ";s:16:"country_areacode";s:4:"+590";}i:87;a:3:{s:10:"country_id";s:2:"gu";s:12:"country_name";s:5:"Guam ";s:16:"country_areacode";s:4:"+167";}i:88;a:3:{s:10:"country_id";s:2:"gt";s:12:"country_name";s:10:"Guatemala ";s:16:"country_areacode";s:4:"+502";}i:89;a:3:{s:10:"country_id";s:2:"gg";s:12:"country_name";s:9:"Guernsey ";s:16:"country_areacode";s:3:"+44";}i:90;a:3:{s:10:"country_id";s:2:"gn";s:12:"country_name";s:7:"Guinea ";s:16:"country_areacode";s:4:"+224";}i:91;a:3:{s:10:"country_id";s:2:"gw";s:12:"country_name";s:13:"GuineaBissau ";s:16:"country_areacode";s:4:"+245";}i:92;a:3:{s:10:"country_id";s:2:"gy";s:12:"country_name";s:7:"Guyana ";s:16:"country_areacode";s:4:"+592";}i:93;a:3:{s:10:"country_id";s:2:"ht";s:12:"country_name";s:6:"Haiti ";s:16:"country_areacode";s:4:"+509";}i:94;a:3:{s:10:"country_id";s:2:"hm";s:12:"country_name";s:34:"Heard Island And Mcdonald Islands ";s:16:"country_areacode";s:4:"+672";}i:95;a:3:{s:10:"country_id";s:2:"hn";s:12:"country_name";s:9:"Honduras ";s:16:"country_areacode";s:4:"+504";}i:96;a:3:{s:10:"country_id";s:2:"hk";s:12:"country_name";s:10:"Hong Kong ";s:16:"country_areacode";s:4:"+852";}i:97;a:3:{s:10:"country_id";s:2:"hu";s:12:"country_name";s:8:"Hungary ";s:16:"country_areacode";s:3:"+36";}i:98;a:3:{s:10:"country_id";s:2:"is";s:12:"country_name";s:8:"Iceland ";s:16:"country_areacode";s:4:"+354";}i:99;a:3:{s:10:"country_id";s:2:"in";s:12:"country_name";s:6:"India ";s:16:"country_areacode";s:3:"+91";}i:100;a:3:{s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";s:16:"country_areacode";s:3:"+62";}i:101;a:3:{s:10:"country_id";s:2:"ir";s:12:"country_name";s:25:"Iran Islamic Republic Of ";s:16:"country_areacode";s:3:"+98";}i:102;a:3:{s:10:"country_id";s:2:"iq";s:12:"country_name";s:5:"Iraq ";s:16:"country_areacode";s:4:"+964";}i:103;a:3:{s:10:"country_id";s:2:"ie";s:12:"country_name";s:8:"Ireland ";s:16:"country_areacode";s:4:"+353";}i:104;a:3:{s:10:"country_id";s:2:"im";s:12:"country_name";s:12:"Isle Of Man ";s:16:"country_areacode";s:3:"+44";}i:105;a:3:{s:10:"country_id";s:2:"il";s:12:"country_name";s:7:"Israel ";s:16:"country_areacode";s:4:"+972";}i:106;a:3:{s:10:"country_id";s:2:"it";s:12:"country_name";s:6:"Italy ";s:16:"country_areacode";s:3:"+39";}i:107;a:3:{s:10:"country_id";s:2:"jm";s:12:"country_name";s:8:"Jamaica ";s:16:"country_areacode";s:4:"+876";}i:108;a:3:{s:10:"country_id";s:2:"jp";s:12:"country_name";s:6:"Japan ";s:16:"country_areacode";s:3:"+81";}i:109;a:3:{s:10:"country_id";s:2:"je";s:12:"country_name";s:7:"Jersey ";s:16:"country_areacode";s:3:"+44";}i:110;a:3:{s:10:"country_id";s:2:"jo";s:12:"country_name";s:7:"Jordan ";s:16:"country_areacode";s:4:"+962";}i:111;a:3:{s:10:"country_id";s:2:"kz";s:12:"country_name";s:11:"Kazakhstan ";s:16:"country_areacode";s:2:"+7";}i:112;a:3:{s:10:"country_id";s:2:"ke";s:12:"country_name";s:6:"Kenya ";s:16:"country_areacode";s:4:"+254";}i:113;a:3:{s:10:"country_id";s:2:"ki";s:12:"country_name";s:9:"Kiribati ";s:16:"country_areacode";s:4:"+686";}i:114;a:3:{s:10:"country_id";s:2:"kw";s:12:"country_name";s:7:"Kuwait ";s:16:"country_areacode";s:4:"+965";}i:115;a:3:{s:10:"country_id";s:2:"kg";s:12:"country_name";s:11:"Kyrgyzstan ";s:16:"country_areacode";s:4:"+996";}i:116;a:3:{s:10:"country_id";s:2:"la";s:12:"country_name";s:4:"Laos";s:16:"country_areacode";s:4:"+856";}i:117;a:3:{s:10:"country_id";s:2:"lv";s:12:"country_name";s:7:"Latvia ";s:16:"country_areacode";s:4:"+371";}i:118;a:3:{s:10:"country_id";s:2:"lb";s:12:"country_name";s:8:"Lebanon ";s:16:"country_areacode";s:4:"+961";}i:119;a:3:{s:10:"country_id";s:2:"ls";s:12:"country_name";s:8:"Lesotho ";s:16:"country_areacode";s:4:"+266";}i:120;a:3:{s:10:"country_id";s:2:"lr";s:12:"country_name";s:8:"Liberia ";s:16:"country_areacode";s:4:"+231";}i:121;a:3:{s:10:"country_id";s:2:"ly";s:12:"country_name";s:23:"Libyan Arab Jamahiriya ";s:16:"country_areacode";s:4:"+218";}i:122;a:3:{s:10:"country_id";s:2:"li";s:12:"country_name";s:14:"Liechtenstein ";s:16:"country_areacode";s:4:"+423";}i:123;a:3:{s:10:"country_id";s:2:"lt";s:12:"country_name";s:10:"Lithuania ";s:16:"country_areacode";s:4:"+370";}i:124;a:3:{s:10:"country_id";s:2:"lu";s:12:"country_name";s:11:"Luxembourg ";s:16:"country_areacode";s:4:"+352";}i:125;a:3:{s:10:"country_id";s:2:"mo";s:12:"country_name";s:6:"Macau ";s:16:"country_areacode";s:4:"+853";}i:126;a:3:{s:10:"country_id";s:2:"mk";s:12:"country_name";s:42:"Macedonia The Former Yugoslav Republic Of ";s:16:"country_areacode";s:4:"+389";}i:127;a:3:{s:10:"country_id";s:2:"mg";s:12:"country_name";s:11:"Madagascar ";s:16:"country_areacode";s:4:"+261";}i:128;a:3:{s:10:"country_id";s:2:"mw";s:12:"country_name";s:7:"Malawi ";s:16:"country_areacode";s:4:"+265";}i:129;a:3:{s:10:"country_id";s:2:"my";s:12:"country_name";s:9:"Malaysia ";s:16:"country_areacode";s:3:"+60";}i:130;a:3:{s:10:"country_id";s:2:"mv";s:12:"country_name";s:9:"Maldives ";s:16:"country_areacode";s:4:"+960";}i:131;a:3:{s:10:"country_id";s:2:"ml";s:12:"country_name";s:5:"Mali ";s:16:"country_areacode";s:4:"+223";}i:132;a:3:{s:10:"country_id";s:2:"mt";s:12:"country_name";s:6:"Malta ";s:16:"country_areacode";s:4:"+356";}i:133;a:3:{s:10:"country_id";s:2:"mh";s:12:"country_name";s:17:"Marshall Islands ";s:16:"country_areacode";s:4:"+692";}i:134;a:3:{s:10:"country_id";s:2:"mq";s:12:"country_name";s:11:"Martinique ";s:16:"country_areacode";s:4:"+596";}i:135;a:3:{s:10:"country_id";s:2:"mr";s:12:"country_name";s:11:"Mauritania ";s:16:"country_areacode";s:4:"+222";}i:136;a:3:{s:10:"country_id";s:2:"mu";s:12:"country_name";s:10:"Mauritius ";s:16:"country_areacode";s:4:"+230";}i:137;a:3:{s:10:"country_id";s:2:"yt";s:12:"country_name";s:8:"Mayotte ";s:16:"country_areacode";s:4:"+269";}i:138;a:3:{s:10:"country_id";s:2:"mx";s:12:"country_name";s:7:"Mexico ";s:16:"country_areacode";s:3:"+52";}i:139;a:3:{s:10:"country_id";s:2:"fm";s:12:"country_name";s:31:"Micronesia Federated States Of ";s:16:"country_areacode";s:4:"+691";}i:140;a:3:{s:10:"country_id";s:2:"md";s:12:"country_name";s:8:"Moldova ";s:16:"country_areacode";s:4:"+373";}i:141;a:3:{s:10:"country_id";s:2:"mc";s:12:"country_name";s:7:"Monaco ";s:16:"country_areacode";s:4:"+377";}i:142;a:3:{s:10:"country_id";s:2:"mn";s:12:"country_name";s:9:"Mongolia ";s:16:"country_areacode";s:4:"+976";}i:143;a:3:{s:10:"country_id";s:2:"me";s:12:"country_name";s:11:"Montenegro ";s:16:"country_areacode";s:4:"+382";}i:144;a:3:{s:10:"country_id";s:2:"ms";s:12:"country_name";s:11:"Montserrat ";s:16:"country_areacode";s:4:"+166";}i:145;a:3:{s:10:"country_id";s:2:"ma";s:12:"country_name";s:8:"Morocco ";s:16:"country_areacode";s:4:"+212";}i:146;a:3:{s:10:"country_id";s:2:"mz";s:12:"country_name";s:11:"Mozambique ";s:16:"country_areacode";s:4:"+258";}i:147;a:3:{s:10:"country_id";s:2:"mm";s:12:"country_name";s:8:"Myanmar ";s:16:"country_areacode";s:3:"+95";}i:148;a:3:{s:10:"country_id";s:2:"na";s:12:"country_name";s:8:"Namibia ";s:16:"country_areacode";s:4:"+264";}i:149;a:3:{s:10:"country_id";s:2:"nr";s:12:"country_name";s:6:"Nauru ";s:16:"country_areacode";s:4:"+674";}i:150;a:3:{s:10:"country_id";s:2:"np";s:12:"country_name";s:6:"Nepal ";s:16:"country_areacode";s:4:"+977";}i:151;a:3:{s:10:"country_id";s:2:"nl";s:12:"country_name";s:12:"Netherlands ";s:16:"country_areacode";s:3:"+31";}i:152;a:3:{s:10:"country_id";s:2:"an";s:12:"country_name";s:21:"Netherlands Antilles ";s:16:"country_areacode";s:4:"+599";}i:153;a:3:{s:10:"country_id";s:2:"nc";s:12:"country_name";s:14:"New Caledonia ";s:16:"country_areacode";s:4:"+687";}i:154;a:3:{s:10:"country_id";s:2:"nz";s:12:"country_name";s:12:"New Zealand ";s:16:"country_areacode";s:3:"+64";}i:155;a:3:{s:10:"country_id";s:2:"ni";s:12:"country_name";s:10:"Nicaragua ";s:16:"country_areacode";s:4:"+505";}i:156;a:3:{s:10:"country_id";s:2:"ne";s:12:"country_name";s:6:"Niger ";s:16:"country_areacode";s:4:"+227";}i:157;a:3:{s:10:"country_id";s:2:"ng";s:12:"country_name";s:8:"Nigeria ";s:16:"country_areacode";s:4:"+234";}i:158;a:3:{s:10:"country_id";s:2:"nu";s:12:"country_name";s:5:"Niue ";s:16:"country_areacode";s:4:"+683";}i:159;a:3:{s:10:"country_id";s:2:"nf";s:12:"country_name";s:15:"Norfolk Island ";s:16:"country_areacode";s:4:"+672";}i:160;a:3:{s:10:"country_id";s:2:"kp";s:12:"country_name";s:11:"North Korea";s:16:"country_areacode";s:4:"+850";}i:161;a:3:{s:10:"country_id";s:2:"mp";s:12:"country_name";s:25:"Northern Mariana Islands ";s:16:"country_areacode";s:4:"+670";}i:162;a:3:{s:10:"country_id";s:2:"no";s:12:"country_name";s:7:"Norway ";s:16:"country_areacode";s:3:"+47";}i:163;a:3:{s:10:"country_id";s:2:"om";s:12:"country_name";s:5:"Oman ";s:16:"country_areacode";s:4:"+968";}i:164;a:3:{s:10:"country_id";s:2:"pk";s:12:"country_name";s:9:"Pakistan ";s:16:"country_areacode";s:3:"+92";}i:165;a:3:{s:10:"country_id";s:2:"pw";s:12:"country_name";s:6:"Palau ";s:16:"country_areacode";s:4:"+680";}i:166;a:3:{s:10:"country_id";s:2:"ps";s:12:"country_name";s:31:"Palestinian Territory Occupied ";s:16:"country_areacode";s:4:"+970";}i:167;a:3:{s:10:"country_id";s:2:"pa";s:12:"country_name";s:7:"Panama ";s:16:"country_areacode";s:4:"+507";}i:168;a:3:{s:10:"country_id";s:2:"pg";s:12:"country_name";s:17:"Papua New Guinea ";s:16:"country_areacode";s:4:"+675";}i:169;a:3:{s:10:"country_id";s:2:"py";s:12:"country_name";s:9:"Paraguay ";s:16:"country_areacode";s:4:"+595";}i:170;a:3:{s:10:"country_id";s:2:"pe";s:12:"country_name";s:5:"Peru ";s:16:"country_areacode";s:3:"+51";}i:171;a:3:{s:10:"country_id";s:2:"ph";s:12:"country_name";s:12:"Philippines ";s:16:"country_areacode";s:3:"+63";}i:172;a:3:{s:10:"country_id";s:2:"pn";s:12:"country_name";s:9:"Pitcairn ";s:16:"country_areacode";s:4:"+870";}i:173;a:3:{s:10:"country_id";s:2:"pl";s:12:"country_name";s:7:"Poland ";s:16:"country_areacode";s:3:"+48";}i:174;a:3:{s:10:"country_id";s:2:"pt";s:12:"country_name";s:9:"Portugal ";s:16:"country_areacode";s:4:"+351";}i:175;a:3:{s:10:"country_id";s:2:"pr";s:12:"country_name";s:12:"Puerto Rico ";s:16:"country_areacode";s:4:"+787";}i:176;a:3:{s:10:"country_id";s:2:"qa";s:12:"country_name";s:6:"Qatar ";s:16:"country_areacode";s:4:"+974";}i:177;a:3:{s:10:"country_id";s:2:"re";s:12:"country_name";s:7:"Runion ";s:16:"country_areacode";s:4:"+262";}i:178;a:3:{s:10:"country_id";s:2:"ro";s:12:"country_name";s:8:"Romania ";s:16:"country_areacode";s:3:"+40";}i:179;a:3:{s:10:"country_id";s:2:"ru";s:12:"country_name";s:6:"Russia";s:16:"country_areacode";s:2:"+7";}i:180;a:3:{s:10:"country_id";s:2:"rw";s:12:"country_name";s:7:"Rwanda ";s:16:"country_areacode";s:4:"+250";}i:181;a:3:{s:10:"country_id";s:2:"bl";s:12:"country_name";s:16:"Saint Barthlemy ";s:16:"country_areacode";s:4:"+590";}i:182;a:3:{s:10:"country_id";s:2:"sh";s:12:"country_name";s:13:"Saint Helena ";s:16:"country_areacode";s:4:"+290";}i:183;a:3:{s:10:"country_id";s:2:"kn";s:12:"country_name";s:22:"Saint Kitts And Nevis ";s:16:"country_areacode";s:4:"+186";}i:184;a:3:{s:10:"country_id";s:2:"lc";s:12:"country_name";s:12:"Saint Lucia ";s:16:"country_areacode";s:4:"+175";}i:185;a:3:{s:10:"country_id";s:2:"mf";s:12:"country_name";s:13:"Saint Martin ";s:16:"country_areacode";s:4:"+159";}i:186;a:3:{s:10:"country_id";s:2:"pm";s:12:"country_name";s:26:"Saint Pierre And Miquelon ";s:16:"country_areacode";s:4:"+508";}i:187;a:3:{s:10:"country_id";s:2:"vc";s:12:"country_name";s:33:"Saint Vincent And The Grenadines ";s:16:"country_areacode";s:4:"+178";}i:188;a:3:{s:10:"country_id";s:2:"ws";s:12:"country_name";s:6:"Samoa ";s:16:"country_areacode";s:4:"+685";}i:189;a:3:{s:10:"country_id";s:2:"sm";s:12:"country_name";s:11:"San Marino ";s:16:"country_areacode";s:4:"+378";}i:190;a:3:{s:10:"country_id";s:2:"st";s:12:"country_name";s:22:"Sao Tome And Principe ";s:16:"country_areacode";s:4:"+239";}i:191;a:3:{s:10:"country_id";s:2:"sa";s:12:"country_name";s:13:"Saudi Arabia ";s:16:"country_areacode";s:4:"+966";}i:192;a:3:{s:10:"country_id";s:2:"sn";s:12:"country_name";s:8:"Senegal ";s:16:"country_areacode";s:4:"+221";}i:193;a:3:{s:10:"country_id";s:2:"rs";s:12:"country_name";s:7:"Serbia ";s:16:"country_areacode";s:4:"+381";}i:194;a:3:{s:10:"country_id";s:2:"sc";s:12:"country_name";s:11:"Seychelles ";s:16:"country_areacode";s:4:"+248";}i:195;a:3:{s:10:"country_id";s:2:"sl";s:12:"country_name";s:13:"Sierra Leone ";s:16:"country_areacode";s:4:"+232";}i:196;a:3:{s:10:"country_id";s:2:"sg";s:12:"country_name";s:10:"Singapore ";s:16:"country_areacode";s:3:"+65";}i:197;a:3:{s:10:"country_id";s:2:"sk";s:12:"country_name";s:9:"Slovakia ";s:16:"country_areacode";s:4:"+421";}i:198;a:3:{s:10:"country_id";s:2:"si";s:12:"country_name";s:9:"Slovenia ";s:16:"country_areacode";s:4:"+386";}i:199;a:3:{s:10:"country_id";s:2:"sb";s:12:"country_name";s:16:"Solomon Islands ";s:16:"country_areacode";s:4:"+677";}i:200;a:3:{s:10:"country_id";s:2:"so";s:12:"country_name";s:8:"Somalia ";s:16:"country_areacode";s:4:"+252";}i:201;a:3:{s:10:"country_id";s:2:"za";s:12:"country_name";s:13:"South Africa ";s:16:"country_areacode";s:3:"+27";}i:202;a:3:{s:10:"country_id";s:2:"gs";s:12:"country_name";s:45:"South Georgia And The South Sandwich Islands ";s:16:"country_areacode";s:4:"+500";}i:203;a:3:{s:10:"country_id";s:2:"kr";s:12:"country_name";s:11:"South Korea";s:16:"country_areacode";s:3:"+82";}i:204;a:3:{s:10:"country_id";s:2:"es";s:12:"country_name";s:6:"Spain ";s:16:"country_areacode";s:3:"+34";}i:205;a:3:{s:10:"country_id";s:2:"lk";s:12:"country_name";s:10:"Sri Lanka ";s:16:"country_areacode";s:3:"+94";}i:206;a:3:{s:10:"country_id";s:2:"sd";s:12:"country_name";s:6:"Sudan ";s:16:"country_areacode";s:4:"+249";}i:207;a:3:{s:10:"country_id";s:2:"sr";s:12:"country_name";s:9:"Suriname ";s:16:"country_areacode";s:4:"+597";}i:208;a:3:{s:10:"country_id";s:2:"sj";s:12:"country_name";s:23:"Svalbard And Jan Mayen ";s:16:"country_areacode";s:3:"+47";}i:209;a:3:{s:10:"country_id";s:2:"sz";s:12:"country_name";s:10:"Swaziland ";s:16:"country_areacode";s:4:"+268";}i:210;a:3:{s:10:"country_id";s:2:"se";s:12:"country_name";s:7:"Sweden ";s:16:"country_areacode";s:3:"+46";}i:211;a:3:{s:10:"country_id";s:2:"ch";s:12:"country_name";s:12:"Switzerland ";s:16:"country_areacode";s:3:"+41";}i:212;a:3:{s:10:"country_id";s:2:"sy";s:12:"country_name";s:21:"Syrian Arab Republic ";s:16:"country_areacode";s:4:"+963";}i:213;a:3:{s:10:"country_id";s:2:"tw";s:12:"country_name";s:6:"Taiwan";s:16:"country_areacode";s:4:"+886";}i:214;a:3:{s:10:"country_id";s:2:"tj";s:12:"country_name";s:11:"Tajikistan ";s:16:"country_areacode";s:4:"+992";}i:215;a:3:{s:10:"country_id";s:2:"tz";s:12:"country_name";s:8:"Tanzania";s:16:"country_areacode";s:4:"+255";}i:216;a:3:{s:10:"country_id";s:2:"th";s:12:"country_name";s:9:"Thailand ";s:16:"country_areacode";s:3:"+66";}i:217;a:3:{s:10:"country_id";s:2:"tl";s:12:"country_name";s:11:"TimorLeste ";s:16:"country_areacode";s:4:"+670";}i:218;a:3:{s:10:"country_id";s:2:"tg";s:12:"country_name";s:5:"Togo ";s:16:"country_areacode";s:4:"+228";}i:219;a:3:{s:10:"country_id";s:2:"tk";s:12:"country_name";s:8:"Tokelau ";s:16:"country_areacode";s:4:"+690";}i:220;a:3:{s:10:"country_id";s:2:"to";s:12:"country_name";s:6:"Tonga ";s:16:"country_areacode";s:4:"+676";}i:221;a:3:{s:10:"country_id";s:2:"tt";s:12:"country_name";s:20:"Trinidad And Tobago ";s:16:"country_areacode";s:4:"+868";}i:222;a:3:{s:10:"country_id";s:2:"tn";s:12:"country_name";s:8:"Tunisia ";s:16:"country_areacode";s:4:"+216";}i:223;a:3:{s:10:"country_id";s:2:"tr";s:12:"country_name";s:7:"Turkey ";s:16:"country_areacode";s:3:"+90";}i:224;a:3:{s:10:"country_id";s:2:"tm";s:12:"country_name";s:13:"Turkmenistan ";s:16:"country_areacode";s:4:"+993";}i:225;a:3:{s:10:"country_id";s:2:"tc";s:12:"country_name";s:25:"Turks And Caicos Islands ";s:16:"country_areacode";s:4:"+649";}i:226;a:3:{s:10:"country_id";s:2:"tv";s:12:"country_name";s:7:"Tuvalu ";s:16:"country_areacode";s:4:"+688";}i:227;a:3:{s:10:"country_id";s:2:"ug";s:12:"country_name";s:7:"Uganda ";s:16:"country_areacode";s:4:"+256";}i:228;a:3:{s:10:"country_id";s:2:"ua";s:12:"country_name";s:8:"Ukraine ";s:16:"country_areacode";s:4:"+380";}i:229;a:3:{s:10:"country_id";s:2:"ae";s:12:"country_name";s:21:"United Arab Emirates ";s:16:"country_areacode";s:4:"+971";}i:230;a:3:{s:10:"country_id";s:2:"gb";s:12:"country_name";s:15:"United Kingdom ";s:16:"country_areacode";s:3:"+44";}i:231;a:3:{s:10:"country_id";s:2:"us";s:12:"country_name";s:14:"United States ";s:16:"country_areacode";s:2:"+1";}i:232;a:3:{s:10:"country_id";s:2:"um";s:12:"country_name";s:37:"United States Minor Outlying Islands ";s:16:"country_areacode";s:2:"+1";}i:233;a:3:{s:10:"country_id";s:2:"uy";s:12:"country_name";s:8:"Uruguay ";s:16:"country_areacode";s:4:"+598";}i:234;a:3:{s:10:"country_id";s:2:"uz";s:12:"country_name";s:11:"Uzbekistan ";s:16:"country_areacode";s:4:"+998";}i:235;a:3:{s:10:"country_id";s:2:"vu";s:12:"country_name";s:8:"Vanuatu ";s:16:"country_areacode";s:4:"+678";}i:236;a:3:{s:10:"country_id";s:2:"va";s:12:"country_name";s:19:"Vatican City State ";s:16:"country_areacode";s:4:"+379";}i:237;a:3:{s:10:"country_id";s:2:"ve";s:12:"country_name";s:10:"Venezuela ";s:16:"country_areacode";s:3:"+58";}i:238;a:3:{s:10:"country_id";s:2:"vn";s:12:"country_name";s:8:"Vietnam ";s:16:"country_areacode";s:3:"+84";}i:239;a:3:{s:10:"country_id";s:2:"vg";s:12:"country_name";s:23:"Virgin Islands British ";s:16:"country_areacode";s:4:"+128";}i:240;a:3:{s:10:"country_id";s:2:"vi";s:12:"country_name";s:18:"Virgin Islands US ";s:16:"country_areacode";s:4:"+134";}i:241;a:3:{s:10:"country_id";s:2:"wf";s:12:"country_name";s:18:"Wallis And Futuna ";s:16:"country_areacode";s:4:"+681";}i:242;a:3:{s:10:"country_id";s:2:"eh";s:12:"country_name";s:15:"Western Sahara ";s:16:"country_areacode";s:4:"+212";}i:243;a:3:{s:10:"country_id";s:2:"ye";s:12:"country_name";s:6:"Yemen ";s:16:"country_areacode";s:4:"+967";}i:244;a:3:{s:10:"country_id";s:2:"zm";s:12:"country_name";s:7:"Zambia ";s:16:"country_areacode";s:4:"+260";}i:245;a:3:{s:10:"country_id";s:2:"zw";s:12:"country_name";s:8:"Zimbabwe";s:16:"country_areacode";s:4:"+263";}}s:12:"login_status";s:5:"false";s:5:"token";s:40:"f9b29ac359ca5d77755e7588751c089bf96f0dc9";}
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
<?xml version="1.0" encoding="utf-8"?>
<tiket>
    <diagnostic>
        <status>200</status>
        <elapsetime>0.0785</elapsetime>
        <memoryusage>5.06MB</memoryusage>
        <unix_timestamp>1470211883</unix_timestamp>
        <confirm>success</confirm>
        <lang>id</lang>
        <currency>IDR</currency>
    </diagnostic>
    <output_type>xml</output_type>
    <policies>
        <klikbca>
            <name>KlikBCA</name>
            <before>User ID KlikBCA yang dimasukkan harus sesuai dengan User ID KlikBCA anda.</before>
            <before>Transaksi akan dibatalkan (berakhir) jika anda tidak melakukan pembayaran pada periode waktu yang telah ditentukan</before>
            <before>E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan</before>
        </klikbca>
        <cimbclicks>
            <name>CIMB Clicks</name>
            <before>Anda akan diarahkan ke website CIMB Clicks setelah menekan tombol \"Selesaikan Pemesanan\"</before>
            <before>Pembayaran harus dilakukan maksimal 60 menit setelah pemesanan.</before>
            <before>Transaksi dibatalkan</before>
            <before>Untuk konfirmasi dan pencetakan bukti pembayaran, silakan login kembali ke Tiket.com</before>
            <before>E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan</before>
        </cimbclicks>
        <jatis>
            <name>ATM Transfer</name>
            <before>Metode pembayaran ini hanya untuk pembayaran melalui mesin ATM</before>
            <before>Pembayaran harus dilakukan maksimal 60 menit(untuk Pesawat,Kereta Api,Sewa Mobil) dan 3 jam (untuk Hotel dan Event).</before>
            <before>Khusus pengguna ATM Mandiri, Minimum transaksi adalah IDR 50.000</before>
            <before>Untuk internet banking, mobile banking / transfer melalui teller. Silakan gunakan Setor Tunai and m-banking</before>
            <before>E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan</before>
            <after>Untuk internet banking, mobile banking / transfer melalui teller. Silakan gunakan Setor Tunai and m-banking</after>
            <after>8 Digit terakhir nomor Virtual Account adalah order id anda</after>
            <after>Khusus pengguna ATM Mandiri, Minimum transaksi adalah IDR 50.000</after>
            <after>Bank tertentu menetapkan jumlah minimum untuk transfer melalui ATM, harap anda memperhatikan ketentuan ini pada ATM yang anda gunakan.</after>
        </jatis>
        <artajasa>
            <name>ATM Transfer (via ATM Bersama)</name>
            <before>Khusus pengguna ATM Mandiri, Minimum transaksi adalah IDR 50.000</before>
            <before>Bank tertentu menetapkan jumlah minimum untuk transfer melalui ATM, harap anda memperhatikan ketentuan ini pada ATM yang anda gunakan.</before>
            <before>Transaksi dibatalkan</before>
            <before>Untuk konfirmasi dan pencetakan bukti pembayaran, silakan login kembali ke Tiket.com</before>
            <before>E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan</before>
            <after>Khusus pengguna ATM Mandiri, Minimum transaksi adalah IDR 50.000</after>
            <after>Bank tertentu menetapkan jumlah minimum untuk transfer melalui ATM, harap anda memperhatikan ketentuan ini pada ATM yang anda gunakan.</after>
        </artajasa>
        <manual>
            <name>Transfer Online and M-Banking</name>
            <before>Metode pembayaran ini menerima transfer melalui Mesin Setor Tunai, Internet Banking, SMS Banking, atau Teller (Non ATM)</before>
            <before>Pembayaran harus dilakukan maksimal 60 menit(untuk Pesawat,Kereta Api,Sewa Mobil) dan 3 jam (untuk Hotel dan Event).</before>
            <before>Pastikan jumlah dana yang anda transfer sesuai dengan Total Akhir({#total_payment#}) yang tertera diatas.</before>
            <before>Masukan ID pemesan anda dalam kolom berita transfer and simpan bukti pembayaran anda</before>
            <before>Transaksi akan dibatalkan (berakhir) jika anda tidak melakukan pembayaran pada periode waktu yang telah ditentukan atau nominal yang ditransfer tidak sesuai dengan total pembayaran</before>
            <before>E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan</before>
        </manual>
        <mynt>
            <name>Mynt e-Money</name>
            <before>Anda akan diarahkan ke website Mynt E-Money setelah menekan tombol \"Selesaikan Pemesanan\"</before>
            <before>Pembayaran harus dilakukan maksimal 60 menit setelah pemesanan.</before>
            <before>Transaksi dibatalkan</before>
            <before>Untuk konfirmasi dan pencetakan bukti pembayaran, silakan login kembali ke Tiket.com</before>
            <before>E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan</before>
        </mynt>
        <rintis>
            <name>ATM BCA</name>
            <before>Pembayaran hanya dapat dilakukan menggunakan kartu Debit BCA melalui ATM BCA</before>
            <before>Transaksi dibatalkan</before>
            <before>Untuk konfirmasi dan pencetakan bukti pembayaran, silakan login kembali ke Tiket.com</before>
            <before>E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan</before>
            <before>Mohon menyetujui dahulu untuk mentransfer hanya menggunakan Kartu Debit BCA melalui ATM BCA</before>
        </rintis>
        <mandiri_clickpay>
            <name>Mandiri Clickpay</name>
            <before>Aktifkan token MANDIRI anda dengan menekan tombol</before>
            <before>Masukkan password token MANDIRI anda</before>
            <before>Tekan \"3\" ketika muncul pesan \"APPLI\"</before>
            <before>10 Digit Terakhir Nomor Kartu Debit ({#10_digit_card_number#}) dan tekan tombol selama 3 detik</before>
            <before>Total Jumlah Transaksi ({#total_payment#}) dan tekan tombol selama 3 detik</before>
            <before>No Transaksi ({#order_id#}) dan tekan tombol selama 3 detik</before>
            <before>Response Token Mandiri</before>
            <before>Transaksi akan dibatalkan (berakhir) jika anda tidak melakukan pembayaran pada periode waktu yang telah ditentukan</before>
            <before>E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan</before>
        </mandiri_clickpay>
        <epay_bri>
            <name>ePay BRI</name>
            <before>Anda akan diarahkan ke website BRI setelah menekan tombol \"Selesaikan Pemesanan\"</before>
            <before>Pembayaran harus dilakukan maksimal 60 menit setelah pemesanan.</before>
            <before>Transaksi dibatalkan</before>
            <before>Untuk konfirmasi dan pencetakan bukti pembayaran, silakan login kembali ke Tiket.com</before>
            <before>E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan</before>
        </epay_bri>
        <xl_tunai>
            <name>XL Tunai</name>
            <before>Klik tombol 'Lanjutkan'</before>
        </xl_tunai>
    </policies>
    <login_status>false</login_status>
    <token>f9b29ac359ca5d77755e7588751c089bf96f0dc9</token>
</tiket>
```

```json
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.0758",
    "memoryusage": "5.04MB",
    "unix_timestamp": 1470212153,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "policies": {
    "klikbca": {
      "name": "KlikBCA",
      "before": [
        "User ID KlikBCA yang dimasukkan harus sesuai dengan User ID KlikBCA anda.",
        "Transaksi akan dibatalkan (berakhir) jika anda tidak melakukan pembayaran pada periode waktu yang telah ditentukan",
        "E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan"
      ],
      "after": []
    },
    "cimbclicks": {
      "name": "CIMB Clicks",
      "before": [
        "Anda akan diarahkan ke website CIMB Clicks setelah menekan tombol \"Selesaikan Pemesanan\"",
        "Pembayaran harus dilakukan maksimal 60 menit setelah pemesanan.",
        "Transaksi dibatalkan",
        "Untuk konfirmasi dan pencetakan bukti pembayaran, silakan login kembali ke Tiket.com",
        "E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan"
      ],
      "after": []
    },
    "jatis": {
      "name": "ATM Transfer",
      "before": [
        "Metode pembayaran ini hanya untuk pembayaran melalui mesin ATM",
        "Pembayaran harus dilakukan maksimal 60 menit(untuk Pesawat,Kereta Api,Sewa Mobil) dan 3 jam (untuk Hotel dan Event).",
        "Khusus pengguna ATM Mandiri, Minimum transaksi adalah IDR 50.000",
        "Untuk internet banking, mobile banking / transfer melalui teller. Silakan gunakan Setor Tunai and m-banking",
        "E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan"
      ],
      "after": [
        "Untuk internet banking, mobile banking / transfer melalui teller. Silakan gunakan Setor Tunai and m-banking",
        "8 Digit terakhir nomor Virtual Account adalah order id anda",
        "Khusus pengguna ATM Mandiri, Minimum transaksi adalah IDR 50.000",
        "Bank tertentu menetapkan jumlah minimum untuk transfer melalui ATM, harap anda memperhatikan ketentuan ini pada ATM yang anda gunakan."
      ]
    },
    "artajasa": {
      "name": "ATM Transfer (via ATM Bersama)",
      "before": [
        "Khusus pengguna ATM Mandiri, Minimum transaksi adalah IDR 50.000",
        "Bank tertentu menetapkan jumlah minimum untuk transfer melalui ATM, harap anda memperhatikan ketentuan ini pada ATM yang anda gunakan.",
        "Transaksi dibatalkan",
        "Untuk konfirmasi dan pencetakan bukti pembayaran, silakan login kembali ke Tiket.com",
        "E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan"
      ],
      "after": [
        "Khusus pengguna ATM Mandiri, Minimum transaksi adalah IDR 50.000",
        "Bank tertentu menetapkan jumlah minimum untuk transfer melalui ATM, harap anda memperhatikan ketentuan ini pada ATM yang anda gunakan."
      ]
    },
    "manual": {
      "name": "Transfer Online and M-Banking",
      "before": [
        "Metode pembayaran ini menerima transfer melalui Mesin Setor Tunai, Internet Banking, SMS Banking, atau Teller (Non ATM)",
        "Pembayaran harus dilakukan maksimal 60 menit(untuk Pesawat,Kereta Api,Sewa Mobil) dan 3 jam (untuk Hotel dan Event).",
        "Pastikan jumlah dana yang anda transfer sesuai dengan Total Akhir({#total_payment#}) yang tertera diatas.",
        "Masukan ID pemesan anda dalam kolom berita transfer and simpan bukti pembayaran anda",
        "Transaksi akan dibatalkan (berakhir) jika anda tidak melakukan pembayaran pada periode waktu yang telah ditentukan atau nominal yang ditransfer tidak sesuai dengan total pembayaran",
        "E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan"
      ],
      "after": []
    },
    "mynt": {
      "name": "Mynt e-Money",
      "before": [
        "Anda akan diarahkan ke website Mynt E-Money setelah menekan tombol \"Selesaikan Pemesanan\"",
        "Pembayaran harus dilakukan maksimal 60 menit setelah pemesanan.",
        "Transaksi dibatalkan",
        "Untuk konfirmasi dan pencetakan bukti pembayaran, silakan login kembali ke Tiket.com",
        "E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan"
      ],
      "after": []
    },
    "rintis": {
      "name": "ATM BCA",
      "before": [
        "Pembayaran hanya dapat dilakukan menggunakan kartu Debit BCA melalui ATM BCA",
        "Transaksi dibatalkan",
        "Untuk konfirmasi dan pencetakan bukti pembayaran, silakan login kembali ke Tiket.com",
        "E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan",
        "Mohon menyetujui dahulu untuk mentransfer hanya menggunakan Kartu Debit BCA melalui ATM BCA"
      ],
      "after": []
    },
    "mandiri_clickpay": {
      "name": "Mandiri Clickpay",
      "before": [
        "Aktifkan token MANDIRI anda dengan menekan tombol",
        "Masukkan password token MANDIRI anda",
        "Tekan \"3\" ketika muncul pesan \"APPLI\"",
        "10 Digit Terakhir Nomor Kartu Debit ({#10_digit_card_number#}) dan tekan tombol selama 3 detik",
        "Total Jumlah Transaksi ({#total_payment#}) dan tekan tombol selama 3 detik",
        "No Transaksi ({#order_id#}) dan tekan tombol selama 3 detik",
        "Response Token Mandiri",
        "Transaksi akan dibatalkan (berakhir) jika anda tidak melakukan pembayaran pada periode waktu yang telah ditentukan",
        "E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan"
      ],
      "after": []
    },
    "epay_bri": {
      "name": "ePay BRI",
      "before": [
        "Anda akan diarahkan ke website BRI setelah menekan tombol \"Selesaikan Pemesanan\"",
        "Pembayaran harus dilakukan maksimal 60 menit setelah pemesanan.",
        "Transaksi dibatalkan",
        "Untuk konfirmasi dan pencetakan bukti pembayaran, silakan login kembali ke Tiket.com",
        "E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan"
      ],
      "after": []
    },
    "xl_tunai": {
      "name": "XL Tunai",
      "before": [
        "Klik tombol 'Lanjutkan'"
      ],
      "after": []
    }
  },
  "login_status": "false",
  "token": "f9b29ac359ca5d77755e7588751c089bf96f0dc9"
}
```

```matlab
a:5:{s:10:"diagnostic";a:7:{s:6:"status";i:200;s:10:"elapsetime";s:14:"0.0796";s:11:"memoryusage";s:14:"5.05MB";s:14:"unix_timestamp";i:1470212259;s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:11:"output_type";s:9:"serialize";s:8:"policies";a:10:{s:7:"klikbca";a:3:{s:4:"name";s:7:"KlikBCA";s:6:"before";a:3:{i:0;s:36:"User ID KlikBCA yang dimasukkan harus sesuai dengan User ID KlikBCA anda.";i:1;s:47:"Transaksi akan dibatalkan (berakhir) jika anda tidak melakukan pembayaran pada periode waktu yang telah ditentukan";i:2;s:34:"E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan";}s:5:"after";a:0:{}}s:10:"cimbclicks";a:3:{s:4:"name";s:11:"CIMB Clicks";s:6:"before";a:5:{i:0;s:28:"Anda akan diarahkan ke website CIMB Clicks setelah menekan tombol \"Selesaikan Pemesanan\"";i:1;s:36:"Pembayaran harus dilakukan maksimal 60 menit setelah pemesanan.";i:2;s:32:"Transaksi dibatalkan";i:3;s:36:"Untuk konfirmasi dan pencetakan bukti pembayaran, silakan login kembali ke Tiket.com";i:4;s:34:"E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan";}s:5:"after";a:0:{}}s:5:"jatis";a:3:{s:4:"name";s:12:"ATM Transfer";s:6:"before";a:5:{i:0;s:25:"Metode pembayaran ini hanya untuk pembayaran melalui mesin ATM";i:1;s:41:"Pembayaran harus dilakukan maksimal 60 menit(untuk Pesawat,Kereta Api,Sewa Mobil) dan 3 jam (untuk Hotel dan Event).";i:2;s:35:"Khusus pengguna ATM Mandiri, Minimum transaksi adalah IDR 50.000";i:3;s:36:"Untuk internet banking, mobile banking / transfer melalui teller. Silakan gunakan Setor Tunai and m-banking";i:4;s:34:"E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan";}s:5:"after";a:4:{i:0;s:36:"Untuk internet banking, mobile banking / transfer melalui teller. Silakan gunakan Setor Tunai and m-banking";i:1;s:19:"8 Digit terakhir nomor Virtual Account adalah order id anda";i:2;s:35:"Khusus pengguna ATM Mandiri, Minimum transaksi adalah IDR 50.000";i:3;s:26:"Bank tertentu menetapkan jumlah minimum untuk transfer melalui ATM, harap anda memperhatikan ketentuan ini pada ATM yang anda gunakan.";}}s:8:"artajasa";a:3:{s:4:"name";s:30:"ATM Transfer (via ATM Bersama)";s:6:"before";a:5:{i:0;s:35:"Khusus pengguna ATM Mandiri, Minimum transaksi adalah IDR 50.000";i:1;s:26:"Bank tertentu menetapkan jumlah minimum untuk transfer melalui ATM, harap anda memperhatikan ketentuan ini pada ATM yang anda gunakan.";i:2;s:32:"Transaksi dibatalkan";i:3;s:36:"Untuk konfirmasi dan pencetakan bukti pembayaran, silakan login kembali ke Tiket.com";i:4;s:34:"E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan";}s:5:"after";a:2:{i:0;s:35:"Khusus pengguna ATM Mandiri, Minimum transaksi adalah IDR 50.000";i:1;s:26:"Bank tertentu menetapkan jumlah minimum untuk transfer melalui ATM, harap anda memperhatikan ketentuan ini pada ATM yang anda gunakan.";}}s:6:"manual";a:3:{s:4:"name";s:24:"Transfer Online and M-Banking";s:6:"before";a:6:{i:0;s:27:"Metode pembayaran ini menerima transfer melalui Mesin Setor Tunai, Internet Banking, SMS Banking, atau Teller (Non ATM)";i:1;s:41:"Pembayaran harus dilakukan maksimal 60 menit(untuk Pesawat,Kereta Api,Sewa Mobil) dan 3 jam (untuk Hotel dan Event).";i:2;s:26:"Pastikan jumlah dana yang anda transfer sesuai dengan Total Akhir({#total_payment#}) yang tertera diatas.";i:3;s:21:"Masukan ID pemesan anda dalam kolom berita transfer and simpan bukti pembayaran anda";i:4;s:62:"Transaksi akan dibatalkan (berakhir) jika anda tidak melakukan pembayaran pada periode waktu yang telah ditentukan atau nominal yang ditransfer tidak sesuai dengan total pembayaran";i:5;s:34:"E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan";}s:5:"after";a:0:{}}s:4:"mynt";a:3:{s:4:"name";s:12:"Mynt e-Money";s:6:"before";a:5:{i:0;s:27:"Anda akan diarahkan ke website Mynt E-Money setelah menekan tombol \"Selesaikan Pemesanan\"";i:1;s:36:"Pembayaran harus dilakukan maksimal 60 menit setelah pemesanan.";i:2;s:32:"Transaksi dibatalkan";i:3;s:36:"Untuk konfirmasi dan pencetakan bukti pembayaran, silakan login kembali ke Tiket.com";i:4;s:34:"E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan";}s:5:"after";a:0:{}}s:6:"rintis";a:3:{s:4:"name";s:7:"ATM BCA";s:6:"before";a:5:{i:0;s:21:"Pembayaran hanya dapat dilakukan menggunakan kartu Debit BCA melalui ATM BCA";i:1;s:32:"Transaksi dibatalkan";i:2;s:36:"Untuk konfirmasi dan pencetakan bukti pembayaran, silakan login kembali ke Tiket.com";i:3;s:34:"E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan";i:4;s:29:"Mohon menyetujui dahulu untuk mentransfer hanya menggunakan Kartu Debit BCA melalui ATM BCA";}s:5:"after";a:0:{}}s:16:"mandiri_clickpay";a:3:{s:4:"name";s:16:"Mandiri Clickpay";s:6:"before";a:9:{i:0;s:24:"Aktifkan token MANDIRI anda dengan menekan tombol";i:1;s:33:"Masukkan password token MANDIRI anda";i:2;s:30:"Tekan \"3\" ketika muncul pesan \"APPLI\"";i:3;s:114:"10 Digit Terakhir Nomor Kartu Debit ({#10_digit_card_number#}) dan tekan tombol selama 3 detik";i:4;s:88:"Total Jumlah Transaksi ({#total_payment#}) dan tekan tombol selama 3 detik";i:5;s:93:"No Transaksi ({#order_id#}) dan tekan tombol selama 3 detik";i:6;s:33:"Response Token Mandiri";i:7;s:47:"Transaksi akan dibatalkan (berakhir) jika anda tidak melakukan pembayaran pada periode waktu yang telah ditentukan";i:8;s:34:"E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan";}s:5:"after";a:0:{}}s:8:"epay_bri";a:3:{s:4:"name";s:8:"ePay BRI";s:6:"before";a:5:{i:0;s:27:"Anda akan diarahkan ke website BRI setelah menekan tombol \"Selesaikan Pemesanan\"";i:1;s:36:"Pembayaran harus dilakukan maksimal 60 menit setelah pemesanan.";i:2;s:32:"Transaksi dibatalkan";i:3;s:36:"Untuk konfirmasi dan pencetakan bukti pembayaran, silakan login kembali ke Tiket.com";i:4;s:34:"E-Tiket atau Voucher akan dikirimkan melalui email setelah pembayaran selesai dilakukan";}s:5:"after";a:0:{}}s:8:"xl_tunai";a:3:{s:4:"name";s:8:"XL Tunai";s:6:"before";a:1:{i:0;s:24:"Klik tombol 'Lanjutkan'";}s:5:"after";a:0:{}}}s:12:"login_status";s:5:"false";s:5:"token";s:40:"f9b29ac359ca5d77755e7588751c089bf96f0dc9";}
```

Text to be used on you checkout process. <code>before</code> means the text is placed before customer finalize payment. <code>after</code> means the text is placed right after customer finish checking out.

#### HTTP Request

`GET https://api-sandbox.tiket.com/general_api/getPolicies?token=c992866a6ffb08e59a86fc6a050ca7c7bdec6c2f&lang=id`

#### Parameter

Name | Description | Format    | Default   | Mandatory
--------- | ------- | ----------- | ----------- | -----------
token | Token acquired from gettoken | CHAR(128) |  | TRUE
lang  | The [language](#list-language) used | CHAR(2) | id | FALSE





