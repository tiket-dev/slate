# Hotel API

NOTE :  
*Data that is provided for testing is different from the actual

These are the API command for Hotel

Diagram flow for Hotel API:  

[![](http://docs.tiket.com/wp-content/uploads/2012/07/API-hotel-148x300.jpg "API hotel")](http://docs.tiket.com/wp-content/uploads/2012/07/API-hotel.jpg)


## Search Hotel

#### Parameters

[table]  
Name,Description,Format,Default,Mandatory  
q,"Keyword (hotel name / location )",CHAR (50),,TRUE  
startdate,Check in date,DATE,date of today,TRUE  
night,Total night to stay,INT(5),1,TRUE  
enddate,Check out date,DATE,date of tomorrow,TRUE  
room,Total room that will booked by customer,INT(5),1,TRUE  
adult,Total adult,INT(5),2,TRUE  
child,Total child,INT(5),0,FALSE  
sort,sort by (popular/starasc/stardesc/priceasc/pricedesc),varchar(10),popular,FALSE  
minprice,set minimum price,int(9),0,FALSE  
maxprice,set maximum price,int(9),0,FALSE  
minstar,set minimum star hotel,int(1),0,FALSE  
maxstar,set maximum star,int(9),0,FALSE  
latitude,"set the latitude of the search. Sort will be automatically uses sort by distance",float(10),0,FALSE  
longitude,"set the longitude of the search. Sort will be automatically uses sort by distance",float(10),0,FALSE  
token,for saving transaction that done by user,CHAR(128),,TRUE  
[/table]

#### Input

    `https://api-sandbox.tiket.com/search/hotel?q=Indonesia&startdate=2012-06-11&night=1&enddate=2012-06-12&room=1&adult=2&child=0&token=1c78d7bc29690cd96dfce9e0350cfc51&output=json`

#### Output

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
    			Non smoking rooms|In room safe|Air conditioning|Internet access – LAN (complimentary)|Television LCD/plasma screen|Desk|Shower|Bathrobes|Hair dryer|Mini bar|Complimentary bottled water|Television|Telephone|Slipper|Iron board on request|Hair dryer on request|Include Breakfast
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
    {"output_type":"json","diagnostic":{"status":200,"elapsetime":"2.0788","memoryusage":"19.58MB","confirm":"success","lang":"en","currency":"IDR"},"search_queries":{"q":"Indonesia","uid":"","startdate":"2012-06-11","enddate":"2012-06-12","night":"1","room":"1","adult":"2","child":0},"result":[{"id":"2556003619","latitude":"-0.152117","longitude":"2.010164","business_uri":"https:\/\/api-sandbox.tiket.com\/the-101-legian?startdate=2012-06-11&enddate=2012-06-12&night=1&room=1&adult=2&child=0&uid=business%3A4108","province_name":"Bali","kecamatan_name":"Kuta","kelurahan_name":"Legian","photo_primary":"http:\/\/www.sandbox.tiket.com\/img\/business\/s\/k\/business-sky_pool.sq2.jpg","room_facility_name":"Non smoking rooms|In room safe|Air conditioning|Internet access â€“ LAN (complimentary)|%hotel_lcd\/plasma%|Desk|Shower|Bathrobes|Hair dryer|Mini bar|Complimentary bottled water|Television|Telephone|Slipper|Iron board on request|Hair dryer on request|Include Breakfast","wifi":"Wi-Fi available","promo_name":"","price":"478080.00","regional":"Legian - Kuta - Bali","rating":"","name":"The 101 Legian"},{"id":"2696265251","latitude":"-0.151962","longitude":"2.010245","business_uri":"https:\/\/api-sandbox.tiket.com\/the-sunset-hotel-bali?startdate=2012-06-11&enddate=2012-06-12&night=1&room=1&adult=2&child=0&uid=business%3A3623","province_name":"Bali","kecamatan_name":"","kelurahan_name":"","photo_primary":"http:\/\/www.sandbox.tiket.com\/img\/business\/s\/u\/business-sunset-hotel-001.sq2.jpg","room_facility_name":null,"wifi":"","promo_name":"","price":"377318.00","regional":"Bali","rating":"","name":"The Sunset Bali Hotel"}],"token":"1c78d7bc29690cd96dfce9e0350cfc51"}
```



```matlab
    a:5:{s:11:"output_type";s:9:"serialize";s:10:"diagnostic";a:6:{s:6:"status";i:200;s:10:"elapsetime";s:14:"2.3215";s:11:"memoryusage";s:14:"19.26MB";s:7:"confirm";s:7:"success";s:4:"lang";s:2:"en";s:8:"currency";s:3:"IDR";}s:14:"search_queries";a:8:{s:1:"q";s:9:"Indonesia";s:3:"uid";s:0:"";s:9:"startdate";s:10:"2012-06-11";s:7:"enddate";s:10:"2012-06-12";s:5:"night";s:1:"1";s:4:"room";s:1:"1";s:5:"adult";s:1:"2";s:5:"child";i:0;}s:6:"result";a:15:{i:0;a:15:{s:2:"id";s:10:"2556003619";s:8:"latitude";s:9:"-0.152117";s:9:"longitude";s:8:"2.010164";s:12:"business_uri";s:135:"https://api-sandbox.tiket.com/the-101-legian?startdate=2012-06-11&enddate=2012-06-12&night=1&room=1&adult=2&child=0&uid=business%3A4108";s:13:"province_name";s:4:"Bali";s:14:"kecamatan_name";s:4:"Kuta";s:14:"kelurahan_name";s:6:"Legian";s:13:"photo_primary";s:72:"http://www.sandbox.tiket.com/img/business/s/k/business-sky_pool.sq2.jpg";s:18:"room_facility_name";s:347:"Non smoking rooms|In room safe|Air conditioning|Internet access â€“ LAN (complimentary)|Television LCD/plasma screen|Desk|Shower|Bathrobes|Hair dryer|Mini bar|Complimentary bottled water|Television|Telephone|Slipper|Iron board on request|Hair dryer on request|Include Breakfast";s:4:"wifi";s:23:"Wi-Fi available";s:10:"promo_name";s:0:"";s:5:"price";s:9:"478080.00";s:8:"regional";s:20:"Legian - Kuta - Bali";s:6:"rating";s:0:"";s:4:"name";s:14:"The 101 Legian";}i:1;a:15:{s:2:"id";s:10:"2696265251";s:8:"latitude";s:9:"-0.151962";s:9:"longitude";s:8:"2.010245";s:12:"business_uri";s:142:"https://api-sandbox.tiket.com/the-sunset-hotel-bali?startdate=2012-06-11&enddate=2012-06-12&night=1&room=1&adult=2&child=0&uid=business%3A3623";s:13:"province_name";s:4:"Bali";s:14:"kecamatan_name";s:0:"";s:14:"kelurahan_name";s:0:"";s:13:"photo_primary";s:80:"http://www.sandbox.tiket.com/img/business/s/u/business-sunset-hotel-001.sq2.jpg";s:18:"room_facility_name";N;s:4:"wifi";s:0:"";s:10:"promo_name";s:0:"";s:5:"price";s:9:"377318.00";s:8:"regional";s:4:"Bali";s:6:"rating";s:0:"";s:4:"name";s:21:"The Sunset Bali Hotel";}}s:5:"token";s:32:"1c78d7bc29690cd96dfce9e0350cfc51";}
```
    
    
## Search by Area

#### Parameters

[table]  
Name,Description,Contoh,  
UID,"Id, country, province, city, kecamatan","Country:id, Province:17",Jika diberikan country:id maka akan menampilkan semua province di country indonesia  
Type,Tipe yang mau dicari, "Province, city, kecamatan", Jika diberikan value province akan memberikan list province dengan keyword yang diberikan  
Q, Keyword, Jakarta, Akan kenampilkan list city yang mengandung kata jakarta  
[/table]

#### Input

    `http://api-sandbox.tiket.com/search/search_area?uid=city:178&token=a2f50046418672585367579f730e50c0`

#### Output

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
    "diagnostic":
    {
        "status":"200",
        "elapsetime":"0.3305",
        "memoryusage":"14.88MB",
        "confirm":"success",
        "lang":"id",
        "currency":"IDR"
    },
    "output_type":"json",
    "results":
        {
            "result":
            [
                {
                    "uid":"kecamatan:15",
                    "value":"Matraman",
                    "uri":"https:\/\/api-sandbox.tiket.com\/search\/hotel?uid=kecamatan:15",
                    "category":"Kecamatan"
                },
                {
                    "uid":"kecamatan:16",
                    "value":"Pulo Gadung",
                    "uri":"https:\/\/api-sandbox.tiket.com\/search\/hotel?uid=kecamatan:16",
                    "category":"Kecamatan"
                },
                {
                    "uid":"kecamatan:27",
                    "value":"Jatinegara",
                    "uri":"https:\/\/api-sandbox.tiket.com\/search\/hotel?uid=kecamatan:27",
                    "category":"Kecamatan"
                },
                {
                    "uid":"kecamatan:34",
                    "value":"Makasar",
                    "uri":"https:\/\/api-sandbox.tiket.com\/search\/hotel?uid=kecamatan:34",
                    "category":"Kecamatan"
                }
            ]
        },
    "login_status":"false","token":"a2f50046418672585367579f730e50c0"
    }
```



```matlab
    a:5:{s:10:"diagnostic";a:6:{s:6:"status";s:3:"200";s:10:"elapsetime";s:14:"0.3288";s:11:"memoryusage";s:14:"14.88MB";s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:11:"output_type";s:9:"serialize";s:7:"results";a:1:{s:6:"result";a:10:{i:0;a:4:{s:3:"uid";s:12:"kecamatan:15";s:5:"value";s:8:"Matraman";s:3:"uri";s:60:"https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:15";s:8:"category";s:18:"Kecamatan";}i:1;a:4:{s:3:"uid";s:12:"kecamatan:16";s:5:"value";s:11:"Pulo Gadung";s:3:"uri";s:60:"https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:16";s:8:"category";s:18:"Kecamatan";}i:2;a:4:{s:3:"uid";s:12:"kecamatan:27";s:5:"value";s:10:"Jatinegara";s:3:"uri";s:60:"https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:27";s:8:"category";s:18:"Kecamatan";}i:3;a:4:{s:3:"uid";s:12:"kecamatan:28";s:5:"value";s:11:"Duren Sawit";s:3:"uri";s:60:"https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:28";s:8:"category";s:18:"Kecamatan";}i:4;a:4:{s:3:"uid";s:12:"kecamatan:29";s:5:"value";s:11:"Kramat Jati";s:3:"uri";s:60:"https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:29";s:8:"category";s:18:"Kecamatan";}i:5;a:4:{s:3:"uid";s:12:"kecamatan:30";s:5:"value";s:10:"Pasar Rebo";s:3:"uri";s:60:"https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:30";s:8:"category";s:18:"Kecamatan";}i:6;a:4:{s:3:"uid";s:12:"kecamatan:31";s:5:"value";s:7:"Ciracas";s:3:"uri";s:60:"https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:31";s:8:"category";s:18:"Kecamatan";}i:7;a:4:{s:3:"uid";s:12:"kecamatan:32";s:5:"value";s:8:"Cipayung";s:3:"uri";s:60:"https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:32";s:8:"category";s:18:"Kecamatan";}i:8;a:4:{s:3:"uid";s:12:"kecamatan:33";s:5:"value";s:6:"Cakung";s:3:"uri";s:60:"https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:33";s:8:"category";s:18:"Kecamatan";}i:9;a:4:{s:3:"uid";s:12:"kecamatan:34";s:5:"value";s:7:"Makasar";s:3:"uri";s:60:"https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:34";s:8:"category";s:18:"Kecamatan";}}}s:12:"login_status";s:5:"false";s:5:"token";s:32:"a2f50046418672585367579f730e50c0";}
```
    
    
## Search Hotel Promo

#### Parameters

[table]  
Name,Description,Format,Default,Mandatory  
token,for saving transaction that done by user,CHAR(128),,TRUE  
page,pagging page,INT,,FALSE  
startdate,startdate for hotel promo,INT,,FALSE  
enddate,enddate for hotel promo,INT,,FALSE  
[/table]

#### Input

    `https://api-sandbox.tiket.com/home/hotelDeals?token=28a6c5f0882a94a078e82ffdb1df7744&output=json`

#### Output

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
    			https://api.tiket.com/hotel/indonesia/gianyar/pande-permai-bungalow?startdate=2012-11-	23&enddate=2012-11-	24&night=1&room=1&adult=2&child=0&business_id%5B0%5D=22707&business_id%5B1%5D=129881&business_id%5B2%5D=2923&business_id%5B3%5D=117990&business_id%5B4%5D=233&business_id%5B5%5D=43&business_id%5B6%5D=15668&business_id%5B7%5D=86&uid=business%3A129881
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
    {"output_type":"json","search_queries":{"q":"Indonesia","startdate":"2012-11-23","enddate":"2012-11-30"},"pagination":{"total_found":5,"current_page":1,"offset":10,"last_page":1},"results":{"result":[{"regional":"Ubud - Ubud - Bali","price":"IDR 345.519,00","province_name":"Bali","deal_startdate":"2012-11-20 00:00:00","deal_enddate":"2012-11-26 23:59:59","room_name":"Deluxe AC","travel_startdate":"2012-10-20","travel_enddate":"2012-12-19","booking_startdate":"0000-00-00","booking_enddate":"0000-00-00","id":"129881","room_available":"2","star_rating":"1","business_uri":"https:\/\/api.tiket.com\/hotel\/indonesia\/gianyar\/pande-permai-bungalow?startdate=2012-11-23&enddate=2012-11-24&night=1&room=1&adult=2&child=0&business_id%5B0%5D=22707&business_id%5B1%5D=129881&business_id%5B2%5D=2923&business_id%5B3%5D=117990&business_id%5B4%5D=233&business_id%5B5%5D=43&business_id%5B6%5D=15668&business_id%5B7%5D=86&uid=business%3A129881","photo_primary":"http:\/\/www.tiket.com\/img\/business\/i\/m\/business-img_0041.featured322x147.jpg","promo_name":"Discount  15%","name":"Pande Permai Bungalow"},{"regional":"Melintang - Rangkui - Kepulauan Bangka-Belitung","price":"IDR 384.705,00","province_name":"Kepulauan Bangka-Belitung","deal_startdate":"2012-11-19 00:00:00","deal_enddate":"2012-11-25 23:59:59","room_name":"Superior","travel_startdate":"2012-10-17","travel_enddate":"2012-11-30","booking_startdate":"0000-00-00","booking_enddate":"0000-00-00","id":"2923","room_available":"3","star_rating":"3","business_uri":"https:\/\/api.tiket.com\/hotel\/indonesia\/bangka-tengah\/hotel-santika-bangka?startdate=2012-11-23&enddate=2012-11-24&night=1&room=1&adult=2&child=0&business_id%5B0%5D=22707&business_id%5B1%5D=129881&business_id%5B2%5D=2923&business_id%5B3%5D=117990&business_id%5B4%5D=233&business_id%5B5%5D=43&business_id%5B6%5D=15668&business_id%5B7%5D=86&uid=business%3A2923","photo_primary":"http:\/\/www.tiket.com\/img\/business\/s\/a\/business-santika-bangka_L.featured322x147.jpg","promo_name":"Discount  10%","name":"Hotel Santika Bangka"}]},"diagnostic":{"status":200,"elapsetime":"0.6928","memoryusage":"8.95MB","confirm":"success","lang":"id","currency":"IDR"},"token":"b21ff0ede5de530e35ecb99f2b3cd3b2"}
```



```matlab
    a:6:{s:11:"output_type";s:9:"serialize";s:14:"search_queries";a:3:{s:1:"q";s:9:"Indonesia";s:9:"startdate";s:10:"2012-11-23";s:7:"enddate";s:10:"2012-11-30";}s:10:"pagination";a:4:{s:11:"total_found";i:5;s:12:"current_page";i:1;s:6:"offset";i:10;s:9:"last_page";d:1;}s:7:"results";a:1:{s:6:"result";i:2;a:17:{s:8:"regional";s:47:"Melintang - Rangkui - Kepulauan Bangka-Belitung";s:5:"price";s:14:"IDR 384.705,00";s:13:"province_name";s:25:"Kepulauan Bangka-Belitung";s:14:"deal_startdate";s:19:"2012-11-19 00:00:00";s:12:"deal_enddate";s:19:"2012-11-25 23:59:59";s:9:"room_name";s:8:"Superior";s:16:"travel_startdate";s:10:"2012-10-17";s:14:"travel_enddate";s:10:"2012-11-30";s:17:"booking_startdate";s:10:"0000-00-00";s:15:"booking_enddate";s:10:"0000-00-00";s:2:"id";s:4:"2923";s:14:"room_available";s:1:"3";s:11:"star_rating";s:1:"3";s:12:"business_uri";s:356:"https://api.tiket.com/hotel/indonesia/bangka-tengah/hotel-santika-bangka?startdate=2012-11-23&enddate=2012-11-24&night=1&room=1&adult=2&child=0&business_id%5B0%5D=22707&business_id%5B1%5D=129881&business_id%5B2%5D=2923&business_id%5B3%5D=117990&business_id%5B4%5D=233&business_id%5B5%5D=43&business_id%5B6%5D=15668&business_id%5B7%5D=86&uid=business%3A2923";s:13:"photo_primary";s:83:"http://www.tiket.com/img/business/s/a/business-santika-bangka_L.featured322x147.jpg";s:10:"promo_name";s:13:"Discount 10%";s:4:"name";s:20:"Hotel Santika Bangka";}i:3;a:17:{s:8:"regional";s:47:"Gili Trawangan - Pemenang - Nusa Tenggara Barat";s:5:"price";s:16:"IDR 1.526.516,00";s:13:"province_name";s:19:"Nusa Tenggara Barat";s:14:"deal_startdate";s:19:"2012-11-19 00:00:00";s:12:"deal_enddate";s:19:"2012-11-25 23:59:59";s:9:"room_name";s:24:"Superior Lumbung Terrace";s:16:"travel_startdate";s:10:"2012-09-11";s:14:"travel_enddate";s:10:"2012-09-30";s:17:"booking_startdate";s:10:"0000-00-00";s:15:"booking_enddate";s:10:"0000-00-00";s:2:"id";s:6:"117990";s:14:"room_available";s:2:"62";s:11:"star_rating";s:1:"4";s:12:"business_uri";s:353:"https://api.tiket.com/hotel/indonesia/lombok-utara/hotel-vila-ombak?startdate=2012-11-23&enddate=2012-11-24&night=1&room=1&adult=2&child=0&business_id%5B0%5D=22707&business_id%5B1%5D=129881&business_id%5B2%5D=2923&business_id%5B3%5D=117990&business_id%5B4%5D=233&business_id%5B5%5D=43&business_id%5B6%5D=15668&business_id%5B7%5D=86&uid=business%3A117990";s:13:"photo_primary";s:78:"http://www.tiket.com/img/business/l/a/business-large-fromt.featured322x147.jpg";s:10:"promo_name";s:22:"Last Minute Offer 15%";s:4:"name";s:16:"Hotel Vila Ombak";}}s:10:"diagnostic";a:6:{s:6:"status";i:200;s:10:"elapsetime";s:14:"1.0974";s:11:"memoryusage";s:14:"8.95MB";s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:5:"token";s:32:"b21ff0ede5de530e35ecb99f2b3cd3b2";}
```
    
    
    
## Search Autocomplete

#### Parameters

[table]  
Name,Description,Format,Default,Mandatory  
q,"Keyword (hotel name / location )",CHAR (50),,TRUE  
token,for saving transaction that done by user,CHAR(128),,TRUE  
[/table]

#### Input

    `https://api-sandbox.tiket.com/search/autocomplete/hotel?q=mah&token=90d2fad44172390b11527557e6250e50&output=json`

#### Output

```xml
    <tiket>
    	<output_type>xml</output_type>
    	<diagnostic>
    		<elapsetime>0.1295</elapsetime>
    		<memoryusage>6.34MB</memoryusage>
    		<lang>id</lang>
    		<currency>IDR</currency>
    	</diagnostic>
    	<results>
    		<result>
    		<id>business:3772</id>
    			<label>
    			Puri Maharani Boutique Hotel & Spa - Denpasar, Denpasar Timur, Kesiman Kertalangu
    			</label>
    			<value>Puri Maharani Boutique Hotel & Spa</value>
    			<category>Hotel</category>
    		</result>
    		<result>
    			<id>business:3852</id>
    			<label>Maharani Hotel - Jakarta Selatan</label>
    			<value>Maharani Hotel</value>
    			<category>Hotel</category>
    		</result>
    		<result>
    			<id>business:3874</id>
    			<label>
    				Maharadja Hotel - Jakarta Selatan, Mampang Prapatan, Tegal Parang
    			</label>
    			<value>Maharadja Hotel</value>
    			<category>Hotel</category>
    		</result>
    		<result>
    			<id>business:4776</id>
    			<label>Pita Maha Resort and Spa - Gianyar, Ubud, Ubud</label>
    			<value>Pita Maha Resort and Spa</value>
    			<category>Hotel</category>
    		</result>
    		<result>
    			<id>business:4779</id>
    			<label>
    				The Royal Pita Maha Resort and Spa - Gianyar, Ubud, Kedewatan
    			</label>
    			<value>The Royal Pita Maha Resort and Spa</value>
    			<category>Hotel</category>
    		</result>
    		<result>
    			<id>business:18420</id>
    			<label>
    				Villa Mahapala Bali - Denpasar, Denpasar Selatan, Sanur
    			</label>
    			<value>Villa Mahapala Bali</value>
    			<category>Hotel</category>
    		</result>
    		<result>
    			<id>business:105246</id>
    			<label>
    				Mahagiri Dreamland Villas &amp; Spa - Badung, Kuta Selatan, Pecatu
    			</label>
    			<value>Mahagiri Dreamland Villas &amp; Spa</value>
    			<category>Hotel</category>
    		</result>
    	</results>
    	<token>90d2fad44172390b11527557e6250e50</token>
    </tiket>
```

```json
    {"output_type":"json","diagnostic":{"elapsetime":"0.1383","memoryusage":"6.33MB","lang":"id","currency":"IDR"},"result":[{"id":"business:3772","label":"Puri Maharani Boutique Hotel & Spa - Denpasar, Denpasar Timur, Kesiman Kertalangu","value":"Puri Maharani Boutique Hotel & Spa","category":"Hotel"},{"id":"business:3852","label":"Maharani Hotel - Jakarta Selatan","value":"Maharani Hotel ","category":"Hotel"},{"id":"business:3874","label":"Maharadja Hotel - Jakarta Selatan, Mampang Prapatan, Tegal Parang","value":"Maharadja Hotel","category":"Hotel"},{"id":"business:4776","label":"Pita Maha Resort and Spa - Gianyar, Ubud, Ubud","value":"Pita Maha Resort and Spa","category":"Hotel"},{"id":"business:4779","label":"The Royal Pita Maha Resort and Spa - Gianyar, Ubud, Kedewatan","value":"The Royal Pita Maha Resort and Spa","category":"Hotel"},{"id":"business:18420","label":"Villa Mahapala Bali - Denpasar, Denpasar Selatan, Sanur","value":"Villa Mahapala Bali","category":"Hotel"},{"id":"business:105246","label":"Mahagiri Dreamland Villas & Spa - Badung, Kuta Selatan, Pecatu","value":"Mahagiri Dreamland Villas & Spa","category":"Hotel"}],"token":"90d2fad44172390b11527557e6250e50"}
```

```matlab
    a:4:{s:11:"output_type";s:9:"serialize";s:10:"diagnostic";a:4:{s:10:"elapsetime";s:14:"0.1258";s:11:"memoryusage";s:14:"6.32MB";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:6:"result";a:7:{i:0;a:4:{s:2:"id";s:13:"business:3772";s:5:"label";s:81:"Puri Maharani Boutique Hotel & Spa - Denpasar, Denpasar Timur, Kesiman Kertalangu";s:5:"value";s:34:"Puri Maharani Boutique Hotel & Spa";s:8:"category";s:14:"Hotel";}i:1;a:4:{s:2:"id";s:13:"business:3852";s:5:"label";s:33:"Maharani Hotel - Jakarta Selatan";s:5:"value";s:15:"Maharani Hotel ";s:8:"category";s:14:"Hotel";}i:2;a:4:{s:2:"id";s:13:"business:3874";s:5:"label";s:65:"Maharadja Hotel - Jakarta Selatan, Mampang Prapatan, Tegal Parang";s:5:"value";s:15:"Maharadja Hotel";s:8:"category";s:14:"Hotel";}i:3;a:4:{s:2:"id";s:13:"business:4776";s:5:"label";s:46:"Pita Maha Resort and Spa - Gianyar, Ubud, Ubud";s:5:"value";s:24:"Pita Maha Resort and Spa";s:8:"category";s:14:"Hotel";}i:4;a:4:{s:2:"id";s:13:"business:4779";s:5:"label";s:61:"The Royal Pita Maha Resort and Spa - Gianyar, Ubud, Kedewatan";s:5:"value";s:34:"The Royal Pita Maha Resort and Spa";s:8:"category";s:14:"Hotel";}i:5;a:4:{s:2:"id";s:14:"business:18420";s:5:"label";s:55:"Villa Mahapala Bali - Denpasar, Denpasar Selatan, Sanur";s:5:"value";s:19:"Villa Mahapala Bali";s:8:"category";s:14:"Hotel";}i:6;a:4:{s:2:"id";s:15:"business:105246";s:5:"label";s:66:"Mahagiri Dreamland Villas & Spa - Badung, Kuta Selatan, Pecatu";s:5:"value";s:35:"Mahagiri Dreamland Villas & Spa";s:8:"category";s:14:"Hotel";}}s:5:"token";s:32:"90d2fad44172390b11527557e6250e50";}
```
    
    
    
    
## View Detail Hotel

#### Parameters

link url to view detail can be get from search hotel, variable business_uri  
user just need to add token in the parameter.

[table]  
Name,Description,Format,Default,Mandatory  
startdate,Check in date,DATE,date of today,TRUE  
night,Total night to stay,INT(5),1,TRUE  
enddate,Check out date,DATE,date of tomorrow,TRUE  
room,Total room that will booked by customer,INT(5),1,TRUE  
adult,Total adult,INT(5),2,TRUE  
child,Total child,INT(5),0,  
token,for saving transaction that done by user,CHAR(128),,TRUE  
[/table]

#### Input

    `https://api-sandbox.tiket.com/the-101-legian?startdate=2012-06-11&enddate=2012-06-12&night=1&room=1&adult=2&child=0&uid=business%3A4108&token=1c78d7bc29690cd96dfce9e0350cfc51&output=json`

#### Output

```xml
    <tiket>
    	<output_type>xml</output_type>
    	<diagnostic>
    		<status>200</status>
    		<elapsetime>0.3753</elapsetime>
    		<memoryusage>21.7MB</memoryusage>
    		<confirm>success</confirm>
    		<lang>en</lang>
    		<currency>IDR</currency>
    	</diagnostic>
    	<primaryPhotos>
    		http://www.sandbox.tiket.com/img/business/d/p/business-dps01184-01.s.jpg
    	</primaryPhotos>
    	<all_photo>
    		<photo>
    			<file_name>
    				http://www.sandbox.tiket.com/img/business/1/0/business-10111.s.jpg
    			</file_name>
    			<photo_type>Swimming Pool</photo_type>
    		</photo>
    		<photo>
    			<file_name>
    				http://www.sandbox.tiket.com/img/business/1/0/business-10131.s.jpg
    			</file_name>
    			<photo_type>Main Pool</photo_type>
    		</photo>
    	</all_photo>
    	<breadcrumb>
    		<business_uri>https://www.sandbox.tiket.com/the-101-legian</business_uri>
    		<business_name>The 101 Legian</business_name>
    		<kelurahan_name>Legian</kelurahan_name>
    		<kecamatan_name>Kuta</kecamatan_name>
    		<city_name>Badung</city_name>
    		<province_name>Bali</province_name>
    		<country_name>Indonesia</country_name>
    		<continent_name>Asia</continent_name>
    		<kelurahan_uri>
    			https://www.sandbox.tiket.com/search/hotel?uid=city:258
    		</kelurahan_uri>
    		<kecamatan_uri>
    			https://www.sandbox.tiket.com/search/hotel?uid=kecamatan:4172
    		</kecamatan_uri>
    		<province_uri>
    			https://www.sandbox.tiket.com/search/hotel?uid=province:17
    		</province_uri>
    		<country_uri>
    			https://www.sandbox.tiket.com/search/hotel?uid=country:id
    		</country_uri>
    		<continent_uri>
    			https://www.sandbox.tiket.com/search/hotel?uid=continent:1
    		</continent_uri>
    		<star_rating>3</star_rating>
    	</breadcrumb>
    	<results>
    		<result>
    			<id>2556003619</id>
    			<room_available>10</room_available>
    			<currency>IDR</currency>
    			<photo_url>
    				http://www.sandbox.tiket.com/img/business/1/0/business-10211.s.jpg
    			</photo_url>
    			<oldprice>880337.00</oldprice>
    			<price>478080.00</price>
    			<bookUri>
    				https://api-sandbox.tiket.com/order/add/hotel?startdate=2012-06-11&enddate=2012-06-	12&night=1&room=1&adult=2&child=0&minstar=0&maxstar=5&minprice=0&maxprice=1000&hotelname=0&room_id=1185&hasPromo=0
    			</bookUri>
    		</result>
    		<result>
    			<id>2195611171</id>
    			<room_available>15</room_available>
    			<currency>IDR</currency>
    			<photo_url>
    				http://www.sandbox.tiket.com/img/business/r/o/business-room20.s.jpg
    			</photo_url>
    			<oldprice>3668069.00</oldprice>
    			<price>1992000.00</price>
    			<bookUri>
    				https://api-sandbox.tiket.com/order/add/hotel?startdate=2012-06-11&enddate=2012-06-12&night=1&room=1&adult=2&child=0&minstar=0&maxstar=5&minprice=0&maxprice=1000&hotelname=0&room_id=666&hasPromo=0
    			</bookUri>
    		</result>
    	</results>
    	<addinfos>
    		<addinfo>Airport Transfer Fee : USD 18.15</addinfo>
    		<addinfo>Checkout : 12:00</addinfo>
    	</addinfos>
    	<avail_facilities>
    		<avail_facility>
    			<facility_type>hotel</facility_type>
    			<facility_name>24hr Room Service</facility_name>
    		</avail_facility>
    		<avail_facility>
    			<facility_type>hotel</facility_type>
    			<facility_name>Airport Transfer Chargeable</facility_name>
    		</avail_facility>
    	</avail_facilities>
    	<nearby_attractions>
    		<nearby_attraction>
    			<distance>475</distance>
    			<business_primary_photo>
    				http://www.sandbox.tiket.com/img/business/3/3/business-333-korirestaurantbar.s.jpg
    			</business_primary_photo>
    			<business_name>KORI Restaurant & Bar</business_name>
    			<business_uri>http://www.sandbox.tiket.com/kori-restaurant-bar</business_uri>
    		</nearby_attraction>
    		<nearby_attraction>
    			<distance>744</distance>
    			<business_primary_photo>
    				http://www.sandbox.tiket.com/img/business/t/h/business-this-is-what-they-gave.s.jpg
    			</business_primary_photo>
    			<business_name>Little Italy Resto</business_name>
    			<business_uri>https://www.sandbox.tiket.com/little-italy-resto</business_uri>
    		</nearby_attraction>
    	</nearby_attractions>
    	<general>
    		<address>
    		Jalan AIPDA KS Tubun No.7, Slipi , Palmerah, Jakarta Barat
    		</address>
    		<description>
    	Conveniently+located+close+to+the+city%27s+central+business+district%2C+yet+only+30+minutes+from+Soekarno-Hatta+International+Airport.+This+hotel+is+close+to+Forestry+Museum%2C+Bung+Karno+Stadium%2C+and+Textile+Museum.+Also+nearby+are+Thamrin+City+Shopping+Mall+and+Jakarta+Convention+Center.%3Cbr+%2F%3E%0AThis+elegant+hotel+designed+with+its+distinctive+yet+unimposing+Indonesian+ambience%2C+Santika+Premiere+Jakarta+offers+unsurpassed+facilities%2C+a+choice+of+restaurants+and+friendly%2C+helpful+staff.+In+addition+to+a+restaurant%2C+Hotel+Santika+Premiere+Jakarta+features+an+outdoor+pool.+Other+amenities+include+a+bar%2Flounge+and+a+coffee+shop%2Fcafe.%3Cbr+%2F%3E%0AEach+room+equipped+with+televisions+come+with+satellite+channels.+Guestrooms+also+feature+air+conditioning%2C+minibars%2C+and+safes.
    		</description>
    	</general>
    	<token>1c78d7bc29690cd96dfce9e0350cfc51</token>
    </tiket>
```

```json
    {"output_type":"json","diagnostic":{"status":200,"elapsetime":"0.3705","memoryusage":"21.66MB","confirm":"success","lang":"en","currency":"IDR"},"primaryPhotos":"http:\/\/www.sandbox.tiket.com\/img\/business\/d\/p\/business-dps01184-01.s.jpg","photos":[{"file_name":"http:\/\/www.sandbox.tiket.com\/img\/business\/1\/0\/business-10111.s.jpg","photo_type":"Swimming Pool"},{"file_name":"http:\/\/www.sandbox.tiket.com\/img\/business\/1\/0\/business-10131.s.jpg","photo_type":"Main Pool"}],"breadcrumb":{"business_uri":"http:\/\/www.sandbox.tiket.com\/the-101-legian","business_name":"The 101 Legian","kelurahan_name":"Legian","kecamatan_name":"Kuta","city_name":"Badung","province_name":"Bali","country_name":"Indonesia ","continent_name":"Asia","kelurahan_uri":"http:\/\/www.sandbox.tiket.com\/search\/hotel?uid=city:258","kecamatan_uri":"http:\/\/www.sandbox.tiket.com\/search\/hotel?uid=kecamatan:4172","province_uri":"http:\/\/www.sandbox.tiket.com\/search\/hotel?uid=province:17","country_uri":"http:\/\/www.sandbox.tiket.com\/search\/hotel?uid=country:id","continent_uri":"http:\/\/www.sandbox.tiket.com\/search\/hotel?uid=continent:1","star_rating":"3"},"nearby_attraction":[{"distance":475,"business_primary_photo":"http:\/\/www.sandbox.tiket.com\/img\/business\/3\/3\/business-333-korirestaurantbar.s.jpg","business_name":"KORI Restaurant & Bar","business_uri":"http:\/\/www.sandbox.tiket.com\/kori-restaurant-bar"},{"distance":744,"business_primary_photo":"http:\/\/www.sandbox.tiket.com\/img\/business\/t\/h\/business-this-is-what-they-gave.s.jpg","business_name":"Little Italy Resto","business_uri":"http:\/\/www.sandbox.tiket.com\/little-italy-resto"}],"addinfo":["Airport Transfer Fee : USD 18.15","Checkout : 12:00","Distance From City : 3 Km"],"avail_facilities":[{"facility_type":"hotel","facility_name":"24hr Room Service"},{"facility_type":"hotel","facility_name":"Airport Transfer Chargeable"}],"token":"1c78d7bc29690cd96dfce9e0350cfc51"}
```

```matlab
    a:10:{s:11:"output_type";s:9:"serialize";s:10:"diagnostic";a:6:{s:6:"status";i:200;s:10:"elapsetime";s:14:"0.3572";s:11:"memoryusage";s:14:"21.67MB";s:7:"confirm";s:7:"success";s:4:"lang";s:2:"en";s:8:"currency";s:3:"IDR";}s:13:"primaryPhotos";s:73:"http://www.sandbox.tiket.com/img/business/d/p/business-dps01184-01.s.jpg";s:6:"photos";a:16:{i:0;a:2:{s:9:"file_name";s:67:"http://www.sandbox.tiket.com/img/business/1/0/business-10111.s.jpg";s:10:"photo_type";s:21:"Swimming Pool";}i:1;a:2:{s:9:"file_name";s:67:"http://www.sandbox.tiket.com/img/business/1/0/business-10131.s.jpg";s:10:"photo_type";s:17:"Main Pool";}}s:10:"breadcrumb";a:14:{s:12:"business_uri";s:44:"http://www.sandbox.tiket.com/the-101-legian";s:13:"business_name";s:14:"The 101 Legian";s:14:"kelurahan_name";s:6:"Legian";s:14:"kecamatan_name";s:4:"Kuta";s:9:"city_name";s:6:"Badung";s:13:"province_name";s:4:"Bali";s:12:"country_name";s:10:"Indonesia ";s:14:"continent_name";s:4:"Asia";s:13:"kelurahan_uri";s:55:"http://www.sandbox.tiket.com/search/hotel?uid=city:258";s:13:"kecamatan_uri";s:61:"http://www.sandbox.tiket.com/search/hotel?uid=kecamatan:4172";s:12:"province_uri";s:58:"http://www.sandbox.tiket.com/search/hotel?uid=province:17";s:11:"country_uri";s:57:"http://www.sandbox.tiket.com/search/hotel?uid=country:id";s:13:"continent_uri";s:58:"http://www.sandbox.tiket.com/search/hotel?uid=continent:1";s:11:"star_rating";s:1:"3";}s:17:"nearby_attraction";a:4:{i:0;a:4:{s:8:"distance";d:475;s:22:"business_primary_photo";s:83:"http://www.sandbox.tiket.com/img/business/3/3/business-333-korirestaurantbar.s.jpg";s:13:"business_name";s:21:"KORI Restaurant & Bar";s:12:"business_uri";s:49:"http://www.sandbox.tiket.com/kori-restaurant-bar";}i:1;a:4:{s:8:"distance";d:744;s:22:"business_primary_photo";s:84:"http://www.sandbox.tiket.com/img/business/t/h/business-this-is-what-they-gave.s.jpg";s:13:"business_name";s:18:"Little Italy Resto";s:12:"business_uri";s:48:"http://www.sandbox.tiket.com/little-italy-resto";}}s:6:"result";a:2:{i:0;a:7:{s:2:"id";s:10:"2556003619";s:14:"room_available";s:2:"10";s:8:"currency";s:3:"IDR";s:9:"photo_url";s:67:"http://www.sandbox.tiket.com/img/business/1/0/business-10211.s.jpg";s:8:"oldprice";s:9:"880337.00";s:5:"price";s:9:"478080.00";s:7:"bookUri";s:198:"https://api-sandbox.tiket.com/order/add/hotel?startdate=2012-06-11&enddate=2012-06-12&night=1&room=1&adult=2&child=0&minstar=0&maxstar=5&minprice=0&maxprice=1000&hotelname=0&room_id=1185&hasPromo=0";}i:1;a:7:{s:2:"id";s:10:"2195611171";s:14:"room_available";s:2:"15";s:8:"currency";s:3:"IDR";s:9:"photo_url";s:68:"http://www.sandbox.tiket.com/img/business/r/o/business-room20.s.jpg";s:8:"oldprice";s:10:"3668069.00";s:5:"price";s:10:"1992000.00";s:7:"bookUri";s:197:"https://api-sandbox.tiket.com/order/add/hotel?startdate=2012-06-11&enddate=2012-06-12&night=1&room=1&adult=2&child=0&minstar=0&maxstar=5&minprice=0&maxprice=1000&hotelname=0&room_id=666&hasPromo=0";}}s:7:"addinfo";a:8:{i:0;s:40:"Airport Transfer Fee : USD 18.15";i:1;s:24:"Checkout : 12:00";}s:16:"avail_facilities";a:38:{i:0;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:22:"24hr Room Service";}i:1;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:35:"Airport Transfer Chargeable";}}s:5:"token";s:32:"1c78d7bc29690cd96dfce9e0350cfc51";}
```
    
    
    
## Add Order

Add hotel order to shopping cart.

#### Parameters

Plink url to view detail can be get from view detail hotel, variable book_uri  
user just need to add token in the parameter.

[table]  
Name,Description,Format,Default,Mandatory  
startdate,check-in date,YYYY-MM-DD,date of today,TRUE  
enddate,check-out date,YYYY-MM-DD,date of tomorrow,TRUE  
night,number of night,INT(5),1,TRUE  
room,Total room that will booked by customer,INT(5),1,TRUE  
adult,number of adult,INT(5),2,TRUE  
child,number of child,INT(5),0,FALSE  
minstar,hotel star,INT(5),,  
minprice,cheapest hotel price,INT(5),,  
hotelname,hotel name,CHAR(50),,  
room_id,room id that will ordered,CHAR(10),,  
hasPromo,if the room has promo between 1 or 0,INT(5),,  
token,for saving transaction that done by user,CHAR(128),,TRUE  
[/table]

#### Input

    `https://api-sandbox.tiket.com/order/add/hotel?startdate=2012-06-11&enddate=2012-06-12&night=1&room=1&adult=2&child=0&minstar=0&maxstar=5&minprice=0&maxprice=1000&hotelname=0&room_id=666&hasPromo=0&token=1c78d7bc29690cd96dfce9e0350cfc51&output=json`

#### Output

```xml
    <tiket>
        <output_type>xml</output_type>
        <error>0</error>
        <diagnostic>
            <elapstime>7.7606</elapstime>
            <memoryusage>12.17MB</memoryusage>
            <status>200</status>
            <lang>en</lang>
            <currency>IDR</currency>
        </diagnostic>
        <status>success booking train</status>
        <token>1c78d7bc29690cd96dfce9e0350cfc51</token>
    </tiket>
```

```json
    {"output_type":"json","error":"0","diagnostic":{"elapstime":"9.5301","memoryusage":"12.15MB","status":"200","lang":"en","currency":"IDR"},"status":"success booking train","token":"1c78d7bc29690cd96dfce9e0350cfc51"}
```

```matlab
    a:5:{s:11:"output_type";s:9:"serialize";s:5:"error";s:1:"0";s:10:"diagnostic";a:5:{s:9:"elapstime";s:14:"5.9200";s:11:"memoryusage";s:14:"12.15MB";s:6:"status";s:3:"200";s:4:"lang";s:2:"en";s:8:"currency";s:3:"IDR";}s:6:"status";s:21:"success booking train";s:5:"token";s:32:"1c78d7bc29690cd96dfce9e0350cfc51";}
```
    
    
    
## Order

#### Parameters

[table]  
Name,Description,Format,Default,Mandatory  
token,for saving transaction that done by user,CHAR(128),,TRUE  
[/table]

#### Input

    `https://api-sandbox.tiket.com/order?token=8f683005261f872fe5c044f9b7085162&output=json`

#### Output

```xml
    <tiket>
    	<output_type>xml</output_type>
    	<myorder>
    		<order_id>120152</order_id>
    		<data>
    			<expire>60</expire>
    			<order_detail_id>31406</order_detail_id>
    			<order_type>hotel</order_type>
    			<order_name>The 101 Legian</order_name>
    			<order_name_detail>Superior (Room Only)</order_name_detail>
    			<tenor>0</tenor>
    			<detail>
    				<order_detail_id>31406</order_detail_id>
    				<room_id>1185</room_id>
    				<rooms>1</rooms>
    				<adult>2</adult>
    				<child>0</child>
    				<startdate>11 Jun 2012</startdate>
    				<enddate>12 Jun 2012</enddate>
    				<nights>1</nights>
    				<price>517920</price>
    			</detail>
    			<order_photo>
    				http://www.sandbox.tiket.com/img/business/1/0/business-10211.s.jpg
    			</order_photo>
    			<tax>106080</tax>
    			<item_charge>0</item_charge>
    			<subtotal_and_charge>624000.00</subtotal_and_charge>
    			<delete_uri>
    				https://api-sandbox.tiket.com/order/delete_order?order_detail_id=31406
    			</delete_uri>
    		</data>
    		<total>624000</total>
    		<total_tax>106080</total_tax>
    		<total_without_tax>517920</total_without_tax>
    		<count_installment>0</count_installment>
    	</myorder>
    	<diagnostic>
    		<status>200</status>
    		<elapsetime>0.2612</elapsetime>
    		<memoryusage>17.87MB</memoryusage>
    		<confirm>success</confirm>
    		<lang>en</lang>
    		<currency>IDR</currency>
    	</diagnostic>
    	<checkout>
    		https://api-sandbox.tiket.com/order/checkout/120152/IDR
    	</checkout>
    	<login_status>false</login_status>
    	<token>8f683005261f872fe5c044f9b7085162</token>
    </tiket>
```

```json
    {"output_type":"json","myorder":{"order_id":"120152","data":[{"expire":60,"order_detail_id":"31406","order_type":"hotel","order_name":"The 101 Legian","order_name_detail":"Superior (Room Only)","tenor":"0","detail":{"order_detail_id":"31406","room_id":"1185","rooms":"1","adult":"2","child":"0","startdate":"11 Jun 2012","enddate":"12 Jun 2012","nights":"1","price":517920},"order_photo":"http:\/\/www.sandbox.tiket.com\/img\/business\/1\/0\/business-10211.s.jpg","tax":106080,"item_charge":0,"subtotal_and_charge":"624000.00","delete_uri":"https:\/\/api-sandbox.tiket.com\/order\/delete_order?order_detail_id=31406"}],"total":624000,"total_tax":106080,"total_without_tax":517920,"count_installment":0},"diagnostic":{"status":200,"elapsetime":"0.2683","memoryusage":"17.85MB","confirm":"success","lang":"en","currency":"IDR"},"checkout":"https:\/\/api-sandbox.tiket.com\/order\/checkout\/120152\/IDR","login_status":"false","token":"8f683005261f872fe5c044f9b7085162"}
```

```matlab
    a:6:{s:11:"output_type";s:9:"serialize";s:7:"myorder";a:6:{s:8:"order_id";s:6:"120152";s:4:"data";a:1:{i:0;a:12:{s:6:"expire";i:60;s:15:"order_detail_id";s:5:"31406";s:10:"order_type";s:5:"hotel";s:10:"order_name";s:14:"The 101 Legian";s:17:"order_name_detail";s:20:"Superior (Room Only)";s:5:"tenor";s:1:"0";s:6:"detail";a:9:{s:15:"order_detail_id";s:5:"31406";s:7:"room_id";s:4:"1185";s:5:"rooms";s:1:"1";s:5:"adult";s:1:"2";s:5:"child";s:1:"0";s:9:"startdate";s:11:"11 Jun 2012";s:7:"enddate";s:11:"12 Jun 2012";s:6:"nights";s:1:"1";s:5:"price";d:517920;}s:11:"order_photo";s:67:"http://www.sandbox.tiket.com/img/business/1/0/business-10211.s.jpg";s:3:"tax";d:106080;s:11:"item_charge";i:0;s:19:"subtotal_and_charge";s:9:"624000.00";s:10:"delete_uri";s:71:"https://api-sandbox.tiket.com/order/delete_order?order_detail_id=31406";}}s:5:"total";d:624000;s:9:"total_tax";d:106080;s:17:"total_without_tax";d:517920;s:17:"count_installment";i:0;}s:10:"diagnostic";a:6:{s:6:"status";i:200;s:10:"elapsetime";s:14:"0.3174";s:11:"memoryusage";s:14:"17.85MB";s:7:"confirm";s:7:"success";s:4:"lang";s:2:"en";s:8:"currency";s:3:"IDR";}s:8:"checkout";s:56:"https://api-sandbox.tiket.com/order/checkout/120152/IDR";s:12:"login_status";s:5:"false";s:5:"token";s:32:"8f683005261f872fe5c044f9b7085162";}
```
    
    
## Checkout Page Request

Early stage to access checkout.

#### Parameters

[table]  
Name,Description,Format,Default,Mandatory  
token,for saving transaction that done by user,CHAR(128),,TRUE  
[/table]

#### Input

    `https://api-sandbox.tiket.com/order/checkout/119978/IDR?token=9991e3092aea96042964220181374b60&output=json`

Get from order page in checkout variable.

#### Output

```xml
    <tiket>
    	<output_type>xml</output_type>
    	<next_checkout_uri>
    		httpss://api-sandbox.tiket.com/checkout/checkout_customer
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
    {"output_type":"json","next_checkout_uri":"httpss:\/\/api-sandbox.tiket.com\/checkout\/checkout_customer","diagnostic":{"status":200,"elapsetime":"0.1157","memoryusage":"6.43MB","confirm":"success","lang":"id","currency":"IDR"},"login_status":"false","token":"9991e3092aea96042964220181374b60"}
```

```matlab
    a:5:{s:11:"output_type";s:9:"serialize";s:17:"next_checkout_uri";s:57:"httpss://api-sandbox.tiket.com/checkout/checkout_customer";s:10:"diagnostic";a:7:{s:6:"status";i:200;s:10:"elapsetime";s:14:"0.1132";s:11:"memoryusage";s:14:"6.43MB";s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:12:"login_status";s:5:"false";s:5:"token";s:32:"9991e3092aea96042964220181374b60";}
```
    
    
## Checkout Login

#### Parameters

[table]  
Name,Description,Format,Default,Mandatory  
salutation,"your title( ex: Mr.,Mrs.,Ms.)",CHAR(5),,TRUE  
firstName,your first name,CHAR(50),,TRUE  
lastName,your last name,CHAR(50),,TRUE  
emailAddress,your email,CHAR(50),,TRUE  
phone,"your phone, ex: 081232323343 or +62324324234234. Don't forget to urlencode + into %2B in the GET parameter",CHAR(20),,TRUE  
saveContinue,"Flag for save unregistered user data (value=2)",,,TRUE  
[/table]

#### Input

    `https://api-sandbox.tiket.com/checkout/checkout_customer?token=87da88eaaa429d5513a3a3658b01701e&salutation=Ms&firstName=ba&lastName=ca&emailAddress=testing@yahoocom&phone=%2B62878434343&saveContinue=2&output=json`

Setelah merequest link tersebut maka user akan dibuatkan account di tiket.com  
user akan dikirimkan email untuk mengubah password loginnya.

#### Output

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
    {"output_type":"json","diagnostic":{"status":200,"elapsetime":"0.1443","memoryusage":"7.77MB","confirm":"success","error_msgs":"","lang":"en","currency":"IDR"},"login_status":"true","guest_id":"21688","token":"5a80dc2ccce351eeb412e835b651edb9"}
```



```matlab
    [a:5:{s:11:"output_type";s:9:"serialize";s:10:"diagnostic";a:7:{s:6:"status";i:200;s:10:"elapsetime";s:14:"0.1628";s:11:"memoryusage";s:14:"7.77MB";s:7:"confirm";s:7:"success";s:10:"error_msgs";s:0:"";s:4:"lang";s:2:"en";s:8:"currency";s:3:"IDR";}s:12:"login_status";s:4:"true";s:8:"guest_id";s:5:"21688";s:5:"token";s:32:"9d4ccf0c966e37a4c112c59ac2bc2e97";}
```
    
    
## Checkout Customer

#### Parameters

[table]  
Name,Description,Format,Default,Mandatory  
token,for saving transaction that done by user,CHAR(128),,TRUE  
salutation,"your title( ex: Mr.,Mrs.,Ms.)",CHAR(5),,TRUE  
firstName,your first name,CHAR(50),,TRUE  
lastName,your last name CHAR(50),,TRUE  
phone,"your phone, ex: 081232323343 or +62324324234234. Don't forget to urlencode + into %2B in the GET parameter",CHAR(20),,TRUE  
conSalutation,"contact person title ( ex: Mr.,Mrs.,Ms.)",CHAR(5),,TRUE  
conFirstName,contact person first name,CHAR(50),,TRUE  
conLastName,contact person last name,CHAR(50),,TRUE  
conEmailAddress,contact person email address,CHAR(50),,TRUE  
conPhone,"contact person phone, ex: 081232323343 or +62324324234234. Don't forget to urlencode + into %2B in the GET parameter",CHAR(20),,TRUE  
detailId,your order detail id,NUMBER,,TRUE  
country,User country,CHAR(5),,TRUE  
[/table]

#### Input

    `https://api-sandbox.tiket.com/checkout/checkout_customer?token=8f683005261f872fe5c044f9b7085162&salutation=Mrs&firstName=ba&lastName=ca&emailAddress=bibi@yahoocom&phone=%2B628888843&conSalutation=Mrs&conFirstName=a&conLastName=a&conEmailAddress=bibi@yahoocom&conPhone=%2B628888843&detailId=31406&country=id&output=json`

#### Output

```xml
    <tiket>
    	<output_type>xml</output_type>
    	<diagnostic>
    		<status>201</status>
    		<elapsetime>0.2901</elapsetime>
    		<memoryusage>19.21MB</memoryusage>
    		<error_msgs>Your Contact Person details has been saved.</error_msgs>
    		<lang>en</lang>
    		<currency>IDR</currency>
    	</diagnostic>
    	<currProfileArr>
    		<account_id>106238</account_id>
    		<account_first_name>a</account_first_name>
    		<account_last_name>a</account_last_name>
    		<account_mobile>+62811123123</account_mobile>
    		<account_salutation_name>Mrs</account_salutation_name>
    		<account_phone>+628888843</account_phone>
    		<account_username>youjulin@gmailcom</account_username>
    		<profile_id>15772</profile_id>
    		<Name>a a</Name>
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
    		<account_profile_modified>2012-06-11 17:10:29</account_profile_modified>
    		<account_birthdate/>
    		<account_gender>F</account_gender>
    		<account_id_card/>
    	</currProfileArr>
    	<currProfileId>15772</currProfileId>
    	<travellerProfileArr>
    		<account_salutation_name>Mrs</account_salutation_name>
    		<account_first_name>ba</account_first_name>
    		<account_last_name>ca</account_last_name>
    		<account_phone>+628888843</account_phone>
    	</travellerProfileArr>
    	<contactProfileArr>
    		<account_salutation_name>Mrs</account_salutation_name>
    		<account_first_name>a</account_first_name>
    		<account_last_name>a</account_last_name>
    		<account_username>bibi@yahoocom</account_username>
    		<account_phone>+628888843</account_phone>
    	</contactProfileArr>
    	<statusClass>ok</statusClass>
    	<SideArr>
    		<currBookingArr>
    			<detail_id>31406</detail_id>
    			<type>hotel</type>
    			<master_name>The 101 Legian</master_name>
    			<detail_name>Superior (Room Only)</detail_name>
    			<contact_person>15772</contact_person>
    			<last_update_contact_person>0</last_update_contact_person>
    			<order_type>hotel</order_type>
    			<hotel_name>The 101 Legian</hotel_name>
    			<nights>1</nights>
    			<check_in_first>11 Jun 2012</check_in_first>
    			<check_in_last>12 Jun 2012</check_in_last>
    			<adult>2</adult>
    			<child>0</child>
    			<rooms>1</rooms>
    			<file_name/>
    			<last_update_cp>0</last_update_cp>
    			<master_id>4108</master_id>
    			<room_id>1185</room_id>
    			<need_process>1</need_process>
    		</currBookingArr>
    	</SideArr>
    	<login_status>true</login_status>
    	<id>106238</id>
    	<token>8f683005261f872fe5c044f9b7085162</token>
    </tiket>
```

```json
    {"output_type":"json","diagnostic":{"status":201,"elapsetime":"0.3014","memoryusage":"19.19MB","error_msgs":"Your Contact Person details has been saved.","lang":"en","currency":"IDR"},"currProfileArr":{"account_id":"106238","account_first_name":"a","account_last_name":"a","account_mobile":"+62811123123","account_salutation_name":"Mrs.","account_phone":"+628888843","account_username":"you.jul.in@gmail.com","profile_id":"15774","Name":"a a","address_country":null,"address_address1":null,"address_address2":null,"address_kabupaten":null,"address_province":null,"address_zipcode":null,"account_created":"2012-06-11 11:24:28","account_password":"021768c0b31cd2ad68b201213ff0e102","account_source":"tiket","photo":"default-default.jpg","account_profile_modified":"2012-06-11 17:10:53","account_birthdate":null,"account_gender":"F","account_id_card":null},"currProfileId":"15774","travellerProfileArr":{"account_salutation_name":"Mrs.","account_first_name":"ba","account_last_name":"ca","account_phone":"+628888843"},"contactProfileArr":{"account_salutation_name":"Mrs.","account_first_name":"a","account_last_name":"a","account_username":"bibi@ads.com","account_phone":"+628888843"},"statusClass":"ok","next":"http:\/\/api-sandbox.tiket.com\/checkout\/checkout_payment","SideArr":{"currBookingArr":{"detail_id":"31406","type":"hotel","master_name":"The 101 Legian","detail_name":"Superior (Room Only)","contact_person":"15774","last_update_contact_person":"0","order_type":"hotel","hotel_name":"The 101 Legian","nights":"1","check_in_first":"11 Jun 2012","check_in_last":"12 Jun 2012","adult":"2","child":"0","rooms":"1","file_name":null,"last_update_cp":"0","master_id":"4108","room_id":"1185","need_process":1}},"login_status":"true","id":"106238","token":"8f683005261f872fe5c044f9b7085162"}
```

```matlab
    a:11:{s:11:"output_type";s:9:"serialize";s:10:"diagnostic";a:6:{s:6:"status";i:201;s:10:"elapsetime";s:14:"0.2899";s:11:"memoryusage";s:14:"19.2MB";s:10:"error_msgs";s:42:"Your Contact Person details has been saved.";s:4:"lang";s:2:"en";s:8:"currency";s:3:"IDR";}s:14:"currProfileArr";a:23:{s:10:"account_id";s:6:"106238";s:18:"account_first_name";s:1:"a";s:17:"account_last_name";s:1:"a";s:14:"account_mobile";s:6:"021343";s:23:"account_salutation_name";s:4:"Mrs.";s:13:"account_phone";s:8:"+628888843";s:16:"account_username";s:20:"you.jul.in@gmail.com";s:10:"profile_id";s:5:"15775";s:4:"Name";s:3:"a a";s:15:"address_country";N;s:16:"address_address1";N;s:16:"address_address2";N;s:17:"address_kabupaten";N;s:16:"address_province";N;s:15:"address_zipcode";N;s:15:"account_created";s:19:"2012-06-11 11:24:28";s:16:"account_password";s:32:"021768c0b31cd2ad68b201213ff0e102";s:14:"account_source";s:5:"tiket";s:5:"photo";s:19:"default-default.jpg";s:24:"account_profile_modified";s:19:"2012-06-11 17:12:43";s:17:"account_birthdate";N;s:14:"account_gender";s:1:"F";s:15:"account_id_card";N;}s:13:"currProfileId";s:5:"15775";s:19:"travellerProfileArr";a:4:{s:23:"account_salutation_name";s:4:"Mrs.";s:18:"account_first_name";s:2:"ba";s:17:"account_last_name";s:2:"ca";s:13:"account_phone";s:8:"+628888843";}s:17:"contactProfileArr";a:5:{s:23:"account_salutation_name";s:4:"Mrs.";s:18:"account_first_name";s:1:"a";s:17:"account_last_name";s:1:"a";s:16:"account_username";s:12:"bibi@ads.com";s:13:"account_phone";s:8:"+628888843";}s:11:"statusClass";s:2:"ok";s:7:"SideArr";a:1:{s:14:"currBookingArr";a:19:{s:9:"detail_id";s:5:"31406";s:4:"type";s:5:"hotel";s:11:"master_name";s:14:"The 101 Legian";s:11:"detail_name";s:20:"Superior (Room Only)";s:14:"contact_person";s:5:"15775";s:26:"last_update_contact_person";s:1:"0";s:10:"order_type";s:5:"hotel";s:10:"hotel_name";s:14:"The 101 Legian";s:6:"nights";s:1:"1";s:14:"check_in_first";s:11:"11 Jun 2012";s:13:"check_in_last";s:11:"12 Jun 2012";s:5:"adult";s:1:"2";s:5:"child";s:1:"0";s:5:"rooms";s:1:"1";s:9:"file_name";N;s:14:"last_update_cp";s:1:"0";s:9:"master_id";s:4:"4108";s:7:"room_id";s:4:"1185";s:12:"need_process";i:1;}}s:12:"login_status";s:4:"true";s:2:"id";s:6:"106238";s:5:"token";s:32:"8f683005261f872fe5c044f9b7085162";}
```
    


## Available Payment

#### Parameters

[table]  
Name,Description,Format,Default,Mandatory  
token,for saving transaction that done by user,CHAR(128),,TRUE  
[/table]

#### Input

    `http://api-sandbox.tiket.com/checkout/checkout_payment?token=87da88eaaa429d5513a3a3658b01701e`

#### Output

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
    		<link>
    			https://api-sandbox.tiket.com/checkout/checkout_payment/1
    		</link>
    		<text>Kartu Kredit</text>
    		<message/>
    	</available_payment>
    	<available_payment>
    		<link>
    			https://api-sandbox.tiket.com/checkout/checkout_payment/2
    		</link>
    		<text>Transfer Lewat Bank</text>
    		<message/>
    	</available_payment>
    	<available_payment>
    		<link>
    			https://api-sandbox.tiket.com/checkout/checkout_payment/3
    		</link>
    		<text>KlikBCA</text>
    		<message/>
    	</available_payment>
    	<available_payment>
    		<link>
    			https://api-sandbox.tiket.com/checkout/checkout_payment/4
    		</link>
    		<text>BCA KlikPay</text>
    		<message/>
    	</available_payment>
    	<available_payment>
    		<link>
    			https://api-sandbox.tiket.com/checkout/checkout_payment/20
    		</link>
    		<text>COD</text>
    		<message/>
    	</available_payment>
    	<token>62bc0e3bd0c127c5690125a76e11c23c</token>
    </tiket>
```



```json
    {"output_type":"json","diagnostic":{"status":200,"elapsetime":"0.5625","memoryusage":"18.74MB","confirm":"success","lang":"id","currency":"IDR"},"available_payment":[{"link":"https:\/\/api-sandbox.tiket.com\/checkout\/checkout_payment\/1","text":"Kartu Kredit","message":""},{"link":"https:\/\/api-sandbox.tiket.com\/checkout\/checkout_payment\/2","text":"Transfer Lewat Bank","message":""},{"link":"https:\/\/api-sandbox.tiket.com\/checkout\/checkout_payment\/3","text":"KlikBCA","message":""},{"link":"https:\/\/api-sandbox.tiket.com\/checkout\/checkout_payment\/4","text":"BCA KlikPay","message":""},{"link":"https:\/\/api-sandbox.tiket.com\/checkout\/checkout_payment\/20","text":"COD","message":""}],"token":"62bc0e3bd0c127c5690125a76e11c23c"}
```



```matlab
    a:4:{s:11:"output_type";s:9:"serialize";s:10:"diagnostic";a:6:{s:6:"status";i:200;s:10:"elapsetime";s:14:"0.5329";s:11:"memoryusage";s:14:"18.74MB";s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:17:"available_payment";a:5:{i:0;a:3:{s:4:"link";s:58:"https://api-sandbox.tiket.com/checkout/checkout_payment/1";s:4:"text";s:22:"Kartu Kredit";s:7:"message";s:0:"";}i:1;a:3:{s:4:"link";s:58:"https://api-sandbox.tiket.com/checkout/checkout_payment/2";s:4:"text";s:24:"Transfer Lewat Bank";s:7:"message";s:0:"";}i:2;a:3:{s:4:"link";s:58:"https://api-sandbox.tiket.com/checkout/checkout_payment/3";s:4:"text";s:7:"KlikBCA";s:7:"message";s:0:"";}i:3;a:3:{s:4:"link";s:58:"https://api-sandbox.tiket.com/checkout/checkout_payment/4";s:4:"text";s:11:"BCA KlikPay";s:7:"message";s:0:"";}i:4;a:3:{s:4:"link";s:59:"https://api-sandbox.tiket.com/checkout/checkout_payment/20";s:4:"text";s:3:"COD";s:7:"message";s:0:"";}}s:5:"token";s:32:"62bc0e3bd0c127c5690125a76e11c23c";}
```
    
    
## Checkout Payment

Please see [Checkout Payment](http://docs.tiket.com/#checkout-payment-309) in General API

























