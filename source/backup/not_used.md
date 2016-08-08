## Get All Flight Routes


```xml
<?xml version="1.0" encoding="UTF-8"?>
<tiket>
  <diagnostic>
    <status>200</status>
    <elapsetime>2.5933</elapsetime>
    <memoryusage>24.52MB</memoryusage>
    <confirm>success</confirm>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <output_type>xml</output_type>
  <allroute>
    <from>BPN</from>
    <from_en />
    <from_id />
    <to>DPS</to>
    <to_en />
    <to_id />
    <airlines>SRIWIJAYA</airlines>
    <last_update>2013-12-04 06:25:01</last_update>
  </allroute>
  <allroute>
    <from>CGK</from>
    <from_en />
    <from_id />
    <to>DIL</to>
    <to_en />
    <to_id />
    <airlines>SRIWIJAYA,MERPATI</airlines>
    <last_update>2013-12-03 22:51:08</last_update>
  </allroute>
  <allroute>
    <from>$D</from>
    <from_en />
    <from_id />
    <to>$A</to>
    <to_en />
    <to_id />
    <airlines />
    <last_update>2013-12-06 18:52:48</last_update>
  </allroute>
  <allroute>
    <from>(POPULAR)</from>
    <from_en />
    <from_id />
    <to>CGK</to>
    <to_en>Soekarno-Hatta International Airport</to_en>
    <to_id>Bandara Internasional Soekarno-Hatta</to_id>
    <airlines />
    <last_update>2013-12-02 08:14:56</last_update>
  </allroute>
  <allroute>
    <from>ABU</from>
    <from_en />
    <from_id />
    <to>KOE</to>
    <to_en>El Tari Airport</to_en>
    <to_id>Bandara El Tari</to_id>
    <airlines>MERPATI</airlines>
    <last_update>2013-11-15 14:07:05</last_update>
  </allroute>
  <allroute>
    <from>ADL</from>
    <from_en />
    <from_id />
    <to>DPS</to>
    <to_en>Ngurah Rai International Airport</to_en>
    <to_id>Bandara Internasional Ngurah Rai</to_id>
    <airlines>LION</airlines>
    <last_update>2013-12-15 09:39:29</last_update>
  </allroute>
  <login_status>true</login_status>
  <id>19845295</id>
  <token>6a95beb8efe5fb601824430a12826c48</token>
</tiket>
```

```json
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "1.0039",
    "memoryusage": "23.45MB",
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "allroute": [{
    "from": " BPN",
    "from_en": null,
    "from_id": null,
    "to": " DPS",
    "to_en": null,
    "to_id": null,
    "airlines": "SRIWIJAYA",
    "last_update": "2013-12-04 06:25:01"
  }, {
    "from": " CGK",
    "from_en": null,
    "from_id": null,
    "to": " DIL",
    "to_en": null,
    "to_id": null,
    "airlines": "SRIWIJAYA,MERPATI",
    "last_update": "2013-12-03 22:51:08"
  }, {
    "from": "$D",
    "from_en": null,
    "from_id": null,
    "to": "$A",
    "to_en": null,
    "to_id": null,
    "airlines": "",
    "last_update": "2013-12-06 18:52:48"
  }],
  "login_status": "true",
  "id": "19845295",
  "token": "6a95beb8efe5fb601824430a12826c48"
}
```



```matlab
a: 6: {
  s: 10: "diagnostic";a: 6: {
    s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.9392";s: 11: "memoryusage";s: 14: "24.64MB";s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "id";s: 8: "currency";s: 3: "IDR";
  }
  s: 11: "output_type";s: 9: "serialize";s: 8: "allroute";a: 10166: {
    i: 0;a: 8: {
      s: 4: "from";s: 4: " BPN";s: 7: "from_en";N;s: 7: "from_id";N;s: 2: "to";s: 4: " DPS";s: 5: "to_en";N;s: 5: "to_id";N;s: 8: "airlines";s: 9: "SRIWIJAYA";s: 11: "last_update";s: 19: "2013-12-04 06:25:01";
    }
    i: 1;a: 8: {
      s: 4: "from";s: 4: " CGK";s: 7: "from_en";N;s: 7: "from_id";N;s: 2: "to";s: 4: " DIL";s: 5: "to_en";N;s: 5: "to_id";N;s: 8: "airlines";s: 17: "SRIWIJAYA,MERPATI";s: 11: "last_update";s: 19: "2013-12-03 22:51:08";
    }
    i: 2;a: 8: {
      s: 4: "from";s: 2: "$D";s: 7: "from_en";N;s: 7: "from_id";N;s: 2: "to";s: 2: "$A";s: 5: "to_en";N;s: 5: "to_id";N;s: 8: "airlines";s: 0: "";s: 11: "last_update";s: 19: "2013-12-06 18:52:48";
    }
    i: 3;a: 8: {
      s: 4: "from";s: 9: "(POPULAR)";s: 7: "from_en";N;s: 7: "from_id";N;s: 2: "to";s: 3: "CGK";s: 5: "to_en";s: 36: "Soekarno-Hatta International Airport";s: 5: "to_id";s: 36: "Bandara Internasional Soekarno-Hatta";s: 8: "airlines";s: 0: "";s: 11: "last_update";s: 19: "2013-12-02 08:14:56";
    }
    i: 4;a: 8: {
      s: 4: "from";s: 3: "ABU";s: 7: "from_en";N;s: 7: "from_id";N;s: 2: "to";s: 3: "KOE";s: 5: "to_en";s: 15: "El Tari Airport";s: 5: "to_id";s: 15: "Bandara El Tari";s: 8: "airlines";s: 7: "MERPATI";s: 11: "last_update";s: 19: "2013-11-15 14:07:05";
    }
  }
  s: 12: "login_status";s: 4: "true";s: 2: "id";s: 8: "19845295";s: 5: "token";s: 32: "6a95beb8efe5fb601824430a12826c48";
}
```

List of all available flight routes

#### HTTP Request

`GET https://api-sandbox.tiket.com/flight_api/getAllRouteList?token=6a95beb8efe5fb601824430a12826c48`

#### Parameters

Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------
token | for saving transaction that done by user | CHAR(128) |  | TRUE  


## Search Hotel Promo

```xml
   This XML file does not appear to have any style information associated with it. The document tree is shown below.
<tiket>
  <output_type>xml</output_type>
  <search_queries>
    <q>Indonesia</q>
    <startdate>2012-11-23</startdate>
    <enddate>2012-11-30</enddate>
  </search_queries>
  <pagination>
    <total_found>5</total_found>
    <current_page>1</current_page>
    <offset>10</offset>
    <last_page>1</last_page>
  </pagination>
  <results>
    <result>
      <regional>Ubud - Ubud - Bali</regional>
      <price>IDR 345.519,00</price>
      <province_name>Bali</province_name>
      <deal_startdate>2012-11-20 00:00:00</deal_startdate>
      <deal_enddate>2012-11-26 23:59:59</deal_enddate>
      <room_name>Deluxe AC</room_name>
      <travel_startdate>2012-10-20</travel_startdate>
      <travel_enddate>2012-12-19</travel_enddate>
      <booking_startdate>0000-00-00</booking_startdate>
      <booking_enddate>0000-00-00</booking_enddate>
      <id>129881</id>
      <room_available>2</room_available>
      <star_rating>1</star_rating>
      <business_uri>
        https://api.tiket.com/hotel/indonesia/gianyar/pande-permai-bungalow?startdate=2012-11- 23&enddate=2012-11- 24&night=1&room=1&adult=2&child=0&business_id%5B0%5D=22707&business_id%5B1%5D=129881&business_id%5B2%5D=2923&business_id%5B3%5D=117990&business_id%5B4%5D=233&business_id%5B5%5D=43&business_id%5B6%5D=15668&business_id%5B7%5D=86&uid=business%3A129881
      </business_uri>
      <photo_primary>
        http://www.tiket.com/img/business/i/m/business-img_0041.featured322x147.jpg
      </photo_primary>
      <promo_name>Discount 15%</promo_name>
      <name>Pande Permai Bungalow</name>
    </result>
    <result>
      <regional>Melintang - Rangkui - Kepulauan Bangka-Belitung</regional>
      <price>IDR 384.705,00</price>
      <province_name>Kepulauan Bangka-Belitung</province_name>
      <deal_startdate>2012-11-19 00:00:00</deal_startdate>
      <deal_enddate>2012-11-25 23:59:59</deal_enddate>
      <room_name>Superior</room_name>
      <travel_startdate>2012-10-17</travel_startdate>
      <travel_enddate>2012-11-30</travel_enddate>
      <booking_startdate>0000-00-00</booking_startdate>
      <booking_enddate>0000-00-00</booking_enddate>
      <id>2923</id>
      <room_available>3</room_available>
      <star_rating>3</star_rating>
      <business_uri>
        https://api.tiket.com/hotel/indonesia/bangka-tengah/hotel-santika-bangka?startdate=2012-11-23&enddate=2012-11-24&night=1&room=1&adult=2&child=0&business_id%5B0%5D=22707&business_id%5B1%5D=129881&business_id%5B2%5D=2923&business_id%5B3%5D=117990&business_id%5B4%5D=233&business_id%5B5%5D=43&business_id%5B6%5D=15668&business_id%5B7%5D=86&uid=business%3A2923
      </business_uri>
      <photo_primary>
        http://www.tiket.com/img/business/s/a/business-santika-bangka_L.featured322x147.jpg
      </photo_primary>
      <promo_name>Discount 10%</promo_name>
      <name>Hotel Santika Bangka</name>
    </result>
  </results>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.7366</elapsetime>
    <memoryusage>8.94MB</memoryusage>
    <confirm>success</confirm>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <token>b21ff0ede5de530e35ecb99f2b3cd3b2</token>
</tiket>

```

```json
{
  "output_type": "json",
  "search_queries": {
    "q": "Indonesia",
    "startdate": "2012-11-23",
    "enddate": "2012-11-30"
  },
  "pagination": {
    "total_found": 5,
    "current_page": 1,
    "offset": 10,
    "last_page": 1
  },
  "results": {
    "result": [{
      "regional": "Ubud - Ubud - Bali",
      "price": "IDR 345.519,00",
      "province_name": "Bali",
      "deal_startdate": "2012-11-20 00:00:00",
      "deal_enddate": "2012-11-26 23:59:59",
      "room_name": "Deluxe AC",
      "travel_startdate": "2012-10-20",
      "travel_enddate": "2012-12-19",
      "booking_startdate": "0000-00-00",
      "booking_enddate": "0000-00-00",
      "id": "129881",
      "room_available": "2",
      "star_rating": "1",
      "business_uri": "https:\/\/api.tiket.com\/hotel\/indonesia\/gianyar\/pande-permai-bungalow?startdate=2012-11-23&enddate=2012-11-24&night=1&room=1&adult=2&child=0&business_id%5B0%5D=22707&business_id%5B1%5D=129881&business_id%5B2%5D=2923&business_id%5B3%5D=117990&business_id%5B4%5D=233&business_id%5B5%5D=43&business_id%5B6%5D=15668&business_id%5B7%5D=86&uid=business%3A129881",
      "photo_primary": "http:\/\/www.tiket.com\/img\/business\/i\/m\/business-img_0041.featured322x147.jpg",
      "promo_name": "Discount  15%",
      "name": "Pande Permai Bungalow"
    }, {
      "regional": "Melintang - Rangkui - Kepulauan Bangka-Belitung",
      "price": "IDR 384.705,00",
      "province_name": "Kepulauan Bangka-Belitung",
      "deal_startdate": "2012-11-19 00:00:00",
      "deal_enddate": "2012-11-25 23:59:59",
      "room_name": "Superior",
      "travel_startdate": "2012-10-17",
      "travel_enddate": "2012-11-30",
      "booking_startdate": "0000-00-00",
      "booking_enddate": "0000-00-00",
      "id": "2923",
      "room_available": "3",
      "star_rating": "3",
      "business_uri": "https:\/\/api.tiket.com\/hotel\/indonesia\/bangka-tengah\/hotel-santika-bangka?startdate=2012-11-23&enddate=2012-11-24&night=1&room=1&adult=2&child=0&business_id%5B0%5D=22707&business_id%5B1%5D=129881&business_id%5B2%5D=2923&business_id%5B3%5D=117990&business_id%5B4%5D=233&business_id%5B5%5D=43&business_id%5B6%5D=15668&business_id%5B7%5D=86&uid=business%3A2923",
      "photo_primary": "http:\/\/www.tiket.com\/img\/business\/s\/a\/business-santika-bangka_L.featured322x147.jpg",
      "promo_name": "Discount  10%",
      "name": "Hotel Santika Bangka"
    }]
  },
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.6928",
    "memoryusage": "8.95MB",
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "token": "b21ff0ede5de530e35ecb99f2b3cd3b2"
}

```

```matlab
a: 6: {
  s: 11: "output_type";s: 9: "serialize";s: 14: "search_queries";a: 3: {
    s: 1: "q";s: 9: "Indonesia";s: 9: "startdate";s: 10: "2012-11-23";s: 7: "enddate";s: 10: "2012-11-30";
  }
  s: 10: "pagination";a: 4: {
    s: 11: "total_found";i: 5;s: 12: "current_page";i: 1;s: 6: "offset";i: 10;s: 9: "last_page";d: 1;
  }
  s: 7: "results";a: 1: {
    s: 6: "result";i: 2;a: 17: {
      s: 8: "regional";s: 47: "Melintang - Rangkui - Kepulauan Bangka-Belitung";s: 5: "price";s: 14: "IDR 384.705,00";s: 13: "province_name";s: 25: "Kepulauan Bangka-Belitung";s: 14: "deal_startdate";s: 19: "2012-11-19 00:00:00";s: 12: "deal_enddate";s: 19: "2012-11-25 23:59:59";s: 9: "room_name";s: 8: "Superior";s: 16: "travel_startdate";s: 10: "2012-10-17";s: 14: "travel_enddate";s: 10: "2012-11-30";s: 17: "booking_startdate";s: 10: "0000-00-00";s: 15: "booking_enddate";s: 10: "0000-00-00";s: 2: "id";s: 4: "2923";s: 14: "room_available";s: 1: "3";s: 11: "star_rating";s: 1: "3";s: 12: "business_uri";s: 356: "https://api.tiket.com/hotel/indonesia/bangka-tengah/hotel-santika-bangka?startdate=2012-11-23&enddate=2012-11-24&night=1&room=1&adult=2&child=0&business_id%5B0%5D=22707&business_id%5B1%5D=129881&business_id%5B2%5D=2923&business_id%5B3%5D=117990&business_id%5B4%5D=233&business_id%5B5%5D=43&business_id%5B6%5D=15668&business_id%5B7%5D=86&uid=business%3A2923";s: 13: "photo_primary";s: 83: "http://www.tiket.com/img/business/s/a/business-santika-bangka_L.featured322x147.jpg";s: 10: "promo_name";s: 13: "Discount 10%";s: 4: "name";s: 20: "Hotel Santika Bangka";
    }
    i: 3;a: 17: {
      s: 8: "regional";s: 47: "Gili Trawangan - Pemenang - Nusa Tenggara Barat";s: 5: "price";s: 16: "IDR 1.526.516,00";s: 13: "province_name";s: 19: "Nusa Tenggara Barat";s: 14: "deal_startdate";s: 19: "2012-11-19 00:00:00";s: 12: "deal_enddate";s: 19: "2012-11-25 23:59:59";s: 9: "room_name";s: 24: "Superior Lumbung Terrace";s: 16: "travel_startdate";s: 10: "2012-09-11";s: 14: "travel_enddate";s: 10: "2012-09-30";s: 17: "booking_startdate";s: 10: "0000-00-00";s: 15: "booking_enddate";s: 10: "0000-00-00";s: 2: "id";s: 6: "117990";s: 14: "room_available";s: 2: "62";s: 11: "star_rating";s: 1: "4";s: 12: "business_uri";s: 353: "https://api.tiket.com/hotel/indonesia/lombok-utara/hotel-vila-ombak?startdate=2012-11-23&enddate=2012-11-24&night=1&room=1&adult=2&child=0&business_id%5B0%5D=22707&business_id%5B1%5D=129881&business_id%5B2%5D=2923&business_id%5B3%5D=117990&business_id%5B4%5D=233&business_id%5B5%5D=43&business_id%5B6%5D=15668&business_id%5B7%5D=86&uid=business%3A117990";s: 13: "photo_primary";s: 78: "http://www.tiket.com/img/business/l/a/business-large-fromt.featured322x147.jpg";s: 10: "promo_name";s: 22: "Last Minute Offer 15%";s: 4: "name";s: 16: "Hotel Vila Ombak";
    }
  }
  s: 10: "diagnostic";a: 6: {
    s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "1.0974";s: 11: "memoryusage";s: 14: "8.95MB";s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "id";s: 8: "currency";s: 3: "IDR";
  }
  s: 5: "token";s: 32: "b21ff0ede5de530e35ecb99f2b3cd3b2";
}

```

#### HTTP Request

    `GET https://api-sandbox.tiket.com/home/hotelDeals?token=28a6c5f0882a94a078e82ffdb1df7744&output=json`


#### Parameters
  
Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------  
token | for saving transaction that done by user | CHAR(128) |  | TRUE  
page | pagging page | INT |  | FALSE  
startdate | startdate for hotel promo | INT |  | FALSE  
enddate | enddate for hotel promo | INT |  | FALSE



//===============
## Search Hotel

```xml
<tiket>
  <output_type>xml</output_type>
  <diagnostic>
    <status>200</status>
    <elapsetime>2.2848</elapsetime>
    <memoryusage>19.61MB</memoryusage>
    <confirm>success</confirm>
    <lang>en</lang>
    <currency>IDR</currency>
  </diagnostic>
  <search_queries>
    <q>Indonesia</q>
    <uid/>
    <startdate>2012-06-11</startdate>
    <enddate>2012-06-12</enddate>
    <night>1</night>
    <room>1</room>
    <adult>2</adult>
    <child>0</child>
  </search_queries>
  <result>
    <id>2556003619</id>
    <latitude>-0.152117</latitude>
    <longitude>2.010164</longitude>
    <business_uri>
      https://api-sandbox.tiket.com/the-101-legian?startdate=2012-06-11&enddate=2012-06-12&night=1&room=1&adult=2&child=0&uid=business%3A4108
    </business_uri>
    <province_name>Bali</province_name>
    <kecamatan_name>Kuta</kecamatan_name>
    <kelurahan_name>Legian</kelurahan_name>
    <photo_primary>
      https://www.sandbox.tiket.com/img/business/s/k/business-sky_pool.sq2.jpg
    </photo_primary>
    <room_facility_name>
      Non smoking rooms|In room safe|Air conditioning|Internet access – LAN (complimentary)|Television LCD/plasma screen|Desk|Shower|Bathrobes|Hair dryer|Mini bar|Complimentary bottled water|Television|Telephone|Slipper|Iron board on request|Hair dryer on request|Include
      Breakfast
    </room_facility_name>
    <wifi>Wi-Fi available</wifi>
    <promo_name/>
    <price>478080.00</price>
    <regional>Legian - Kuta - Bali</regional>
    <rating/>
    <name>The 101 Legian</name>
    <address>Jalan Hayam Wuruk Raya No.79B Jakarta - Indonesia
     , Taman Sari, Jakarta Barat</address>
  </result>
  <result>
    <id>2696265251</id>
    <latitude>-0.151962</latitude>
    <longitude>2.010245</longitude>
    <business_uri>
      https://api-sandbox.tiket.com/the-sunset-hotel-bali?startdate=2012-06-11&enddate=2012-06-12&night=1&room=1&adult=2&child=0&uid=business%3A3623
    </business_uri>
    <province_name>Bali</province_name>
    <kecamatan_name/>
    <kelurahan_name/>
    <photo_primary>
      https://www.sandbox.tiket.com/img/business/s/u/business-sunset-hotel-001.sq2.jpg
    </photo_primary>
    <room_facility_name/>
    <wifi/>
    <promo_name/>
    <price>377318.00</price>
    <regional>Bali</regional>
    <rating/>
    <name>The Sunset Bali Hotel</name>
    <address>Jalan Hayam Wuruk Raya No.79B Jakarta - Indonesia
     , Taman Sari, Jakarta Barat</address>
  </result>
  <token>1c78d7bc29690cd96dfce9e0350cfc51</token>
</tiket>
```

```json
{
  "output_type": "json",
  "diagnostic": {
    "status": 200,
    "elapsetime": "2.0788",
    "memoryusage": "19.58MB",
    "confirm": "success",
    "lang": "en",
    "currency": "IDR"
  },
  "search_queries": {
    "q": "Indonesia",
    "uid": "",
    "startdate": "2012-06-11",
    "enddate": "2012-06-12",
    "night": "1",
    "room": "1",
    "adult": "2",
    "child": 0
  },
  "result": [{
    "id": "2556003619",
    "latitude": "-0.152117",
    "longitude": "2.010164",
    "business_uri": "https:\/\/api-sandbox.tiket.com\/the-101-legian?startdate=2012-06-11&enddate=2012-06-12&night=1&room=1&adult=2&child=0&uid=business%3A4108",
    "province_name": "Bali",
    "kecamatan_name": "Kuta",
    "kelurahan_name": "Legian",
    "photo_primary": "http:\/\/www.sandbox.tiket.com\/img\/business\/s\/k\/business-sky_pool.sq2.jpg",
    "room_facility_name": "Non smoking rooms|In room safe|Air conditioning|Internet access â€“ LAN (complimentary)|%hotel_lcd\/plasma%|Desk|Shower|Bathrobes|Hair dryer|Mini bar|Complimentary bottled water|Television|Telephone|Slipper|Iron board on request|Hair dryer on request|Include Breakfast",
    "wifi": "Wi-Fi available",
    "promo_name": "",
    "price": "478080.00",
    "regional": "Legian - Kuta - Bali",
    "rating": "",
    "name": "The 101 Legian"
  }, {
    "id": "2696265251",
    "latitude": "-0.151962",
    "longitude": "2.010245",
    "business_uri": "https:\/\/api-sandbox.tiket.com\/the-sunset-hotel-bali?startdate=2012-06-11&enddate=2012-06-12&night=1&room=1&adult=2&child=0&uid=business%3A3623",
    "province_name": "Bali",
    "kecamatan_name": "",
    "kelurahan_name": "",
    "photo_primary": "http:\/\/www.sandbox.tiket.com\/img\/business\/s\/u\/business-sunset-hotel-001.sq2.jpg",
    "room_facility_name": null,
    "wifi": "",
    "promo_name": "",
    "price": "377318.00",
    "regional": "Bali",
    "rating": "",
    "name": "The Sunset Bali Hotel"
  }],
  "token": "1c78d7bc29690cd96dfce9e0350cfc51"
}```


```matlab
a: 5: {
  s: 11: "output_type";s: 9: "serialize";s: 10: "diagnostic";a: 6: {
    s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "2.3215";s: 11: "memoryusage";s: 14: "19.26MB";s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "en";s: 8: "currency";s: 3: "IDR";
  }
  s: 14: "search_queries";a: 8: {
    s: 1: "q";s: 9: "Indonesia";s: 3: "uid";s: 0: "";s: 9: "startdate";s: 10: "2012-06-11";s: 7: "enddate";s: 10: "2012-06-12";s: 5: "night";s: 1: "1";s: 4: "room";s: 1: "1";s: 5: "adult";s: 1: "2";s: 5: "child";i: 0;
  }
  s: 6: "result";a: 15: {
    i: 0;a: 15: {
      s: 2: "id";s: 10: "2556003619";s: 8: "latitude";s: 9: "-0.152117";s: 9: "longitude";s: 8: "2.010164";s: 12: "business_uri";s: 135: "https://api-sandbox.tiket.com/the-101-legian?startdate=2012-06-11&enddate=2012-06-12&night=1&room=1&adult=2&child=0&uid=business%3A4108";s: 13: "province_name";s: 4: "Bali";s: 14: "kecamatan_name";s: 4: "Kuta";s: 14: "kelurahan_name";s: 6: "Legian";s: 13: "photo_primary";s: 72: "http://www.sandbox.tiket.com/img/business/s/k/business-sky_pool.sq2.jpg";s: 18: "room_facility_name";s: 347: "Non smoking rooms|In room safe|Air conditioning|Internet access â€“ LAN (complimentary)|Television LCD/plasma screen|Desk|Shower|Bathrobes|Hair dryer|Mini bar|Complimentary bottled water|Television|Telephone|Slipper|Iron board on request|Hair dryer on request|Include Breakfast";s: 4: "wifi";s: 23: "Wi-Fi available";s: 10: "promo_name";s: 0: "";s: 5: "price";s: 9: "478080.00";s: 8: "regional";s: 20: "Legian - Kuta - Bali";s: 6: "rating";s: 0: "";s: 4: "name";s: 14: "The 101 Legian";
    }
    i: 1;a: 15: {
      s: 2: "id";s: 10: "2696265251";s: 8: "latitude";s: 9: "-0.151962";s: 9: "longitude";s: 8: "2.010245";s: 12: "business_uri";s: 142: "https://api-sandbox.tiket.com/the-sunset-hotel-bali?startdate=2012-06-11&enddate=2012-06-12&night=1&room=1&adult=2&child=0&uid=business%3A3623";s: 13: "province_name";s: 4: "Bali";s: 14: "kecamatan_name";s: 0: "";s: 14: "kelurahan_name";s: 0: "";s: 13: "photo_primary";s: 80: "http://www.sandbox.tiket.com/img/business/s/u/business-sunset-hotel-001.sq2.jpg";s: 18: "room_facility_name";N;s: 4: "wifi";s: 0: "";s: 10: "promo_name";s: 0: "";s: 5: "price";s: 9: "377318.00";s: 8: "regional";s: 4: "Bali";s: 6: "rating";s: 0: "";s: 4: "name";s: 21: "The Sunset Bali Hotel";
    }
  }
  s: 5: "token";s: 32: "1c78d7bc29690cd96dfce9e0350cfc51";
}```

#### HTTP Request

    `GET https://api-sandbox.tiket.com/search/hotel?q=Indonesia&startdate=2012-06-11&night=1&enddate=2012-06-12&room=1&adult=2&child=0&token=1c78d7bc29690cd96dfce9e0350cfc51&output=json`
    

#### Parameters

  
Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------  
q | Keyword (hotel name / location ) | CHAR (50) |  | TRUE  
startdate | Check in date | DATE | date of today | TRUE  
night | Total night to stay | INT(5) | 1 | TRUE  
enddate | Check out date | DATE | date of tomorrow | TRUE  
room | Total room that will booked by customer | INT(5) | 1 | TRUE  
adult | Total adult | INT(5) | 2 | TRUE  
child | Total child | INT(5) | 0 | FALSE  
sort | sort by (popular/starasc/stardesc/priceasc/pricedesc) | varchar(10) | popular | FALSE  
minprice | set minimum price | int(9) | 0 | FALSE  
maxprice | set maximum price | int(9) | 0 | FALSE  
minstar | set minimum star hotel | int(1) | 0 | FALSE  
maxstar | set maximum star | int(9) | 0 | FALSE  
latitude | set the latitude of the search. Sort will be automatically uses sort by distance | float(10) | 0 | FALSE  
longitude | set the longitude of the search. Sort will be automatically uses sort by distance | float(10) | 0 | FALSE  
token | for saving transaction that done by user | CHAR(128) |  | TRUE
  


    
## Search Area Name and ID

```xml 
This XML file does not appear to have any style information associated with it. The document tree is shown below.
<tiket>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.3544</elapsetime>
    <memoryusage>14.91MB</memoryusage>
    <confirm>success</confirm>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <output_type>xml</output_type>
  <results>
    <result>
      <uid>kecamatan:15</uid>
      <value>Matraman</value>
      <uri>
        https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:15
      </uri>
      <category>Kecamatan</category>
    </result>
    <result>
      <uid>kecamatan:16</uid>
      <value>Pulo Gadung</value>
      <uri>
        https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:16
      </uri>
      <category>Kecamatan</category>
    </result>
    <result>
      <uid>kecamatan:27</uid>
      <value>Jatinegara</value>
      <uri>
        https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:27
      </uri>
      <category>Kecamatan</category>
    </result>
    <result>
      <uid>kecamatan:28</uid>
      <value>Duren Sawit</value>
      <uri>
        https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:28
      </uri>
      <category>Kecamatan</category>
    </result>
    <result>
      <uid>kecamatan:29</uid>
      <value>Kramat Jati</value>
      <uri>
        https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:29
      </uri>
      <category>Kecamatan</category>
    </result>
  </results>
  <login_status>false</login_status>
  <token>a2f50046418672585367579f730e50c0</token>
</tiket>

```

```json
{
  "diagnostic": {
    "status": "200",
    "elapsetime": "0.3305",
    "memoryusage": "14.88MB",
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "results": {
    "result": [{
      "uid": "kecamatan:15",
      "value": "Matraman",
      "uri": "https:\/\/api-sandbox.tiket.com\/search\/hotel?uid=kecamatan:15",
      "category": "Kecamatan"
    }, {
      "uid": "kecamatan:16",
      "value": "Pulo Gadung",
      "uri": "https:\/\/api-sandbox.tiket.com\/search\/hotel?uid=kecamatan:16",
      "category": "Kecamatan"
    }, {
      "uid": "kecamatan:27",
      "value": "Jatinegara",
      "uri": "https:\/\/api-sandbox.tiket.com\/search\/hotel?uid=kecamatan:27",
      "category": "Kecamatan"
    }, {
      "uid": "kecamatan:34",
      "value": "Makasar",
      "uri": "https:\/\/api-sandbox.tiket.com\/search\/hotel?uid=kecamatan:34",
      "category": "Kecamatan"
    }]
  },
  "login_status": "false",
  "token": "a2f50046418672585367579f730e50c0"
}

```

```matlab
a: 5: {
  s: 10: "diagnostic";a: 6: {
    s: 6: "status";s: 3: "200";s: 10: "elapsetime";s: 14: "0.3288";s: 11: "memoryusage";s: 14: "14.88MB";s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "id";s: 8: "currency";s: 3: "IDR";
  }
  s: 11: "output_type";s: 9: "serialize";s: 7: "results";a: 1: {
    s: 6: "result";a: 10: {
      i: 0;a: 4: {
        s: 3: "uid";s: 12: "kecamatan:15";s: 5: "value";s: 8: "Matraman";s: 3: "uri";s: 60: "https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:15";s: 8: "category";s: 18: "Kecamatan";
      }
      i: 1;a: 4: {
        s: 3: "uid";s: 12: "kecamatan:16";s: 5: "value";s: 11: "Pulo Gadung";s: 3: "uri";s: 60: "https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:16";s: 8: "category";s: 18: "Kecamatan";
      }
      i: 2;a: 4: {
        s: 3: "uid";s: 12: "kecamatan:27";s: 5: "value";s: 10: "Jatinegara";s: 3: "uri";s: 60: "https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:27";s: 8: "category";s: 18: "Kecamatan";
      }
      i: 3;a: 4: {
        s: 3: "uid";s: 12: "kecamatan:28";s: 5: "value";s: 11: "Duren Sawit";s: 3: "uri";s: 60: "https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:28";s: 8: "category";s: 18: "Kecamatan";
      }
      i: 4;a: 4: {
        s: 3: "uid";s: 12: "kecamatan:29";s: 5: "value";s: 11: "Kramat Jati";s: 3: "uri";s: 60: "https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:29";s: 8: "category";s: 18: "Kecamatan";
      }
      i: 5;a: 4: {
        s: 3: "uid";s: 12: "kecamatan:30";s: 5: "value";s: 10: "Pasar Rebo";s: 3: "uri";s: 60: "https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:30";s: 8: "category";s: 18: "Kecamatan";
      }
      i: 6;a: 4: {
        s: 3: "uid";s: 12: "kecamatan:31";s: 5: "value";s: 7: "Ciracas";s: 3: "uri";s: 60: "https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:31";s: 8: "category";s: 18: "Kecamatan";
      }
      i: 7;a: 4: {
        s: 3: "uid";s: 12: "kecamatan:32";s: 5: "value";s: 8: "Cipayung";s: 3: "uri";s: 60: "https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:32";s: 8: "category";s: 18: "Kecamatan";
      }
      i: 8;a: 4: {
        s: 3: "uid";s: 12: "kecamatan:33";s: 5: "value";s: 6: "Cakung";s: 3: "uri";s: 60: "https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:33";s: 8: "category";s: 18: "Kecamatan";
      }
      i: 9;a: 4: {
        s: 3: "uid";s: 12: "kecamatan:34";s: 5: "value";s: 7: "Makasar";s: 3: "uri";s: 60: "https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:34";s: 8: "category";s: 18: "Kecamatan";
      }
    }
  }
  s: 12: "login_status";s: 5: "false";s: 5: "token";s: 32: "a2f50046418672585367579f730e50c0";
}

```

#### HTTP Request

    `GET https://api-sandbox.tiket.com/search/search_area?uid=city:178&token=a2f50046418672585367579f730e50c0`
    

#### Parameters

  
Name | Description | Example  
---- | ----------  | -------   
UID | Id |  country |  province |  city |  kecamatan | Country:id |  Province:17 | Jika diberikan country:id maka akan menampilkan semua province di country indonesia  
Type | Tipe yang mau dicari |  Province |  city |  kecamatan |  Jika diberikan value province akan memberikan list province dengan keyword yang diberikan  
Q |  Keyword |  Jakarta |  Akan kenampilkan list city yang mengandung kata jakarta