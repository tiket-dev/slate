# Event API

NOTE :  
*Data that is provided for testing is different from the actual

These are the API command for Event

Diagram Flow for Event API:  

![Event API](https://raw.githubusercontent.com/tiket-dev/slate/master/source/images/Flow-Event.png)

## Get All Active Events

```xml
    
    	xml
    
    			20875
    			Jason Mraz & His Band: Tour Is A Four Letter Word
    			Online
    
    				http://www.sandbox.tiket.com/img/business/f/e/business-featured-pic1.jpg
    
    				http://www.sandbox.tiket.com/img/business/b/a/business-banner28.jpg
    
    			2012-06-22 20:00:00
    			2012-06-22 23:00:00
    			http://api-sandbox.tiket.com/jasonmraz
    
    		200
    		0.2167
    		15.48MB
    		success
    		en
    		IDR
    
    	c551ad2aee8e7acf14907c0fac2644d9
    
```


```json
{
"output_type": "json",
"events": [{
  "business_id": "20875",
  "business_name": "Jason Mraz & His Band: Tour Is A Four Letter Word",
  "business_live": "Online",
  "file_name": "http:\/\/www.sandbox.tiket.com\/img\/business\/f\/e\/business-featured-pic1.jpg",
  "event_img": "http:\/\/www.sandbox.tiket.com\/img\/business\/b\/a\/business-banner28.jpg",
  "tiket_event_start": "2012-06-22 20:00:00",
  "tiket_event_end": "2012-06-22 23:00:00",
  "event_uri": "http:\/\/api-sandbox.tiket.com\/jasonmraz"
}],
"diagnostic": {
  "status": 200,
  "elapsetime": "0.2583",
  "memoryusage": "15.46MB",
  "confirm": "success",
  "lang": "en",
  "currency": "IDR"
},
"token": "c551ad2aee8e7acf14907c0fac2644d9"
}
```

```matlab
a: 4: {
s: 11: "output_type";s: 9: "serialize";s: 6: "events";a: 1: {
  i: 0;a: 8: {
    s: 11: "business_id";s: 5: "20875";s: 13: "business_name";s: 49: "Jason Mraz & His Band: Tour Is A Four Letter Word";s: 13: "business_live";s: 6: "Online";s: 9: "file_name";s: 73: "http://www.sandbox.tiket.com/img/business/f/e/business-featured-pic1.jpg";s: 9: "event_img";s: 68: "http://www.sandbox.tiket.com/img/business/b/a/business-banner28.jpg";s: 17: "tiket_event_start";s: 19: "2012-06-22 20:00:00";s: 15: "tiket_event_end";s: 19: "2012-06-22 23:00:00";s: 9: "event_uri";s: 39: "http://api-sandbox.tiket.com/jasonmraz";
  }
}
s: 10: "diagnostic";a: 6: {
  s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.3102";s: 11: "memoryusage";s: 14: "15.45MB";s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "en";s: 8: "currency";s: 3: "IDR";
}
s: 5: "token";s: 32: "c551ad2aee8e7acf14907c0fac2644d9";
}
```

#### HTTP Request

    `GET https://api-sandbox.tiket.com/search/event?token=c551ad2aee8e7acf14907c0fac2644d9&output=json`

#### Parameters
  
Name | Description | Format | Default | Mandatory
---- | ----------- | ------ | ------- | ---------  
token | for saving transaction that done by user | CHAR(128) |  | TRUE  

   
    
## Event Detail

```xml
<tiket>
  <output_type>xml</output_type>
  <breadcrumb>
    <business_uri>http://www.sandbox.tiket.com/jasonmraz</business_uri>
    <business_name>Jason Mraz & His Band: Tour Is A Four Letter Word</business_name>
    <kecamatan_name>Kebayoran Baru</kecamatan_name>
    <city_name>Jakarta Selatan</city_name>
    <province_name>DKI Jakarta</province_name>
    <country_name>Indonesia</country_name>
    <continent_name>Asia</continent_name>
  </breadcrumb>
  <event_profile>
    <business_id>20875</business_id>
    <event_type>B</event_type>
    <tiket_event_start>2012-06-22 20:00:00</tiket_event_start>
    <tiket_event_end>2012-06-22 23:00:00</tiket_event_end>
    <date>22 Jun 2012 - 20:00 to 23:00</date>
    <map>
    			http://api-sandbox.tiket.com/img/business/f/e/business-featured-pic1.map.jpg
    		</map>
    <event_type_description>Event hanya berlangsung 1 hari</event_type_description>
    <policy>
      Non-Refundable. Tickets purchased and confirmed cannot be refunded or exchanged
    </policy>
    <policy>
      The payment methods available are Bank Transfer, KlikBCA Online, and Visa/ Master Credit Card
    </policy>
  </event_profile>
  <event_tiket>
    <tiket_id>65</tiket_id>
    <tiket_total_allotment>1000</tiket_total_allotment>
    <tiket_used_allotment>59</tiket_used_allotment>
    <tiket_start_sell>2012-04-16 14:00:00</tiket_start_sell>
    <tiket_end_sell>2012-06-20 23:59:59</tiket_end_sell>
    <tiket_min_purchase>1</tiket_min_purchase>
    <tiket_max_purchase>5</tiket_max_purchase>
    <tiket_required_info>name,idcard</tiket_required_info>
    <tiket_coming_soon>1</tiket_coming_soon>
    <tiket_set_seating>0</tiket_set_seating>
    <tiket_allow_installment>0</tiket_allow_installment>
    <event_status>start</event_status>
    <tiket_price>420000.00</tiket_price>
    <tiket_name>Regular</tiket_name>
  </event_tiket>
  <event_tiket>
    <tiket_id>64</tiket_id>
    <tiket_total_allotment>1000</tiket_total_allotment>
    <tiket_used_allotment>20</tiket_used_allotment>
    <tiket_start_sell>2012-04-16 14:00:00</tiket_start_sell>
    <tiket_end_sell>2012-06-20 23:59:59</tiket_end_sell>
    <tiket_min_purchase>1</tiket_min_purchase>
    <tiket_max_purchase>5</tiket_max_purchase>
    <tiket_required_info>name,idcard</tiket_required_info>
    <tiket_coming_soon>1</tiket_coming_soon>
    <tiket_set_seating>0</tiket_set_seating>
    <tiket_allow_installment>0</tiket_allow_installment>
    <event_status>start</event_status>
    <tiket_price>780000.00</tiket_price>
    <tiket_name>Premium</tiket_name>
  </event_tiket>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.3239</elapsetime>
    <memoryusage>20.04MB</memoryusage>
    <confirm>success</confirm>
    <lang>en</lang>
    <currency>IDR</currency>
  </diagnostic>
  <primary_photos>
    http://www.sandbox.tiket.com/img/business/f/e/business-featured-pic1.crop.jpg
  </primary_photos>
  <event_photos>
    <file_name>
      http://www.sandbox.tiket.com/img/business/j/a/business-jason-mraz-cover-119441.s.jpg
    </file_name>
  </event_photos>
  <event_photos>
    <file_name>
      http://www.sandbox.tiket.com/img/business/j/a/business-jason-mraz-large-msg-1284936098421.s.jpg
    </file_name>
  </event_photos>
  <nearby_hotel>
    <distance>418</distance>
    <business_primary_photo>
      http://www.sandbox.tiket.com/img/business/h/o/business-hotel-sultan.s.jpg
    </business_primary_photo>
    <business_uri>
      http://www.sandbox.tiket.com/the-sultan-hotel-jakarta
    </business_uri>
  </nearby_hotel>
  <nearby_hotel>
    <distance>2070</distance>
    <business_primary_photo>
      http://www.sandbox.tiket.com/img/business/s/w/business-swimming-pool7.s.jpg
    </business_primary_photo>
    <business_uri>http://www.sandbox.tiket.com/kartika-chandra</business_uri>
  </nearby_hotel>
  <token>c551ad2aee8e7acf14907c0fac2644d9</token>
</tiket>
```

```json
{
"output_type": "json",
"breadcrumb": {
  "business_uri": "http:\/\/www.sandbox.tiket.com\/jasonmraz",
  "business_name": "Jason Mraz & His Band: Tour Is A Four Letter Word",
  "kecamatan_name": "Kebayoran Baru",
  "city_name": "Jakarta Selatan",
  "province_name": "DKI Jakarta",
  "country_name": "Indonesia ",
  "continent_name": "Asia"
},
"event_profile": {
  "business_id": "20875",
  "event_type": "B",
  "tiket_event_start": "2012-06-22 20:00:00",
  "tiket_event_end": "2012-06-22 23:00:00",
  "date": "22 Jun 2012 - 20:00 to 23:00",
  "map": "http:\/\/api-sandbox.tiket.com\/img\/business\/f\/e\/business-featured-pic1.map.jpg",
  "event_type_description": "Event hanya berlangsung 1 hari",
  "policy": ["Non-Refundable. Tickets purchased and confirmed cannot be refunded or exchanged", "The payment methods available are Bank Transfer, KlikBCA Online, and Visa\/ Master Credit Card", "Admin Charge Bank Transfer (per unique code, range from IDR 4000 to IDR 5000). You need to transfer the EXACT amount (Including Unique Code) within 3 hours after the booking. Otherwise your Booking will be expired.", "Admin Charge KlikBCA (IDR 5,000)", "Admin Charge Credit Card (3%)", "All customers are obliged to fill Personal Data to make a purchase", "All customers are obliged to bring Identity Card to exchange physical ticket", "Customers who use Credit Card payment method, is obliged to bring ID & Credit Card to exchange ticket (Photocopy is not allowed)", "Ticket sellings could be stopped or started by Tiket.com per promoter (Committee) policy", "Voucher of Tiket.com doesnt function as entry ticket (have to be exchanged with physical ticket)", "Voucher Exchange to Tickets will be done on D-1 at Tiket.com Counter @ BlitzMegaplex in Grand Indonesia, Jakarta (venue can be changed at anytime)"]
},
"event_tiket": [{
  "tiket_id": "65",
  "tiket_total_allotment": "1000",
  "tiket_used_allotment": "59",
  "tiket_start_sell": "2012-04-16 14:00:00",
  "tiket_end_sell": "2012-06-20 23:59:59",
  "tiket_min_purchase": "1",
  "tiket_max_purchase": "5",
  "tiket_required_info": "name,idcard",
  "tiket_coming_soon": "1",
  "tiket_set_seating": "0",
  "tiket_allow_installment": "0",
  "event_status": "start",
  "tiket_price": "420000.00",
  "tiket_name": "Regular"
}, {
  "tiket_id": "64",
  "tiket_total_allotment": "1000",
  "tiket_used_allotment": "20",
  "tiket_start_sell": "2012-04-16 14:00:00",
  "tiket_end_sell": "2012-06-20 23:59:59",
  "tiket_min_purchase": "1",
  "tiket_max_purchase": "5",
  "tiket_required_info": "name,idcard",
  "tiket_coming_soon": "1",
  "tiket_set_seating": "0",
  "tiket_allow_installment": "0",
  "event_status": "start",
  "tiket_price": "780000.00",
  "tiket_name": "Premium"
}],
"diagnostic": {
  "status": 200,
  "elapsetime": "0.3210",
  "memoryusage": "20.01MB",
  "confirm": "success",
  "lang": "en",
  "currency": "IDR"
},
"primary_photos": "http:\/\/www.sandbox.tiket.com\/img\/business\/f\/e\/business-featured-pic1.crop.jpg",
"event_photos": [{
  "file_name": "http:\/\/www.sandbox.tiket.com\/img\/business\/j\/a\/business-jason-mraz-cover-119441.s.jpg"
}, {
  "file_name": "http:\/\/www.sandbox.tiket.com\/img\/business\/j\/a\/business-jason-mraz-large-msg-1284936098421.s.jpg"
}, {
  "file_name": "http:\/\/www.sandbox.tiket.com\/img\/business\/j\/a\/business-jason-mraz121.s.jpg"
}],
"nearby_hotel": [{
  "distance": 418,
  "business_primary_photo": "http:\/\/www.sandbox.tiket.com\/img\/business\/h\/o\/business-hotel-sultan.s.jpg",
  "business_uri": "http:\/\/www.sandbox.tiket.com\/the-sultan-hotel-jakarta"
}, {
  "distance": 2070,
  "business_primary_photo": "http:\/\/www.sandbox.tiket.com\/img\/business\/s\/w\/business-swimming-pool7.s.jpg",
  "business_uri": "http:\/\/www.sandbox.tiket.com\/kartika-chandra"
}, {
  "distance": 1549,
  "business_primary_photo": "http:\/\/www.sandbox.tiket.com\/img\/business\/p\/b\/business-pbanner_somerset_berlian_jakarta_swimming_pool.s.jpg",
  "business_uri": "http:\/\/www.sandbox.tiket.com\/somerset-berlian-jakarta"
}],
"token": "c551ad2aee8e7acf14907c0fac2644d9"
}
```

```matlab
a: 9: {
s: 11: "output_type";s: 9: "serialize";s: 10: "breadcrumb";a: 7: {
  s: 12: "business_uri";s: 39: "http://www.sandbox.tiket.com/jasonmraz";s: 13: "business_name";s: 49: "Jason Mraz & His Band: Tour Is A Four Letter Word";s: 14: "kecamatan_name";s: 14: "Kebayoran Baru";s: 9: "city_name";s: 15: "Jakarta Selatan";s: 13: "province_name";s: 11: "DKI Jakarta";s: 12: "country_name";s: 10: "Indonesia ";s: 14: "continent_name";s: 4: "Asia";
}
s: 13: "event_profile";a: 8: {
  s: 11: "business_id";s: 5: "20875";s: 10: "event_type";s: 1: "B";s: 17: "tiket_event_start";s: 19: "2012-06-22 20:00:00";s: 15: "tiket_event_end";s: 19: "2012-06-22 23:00:00";s: 4: "date";s: 50: "22 Jun 2012 - 20:00 to 23:00";s: 3: "map";s: 77: "http://api-sandbox.tiket.com/img/business/f/e/business-featured-pic1.map.jpg";s: 22: "event_type_description";s: 30: "Event hanya berlangsung 1 hari";s: 6: "policy";a: 11: {
    i: 0;s: 79: "Non-Refundable. Tickets purchased and confirmed cannot be refunded or exchanged";i: 1;s: 93: "The payment methods available are Bank Transfer, KlikBCA Online, and Visa/ Master Credit Card";i: 2;s: 215: "Admin Charge Bank Transfer (per unique code, range from IDR 4000 to IDR 5000). You need to transfer the EXACT amount (Including Unique Code) within 3 hours after the booking. Otherwise your Booking will be expired.";i: 3;s: 32: "Admin Charge KlikBCA (IDR 5,000)";i: 4;s: 29: "Admin Charge Credit Card (3%)";i: 5;s: 66: "All customers are obliged to fill Personal Data to make a purchase";i: 6;s: 76: "All customers are obliged to bring Identity Card to exchange physical ticket";i: 7;s: 128: "Customers who use Credit Card payment method, is obliged to bring ID & Credit Card to exchange ticket (Photocopy is not allowed)";i: 8;s: 88: "Ticket sellings could be stopped or started by Tiket.com per promoter (Committee) policy";i: 9;s: 96: "Voucher of Tiket.com doesnt function as entry ticket (have to be exchanged with physical ticket)";i: 10;s: 146: "Voucher Exchange to Tickets will be done on D-1 at Tiket.com Counter @ BlitzMegaplex in Grand Indonesia, Jakarta (venue can be changed at anytime)";
  }
}
s: 11: "event_tiket";a: 3: {
  i: 0;a: 14: {
    s: 8: "tiket_id";s: 2: "65";s: 21: "tiket_total_allotment";s: 4: "1000";s: 20: "tiket_used_allotment";s: 2: "59";s: 16: "tiket_start_sell";s: 19: "2012-04-16 14:00:00";s: 14: "tiket_end_sell";s: 19: "2012-06-20 23:59:59";s: 18: "tiket_min_purchase";s: 1: "1";s: 18: "tiket_max_purchase";s: 1: "5";s: 19: "tiket_required_info";s: 11: "name,idcard";s: 17: "tiket_coming_soon";s: 1: "1";s: 17: "tiket_set_seating";s: 1: "0";s: 23: "tiket_allow_installment";s: 1: "0";s: 12: "event_status";s: 5: "start";s: 11: "tiket_price";s: 9: "420000.00";s: 10: "tiket_name";s: 7: "Regular";
  }
  i: 1;a: 14: {
    s: 8: "tiket_id";s: 2: "64";s: 21: "tiket_total_allotment";s: 4: "1000";s: 20: "tiket_used_allotment";s: 2: "20";s: 16: "tiket_start_sell";s: 19: "2012-04-16 14:00:00";s: 14: "tiket_end_sell";s: 19: "2012-06-20 23:59:59";s: 18: "tiket_min_purchase";s: 1: "1";s: 18: "tiket_max_purchase";s: 1: "5";s: 19: "tiket_required_info";s: 11: "name,idcard";s: 17: "tiket_coming_soon";s: 1: "1";s: 17: "tiket_set_seating";s: 1: "0";s: 23: "tiket_allow_installment";s: 1: "0";s: 12: "event_status";s: 5: "start";s: 11: "tiket_price";s: 9: "780000.00";s: 10: "tiket_name";s: 7: "Premium";
  }
}
s: 10: "diagnostic";a: 6: {
  s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.3240";s: 11: "memoryusage";s: 14: "20.02MB";s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "en";s: 8: "currency";s: 3: "IDR";
}
s: 14: "primary_photos";s: 78: "http://www.sandbox.tiket.com/img/business/f/e/business-featured-pic1.crop.jpg";s: 12: "event_photos";a: 8: {
  i: 0;a: 1: {
    s: 9: "file_name";s: 85: "http://www.sandbox.tiket.com/img/business/j/a/business-jason-mraz-cover-119441.s.jpg";
  }
  i: 1;a: 1: {
    s: 9: "file_name";s: 96: "http://www.sandbox.tiket.com/img/business/j/a/business-jason-mraz-large-msg-1284936098421.s.jpg";
  }
  i: 2;a: 1: {
    s: 9: "file_name";s: 75: "http://www.sandbox.tiket.com/img/business/j/a/business-jason-mraz121.s.jpg";
  }
}
s: 12: "nearby_hotel";a: 4: {
  i: 0;a: 3: {
    s: 8: "distance";d: 418;s: 22: "business_primary_photo";s: 74: "http://www.sandbox.tiket.com/img/business/h/o/business-hotel-sultan.s.jpg";s: 12: "business_uri";s: 54: "http://www.sandbox.tiket.com/the-sultan-hotel-jakarta";
  }
  i: 1;a: 3: {
    s: 8: "distance";d: 2070;s: 22: "business_primary_photo";s: 76: "http://www.sandbox.tiket.com/img/business/s/w/business-swimming-pool7.s.jpg";s: 12: "business_uri";s: 45: "http://www.sandbox.tiket.com/kartika-chandra";
  }
}
s: 5: "token";s: 32: "c551ad2aee8e7acf14907c0fac2644d9";
}
```
    
Get from event uri at search event

#### HTTP Request

    `GET https://api-sandbox.tiket.com/jasonmraz?token=c551ad2aee8e7acf14907c0fac2644d9&output=json`

#### Parameters
  
Name | Description | Format | Default | Mandatory
---- | ----------- | ------ | ------- | ---------    
token | for saving transaction that done by user | CHAR(128) |  | TRUE  

    
    
## Add Order

```xml
<tiket>
  <output_type>xml</output_type>
  <diagnostic>
    <status>200</status>
    <elapsetime>55.6874</elapsetime>
    <memoryusage>18.61MB</memoryusage>
    <confirm>success</confirm>
    <lang>en</lang>
    <currency>IDR</currency>
  </diagnostic>
  <token>c551ad2aee8e7acf14907c0fac2644d9</token>
</tiket>
```

```json
{
"output_type": "json",
"diagnostic": {
  "status": 200,
  "elapsetime": "56.6093",
  "memoryusage": "18.59MB",
  "confirm": "success",
  "lang": "en",
  "currency": "IDR"
},
"token": " c551ad2aee8e7acf14907c0fac2644d9"
}
```

```matlab
a: 3: {
s: 11: "output_type";s: 9: "serialize";s: 10: "diagnostic";a: 6: {
  s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "71.7911";s: 11: "memoryusage";s: 14: "18.59MB";s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "en";s: 8: "currency";s: 3: "IDR";
}
s: 5: "token";s: 32: " c551ad2aee8e7acf14907c0fac2644d9";
}
```
   

#### HTTP Request

    `GET http://api-sandbox.tiket.com/order/add/event?token=c551ad2aee8e7acf14907c0fac2644d9&qty[64]=1&qty[65]=2&output=json`

#### Parameters

Name | Description | Format | Default | Mandatory
---- | ----------- | ------ | ------- | ---------  
token | for saving transaction that done by user | CHAR(128) |  | TRUE  
qty[tiket_id] | number of tiket that want to order | INT(5) |  | TRUE  


    
## Order

```xml
<tiket>
  <output_type>xml</output_type>
  <myorder>
    <order_id>120163</order_id>
    <data>
    			<uri>jasonmraz</uri>
    			<order_detail_id>31503</order_detail_id>
    			<order_type>event</order_type>
    			<customer_price>780000.00</customer_price>
    			<order_name>Jason Mraz & His Band: Tour Is A Four Letter Word</order_name>
    			<order_name_detail>Premium</order_name_detail>
    			<order_detail_status>active</order_detail_status>
    			<detail>
    				<order_detail_id>31503</order_detail_id>
    				<tiket_barcode>1124217365758</tiket_barcode>
    				<qty>1</qty>
    				<tiket_seating/>
    				<price>780000</price>
    			</detail>
    			<order_photo>
    				http://www.sandbox.tiket.com/img/business/f/e/business-featured-pic1.s.jpg
    			</order_photo>
    			<order_icon>h3d</order_icon>
    			<tax_and_charge>24362.96</tax_and_charge>
    			<subtotal_and_charge>804362.96</subtotal_and_charge>
    			<delete_uri>
    				https://api-sandbox.tiket.com/order/delete_order?order_detail_id=31503
    			</delete_uri>
    		</data>
    <data>
    			<uri>jasonmraz</uri>
    			<order_detail_id>31504</order_detail_id>
    			<order_type>event</order_type>
    			<customer_price>840000.00</customer_price>
    			<order_name>Jason Mraz & His Band: Tour Is A Four Letter Word</order_name>
    			<order_name_detail>Regular</order_name_detail>
    			<order_detail_status>active</order_detail_status>
    			<detail>
    				<order_detail_id>31504</order_detail_id>
    				<tiket_barcode>1697907046485</tiket_barcode>
    				<qty>2</qty>
    				<tiket_seating>,</tiket_seating>
    				<price>840000</price>
    			</detail>
    			<order_photo>
    				http://www.sandbox.tiket.com/img/business/f/e/business-featured-pic1.s.jpg
    			</order_photo>
    			<order_icon>h3d</order_icon>
    			<tax_and_charge>26237.04</tax_and_charge>
    			<subtotal_and_charge>866237.04</subtotal_and_charge>
    			<delete_uri>
    				https://api-sandbox.tiket.com/order/delete_order?order_detail_id=31504
    			</delete_uri>
    		</data>
    <total>1670600</total>
    <total_tax>50600</total_tax>
    <total_without_tax>1620000</total_without_tax>
    <count_installment>0</count_installment>
  </myorder>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.2638</elapsetime>
    <memoryusage>18MB</memoryusage>
    <confirm>success</confirm>
    <lang>en</lang>
    <currency>IDR</currency>
  </diagnostic>
  <checkout>
    https://api-sandbox.tiket.com/order/checkout/120163/IDR
  </checkout>
  <login_status>false</login_status>
  <token>c551ad2aee8e7acf14907c0fac2644d9</token>
</tiket>
```


```json
{
"output_type": "json",
"myorder": {
  "order_id": "120163",
  "data": [{
    "uri": "jasonmraz",
    "order_detail_id": "31503",
    "order_type": "event",
    "customer_price": "780000.00",
    "order_name": "Jason Mraz & His Band: Tour Is A Four Letter Word",
    "order_name_detail": "Premium",
    "order_detail_status": "active",
    "detail": {
      "order_detail_id": "31503",
      "tiket_barcode": "1124217365758",
      "qty": "1",
      "tiket_seating": "",
      "price": 780000
    },
    "order_photo": "http:\/\/www.sandbox.tiket.com\/img\/business\/f\/e\/business-featured-pic1.s.jpg",
    "order_icon": "h3d",
    "tax_and_charge": "24362.96",
    "subtotal_and_charge": "804362.96",
    "delete_uri": "https:\/\/api-sandbox.tiket.com\/order\/delete_order?order_detail_id=31503"
  }, {
    "uri": "jasonmraz",
    "order_detail_id": "31504",
    "order_type": "event",
    "customer_price": "840000.00",
    "order_name": "Jason Mraz & His Band: Tour Is A Four Letter Word",
    "order_name_detail": "Regular",
    "order_detail_status": "active",
    "detail": {
      "order_detail_id": "31504",
      "tiket_barcode": "1697907046485",
      "qty": "2",
      "tiket_seating": " , ",
      "price": 840000
    },
    "order_photo": "http:\/\/www.sandbox.tiket.com\/img\/business\/f\/e\/business-featured-pic1.s.jpg",
    "order_icon": "h3d",
    "tax_and_charge": "26237.04",
    "subtotal_and_charge": "866237.04",
    "delete_uri": "https:\/\/api-sandbox.tiket.com\/order\/delete_order?order_detail_id=31504"
  }],
  "total": 1670600,
  "total_tax": 50600,
  "total_without_tax": 1620000,
  "count_installment": 0
},
"diagnostic": {
  "status": 200,
  "elapsetime": "0.2684",
  "memoryusage": "17.97MB",
  "confirm": "success",
  "lang": "en",
  "currency": "IDR"
},
"checkout": "https:\/\/api-sandbox.tiket.com\/order\/checkout\/120163\/IDR",
"login_status": "false",
"token": "c551ad2aee8e7acf14907c0fac2644d9"
}
```

```matlab
a: 6: {
s: 11: "output_type";s: 9: "serialize";s: 7: "myorder";a: 6: {
  s: 8: "order_id";s: 6: "120163";s: 4: "data";a: 2: {
    i: 0;a: 13: {
      s: 3: "uri";s: 9: "jasonmraz";s: 15: "order_detail_id";s: 5: "31503";s: 10: "order_type";s: 5: "event";s: 14: "customer_price";s: 9: "780000.00";s: 10: "order_name";s: 49: "Jason Mraz & His Band: Tour Is A Four Letter Word";s: 17: "order_name_detail";s: 7: "Premium";s: 19: "order_detail_status";s: 6: "active";s: 6: "detail";a: 5: {
        s: 15: "order_detail_id";s: 5: "31503";s: 13: "tiket_barcode";s: 13: "1124217365758";s: 3: "qty";s: 1: "1";s: 13: "tiket_seating";s: 0: "";s: 5: "price";d: 780000;
      }
      s: 11: "order_photo";s: 75: "http://www.sandbox.tiket.com/img/business/f/e/business-featured-pic1.s.jpg";s: 10: "order_icon";s: 3: "h3d";s: 14: "tax_and_charge";s: 8: "24362.96";s: 19: "subtotal_and_charge";s: 9: "804362.96";s: 10: "delete_uri";s: 71: "https://api-sandbox.tiket.com/order/delete_order?order_detail_id=31503";
    }
    i: 1;a: 13: {
      s: 3: "uri";s: 9: "jasonmraz";s: 15: "order_detail_id";s: 5: "31504";s: 10: "order_type";s: 5: "event";s: 14: "customer_price";s: 9: "840000.00";s: 10: "order_name";s: 49: "Jason Mraz & His Band: Tour Is A Four Letter Word";s: 17: "order_name_detail";s: 7: "Regular";s: 19: "order_detail_status";s: 6: "active";s: 6: "detail";a: 5: {
        s: 15: "order_detail_id";s: 5: "31504";s: 13: "tiket_barcode";s: 13: "1697907046485";s: 3: "qty";s: 1: "2";s: 13: "tiket_seating";s: 3: " , ";s: 5: "price";d: 840000;
      }
      s: 11: "order_photo";s: 75: "http://www.sandbox.tiket.com/img/business/f/e/business-featured-pic1.s.jpg";s: 10: "order_icon";s: 3: "h3d";s: 14: "tax_and_charge";s: 8: "26237.04";s: 19: "subtotal_and_charge";s: 9: "866237.04";s: 10: "delete_uri";s: 71: "https://api-sandbox.tiket.com/order/delete_order?order_detail_id=31504";
    }
  }
  s: 5: "total";d: 1670600;s: 9: "total_tax";d: 50600;s: 17: "total_without_tax";d: 1620000;s: 17: "count_installment";i: 0;
}
s: 10: "diagnostic";a: 6: {
  s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.3170";s: 11: "memoryusage";s: 14: "17.97MB";s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "en";s: 8: "currency";s: 3: "IDR";
}
s: 8: "checkout";s: 56: "https://api-sandbox.tiket.com/order/checkout/120163/IDR";s: 12: "login_status";s: 5: "false";s: 5: "token";s: 32: "c551ad2aee8e7acf14907c0fac2644d9";
}
```

#### HTTP Request

     `GET https://api-sandbox.tiket.com/order?token=c551ad2aee8e7acf14907c0fac2644d9&output=json`

#### Parameters
  
Name | Description | Format | Default | Mandatory
---- | ----------- | ------ | ------- | --------- 
token | for saving transaction that done by user | CHAR(128) |  | TRUE  



    
## Checkout Page Request

```xml
<tiket>
  <output_type>xml</output_type>
  <next_checkout_uri>
    httpsss://api-sandbox.tiket.com/checkout/checkout_customer
  </next_checkout_uri>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.1525</elapsetime>
    <memoryusage>6.46MB</memoryusage>
    <confirm>success</confirm>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <login_status>false</login_status>
  <token>9991e3092aea96042964220181374b60</token>
</tiket>
```

```json
{
"output_type": "json",
"next_checkout_uri": "httpsss:\/\/api-sandbox.tiket.com\/checkout\/checkout_customer",
"diagnostic": {“
  status ":200,"
  elapsetime ":"
  0.1157 ","
  memoryusage ":"
  6.43 MB ","
  confirm ":"
  success ","
  lang ":"
  id ","
  currency ":"
  IDR "},"
  login_status ":"
  false ","
  token ":"
  9991e3092 aea96042964220181374b60 "
 }
 ```

```matlab
a: 5: {
s: 11: "output_type";s: 9: "serialize";s: 17: "next_checkout_uri";s: 57: "httpsss://api-sandbox.tiket.com/checkout/checkout_customer";s: 10: "diagnostic";a: 7: {
  s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.1132";s: 11: "memoryusage";s: 14: "6.43MB";s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "id";s: 8: "currency";s: 3: "IDR";
}
s: 12: "login_status";s: 5: "false";s: 5: "token";s: 32: "9991e3092aea96042964220181374b60";
}
```

Early stage to access checkout.

link url can be get from order, variable checkout.

#### HTTP Request

    `GET https://api-sandbox.tiket.com/order/checkout/119978/IDR?token=9991e3092aea96042964220181374b60&output=json`

#### Parameters

Name | Description | Format | Default | Mandatory
---- | ----------- | ------ | ------- | ---------   
token | for saving transaction that done by user | CHAR(128) |  | TRUE  

    
    
    
## Checkout Login

```xml
<tiket>
  <output_type>xml</output_type>
  <diagnostic>
    <status>200</status>
    <elapsetime>2.0915</elapsetime>
    <memoryusage>10.3MB</memoryusage>
    <confirm>success</confirm>
    <error_msgs/>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <login_status>true</login_status>
  <id>21693</id>
  <token>87da88eaaa429d5513a3a3658b01701e</token>
</tiket>
```

```json
{
"output_type": "json",
"diagnostic": {
  "status": 200,
  "elapsetime": "0.1443",
  "memoryusage": "7.77MB",
  "confirm": "success",
  "error_msgs": "",
  "lang": "en",
  "currency": "IDR"
},
"login_status": "true",
"guest_id": "21688",
"token": "5a80dc2ccce351eeb412e835b651edb9"
}
```

```matlab
a: 5: {
s: 11: "output_type";s: 9: "serialize";s: 10: "diagnostic";a: 7: {
  s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.1628";s: 11: "memoryusage";s: 14: "7.77MB";s: 7: "confirm";s: 7: "success";s: 10: "error_msgs";s: 0: "";s: 4: "lang";s: 2: "en";s: 8: "currency";s: 3: "IDR";
}
s: 12: "login_status";s: 4: "true";s: 8: "guest_id";s: 5: "21688";s: 5: "token";s: 32: "9d4ccf0c966e37a4c112c59ac2bc2e97";
}
```

#### HTTP Request

    `GET https://api-sandbox.tiket.com/checkout/checkout_customer?token=87da88eaaa429d5513a3a3658b01701e&salutation=Ms&firstName=ba&lastName=ca&emailAddress=testing@gmailcom&phone=%2B62878434343&saveContinue=2&output=json`

setelah merequest link tersebut maka user akan dibuatkan account di tiket.com user akan dikirimkan email untuk mengubah password loginnya.

#### Parameters

Name | Description | Format | Default | Mandatory
---- | ----------- | ------ | ------- | --------- 
salutation | your title( ex: Mr., Mrs., Ms.) | CHAR(5) |  | TRUE  
firstName | your first name | CHAR(50) |  | TRUE  
lastName | your last name | CHAR(50) |  | TRUE  
emailAddress | your email | CHAR(50) |  | TRUE  
phone | your phone, ex: 081232323343 or +62324324234234. Don't forget to urlencode + into %2B in the GET parameter | CHAR(20) |  | TRUE  
saveContinue | Flag for login (value=2) |  |  | TRUE  
   
    
## Checkout Customer

```xml
<tiket>
  <output_type>xml</output_type>
  <diagnostic>
    <status>201</status>
    <elapsetime>0.3005</elapsetime>
    <memoryusage>19.44MB</memoryusage>
    <error_msgs>Your Information details have been saved</error_msgs>
    <lang>en</lang>
    <currency>IDR</currency>
  </diagnostic>
  <contactProfileArr>
    <account_id>106238</account_id>
    <account_first_name>cF</account_first_name>
    <account_last_name>cL</account_last_name>
    <account_mobile>021343</account_mobile>
    <account_salutation_name>Mr.</account_salutation_name>
    <account_phone>+62877777</account_phone>
    <account_username>you.jul.in@gmail.com</account_username>
    <profile_id>15781</profile_id>
    <Name>cF cL</Name>
    <address_country/>
    <address_address1/>
    <address_address2/>
    <address_kabupaten/>
    <address_province/>
    <address_zipcode/>
    <account_created>2012-06-11 11:24:28</account_created>
    <account_password>021768c0b31cd2ad68b201213ff0e102</account_password>
    <account_source>tiket</account_source>
    <photo>default-default.jpg</photo>
    <account_profile_modified>2012-06-13 15:28:20</account_profile_modified>
    <account_birthdate/>
    <account_gender>M</account_gender>
    <account_id_card/>
  </contactProfileArr>
  <CustEventArray>
    <tiket_cust_name>ju</tiket_cust_name>
    <tiket_cust_id>1234</tiket_cust_id>
    <tiket_barcode>1697907046485</tiket_barcode>
    <tiket_no_hp>+62878888</tiket_no_hp>
    <tiket_birth_date>1990-01-01</tiket_birth_date>
    <tiket_gender>m</tiket_gender>
  </CustEventArray>
  <statusClass>ok</statusClass>
  <SideArr>
    <currBookingArr>
      <detail_id>31504</detail_id>
      <type>event</type>
      <event_name>Jason Mraz & His Band: Tour Is A Four Letter Word</event_name>
      <tiket_name>Regular</tiket_name>
      <sale_price>420000.00</sale_price>
      <required_info>name,idcard</required_info>
      <photo>
        http://www.sandbox.tiket.com/img/business/f/e/business-featured-pic1.m.jpg
      </photo>
    </currBookingArr>
  </SideArr>
  <login_status>true</login_status>
  <id>106238</id>
  <token>c551ad2aee8e7acf14907c0fac2644d9</token>
</tiket>
```

```json
{
"output_type": "json",
"diagnostic": {
  "status": 201,
  "elapsetime": "0.3038",
  "memoryusage": "19.42MB",
  "error_msgs": "Your Information details have been saved",
  "lang": "en",
  "currency": "IDR"
},
"contactProfileArr": {
  "account_id": "106238",
  "account_first_name": "cF",
  "account_last_name": "cL",
  "account_mobile": "021343",
  "account_salutation_name": "Mr.",
  "account_phone": "+62877777",
  "account_username": "you.jul.in@gmail.com",
  "profile_id": "15782",
  "Name": "cF cL",
  "address_country": null,
  "address_address1": null,
  "address_address2": null,
  "address_kabupaten": null,
  "address_province": null,
  "address_zipcode": null,
  "account_created": "2012-06-11 11:24:28",
  "account_password": "021768c0b31cd2ad68b201213ff0e102",
  "account_source": "tiket",
  "photo": "default-default.jpg",
  "account_profile_modified": "2012-06-13 15:29:09",
  "account_birthdate": null,
  "account_gender": "M",
  "account_id_card": null
},
"CustEventArray": [{
  "tiket_cust_name": "ju",
  "tiket_cust_id": "1234",
  "tiket_barcode": "1697907046485",
  "tiket_no_hp": "+62878888",
  "tiket_birth_date": "1990-01-01",
  "tiket_gender": "m"
}],
"next": "http:\/\/api-sandbox.tiket.com\/checkout\/checkout_payment",
"statusClass": "ok",
"SideArr": {
  "currBookingArr": {
    "detail_id": "31504",
    "type": "event",
    "event_name": "Jason Mraz & His Band: Tour Is A Four Letter Word",
    "tiket_name": "Regular",
    "sale_price": "420000.00",
    "required_info": "name,idcard",
    "photo": "http:\/\/www.sandbox.tiket.com\/img\/business\/f\/e\/business-featured-pic1.m.jpg"
  }
},
"login_status": "true",
"id": "106238",
"token": "c551ad2aee8e7acf14907c0fac2644d9"
}
```

```matlab
a: 9: {
s: 11: "output_type";s: 9: "serialize";s: 10: "diagnostic";a: 6: {
  s: 6: "status";i: 201;s: 10: "elapsetime";s: 14: "0.2986";s: 11: "memoryusage";s: 14: "19.42MB";s: 10: "error_msgs";s: 29: "Your Information details have been saved";s: 4: "lang";s: 2: "en";s: 8: "currency";s: 3: "IDR";
}
s: 17: "contactProfileArr";a: 23: {
  s: 10: "account_id";s: 6: "106238";s: 18: "account_first_name";s: 2: "cF";s: 17: "account_last_name";s: 2: "cL";s: 14: "account_mobile";s: 6: "021343";s: 23: "account_salutation_name";s: 3: "Mr.";s: 13: "account_phone";s: 5: "08777";s: 16: "account_username";s: 20: "you.jul.in@gmail.com";s: 10: "profile_id";s: 5: "15783";s: 4: "Name";s: 5: "cF cL";s: 15: "address_country";N;s: 16: "address_address1";N;s: 16: "address_address2";N;s: 17: "address_kabupaten";N;s: 16: "address_province";N;s: 15: "address_zipcode";N;s: 15: "account_created";s: 19: "2012-06-11 11:24:28";s: 16: "account_password";s: 32: "021768c0b31cd2ad68b201213ff0e102";s: 14: "account_source";s: 5: "tiket";s: 5: "photo";s: 19: "default-default.jpg";s: 24: "account_profile_modified";s: 19: "2012-06-13 15:29:52";s: 17: "account_birthdate";N;s: 14: "account_gender";s: 1: "M";s: 15: "account_id_card";N;
}
s: 14: "CustEventArray";a: 1: {
  i: 0;a: 6: {
    s: 15: "tiket_cust_name";s: 2: "ju";s: 13: "tiket_cust_id";s: 4: "1234";s: 13: "tiket_barcode";s: 13: "1697907046485";s: 11: "tiket_no_hp";s: 5: "08788";s: 16: "tiket_birth_date";s: 10: "1990-01-01";s: 12: "tiket_gender";s: 1: "m";
  }
}
s: 11: "statusClass";s: 2: "ok";s: 7: "SideArr";a: 1: {
  s: 14: "currBookingArr";a: 7: {
    s: 9: "detail_id";s: 5: "31504";s: 4: "type";s: 5: "event";s: 10: "event_name";s: 49: "Jason Mraz & His Band: Tour Is A Four Letter Word";s: 10: "tiket_name";s: 7: "Regular";s: 10: "sale_price";s: 9: "420000.00";s: 13: "required_info";s: 11: "name,idcard";s: 5: "photo";s: 75: "http://www.sandbox.tiket.com/img/business/f/e/business-featured-pic1.m.jpg";
  }
}
s: 12: "login_status";s: 4: "true";s: 2: "id";s: 6: "106238";s: 5: "token";s: 32: "c551ad2aee8e7acf14907c0fac2644d9";
}
```

#### HTTP Request

     `GET http://api-sandbox.tiket.com/checkout/checkout_customer?token=c551ad2aee8e7acf14907c0fac2644d9&conSalutation=Mr.&conFirstName=cF&conLastName=cL&conEmailAddress=cE@yahoo.com&conPhone=%2B62877777&name=ju&idCard=1234&noHp=%2B62878888&gender=m&birthDate=1990-01-01&detailId=31504&output=json`

#### Parameters

Name | Description | Format | Default | Mandatory
---- | ----------- | ------ | ------- | ---------  
token | for saving transaction that done by user | CHAR(128) |  | TRUE  
conSalutation | contact person title ( ex: Mr., Mrs., Ms.) | CHAR(5) |  | TRUE  
conFirstName | contact person first name | CHAR(50) |  | TRUE  
conLastName |contact person last name | CHAR(50) |  | TRUE  
conEmailAddress | contact person email address | CHAR(50) |  | TRUE  
conPhone | contact person phone, ex: 081232323343 or +62324324234234. Don't forget to urlencode + into %2B in the GET parameter | CHAR(20) |  | TRUE  
name | Customer name | CHAR(50) |  | TRUE  
idCard | Customer Id card | CHAR(50) |  | TRUE  
noHp | Customer phone number | CHAR(20) |  | TRUE  
gender | Customer gender | CHAR(5) |  | TRUE  
birthDate | Customer birth date | DATE |  | TRUE  
detailId | your order detail id | NUMBER |  | TRUE   

    
    
## Available Payment

```xml
<tiket>
  <output_type>xml</output_type>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.5620</elapsetime>
    <memoryusage>18.77MB</memoryusage>
    <confirm>success</confirm>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <available_payment>
    <link> https://api-sandbox.tiket.com/checkout/checkout_payment/1
    </link>
    <text>Kartu Kredit</text>
    <message/>
  </available_payment>
  <available_payment>
    <link> https://api-sandbox.tiket.com/checkout/checkout_payment/2
    </link>
    <text>Transfer Lewat Bank</text>
    <message/>
  </available_payment>
  <available_payment>
    <link> https://api-sandbox.tiket.com/checkout/checkout_payment/3
    </link>
    <text>KlikBCA</text>
    <message/>
  </available_payment>
  <available_payment>
    <link> https://api-sandbox.tiket.com/checkout/checkout_payment/4
    </link>
    <text>BCA KlikPay</text>
    <message/>
  </available_payment>
  <available_payment>
    <link> https://api-sandbox.tiket.com/checkout/checkout_payment/20
    </link>
    <text>COD</text>
    <message/>
  </available_payment>
  <token>62bc0e3bd0c127c5690125a76e11c23c</token>
</tiket>
```


```json
{
"output_type": "json",
"diagnostic": {
  "status": 200,
  "elapsetime": "0.5625",
  "memoryusage": "18.74MB",
  "confirm": "success",
  "lang": "id",
  "currency": "IDR"
},
"available_payment": [{
  "link": "https:\/\/api-sandbox.tiket.com\/checkout\/checkout_payment\/1",
  "text": "Kartu Kredit",
  "message": ""
}, {
  "link": "https:\/\/api-sandbox.tiket.com\/checkout\/checkout_payment\/2",
  "text": "Transfer Lewat Bank",
  "message": ""
}, {
  "link": "https:\/\/api-sandbox.tiket.com\/checkout\/checkout_payment\/3",
  "text": "KlikBCA",
  "message": ""
}, {
  "link": "https:\/\/api-sandbox.tiket.com\/checkout\/checkout_payment\/4",
  "text": "BCA KlikPay",
  "message": ""
}, {
  "link": "https:\/\/api-sandbox.tiket.com\/checkout\/checkout_payment\/20",
  "text": "COD",
  "message": ""
}],
"token": "62bc0e3bd0c127c5690125a76e11c23c"
}
```


```matlab
a: 4: {
s: 11: "output_type";s: 9: "serialize";s: 10: "diagnostic";a: 6: {
  s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.5329";s: 11: "memoryusage";s: 14: "18.74MB";s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "id";s: 8: "currency";s: 3: "IDR";
}
s: 17: "available_payment";a: 5: {
  i: 0;a: 3: {
    s: 4: "link";s: 58: "https://api-sandbox.tiket.com/checkout/checkout_payment/1";s: 4: "text";s: 22: "Kartu Kredit";s: 7: "message";s: 0: "";
  }
  i: 1;a: 3: {
    s: 4: "link";s: 58: "https://api-sandbox.tiket.com/checkout/checkout_payment/2";s: 4: "text";s: 24: "Transfer Lewat Bank";s: 7: "message";s: 0: "";
  }
  i: 2;a: 3: {
    s: 4: "link";s: 58: "https://api-sandbox.tiket.com/checkout/checkout_payment/3";s: 4: "text";s: 7: "KlikBCA";s: 7: "message";s: 0: "";
  }
  i: 3;a: 3: {
    s: 4: "link";s: 58: "https://api-sandbox.tiket.com/checkout/checkout_payment/4";s: 4: "text";s: 11: "BCA KlikPay";s: 7: "message";s: 0: "";
  }
  i: 4;a: 3: {
    s: 4: "link";s: 59: "https://api-sandbox.tiket.com/checkout/checkout_payment/20";s: 4: "text";s: 3: "COD";s: 7: "message";s: 0: "";
  }
}
s: 5: "token";s: 32: "62bc0e3bd0c127c5690125a76e11c23c";
}
```
    

#### HTTP Request

     `GET http://api-sandbox.tiket.com/checkout/checkout_payment?token=87da88eaaa429d5513a3a3658b01701e`

#### Parameters

Name | Description | Format | Default | Mandatory
---- | ----------- | ------ | ------- | --------- 
token | for saving transaction that done by user | CHAR(128) |  | TRUE  


  
## Checkout Payment

    Please see [Checkout Payment](http://docs.tiket.com/#checkout-payment-309) in General API
    





















