# Order History

## Check Order

```xml
<?xml version="1.0" encoding="utf-8"?>
<tiket>
    <diagnostic>
        <status>200</status>
        <elapsetime>0.1624</elapsetime>
        <memoryusage>4.81MB</memoryusage>
        <unix_timestamp>1470298252</unix_timestamp>
        <confirm>success</confirm>
        <lang>id</lang>
        <currency>IDR</currency>
    </diagnostic>
    <output_type>xml</output_type>
    <result>
        <order_id>22385759</order_id>
        <order_timestamp>2016-08-04 14:54:02</order_timestamp>
        <payment_timestamp></payment_timestamp>
        <payment_status>shoppingcart</payment_status>
        <total_customer_price>1261250.00</total_customer_price>
        <customer_currency>IDR</customer_currency>
        <mobile_phone></mobile_phone>
        <all_order_type>flight</all_order_type>
        <order__cart_detail>
            <order_detail_id>12742815</order_detail_id>
            <order_type>flight</order_type>
            <order_name>SUB (Surabaya) - LOP (Lombok, Mataram)</order_name>
            <order_name_detail>Citilink (QG-664 - Depart)</order_name_detail>
            <customer_currency>IDR</customer_currency>
            <customer_price>631760.00</customer_price>
            <total_ticket>1</total_ticket>
            <detail>
                <order_timestamp>2016-08-04 14:54:02</order_timestamp>
                <mobile_phone></mobile_phone>
                <order_detail_status>recheck</order_detail_status>
                <order_expire_datetime>2016-08-04 14:49:10</order_expire_datetime>
                <flight_number>QG 664</flight_number>
                <trip>trip</trip>
                <airlines_name>CITILINK</airlines_name>
                <departure_city>SUB</departure_city>
                <departure_time>2016-08-05 09:25:00</departure_time>
                <arrival_city>LOP</arrival_city>
                <arrival_time>2016-08-05 11:30:00</arrival_time>
                <ticket_class>F</ticket_class>
                <booking_code></booking_code>
                <count_adult>1</count_adult>
                <count_child>0</count_child>
                <count_infant>0</count_infant>
                <contact_title>Mr</contact_title>
                <contact_first_name>roni</contact_first_name>
                <contact_phone>+85642020047</contact_phone>
                <contact_other_phone></contact_other_phone>
                <ticket_status>booked</ticket_status>
                <depart_airport>Juanda</depart_airport>
                <arrival_airport>Lombok</arrival_airport>
            </detail>
            <passanger>
                <passanger_baggage>20</passanger_baggage>
                <passenger_name>Mr jodi wiguna</passenger_name>
                <passenger_age_group>adult</passenger_age_group>
                <passenger_id_number></passenger_id_number>
                <passenger_birth_date></passenger_birth_date>
                <passenger_ticket_number></passenger_ticket_number>
            </passanger>
            <check_in_baggage>20</check_in_baggage>
        </order__cart_detail>
        <order__cart_detail>
            <order_detail_id>12742817</order_detail_id>
            <order_type>flight</order_type>
            <order_name>LOP (Lombok, Mataram) - SUB (Surabaya)</order_name>
            <order_name_detail>Citilink (QG-665 - Return)</order_name_detail>
            <customer_currency>IDR</customer_currency>
            <customer_price>601760.00</customer_price>
            <total_ticket>1</total_ticket>
            <detail>
                <order_timestamp>2016-08-04 14:54:02</order_timestamp>
                <mobile_phone></mobile_phone>
                <order_detail_status>recheck</order_detail_status>
                <order_expire_datetime>2016-08-04 14:49:10</order_expire_datetime>
                <flight_number>QG 665</flight_number>
                <trip>round</trip>
                <airlines_name>CITILINK</airlines_name>
                <departure_city>LOP</departure_city>
                <departure_time>2016-08-06 12:00:00</departure_time>
                <arrival_city>SUB</arrival_city>
                <arrival_time>2016-08-06 12:15:00</arrival_time>
                <ticket_class>F</ticket_class>
                <booking_code></booking_code>
                <count_adult>1</count_adult>
                <count_child>0</count_child>
                <count_infant>0</count_infant>
                <contact_title>Mr</contact_title>
                <contact_first_name>roni</contact_first_name>
                <contact_phone>+85642020047</contact_phone>
                <contact_other_phone></contact_other_phone>
                <ticket_status>booked</ticket_status>
                <depart_airport>Lombok</depart_airport>
                <arrival_airport>Juanda</arrival_airport>
            </detail>
            <passanger>
                <passanger_baggage>20</passanger_baggage>
                <passenger_name>Mr jodi wiguna</passenger_name>
                <passenger_age_group>adult</passenger_age_group>
                <passenger_id_number></passenger_id_number>
                <passenger_birth_date></passenger_birth_date>
                <passenger_ticket_number></passenger_ticket_number>
            </passanger>
        </order__cart_detail>
    </result>
    <login_status>false</login_status>
    <token>8d977ca39cfc63a83e73f6bd24fb33d11df3f039</token>
</tiket>
```



```json
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.1345",
    "memoryusage": "4.8MB",
    "unix_timestamp": 1470297986,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "result": {
    "order_id": "22385759",
    "order_timestamp": "2016-08-04 14:54:02",
    "payment_timestamp": null,
    "payment_status": "shoppingcart",
    "total_customer_price": "1261250.00",
    "customer_currency": "IDR",
    "mobile_phone": null,
    "all_order_type": "flight",
    "order__cart_detail": [
      {
        "order_detail_id": "12742815",
        "order_type": "flight",
        "order_name": "SUB (Surabaya) - LOP (Lombok, Mataram)",
        "order_name_detail": "Citilink (QG-664 - Depart)",
        "customer_currency": "IDR",
        "customer_price": "631760.00",
        "total_ticket": "1",
        "detail": {
          "order_timestamp": "2016-08-04 14:54:02",
          "mobile_phone": null,
          "order_detail_status": "recheck",
          "order_expire_datetime": "2016-08-04 14:49:10",
          "flight_number": "QG 664",
          "trip": "trip",
          "airlines_name": "CITILINK",
          "departure_city": "SUB",
          "departure_time": "2016-08-05 09:25:00",
          "arrival_city": "LOP",
          "arrival_time": "2016-08-05 11:30:00",
          "ticket_class": "F",
          "booking_code": "",
          "count_adult": "1",
          "count_child": "0",
          "count_infant": "0",
          "contact_title": "Mr",
          "contact_first_name": "roni",
          "contact_phone": "+85642020047",
          "contact_other_phone": "",
          "ticket_status": "booked",
          "depart_airport": "Juanda",
          "arrival_airport": "Lombok"
        },
        "passanger": [
          {
            "passanger_baggage": "20",
            "passenger_name": "Mr jodi wiguna",
            "passenger_age_group": "adult",
            "passenger_id_number": "",
            "passenger_birth_date": "",
            "passenger_ticket_number": ""
          }
        ],
        "check_in_baggage": 20
      },
      {
        "order_detail_id": "12742817",
        "order_type": "flight",
        "order_name": "LOP (Lombok, Mataram) - SUB (Surabaya)",
        "order_name_detail": "Citilink (QG-665 - Return)",
        "customer_currency": "IDR",
        "customer_price": "601760.00",
        "total_ticket": "1",
        "detail": {
          "order_timestamp": "2016-08-04 14:54:02",
          "mobile_phone": null,
          "order_detail_status": "recheck",
          "order_expire_datetime": "2016-08-04 14:49:10",
          "flight_number": "QG 665",
          "trip": "round",
          "airlines_name": "CITILINK",
          "departure_city": "LOP",
          "departure_time": "2016-08-06 12:00:00",
          "arrival_city": "SUB",
          "arrival_time": "2016-08-06 12:15:00",
          "ticket_class": "F",
          "booking_code": "",
          "count_adult": "1",
          "count_child": "0",
          "count_infant": "0",
          "contact_title": "Mr",
          "contact_first_name": "roni",
          "contact_phone": "+85642020047",
          "contact_other_phone": "",
          "ticket_status": "booked",
          "depart_airport": "Lombok",
          "arrival_airport": "Juanda"
        },
        "passanger": [
          {
            "passanger_baggage": "20",
            "passenger_name": "Mr jodi wiguna",
            "passenger_age_group": "adult",
            "passenger_id_number": "",
            "passenger_birth_date": "",
            "passenger_ticket_number": ""
          }
        ]
      }
    ],
    "order__payment": [],
    "order__confirmation": []
  },
  "login_status": "false",
  "token": "d5826dae6485a4a67f49eb2a3ab11552fe07e7c4"
}
```



```matlab
a:5:{s:10:"diagnostic";a:7:{s:6:"status";i:200;s:10:"elapsetime";s:14:"0.1386";s:11:"memoryusage";s:14:"4.8MB";s:14:"unix_timestamp";i:1470298315;s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:11:"output_type";s:9:"serialize";s:6:"result";a:11:{s:8:"order_id";s:8:"22385759";s:15:"order_timestamp";s:19:"2016-08-04 14:54:02";s:17:"payment_timestamp";N;s:14:"payment_status";s:12:"shoppingcart";s:20:"total_customer_price";s:10:"1261250.00";s:17:"customer_currency";s:3:"IDR";s:12:"mobile_phone";N;s:14:"all_order_type";s:6:"flight";s:18:"order__cart_detail";a:2:{i:0;a:10:{s:15:"order_detail_id";s:8:"12742815";s:10:"order_type";s:6:"flight";s:10:"order_name";s:38:"SUB (Surabaya) - LOP (Lombok, Mataram)";s:17:"order_name_detail";s:26:"Citilink (QG-664 - Depart)";s:17:"customer_currency";s:3:"IDR";s:14:"customer_price";s:9:"631760.00";s:12:"total_ticket";s:1:"1";s:6:"detail";a:23:{s:15:"order_timestamp";s:19:"2016-08-04 14:54:02";s:12:"mobile_phone";N;s:19:"order_detail_status";s:7:"recheck";s:21:"order_expire_datetime";s:19:"2016-08-04 14:49:10";s:13:"flight_number";s:6:"QG 664";s:4:"trip";s:4:"trip";s:13:"airlines_name";s:8:"CITILINK";s:14:"departure_city";s:3:"SUB";s:14:"departure_time";s:19:"2016-08-05 09:25:00";s:12:"arrival_city";s:3:"LOP";s:12:"arrival_time";s:19:"2016-08-05 11:30:00";s:12:"ticket_class";s:1:"F";s:12:"booking_code";s:0:"";s:11:"count_adult";s:1:"1";s:11:"count_child";s:1:"0";s:12:"count_infant";s:1:"0";s:13:"contact_title";s:2:"Mr";s:18:"contact_first_name";s:4:"roni";s:13:"contact_phone";s:12:"+85642020047";s:19:"contact_other_phone";s:0:"";s:13:"ticket_status";s:6:"booked";s:14:"depart_airport";s:6:"Juanda";s:15:"arrival_airport";s:6:"Lombok";}s:9:"passanger";a:1:{i:0;a:6:{s:17:"passanger_baggage";s:2:"20";s:14:"passenger_name";s:14:"Mr jodi wiguna";s:19:"passenger_age_group";s:5:"adult";s:19:"passenger_id_number";s:0:"";s:20:"passenger_birth_date";s:0:"";s:23:"passenger_ticket_number";s:0:"";}}s:16:"check_in_baggage";i:20;}i:1;a:9:{s:15:"order_detail_id";s:8:"12742817";s:10:"order_type";s:6:"flight";s:10:"order_name";s:38:"LOP (Lombok, Mataram) - SUB (Surabaya)";s:17:"order_name_detail";s:26:"Citilink (QG-665 - Return)";s:17:"customer_currency";s:3:"IDR";s:14:"customer_price";s:9:"601760.00";s:12:"total_ticket";s:1:"1";s:6:"detail";a:23:{s:15:"order_timestamp";s:19:"2016-08-04 14:54:02";s:12:"mobile_phone";N;s:19:"order_detail_status";s:7:"recheck";s:21:"order_expire_datetime";s:19:"2016-08-04 14:49:10";s:13:"flight_number";s:6:"QG 665";s:4:"trip";s:5:"round";s:13:"airlines_name";s:8:"CITILINK";s:14:"departure_city";s:3:"LOP";s:14:"departure_time";s:19:"2016-08-06 12:00:00";s:12:"arrival_city";s:3:"SUB";s:12:"arrival_time";s:19:"2016-08-06 12:15:00";s:12:"ticket_class";s:1:"F";s:12:"booking_code";s:0:"";s:11:"count_adult";s:1:"1";s:11:"count_child";s:1:"0";s:12:"count_infant";s:1:"0";s:13:"contact_title";s:2:"Mr";s:18:"contact_first_name";s:4:"roni";s:13:"contact_phone";s:12:"+85642020047";s:19:"contact_other_phone";s:0:"";s:13:"ticket_status";s:6:"booked";s:14:"depart_airport";s:6:"Lombok";s:15:"arrival_airport";s:6:"Juanda";}s:9:"passanger";a:1:{i:0;a:6:{s:17:"passanger_baggage";s:2:"20";s:14:"passenger_name";s:14:"Mr jodi wiguna";s:19:"passenger_age_group";s:5:"adult";s:19:"passenger_id_number";s:0:"";s:20:"passenger_birth_date";s:0:"";s:23:"passenger_ticket_number";s:0:"";}}}}s:14:"order__payment";a:0:{}s:19:"order__confirmation";a:0:{}}s:12:"login_status";s:5:"false";s:5:"token";s:40:"6c3f752418315d67c3165a1af8a17b9d0ea89b49";}
```


Check Transaction detail


#### HTTP Request

`https://api-sandbox.tiket.com/check_order?order_id=22385759&email=wida.skydev@gmail.com&output=xml&secretkey=24qwe2141bb031a22ef6b623c93a8dc9`

    
#### Parameters

  
Name | Description | Format | Default | Mandatory  
---- | ----------- | -----  | ------- | -----------
email | customer email | VARCHAR | getToken | TRUE  
order_id | order id want to check | NUMERIC | getToken | TRUE  
secretkey | API secret key given by Tiket.com | CHAR(128) | | TRUE  






    
    
