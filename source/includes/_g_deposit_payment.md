# Deposit Payment

There are 2 tipe of payment method

1. **Regular Payment**  
    Payment handled by Tiket.com
2. **Deposit Payment**
    Payment handled by partner

The default of the payment method is **Regular payment**. To change to **Deposit payment** please follow the instructions below:

1. Register your business in https://sandbox.tiket.com/affiliate/
2. Login with the credentials inputed before
3. Go to main menu : 'API' and change the 'Payment Method' from 'Regular' to 'Deposit'.
4. To top up your deposit, go to main menu : 'Saldo' and click button 'Top Up' on upper right.  
    For development you don't need to transfer the money for the deposit and please top up for bigger number like IDR 500,000,000 so you can use it many times for development.
5. Send us your 'Business ID', 'Order ID', and the invoice for your top up for us to approve the top up.


## Set Payment method

Login to:

* production : [www.tiket.com/partner/login](https://www.tiket.com/partner/login)  
* development : [sandbox.tiket.com/partner/login](https://sandbox.tiket.com/partner/login)

go to menu setting, change payment methode to "Deposit"

[![set payment methode](http://docs.tiket.com/wp-content/uploads/2012/11/payment-methode-300x199.png "set payment method")](http://docs.tiket.com/wp-content/uploads/2012/11/payment-methode.png)


## Top Up

Go to menu **Saldo** and then **Top up**

[![top up](http://docs.tiket.com/wp-content/uploads/2012/11/top-up-300x171.png "top up")](http://docs.tiket.com/wp-content/uploads/2012/11/top-up.png)

After top up request, the request should appear in the pending deposit.
For **Development** environment, kindly **directly** email to support@tiket.com for us to approve the deposit payment request.

[![](http://docs.tiket.com/wp-content/uploads/2012/11/waiting-confirm-300x38.png "waiting confirm")](http://docs.tiket.com/wp-content/uploads/2012/11/waiting-confirm.png)

**klikbca**  
after payment it will directly success top up

**bank transfer** (if development please use this),  
you must confirm payment

[![](http://docs.tiket.com/wp-content/uploads/2012/11/confirm-banktransfer-300x202.png "confirm banktransfer")](http://docs.tiket.com/wp-content/uploads/2012/11/confirm-banktransfer.png)

after confirm payment, please wait for our customer service to approve the payment (for development environment, please inform us to through [support@tiket.com](support@tiket.com))

After we approve your payment, you will see your **saldo** topped up.

[![](http://docs.tiket.com/wp-content/uploads/2012/11/success-topup-300x146.png "success topup")](http://docs.tiket.com/wp-content/uploads/2012/11/success-topup.png)


## Check Deposit Balance


```xml
<tiket>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.3991</elapsetime>
    <memoryusage>13.52MB</memoryusage>
    <confirm>success</confirm>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <output_type>xml</output_type>
  <results>1035151.00</results>
  <login_status>false</login_status>
  <token>bafeb06cc887594c1657b6bdcbfd513e</token>
</tiket>
```



```json
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.3516",
    "memoryusage": "13.48MB",
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "results": "1035151.00",
  "login_status": "false",
  "token": "bafeb06cc887594c1657b6bdcbfd513e"
}
```



```matlab
a: 5: {
  s: 10: "diagnostic";a: 6: {
    s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.3394";s: 11: "memoryusage";s: 14: "13.48MB";s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "id";s: 8: "currency";s: 3: "IDR";
  }
  s: 11: "output_type";s: 9: "serialize";s: 7: "results";s: 10: "1035151.00";s: 12: "login_status";s: 5: "false";s: 5: "token";s: 32: "bafeb06cc887594c1657b6bdcbfd513e";
}
```


You can use this request if you want to see your deposit balance.


#### HTTP Request

`http://api-sandbox.tiket.com/partner/transactionApi/get_saldo?secretkey=[your-secret-key-here]&confirmkey=[CONFIRM_KEY]&username=[USERNAME]`


#### Parameters

Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------
secretkey | API secret key given by Tiket.com | CHAR(128) |  | TRUE  
confirmkey | confirmkey given by Tiket.com | CHAR(128) |  | TRUE  
username | your username as the one who link to the business | VARCHAR(20) |  | TRUE  


## Checkout payment using deposit


```xml
<tiket>
  <output_type>xml</output_type>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.6053</elapsetime>
    <memoryusage>14.73MB</memoryusage>
    <confirm>success</confirm>
    <lang>en</lang>
    <currency>IDR</currency>
  </diagnostic>
  <orderId>148847</orderId>
  <message>
    Please transfer the payment to make a booking. You have
    <strong>3 hours</strong> to complete the payment.
  </message>
  <grand_total>250000</grand_total>
  <token>902c1966b790400c2abdce91615019eb</token>
</tiket>
```



```json
{
  output_type: "json",
  diagnostic: {
    status: 200,
    elapsetime: "0.5665",
    memoryusage: "14.69MB",
    confirm: "success",
    lang: "en",
    currency: "IDR"
  },
  orderId: 148848,

  message: "Please transfer the payment to make a booking. You have <strong>3 hours</strong> to complete the 		payment.",
  grand_total: 250000,
  token: "05de09951056763af4b49e7a9ba5229c"
}
```



```matlab
a: 6: {
  s: 11: "output_type";s: 9: "serialize";s: 10: "diagnostic";a: 6: {
    s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.6324";s: 11: "memoryusage";s: 14: "14.69MB";s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "en";s: 8: "currency";s: 3: "IDR";
  }
  s: 7: "orderId";i: 148849;s: 7: "message";s: 35: "Please transfer the payment to make a booking. You have 3 hours to complete the payment.";s: 11: "grand_total";d: 250000;s: 5: "token";s: 32: "90e00ce63c00b92616ca15c7e6ef28d1";
}
```


You can use this request if you want to pay the current user's transaction using your deposit.


#### HTTP Request

    `http://api-sandbox.tiket.com/checkout/checkout_payment/8?btn_booking=1&token=d69843dde291670e75bce3434300f821&output=json`


#### Parameters

  
Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------
token | for saving transaction that done by user | CHAR(128) |  | TRUE  
btn_booking | flag for continue | INT | TRUE  



    
    
## Check Transaction through Tiket.com website

Information about the transactions using your deposit can be accessed at the **Transaction** menu when you access the affiliate administration.

You can do some activity such a **resend voucher**.

[![](http://docs.tiket.com/wp-content/uploads/2012/11/confirm-transaction-300x167.png "confirm transaction")](http://docs.tiket.com/wp-content/uploads/2012/11/confirm-transaction.png)


## Show transaction by API

```xml
<tiket>
  <output_type>xml</output_type>
  <result>
    <order_id>154250</order_id>
    <account_id>105970</account_id>
    <order_timestamp>2012-12-06 16:17:35</order_timestamp>
    <payment_status>checkout</payment_status>
    <total_customer_price>350000.00</total_customer_price>
    <customer_currency>IDR</customer_currency>
    <account_username>you_julin@yahoo.com</account_username>
    <all_order_type>hotel</all_order_type>
    <account_salutation_name>Mr.</account_salutation_name>
    <name>Juli Ami</name>
    <account_phone>087526332</account_phone>
    <order_cart_detail>
      <order_detail_id>36901</order_detail_id>
      <order_type>hotel</order_type>
      <customer_currency>IDR</customer_currency>
      <customer_price>350000.00</customer_price>
      <order_detail_status>active</order_detail_status>
      <total_ticket>1</total_ticket>
      <description>Resort: Hotel Testing (Deluxe Room), For 1 Night</description>
    </order_cart_detail>
    <price>IDR 350.000,00</price>
    <confirm_uri>
      https://api-sandbox.tiket.com/partner/transactionApi/confirmPayment? account_id=105970&order_id=154250&order_type=hotel&price=350000.00&account_username=you_julin@yahoo.com
    </confirm_uri>
    <status>confirm</status>
  </result>
  <search>
    <page>1</page>
    <offset>20</offset>
    <total_data>1</total_data>
    <total_page>1</total_page>
    <startdate>2012-11-05</startdate>
    <enddate>2012-12-06</enddate>
    <searchId/>
  </search>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.3279</elapsetime>
    <memoryusage>10MB</memoryusage>
    <confirm>success</confirm>
    <lang>en</lang>
    <currency>IDR</currency>
  </diagnostic>
  <token>73af5d205a8d9c41efbb1aeeb1462644</token>
</tiket>
```



```json
{
  output_type: "json",
  result: [{
    order_id: "154250",
    account_id: "105970",
    order_timestamp: "2012-12-06 16:17:35",
    payment_status: "checkout",
    total_customer_price: "350000.00",
    customer_currency: "IDR",
    account_username: "you_julin@yahoo.com",
    all_order_type: "hotel",
    account_salutation_name: "Mr.",
    name: "Juli Ami",
    account_phone: "087526332",
    order_cart_detail: [{
      order_detail_id: "36901",
      order_type: "hotel",
      customer_currency: "IDR",
      customer_price: "350000.00",
      order_detail_status: "active",
      total_ticket: "1",
      description: "Resort: Hotel Testing (Deluxe Room), For 1 Night"
    }],
    price: "IDR 350.000,00",
    confirm_uri: "https://api-sandbox.tiket.com/partner/transactionApi/confirmPayment?		account_id=105970&order_id=154250&order_type=hotel&price=350000.00&account_username=you_julin@yahoo.com",
    status: "confirm"
  }],
  search: {
    page: 1,
    offset: 20,
    total_data: 1,
    total_page: 1,
    startdate: "2012-11-05",
    enddate: "2012-12-06",
    searchId: ""
  },
  diagnostic: {
    status: 200,
    elapsetime: "0.3289",
    memoryusage: "9.99MB",
    confirm: "success",
    lang: "en",
    currency: "IDR"
  },
  token: "73af5d205a8d9c41efbb1aeeb1462644"
}
```

```matlab
a: 5: {
  s: 11: "output_type";s: 9: "serialize";s: 6: "result";a: 1: {
    i: 0;a: 15: {
      s: 8: "order_id";s: 6: "154250";s: 10: "account_id";s: 6: "105970";s: 15: "order_timestamp";s: 19: "2012-12-06 16:17:35";s: 14: "payment_status";s: 8: "checkout";s: 20: "total_customer_price";s: 9: "350000.00";s: 17: "customer_currency";s: 3: "IDR";s: 16: "account_username";s: 19: "you_julin@yahoo.com";s: 14: "all_order_type";s: 5: "hotel";s: 23: "account_salutation_name";s: 3: "Mr.";s: 4: "name";s: 8: "Juli Ami";s: 13: "account_phone";s: 9: "087526332";s: 17: "order_cart_detail";a: 1: {
        i: 0;a: 7: {
          s: 15: "order_detail_id";s: 5: "36901";s: 10: "order_type";s: 5: "hotel";s: 17: "customer_currency";s: 3: "IDR";s: 14: "customer_price";s: 9: "350000.00";s: 19: "order_detail_status";s: 6: "active";s: 12: "total_ticket";s: 1: "1";s: 11: "description";s: 48: "Resort: Hotel Testing (Deluxe Room), For 1 Night";
        }
      }
      s: 5: "price";s: 14: "IDR 350.000,00";s: 11: "confirm_uri";s: 172: "https://api-sandbox.tiket.com/partner/transactionApi/confirmPayment?account_id=105970&order_id=154250&order_type=hotel&price=350000.00&account_username=you_julin@yahoo.com";s: 6: "status";s: 7: "confirm";
    }
  }
  s: 6: "search";a: 7: {
    s: 4: "page";i: 1;s: 6: "offset";i: 20;s: 10: "total_data";i: 1;s: 10: "total_page";d: 1;s: 9: "startdate";s: 10: "2012-11-05";s: 7: "enddate";s: 10: "2012-12-06";s: 8: "searchId";s: 0: "";
  }
  s: 10: "diagnostic";a: 6: {
    s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.3691";s: 11: "memoryusage";s: 14: "9.99MB";s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "en";s: 8: "currency";s: 3: "IDR";
  }
  s: 5: "token";s: 32: "73af5d205a8d9c41efbb1aeeb1462644";
}
```


To see the list of deposit transaction.

#### HTTP Request

`GET http://api-sandbox.tiket.com/partner/transactionApi?secretkey=[your-secret-key-here]&confirmkey=7c4d3b&username=youraffiliate@email.com&output=json`

#### Parameters

  
Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------
secretkey | secretkey given by Tiket.com | CHAR(128) |  | TRUE  
confirmkey | confirmkey given by Tiket.com | CHAR(128) |  | TRUE  
username | your username as the one who link to the business | CHAR(128) |  | TRUE  


    
## Confirm Transaction by API

```xml
<tiket>
  <output_type>xml</output_type>
  <diagnostic>
    <status>200</status>
    <elapsetime>2.5284</elapsetime>
    <memoryusage>20.31MB</memoryusage>
    <confirm>success</confirm>
    <lang>en</lang>
    <currency>IDR</currency>
  </diagnostic>
  <token>feb69563ac764ae38276376b8bcbc71f</token>
</tiket>
```

```json
{
  output_type: "json",
  diagnostic: {
    status: "200",
    elapsetime: "0.8818",
    memoryusage: "17.56MB",
    confirm: "success",
    lang: "en",
    currency: "IDR"
  },
  token: "feb69563ac764ae38276376b8bcbc71f"
}
```

```matlab
a: 3: {
    s: 11: "output_type";s: 9: "serialize";s: 10: "diagnostic";a: 6: {
      s: 6: "status";s: 3: "200";s: 10: "elapsetime";s: 14: "1.2691";s: 11: "memoryusage";s: 14: "17.56MB";s: 10: "confirm";s: 39: "success";s: 4: "lang";s: 2: "en";s: 8: "currency";s: 3: "IDR";
    }
    s: 5: "token";s: 32: "feb69563ac764ae38276376b8bcbc71f"
```


Link get from confirm_uri in show transaction by API

#### HTTP Request

`GET https://api-sandbox.tiket.com/partner/transactionApi/confirmPayment?order_id=154250&secretkey=[your-secret-key-here]&confirmkey=7c4d3b&username=you_julin@yahoo.com&textarea_note=test&tanggal=2012-12-06&output=json`

#### Parameters

Name | Description | Format | Default | Mandatory 
---- | ----------  | -----  | ------- | ---------
order_id | for customer order id | CHAR(128) |  | TRUE  
textarea_note | note for the confirmation | CHAR(128) |  | TRUE  
tanggal | confirmation date | YYYY-MM-DD |  | TRUE  
secretkey | secretkey given by Tiket.com | CHAR(128) |  | TRUE  
confirmkey | confirmkey given by Tiket.com | CHAR(128) |  | TRUE  
username | your username as the one who link to the business | CHAR(128) |  | TRUE  








