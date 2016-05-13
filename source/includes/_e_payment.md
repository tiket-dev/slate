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

### Bank Transfer Payment Method

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






