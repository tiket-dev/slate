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

Checkout payment is a method where when you checkout, you will have to ask customer to do certain process outside your website or apps. For instance, for KlikBCA, user will be asked to go to https://klikbca.com to pay. Or if you chooese bank transfer, you will ask user do certain actions via ATM or online banking.

Because Tiket.com domicile in Indonesia, it is mandatory that the payment is in IDR (Indonesia Rupiah). When you checkout using <code>checkout_payment</code>, you must pass the parameter <code>&currency=IDR</code> to ensure that the payment is in IDR.

<aside class="notice">When you submit without <code>btn_booking</code>, then it will only show payment information without processing the payment itself. This is useful if you wanted to know how much is the final price for the selected payment method</aside>












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

Payment using [KlikBCA](https://ibank.klikbca.com/). Once you trigger this and return `200` code, you can proceed by telling customer to do the `<steps>` activity.

#### HTTP Request

`GET https://api-sandbox.tiket.com/checkout/checkout_payment/3?token=2ee91e32f9113e863da4c57e235098d1&btn_booking=1&user_bca=username1234&currency=IDR&output=json`

#### Parameter

Name | Description | Format    | Default   | Mandatory
--------- | ------- | ----------- | ----------- | -----------
token | Token acquired from gettoken | CHAR(128) |  | TRUE
btn_booking | Set to 1 to continue checkout. Set to 0 to check the total price | INT |  | TRUE
currency | For checkout_payment, the value must be IDR | CHAR(3) | | TRUE
user_bca | KlikBCA User ID (ex: username1234) | CHAR(12) | | TRUE

After you receive status code `200`, kindly create a UI that looks similar to the following screenshots:

##### KlikBCA (English) 
![KlikBCA (English)](https://raw.githubusercontent.com/tiket-dev/slate/master/source/images/klikbca-English.jpg)

##### KlikBCA (Indonesia) 
![KlikBCA (Indonesia)](https://raw.githubusercontent.com/tiket-dev/slate/master/source/images/klikbca-indonesia.jpg)















### Bank Transfer (Instant confirmation)

> Status code 200 response

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

Payment using bank transfer through virtual account. Payment will be paid to Bank Permata virtual account. Once you trigger this and return `200` code, you can proceed by telling customer to do the `<steps>` activity.

#### HTTP Request

`GET http://api-sandbox.tiket.com/checkout/checkout_payment/35?token=4c71d60d367bbffa1b293cb663afc4e9&btn_booking=1&currency=IDR&output=json`

#### Parameter

Name | Description | Format    | Default   | Mandatory
--------- | ------- | ----------- | ----------- | -----------
token | Token acquired from gettoken | CHAR(128) |  | TRUE
btn_booking | Set to 1 to continue checkout. Set to 0 to check the total price | INT |  | TRUE
currency | For checkout_payment, the value must be IDR | CHAR(3) | | TRUE

> Status code 209 response

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

##### Bank Transfer (English) 
![Bank Transfer (English)](https://raw.githubusercontent.com/tiket-dev/slate/master/source/images/bank-transfer-english.jpg)

##### Bank Transfer (Indonesia) 
![Bank Transfer (Indonesia)](https://raw.githubusercontent.com/tiket-dev/slate/master/source/images/bank-transfer-indonesia.jpg)







### Bank Transfer (manual confirmation)

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









## Payment Gateway

With this method of payment, you will redirect your customer to Tiket.com's very own payment gateway. The reason for this is because there are certain security measure that cannot be shifted through API, such as hash signature process etc. Also, for Credit Card payment, the domain name **must** be Tiket.com as required for PCI-DSS compliance.

### General Configuration

Below is some general configuration changes that you can do for payment gateway:

#### Change the Logo in the PG or the voucher

1. Login first at http://www.tiket.com/affiliate so that you can access the partner area.
2. Click the Settings > setting menu http://www.tiket.com/partner/logo/
3. You can change the logo by uploading your own. File must be in JPG format and the height will automatically resized to 62 pixels.

#### Display your own contact and address

1. Login first at http://www.tiket.com/affiliate so that you can access the partner area.
2. Click the Settings > setting menu http://www.tiket.com/partner/logo/
3. You can change the address with your own address by ticking the _use own address_ and enter your address and contact informations.

#### Change the background color of PG

1. Login first at http://www.tiket.com/affiliate so that you can access the partner area.
2. Click the Settings > setting menu http://www.tiket.com/partner/logo/
3. You can change the background coor of the PG by choosing from the color picker or write down the color hexcode.

#### Change the redirect page if payment successful or failed

1. Login first at http://www.tiket.com/affiliate so that you can access the partner area.
2. Click the Developer > API menu http://www.tiket.com/partner/api
3. Write down in the _callback url development_ the link where successful transaction will be redirect. The link must be in HTTPS protocol.
    <aside class="warning">Leave it to empty or <code>https://</code> if you don't have your own payment success page. Changing this to a URL that doesn't exists will redirect the page to a 404 file not found error, confuse user, and user will think that the payment didn't succeed, resulting in complaints and refunds request. Use this with caution!</aside>


### Credit Card Payment

This payment gateway checks you out through our Credit Card payment gateway. We have the best and most secure payment gateway, with fraud rate of only 0.01%. The [average fraud chargeback rate is 0.47%](https://payment-services.ingenico.com/~/media/files/2015-global-online-fraud-panorama_en.ashx?la=en). If fraud accured, you as the developer will **not** be held responsible for the fraud.


#### HTTP Request

`GET http://sandbox.tiket.com/payment/checkout_payment?checkouttoken=84ab8cba79dace1eef8edc7081147b49`

<aside class="notice">Notice that the URL is <code>sandbox.tiket.com</code> for development and <code>www.tiket.com</code> for production.</aside>

#### Parameter

Name | Description | Format    | Default   | Mandatory
--------- | ------- | ----------- | ----------- | -----------
checkouttoken | Token acquired from gettoken | CHAR(128) |  | TRUE

#### Testing cards

For testing purpose in the `sandbox.tiket.com`, you can use the following dummy credit cards:

Variable | Value
------------ | ------------------
Credit Card Number | 4000000000000002
  | 4000000000000119
  |  4000000000000101
  | 4000000000000127
  | 5200000000000007
  | 5200000000000114
  | 5200000000000122
  | 5200000000000106
Expiry Date | Any month and year greater than this month
Card Holder Name | Your own name
CVV  | You can use any 3 digits number

#### Output UI


If you are developing an apps, kindly call the HTTP Request above using WebView. The UI will be like this:

##### Credit Card Checkout Page
![Credit Card Checkout Page](https://raw.githubusercontent.com/tiket-dev/slate/master/source/images/Credit-Card-Payment.png)

Once customer entered the correct information and/or finish their 3DS (3 Domain Security) process, then the result is this output:

##### Successful transaction (web version)
![Success web page](https://raw.githubusercontent.com/tiket-dev/slate/master/source/images/Langkah-2.png)

##### Successful transaction (mobile version)
![Success mobile page](https://raw.githubusercontent.com/tiket-dev/slate/master/source/images/CC-Succesfull-Mobile.png)

<aside class="success">You can redirect the final success (or failed) transaction to your own page by <a href="#general-configuration">changing the redirection URL</a></aside>








### Klikpay Payment

Especially for Klikpay payment, you must access this link:

    `http://sandbox.tiket.com/payment/checkout_payment?checkouttoken=84ab8cba79dace1eef8edc7081147b49&payment_type=4`

#### Output

[![klikpay](http://docs.tiket.com/wp-content/uploads/2013/01/klikpay-300x206.png "klikpay")](http://docs.tiket.com/wp-content/uploads/2013/01/klikpay.png)

- fill the data and you will redirect to page redirection

[![klikpay - redirect](http://docs.tiket.com/wp-content/uploads/2013/01/klikpay-redirect-300x148.png "klikpay - redirect")](http://docs.tiket.com/wp-content/uploads/2013/01/klikpay-redirect.png)

- wait for the page to redirect or press the button to redirect to Klikpay web page

[![KlikPay - web](http://docs.tiket.com/wp-content/uploads/2013/01/KlikPay-web-300x146.png "KlikPay - web")](http://docs.tiket.com/wp-content/uploads/2013/01/KlikPay-web.png)

after finish it will immediately redirect to the callback url (see [PG - General ](http://docs.tiket.com/#pg-general-342))

the defualt link

    `https://www.tiket.com/payment/dummyConfirmPage`

Will be redirected to this link with additional parameters :

    `https://www.tiket.com/payment/dummyConfirmPage?checkouttoken=6c47ff90598a6bf05eb264ee76194cca&orderid=147934&referenceid=147934&message=&paymenttype=klikpay&status=200`

if the variable  
status = 200 => success  
status = 300 => failed

if use the default link (dummyConfirmPage) the view generate to API like usual and read the variable  
diagnostic['status']

* what ever the return (200 or 300) the token cannot be used to order anymore


### CIMB Clicks payment

Especially for CIMB Clicks payment, you must access this link:

    `http://sandbox.tiket.com/payment/checkout_payment?checkouttoken=84ab8cba79dace1eef8edc7081147b49&payment_type=31`

#### Output

[![cimbclicks](http://docs.tiket.com/wp-content/uploads/2013/01/cimbclicks-300x188.png "cimbclicks")](http://docs.tiket.com/wp-content/uploads/2013/01/cimbclicks.png)

- fill the data and you will redirect to page redirection

[![cimbclicks - redirect](http://docs.tiket.com/wp-content/uploads/2013/01/cimbclicks-redirect--300x148.png "cimbclicks - redirect")](http://docs.tiket.com/wp-content/uploads/2013/01/cimbclicks-redirect-.png)

- wait for the page to redirect or press the button to redirect to CIMB Clicks web page

[![](http://docs.tiket.com/wp-content/uploads/2013/01/cimbclicks-web-300x136.png "cimbclicks - web")](http://docs.tiket.com/wp-content/uploads/2013/01/cimbclicks-web.png)



after finish it will immediately redirect to the callback url (see [PG - General ](http://docs.tiket.com/#pg-general-342))

the defualt link

    `https://www.tiket.com/payment/dummyConfirmPage`

Will be redirected to this link with additional parameters :

    `https://www.tiket.com/payment/dummyConfirmPage?checkouttoken=6c47ff90598a6bf05eb264ee76194cca&orderid=147934&referenceid=147934&message=&paymenttype=klikpay&status=200`

if the variable  
status = 200 => success  
status = 300 => failed

if use the default link (dummyConfirmPage) the view generate to API like usual and read the variable  
diagnostic['status']

* what ever the return (200 or 300) the token cannot be used to order anymore


### ePay BRI payment

Especially for ePay BRI payment, you must access this link:

    `http://sandbox.tiket.com/payment/checkout_payment?checkouttoken=84ab8cba79dace1eef8edc7081147b49&payment_type=33`

#### Output

[![ePay BRI](http://docs.tiket.com/wp-content/uploads/2013/01/ePay-BRI--300x195.png "ePay BRI")](http://docs.tiket.com/wp-content/uploads/2013/01/ePay-BRI-.png)

- fill the data and you will redirect to page redirection

[![ePay BRI - redirect](http://docs.tiket.com/wp-content/uploads/2013/01/ePay-BRI-redirect-300x148.png "ePay BRI - redirect")](http://docs.tiket.com/wp-content/uploads/2013/01/ePay-BRI-redirect.png)

- wait for the page to redirect or press the button to redirect to ePay BRI web page

[![ePay BRI - web](http://docs.tiket.com/wp-content/uploads/2013/01/ePay-BRI-web-300x225.png "ePay BRI - web")](http://docs.tiket.com/wp-content/uploads/2013/01/ePay-BRI-web.png)

after finish it will immediately redirect to the callback url (see [PG - General ](http://docs.tiket.com/#pg-general-342))

the defualt link

    `https://www.tiket.com/payment/dummyConfirmPage`

Will be redirected to this link with additional parameters :

    `https://www.tiket.com/payment/dummyConfirmPage?checkouttoken=6c47ff90598a6bf05eb264ee76194cca&orderid=147934&referenceid=147934&message=&paymenttype=klikpay&status=200`

if the variable  
status = 200 => success  
status = 300 => failed

if use the default link (dummyConfirmPage) the view generate to API like usual and read the variable  
diagnostic['status']

* what ever the return (200 or 300) the token cannot be used to order anymore






