# Payment

## Checkout Payment

```xml
<tiket>
  <output_type>xml</output_type>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.5302</elapsetime>
    <memoryusage>14.77MB</memoryusage>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <result>
    <payment_discount>32665</payment_discount>
    <order_id>149584</order_id>
    <currency>IDR</currency>
    <payment_charge>4000</payment_charge>
    <sub_total>1386600</sub_total>
    <unique_code>0</unique_code>
    <grand_total>1390600</grand_total>
    <grand_subtotal>1423265</grand_subtotal>
  </result>
  <token>136637980b7b0e13ef3af9adbe571304</token>
</tiket>
```

```json
{"See XML tab for example"}
```

```matlab
{"See XML tab for example"}
```

> Grand_subtotal - payment_discount = sub_total

> subtotal + payment_charge + unique_code = grand_total

Completing checkout process with selected payment method.

Because Tiket.com domicile in Indonesia, it is mandatory that the payment is in IDR (Indonesia Rupiah). When you checkout using <code>checkout_payment</code>, you must pass the parameter <code>&currency=IDR</code> to ensure that the payment is in IDR.

<aside class="notice">When you submit without <code>btn_booking</code>, then it will only show payment information without processing the payment itself. This is useful if you wanted to know how much is the final price for the selected payment method</aside>

### Bank Transfer

```http
GET /checkout/checkout_payment/2?token=2ee91e32f9113e863da4c57e235098d1&currency=IDR&btn_booking=1 HTTP/1.1
Host: api-sandbox.tiket.com
User-Agent: twh:123456789;Partner Name;
Content-Type: text/plain
```

```xml
<tiket>
  <output_type>xml</output_type>
  <diagnostic>
    <status>200</status>
    <elapsetime>1.7780</elapsetime>
    <memoryusage>11.14MB</memoryusage>
    <confirm>success</confirm>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <orderId>120004</orderId>
  <banks>
    <bank>
      <photo_1>httpss://www.sandbox.tiket.com/images/ico_bca.png</photo_1>
      <photo_2>httpss://www.sandbox.tiket.com/images/ico_prima.png</photo_2>
      <Nama>PT. Global Tiket Network</Nama>
      <Bank>BCA</Bank>
      <Cabang>Jakarta</Cabang>
      <NoRekening>52 6032 2488</NoRekening>
    </bank>
    <bank>
      <photo_1>
        httpss://www.sandbox.tiket.com/images/ico_mandiri.png
      </photo_1>
      <photo_2>httpss://www.sandbox.tiket.com/images/ico_atm.png</photo_2>
      <Nama>PT. Global Tiket Network</Nama>
      <Bank>Mandiri</Bank>
      <Cabang>Pelni</Cabang>
      <NoRekening>11 7000 606 9959</NoRekening>
    </bank>
  </banks>
  <message>
    Silakan transfer pembayaran untuk memesan. Anda memiliki waktu <strong>3 jam</strong> untuk melakukan pembayaran.
  </message>
  <confirm_payment>
    httpss://api-sandbox.tiket.com/confirmpayment/save?orderId=120004&hash=19b4c9956d2b5173ec023d1dbb13a1a3
  </confirm_payment>
  <grand_total>60044</grand_total>
  <token>2ee91e32f9113e863da4c57e235098d1</token>
</tiket>
```

```json
{
  "output_type": "json",
  "diagnostic": {
    "status": 200,
    "elapsetime": "1.7074",
    "memoryusage": "11.09MB",
    "confirm": "success",
    "lang": "en",
    "currency": "IDR"
  },
  "orderId": 120003,
  "banks": [{
    "photo_1": "httpss:\/\/www.sandbox.tiket.com\/images\/ico_bca.png",
    "photo_2": "httpss:\/\/www.sandbox.tiket.com\/images\/ico_prima.png",
    "Nama": "PT. Global Tiket Network",
    "Bank": "BCA",
    "Cabang": "Jakarta",
    "No Rekening": "52 6032 2488"
  }, {
    "photo_1": "httpss:\/\/www.sandbox.tiket.com\/images\/ico_mandiri.png",
    "photo_2": "httpss:\/\/www.sandbox.tiket.com\/images\/ico_atm.png",
    "Nama": "PT. Global Tiket Network",
    "Bank": " Mandiri",
    "Cabang": "Pelni",
    "No Rekening": "11 7000 606 9959"
  }],
  "message": "Please transfer the payment to make a booking. You have <strong>3 hours</strong> to complete the payment.",
  "confirm_payment": "httpss:\/\/api-sandbox.tiket.com\/confirmpayment\/save?orderId=120003&hash=51ea6013f6a4347411e92cbbf98452de",
  "grand_total": 60045,
  "token": "5a80dc2ccce351eeb412e835b651edb9"
}
```

```matlab
a: 8: {
  s: 11: "output_type";s: 9: "serialize";s: 10: "diagnostic";a: 6: {
    s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "2.3195";s: 11: "memoryusage";s: 14: "11.1MB";s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "en";s: 8: "currency";s: 3: "IDR";
  }
  s: 7: "orderId";i: 120010;s: 5: "banks";a: 2: {
    i: 0;a: 6: {
      s: 7: "photo_1";s: 48: "httpss://www.sandbox.tiket.com/images/ico_bca.png";s: 7: "photo_2";s: 50: "httpss://www.sandbox.tiket.com/images/ico_prima.png";s: 4: "Nama";s: 24: "PT. Global Tiket Network";s: 4: "Bank";s: 3: "BCA";s: 6: "Cabang";s: 7: "Jakarta";s: 11: "No Rekening";s: 12: "52 6032 2488";
    }
    i: 1;a: 6: {
      s: 7: "photo_1";s: 52: "httpss://www.sandbox.tiket.com/images/ico_mandiri.png";s: 7: "photo_2";s: 48: "httpss://www.sandbox.tiket.com/images/ico_atm.png";s: 4: "Nama";s: 24: "PT. Global Tiket Network";s: 4: "Bank";s: 8: " Mandiri";s: 6: "Cabang";s: 5: "Pelni";s: 11: "No Rekening";s: 16: "11 7000 606 9959";
    }
  }
  s: 7: "message";s: 35: "Please transfer the payment to make a booking. You have <strong>3 hours</strong> to complete the payment.";s: 15: "confirm_payment";s: 102: "httpss://api-sandbox.tiket.com/confirmpayment/save?orderId=120010&hash=dbd0c974292ebc4c278b7461e4706a4c";s: 11: "grand_total";d: 60050;s: 5: "token";s: 32: "9d4ccf0c966e37a4c112c59ac2bc2e97";
}
```

Bank transfer to Tiket.com regular corporate account. Customer will have to pay an additional amount so that the transfer is unique (unique transfer amount). Please note that the payment will not be instant, because we will have to check it manually. Also, the availability time will vary too. Usually we closes the payment at 7 PM and open again at 9 AM. 

<aside class="warning">This payment method will be deprecated shortly.</aside>

#### HTTP Request

`GET https://api-sandbox.tiket.com/checkout/checkout_payment/2?token=2ee91e32f9113e863da4c57e235098d1&currency=IDR&btn_booking=1&output=json`

#### Parameter

Name | Description | Format    | Default   | Mandatory
--------- | ------- | ----------- | ----------- | -----------
token | Token acquired from gettoken | CHAR(128) |  | TRUE
btn_booking | Set to 1 to continue checkout. Set to 0 to check the total price | INT |  | TRUE
currency | For checkout_payment, the value must be IDR | CHAR(3) | | TRUE

### KlikBCA

```http
GET /checkout/checkout_payment/3?token=2ee91e32f9113e863da4c57e235098d1&btn_booking=1&user_bca=username1234&currency=IDR HTTP/1.1
Host: api-sandbox.tiket.com
User-Agent: twh:123456789;Partner Name;
Content-Type: text/plain
```

```xml
<tiket>
  <output_type>xml</output_type>
  <diagnostic>
    <status>200</status>
    <elapsetime>2.0213</elapsetime>
    <memoryusage>11.78MB</memoryusage>
    <confirm>success</confirm>
    <lang>en</lang>
    <currency>IDR</currency>
  </diagnostic>
  <orderId>129621</orderId>
  <result/>
  <steps>
    <step>
      <![CDATA[Visit KlikBCA website in
            <strong>http://www.klikbca.com/</strong>
            ]]>
    </step>
    <step>
      <![CDATA[Login using your user ID. (username1234)]]>
    </step>
    <step>
      <![CDATA[Go to menu
            <strong>' e-Commerce Payment'</strong>
            ]]>
    </step>
    <step>
      <![CDATA[Choose category
            <strong>'Tour / Travel / Hotel'</strong>
            ]]>
    </step>
    <step>
      <![CDATA[Choose company name
            <strong>'TIKET.COM'</strong>
            ]]>
    </step>
    <step>
      <![CDATA[Click button
            <strong>'Continue'</strong>
            ]]>
    </step>
    <step>
      <![CDATA[Choose transaction with booking code
            <strong>129621</strong>
            then make payment.]]>
    </step>
    <step>
      <![CDATA[After you have completed the payment, you will receive an e-mail within 5 minutes]]>
    </step>
  </steps>
  <grand_total/>
  <message>
    Your transaction has been recorded in KlikBCA, please make payment on KlikBCA.com immediately by login using your KlikBCA UserID.
  </message>
  <token>19fa2a3a3c611d9616970d03e6f66286</token>
</tiket>
```

```json
{
  "output_type": "json",
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.2100",
    "memoryusage": "8.67MB",
    "confirm": "success",
    "lang": "en",
    "currency": "IDR"
  },
  "orderId": 120005,
  "grand_total": 59680,
  "message": "Your transaction has been recorded in KlikBCA, please make payment on KlikBCA.com immediately by login using your KlikBCA UserID.",
  "steps": ["Visit KlikBCA website in <strong>httpss://www.klikbca.com/</strong>", "Login using your user ID.harryant1810", "Go to menu <strong>' e-Commerce Payment'</strong>", "Choose category <strong>'Tour / Travel / Hotel'</strong>", "Choose company name <strong>'TIKET.COM'</strong>", "Click button <strong>'Continue'</strong>", "Choose transaction with booking code <strong> 120005</strong> then make payment.", "After you have completed the payment, <strong>you will receive an e-mail within 5 minutes</strong> containing your <strong>Hotel / Event Voucher for hotel / event purchase or Booking Code & Pass Key for movie purchase</strong>"],
  "token": "a0336694655bbf6fb442c68eb50f98e7"
}
```

```matlab
a: 7: {
  s: 11: "output_type";s: 9: "serialize";s: 10: "diagnostic";a: 6: {
    s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "7.0115";s: 11: "memoryusage";s: 14: "11.33MB";s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "en";s: 8: "currency";s: 3: "IDR";
  }
  s: 7: "orderId";i: 122923;s: 6: "result";a: 15: {
    s: 16: "payment_discount";d: 13000;s: 11: "order_types";a: 1: {
      i: 0;s: 5: "event";
    }
    s: 8: "order_id";i: 122923;s: 8: "currency";s: 3: "IDR";s: 9: "giftPromo";b: 0;s: 14: "payment_charge";d: 4000;s: 9: "sub_total";d: 500000;s: 11: "unique_code";i: 0;s: 11: "grand_total";d: 504000;s: 6: "orders";a: 1: {
      i: 0;a: 38: {
        s: 11: "total_price";d: 500000;s: 8: "quantity";s: 1: "1";s: 8: "order_id";s: 6: "122923";s: 15: "order_detail_id";s: 5: "32856";s: 10: "order_type";s: 5: "event";s: 15: "order_master_id";s: 3: "131";s: 10: "event_name";s: 32: "Gym Class Heroes Live in Jakarta";s: 10: "tiket_name";s: 10: "Festival B";s: 8: "currency";s: 3: "IDR";s: 5: "price";s: 9: "500000.00";s: 13: "selling_price";s: 9: "500000.00";s: 16: "selling_currency";s: 3: "IDR";s: 17: "tiket_event_start";s: 19: "2012-08-11 21:00:00";s: 15: "tiket_event_end";s: 19: "2012-08-11 23:00:00";s: 18: "tiket_with_seating";s: 1: "0";s: 19: "tiket_required_info";s: 11: "name,idcard";s: 18: "tiket_min_purchase";s: 1: "1";s: 18: "tiket_max_purchase";s: 1: "5";s: 3: "uri";s: 16: "gym-class-heroes";s: 9: "file_name";s: 25: "business-banner-baru1.jpg";s: 11: "business_id";s: 6: "111693";s: 17: "business_address1";s: 66: "Gedung Kartika Expo-Balai Kartini Jln. Jend. Gatot Subroto Kav. 37";s: 12: "country_name";s: 10: "Indonesia ";s: 9: "city_name";N;s: 13: "tiket_barcode";s: 13: "4657554478067";s: 12: "checkin_date";N;s: 15: "tiket_cust_name";s: 2: "ju";s: 14: "customer_price";s: 9: "500000.00";s: 17: "customer_currency";s: 3: "IDR";s: 13: "tiket_cust_id";s: 4: "1234";s: 15: "sell_rate_price";s: 9: "500000.00";s: 13: "tiket_seating";s: 0: "";s: 14: "is_installment";s: 1: "0";s: 14: "payment_status";s: 12: "shoppingcart";s: 12: "tiket_detail";a: 1: {
          i: 0;a: 4: {
            s: 13: "tiket_barcode";s: 13: "4657554478067";s: 15: "tiket_cust_name";s: 2: "ju";s: 13: "tiket_cust_id";s: 4: "1234";s: 13: "tiket_seating";s: 0: "";
          }
        }
        s: 14: "tiket_quantity";i: 1;s: 22: "detail_ticket_schedule";s: 33: "11 Aug 2012, 21:00:00 - 23:00:00 ";s: 4: "type";s: 5: "event";
      }
    }
    s: 19: "confirm_page_mobile";b: 0;s: 3: "gaq";s: 0: "";s: 12: "payment_type";i: 3;s: 15: "is_confirmation";b: 0;s: 4: "type";s: 0: "";
  }
  s: 11: "grand_total";d: 504000;s: 7: "message";s: 38: "Your transaction has been recorded in KlikBCA, please make payment on KlikBCA.com immediately by login using your KlikBCA UserID.";s: 5: "token";s: 32: "006a0a65359b5f018761f20959bbb178";
}
```

Payment using [KlikBCA](https://ibank.klikbca.com/).

#### HTTP Request

`GET https://api-sandbox.tiket.com/checkout/checkout_payment/3?token=2ee91e32f9113e863da4c57e235098d1&btn_booking=1&user_bca=username1234&currency=IDR&output=json`

#### Parameter

Name | Description | Format    | Default   | Mandatory
--------- | ------- | ----------- | ----------- | -----------
token | Token acquired from gettoken | CHAR(128) |  | TRUE
btn_booking | Set to 1 to continue checkout. Set to 0 to check the total price | INT |  | TRUE
currency | For checkout_payment, the value must be IDR | CHAR(3) | | TRUE
user_bca | KlikBCA User ID (ex: username1234) | CHAR(12) | | TRUE


### Bank Transfer (Instant confirmation)

```http
GET /checkout/checkout_payment/35?token=2ee91e32f9113e863da4c57e235098d1&btn_booking=1&currency=IDR HTTP/1.1
Host: api-sandbox.tiket.com
User-Agent: twh:123456789;Partner Name;
Content-Type: text/plain
```

```xml
<tiket>
  <output_type>xml</output_type>
  <diagnostic>
    <status>200</status>
    <elapsetime>2.0213</elapsetime>
    <memoryusage>11.78MB</memoryusage>
    <confirm>success</confirm>
    <lang>en</lang>
    <currency>IDR</currency>
  </diagnostic>
  <orderId>129621</orderId>
  <result/>
  <steps>
    <!-- to be generated -->
  </steps>
  <grand_total/>
  <message>
    <![CDATA[Silakan transfer pembayaran untuk memesan. Anda memiliki waktu <strong>3 jam</strong> untuk melakukan pembayaran.]]>
  </message>
  <token>19fa2a3a3c611d9616970d03e6f66286</token>
</tiket>
```

```json
{
  "output_type": "json",
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.2100",
    "memoryusage": "8.67MB",
    "confirm": "success",
    "lang": "en",
    "currency": "IDR"
  },
  "orderId": 120005,
  "grand_total": 59680,
  "message": "Silakan transfer pembayaran untuk memesan. Anda memiliki waktu <strong>3 jam</strong> untuk melakukan pembayaran.",
  "steps": ["// to be generated"],
  "token": "a0336694655bbf6fb442c68eb50f98e7"
}
```

```matlab
// to be generated
```

Payment using bank transfer through virtual account. Payment will be paid to Bank Permata virtual account.

#### HTTP Request

`GET http://api-sandbox.tiket.com/checkout/checkout_payment/35?token=4c71d60d367bbffa1b293cb663afc4e9&btn_booking=1&currency=IDR&output=json`

#### Parameter

Name | Description | Format    | Default   | Mandatory
--------- | ------- | ----------- | ----------- | -----------
token | Token acquired from gettoken | CHAR(128) |  | TRUE
btn_booking | Set to 1 to continue checkout. Set to 0 to check the total price | INT |  | TRUE
currency | For checkout_payment, the value must be IDR | CHAR(3) | | TRUE


```xml
// to be generated. View JSON version for sample output
```

```json
{
  "output_type": "json",
  "diagnostic": {
    "status": 209,
    "error_msgs": "your order has expired please recheck your order",
    "elapsetime": "0.2049",
    "memoryusage": "7.93MB",
    "lang": "en",
    "currency": "IDR"
  },
  "token": "8040d5dab0d283a1be360ffe70fb7e7f"
}
```

```matlab
// to be generated. View JSON version instead
```

<aside class="warning">If the order has expired, it will emit status code <code>209</code> instead. </aside>

After you receive status code `200`, kindly create a UI that looks similar to the following screenshots:

Bank Transfer (English) 
![Bank Transfer (English)](https://raw.githubusercontent.com/tiket-dev/slate/master/source/images/bank-transfer-english.jpg)





