# Hotel API

NOTE :  
* Data that is provided for testing is different from the actual data
* If want to test add order hotel, please use "The Sunset Hotel and Restaurant" on Legian, Bali. Since not all hotel in development server consistently have room allotment to book.

These are the API command for Hotel

Diagram flow for Hotel API:  

![Hotel API](https://raw.githubusercontent.com/tiket-dev/slate/master/source/images/Diagram-Flow-API-Hotel.png)

## Search Hotel

```xml
<?xml version="1.0" encoding="utf-8"?>
<tiket>
    <diagnostic>
        <status>200</status>
        <elapsetime>1.9074</elapsetime>
        <memoryusage>22.8MB</memoryusage>
        <unix_timestamp>1470370396</unix_timestamp>
        <confirm>success</confirm>
        <lang>id</lang>
        <currency>IDR</currency>
    </diagnostic>
    <output_type>xml</output_type>
    <search_queries>
        <q>Yogyakarta</q>
        <uid></uid>
        <startdate>2016-08-11</startdate>
        <enddate>2016-08-12</enddate>
        <night>1</night>
        <room>1</room>
        <adult>2</adult>
        <child>0</child>
        <sort></sort>
        <minstar>0</minstar>
        <maxstar>5</maxstar>
        <minprice>118000.00</minprice>
        <maxprice>1000000000.00</maxprice>
        <distance>100000</distance>
    </search_queries>
    <results>
        <result>
            <province_name>Daerah Istimewa Yogyakarta</province_name>
            <kecamatan_name> </kecamatan_name>
            <kelurahan_name> </kelurahan_name>
            <business_uri>https://api-sandbox.tiket.com/wwwh-boutiquehotelcom?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;is_partner=0&amp;star_rating=0&amp;hotel_chain=0&amp;facilities=0&amp;latitude=0&amp;longitude=0&amp;distance=0&amp;uid=business%3A21298812</business_uri>
            <photo_primary>https://sandbox.tiket.com/img/default/d/e/default-default.sq2.jpg</photo_primary>
            <star_rating>3</star_rating>
            <id>76233820160811</id>
            <room_available>4</room_available>
            <latitude>-7.77923380000000000000</latitude>
            <longitude>110.37961110000003000000</longitude>
            <room_max_occupancies>2</room_max_occupancies>
            <rating></rating>
            <oldprice>539991.00</oldprice>
            <room_facility_name></room_facility_name>
            <address></address>
            <wifi></wifi>
            <promo_name></promo_name>
            <price>345000.00</price>
            <total_price>345000.00</total_price>
            <regional>  -   - Daerah Istimewa Yogyakarta</regional>
            <name></name>
            <hotel_id>21298812</hotel_id>
        </result>
        <result>
            <province_name>Daerah Istimewa Yogyakarta</province_name>
            <kecamatan_name> </kecamatan_name>
            <kelurahan_name> </kelurahan_name>
            <business_uri>https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/gejayan/the-edelweis-hotel-yogyakarta?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;is_partner=0&amp;star_rating=0&amp;hotel_chain=0&amp;facilities=0&amp;latitude=0&amp;longitude=0&amp;distance=0&amp;uid=business%3A15810</business_uri>
            <photo_primary>https://sandbox.tiket.com/img/business/t/w/business-twice_room_2_-312x234-.sq2.jpg</photo_primary>
            <star_rating>3</star_rating>
            <id>62897320160811</id>
            <room_available>10</room_available>
            <latitude>-7.78165320000000000000</latitude>
            <longitude>110.38783779999994000000</longitude>
            <room_max_occupancies>2</room_max_occupancies>
            <rating>8.1</rating>
            <tripadvisor_avg_rating>
                <avg_rating>3.5</avg_rating>
                <image_url>http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.5-18379-4.gif</image_url>
                <review_count>108</review_count>
                <url>http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=2545466&amp;lang=en_US&amp;partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&amp;isTA=true&amp;format=html&amp;display=true</url>
            </tripadvisor_avg_rating>
            <oldprice>586946.00</oldprice>
            <room_facility_name></room_facility_name>
            <address>Jl. Gejayan 17C, Gondokusuman, Yogyakarta</address>
            <wifi></wifi>
            <promo_name></promo_name>
            <price>375000.00</price>
            <total_price>375000.00</total_price>
            <regional>  -   - Daerah Istimewa Yogyakarta</regional>
            <name>The Edelweis Yogyakarta</name>
            <hotel_id>15810</hotel_id>
        </result>
        <result>
            <province_name>Daerah Istimewa Yogyakarta</province_name>
            <kecamatan_name>Sleman</kecamatan_name>
            <kelurahan_name> </kelurahan_name>
            <business_uri>https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/yogyakarta/fortune-fest-hotel-yogyakarta?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;is_partner=0&amp;star_rating=0&amp;hotel_chain=0&amp;facilities=0&amp;latitude=0&amp;longitude=0&amp;distance=0&amp;uid=business%3A20585137</business_uri>
            <photo_primary>https://sandbox.tiket.com/img/business/i/m/business-img_9741.sq2.jpg</photo_primary>
            <star_rating>3</star_rating>
            <id>74956320160811</id>
            <room_available>222</room_available>
            <latitude>-7.76572909999999900000</latitude>
            <longitude>110.41054290000000000000</longitude>
            <room_max_occupancies>2</room_max_occupancies>
            <rating></rating>
            <tripadvisor_avg_rating>
                <avg_rating>3.5</avg_rating>
                <image_url>http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.5-18379-4.gif</image_url>
                <review_count>106</review_count>
                <url>http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=2687978&amp;lang=en_US&amp;partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&amp;isTA=true&amp;format=html&amp;display=true</url>
            </tripadvisor_avg_rating>
            <oldprice>591642.00</oldprice>
            <room_facility_name></room_facility_name>
            <address>Jl. Raya Seturan , Depok, Sleman</address>
            <wifi></wifi>
            <promo_name></promo_name>
            <price>378000.00</price>
            <total_price>378000.00</total_price>
            <regional>  - Sleman - Daerah Istimewa Yogyakarta</regional>
            <name>Fortune Fest Hotel Yogyakarta</name>
            <hotel_id>20585137</hotel_id>
        </result>
        <result>
            <province_name>Daerah Istimewa Yogyakarta</province_name>
            <kecamatan_name> </kecamatan_name>
            <kelurahan_name> </kelurahan_name>
            <business_uri>https://api-sandbox.tiket.com/hotel/indonesia/bandung/kebon-kawung/mutiara-hotel-bandung?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;is_partner=0&amp;star_rating=0&amp;hotel_chain=0&amp;facilities=0&amp;latitude=0&amp;longitude=0&amp;distance=0&amp;uid=business%3A18</business_uri>
            <photo_primary>https://sandbox.tiket.com/img/business/y/u/business-yufgfyu.sq2.jpg</photo_primary>
            <star_rating>3</star_rating>
            <id>56912220160811</id>
            <room_available>10</room_available>
            <latitude>-6.91237020000000100000</latitude>
            <longitude>107.59834820000003000000</longitude>
            <room_max_occupancies>2</room_max_occupancies>
            <rating>7.0</rating>
            <tripadvisor_avg_rating>
                <avg_rating>3.0</avg_rating>
                <image_url>http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.0-18379-4.gif</image_url>
                <review_count>89</review_count>
                <url>http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=1016088&amp;lang=en_US&amp;partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&amp;isTA=true&amp;format=html&amp;display=true</url>
            </tripadvisor_avg_rating>
            <oldprice>499296.00</oldprice>
            <room_facility_name></room_facility_name>
            <address>Kebon Kawung Street 60, Cicendo, Bandung</address>
            <wifi></wifi>
            <promo_name></promo_name>
            <price>319000.00</price>
            <total_price>319000.00</total_price>
            <regional>  -   - Daerah Istimewa Yogyakarta</regional>
            <name>Hotel Mutiara</name>
            <hotel_id>18</hotel_id>
        </result>
        <result>
            <province_name>Daerah Istimewa Yogyakarta</province_name>
            <kecamatan_name> </kecamatan_name>
            <kelurahan_name> </kelurahan_name>
            <business_uri>https://api-sandbox.tiket.com/student-park-hotel-apartment-yogyakarta?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;is_partner=0&amp;star_rating=0&amp;hotel_chain=0&amp;facilities=0&amp;latitude=0&amp;longitude=0&amp;distance=0&amp;uid=business%3A21307287</business_uri>
            <photo_primary>https://sandbox.tiket.com/img/default/d/e/default-default.sq2.jpg</photo_primary>
            <star_rating>3</star_rating>
            <id>57184620160811</id>
            <room_available>1</room_available>
            <latitude>-7.76962580000000000000</latitude>
            <longitude>110.40610650000008000000</longitude>
            <room_max_occupancies>2</room_max_occupancies>
            <rating></rating>
            <tripadvisor_avg_rating>
                <avg_rating>4.5</avg_rating>
                <image_url>http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.5-18379-4.gif</image_url>
                <review_count>33</review_count>
                <url>http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=8037466&amp;lang=en_US&amp;partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&amp;isTA=true&amp;format=html&amp;display=true</url>
            </tripadvisor_avg_rating>
            <oldprice>766943.00</oldprice>
            <room_facility_name></room_facility_name>
            <address></address>
            <wifi></wifi>
            <promo_name></promo_name>
            <price>490000.00</price>
            <total_price>490000.00</total_price>
            <regional>  -   - Daerah Istimewa Yogyakarta</regional>
            <name></name>
            <hotel_id>21307287</hotel_id>
        </result>
        <result>
            <province_name>Daerah Istimewa Yogyakarta</province_name>
            <kecamatan_name>Sleman</kecamatan_name>
            <kelurahan_name> </kelurahan_name>
            <business_uri>https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/sinduadi/crystal-lotus-hotel-yogyakarta-managed-by-prabu?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;is_partner=0&amp;star_rating=0&amp;hotel_chain=0&amp;facilities=0&amp;latitude=0&amp;longitude=0&amp;distance=0&amp;uid=business%3A20087341</business_uri>
            <photo_primary>https://sandbox.tiket.com/img/business/c/r/business-crystal-lotus-exterior1.sq2.jpg</photo_primary>
            <star_rating>4</star_rating>
            <id>48240320160811</id>
            <room_available>30</room_available>
            <latitude>-7.76306949999999900000</latitude>
            <longitude>110.36527960000001000000</longitude>
            <room_max_occupancies>2</room_max_occupancies>
            <rating></rating>
            <tripadvisor_avg_rating>
                <avg_rating>3.5</avg_rating>
                <image_url>http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.5-18379-4.gif</image_url>
                <review_count>83</review_count>
                <url>http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=6557803&amp;lang=en_US&amp;partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&amp;isTA=true&amp;format=html&amp;display=true</url>
            </tripadvisor_avg_rating>
            <room_facility_name>%25hotel_nonsmoking_rooms%25%7C%25hotel_in_room_safe%25%7C%25hotel_ac%25%7C%25hotel_inet_wifi%25%7C%25hotel_inet_wifi_compl%25%7C%25hotel_lcd_plasma%25%7C%25hotel_sat_cable%25%7C%25hotel_desk%25%7C%25hotel_shower%25%7C%25hotel_bathrobes%25%7C%25hotel_bathtub%25%7C%25hotel_hair_dryer%25%7C%25hotel_mini_bar%25%7C%25hotel_coffee_tea+maker%25%7C%25hotel_complimentary_bottled_water%25%7C%25hotel_television%25%7C%25hotel_telephone%25%7C%25hotel_slipper%25%7C%25hotel_mirror%25%7C%25hotel_iron_board_on_request%25%7C%25hotel_refrigerator%25%7C%25hotel_balcony%25%7C%25hotel_free_toiletries%25%7C%25hotel_Hot_Cold_Shower%25</room_facility_name>
            <oldprice>617002.00</oldprice>
            <address>Magelang Street KM.  5,2 Yogyakarta, Sleman, Sleman</address>
            <wifi>Wi-Fi Tersedia</wifi>
            <promo_name></promo_name>
            <price>443478.00</price>
            <total_price>443478.00</total_price>
            <regional>  - Sleman - Daerah Istimewa Yogyakarta</regional>
            <name>Crystal Lotus Hotel Yogyakarta Managed By Prabu</name>
            <hotel_id>20087341</hotel_id>
        </result>
        <result>
            <province_name>Daerah Istimewa Yogyakarta</province_name>
            <kecamatan_name> </kecamatan_name>
            <kelurahan_name> </kelurahan_name>
            <business_uri>https://api-sandbox.tiket.com/pandanaran-hotel-yogyakarta?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;is_partner=0&amp;star_rating=0&amp;hotel_chain=0&amp;facilities=0&amp;latitude=0&amp;longitude=0&amp;distance=0&amp;uid=business%3A21222561</business_uri>
            <photo_primary>https://sandbox.tiket.com/img/default/d/e/default-default.sq2.jpg</photo_primary>
            <star_rating>3</star_rating>
            <id>55003720160811</id>
            <room_available>12</room_available>
            <latitude>-7.81918940000000100000</latitude>
            <longitude>110.37059939999995000000</longitude>
            <room_max_occupancies>2</room_max_occupancies>
            <rating></rating>
            <tripadvisor_avg_rating>
                <avg_rating>4.0</avg_rating>
                <image_url>http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif</image_url>
                <review_count>79</review_count>
                <url>http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=7808044&amp;lang=en_US&amp;partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&amp;isTA=true&amp;format=html&amp;display=true</url>
            </tripadvisor_avg_rating>
            <oldprice>513382.00</oldprice>
            <room_facility_name></room_facility_name>
            <address></address>
            <wifi></wifi>
            <promo_name></promo_name>
            <price>328000.00</price>
            <total_price>328000.00</total_price>
            <regional>  -   - Daerah Istimewa Yogyakarta</regional>
            <name></name>
            <hotel_id>21222561</hotel_id>
        </result>
        <result>
            <province_name>Daerah Istimewa Yogyakarta</province_name>
            <kecamatan_name> </kecamatan_name>
            <kelurahan_name> </kelurahan_name>
            <business_uri>https://api-sandbox.tiket.com/hotel-neo-malioboro?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;is_partner=0&amp;star_rating=0&amp;hotel_chain=0&amp;facilities=0&amp;latitude=0&amp;longitude=0&amp;distance=0&amp;uid=business%3A21402180</business_uri>
            <photo_primary>https://sandbox.tiket.com/img/default/d/e/default-default.sq2.jpg</photo_primary>
            <star_rating>3</star_rating>
            <id>62897720160811</id>
            <room_available>112</room_available>
            <latitude>-7.79001630000000000000</latitude>
            <longitude>110.36312539999994000000</longitude>
            <room_max_occupancies>2</room_max_occupancies>
            <rating></rating>
            <tripadvisor_avg_rating>
                <avg_rating>4.0</avg_rating>
                <image_url>http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif</image_url>
                <review_count>399</review_count>
                <url>http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=8092831&amp;lang=en_US&amp;partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&amp;isTA=true&amp;format=html&amp;display=true</url>
            </tripadvisor_avg_rating>
            <oldprice>771500.00</oldprice>
            <room_facility_name></room_facility_name>
            <address></address>
            <wifi></wifi>
            <promo_name></promo_name>
            <price>481580.00</price>
            <total_price>481580.00</total_price>
            <regional>  -   - Daerah Istimewa Yogyakarta</regional>
            <name></name>
            <hotel_id>21402180</hotel_id>
        </result>
        <result>
            <province_name>Daerah Istimewa Yogyakarta</province_name>
            <kecamatan_name>Mantrijeron</kecamatan_name>
            <kelurahan_name>Suryodiningratan</kelurahan_name>
            <business_uri>https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/seturan/the-victoria-hotel?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;is_partner=0&amp;star_rating=0&amp;hotel_chain=0&amp;facilities=0&amp;latitude=0&amp;longitude=0&amp;distance=0&amp;uid=business%3A3031</business_uri>
            <photo_primary>https://sandbox.tiket.com/img/business/v/i/business-victoria-yogya-pool.sq2.jpg</photo_primary>
            <star_rating>3</star_rating>
            <id>31420160811</id>
            <room_available>3</room_available>
            <latitude>-7.78319030000000000000</latitude>
            <longitude>110.40225609999993000000</longitude>
            <room_max_occupancies>2</room_max_occupancies>
            <rating>7.6</rating>
            <tripadvisor_avg_rating>
                <avg_rating>4.0</avg_rating>
                <image_url>http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif</image_url>
                <review_count>55</review_count>
                <url>http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=2348889&amp;lang=en_US&amp;partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&amp;isTA=true&amp;format=html&amp;display=true</url>
            </tripadvisor_avg_rating>
            <room_facility_name>%25hotel_ac%25%7C%25hotel_inet_wifi%25%7C%25hotel_lcd_plasma%25%7C%25hotel_sat_cable%25%7C%25hotel_desk%25%7C%25hotel_shower%25%7C%25hotel_mini_bar%25%7C%25hotel_coffee_tea+maker%25%7C%25hotel_complimentary_bottled_water%25</room_facility_name>
            <oldprice>1408671.00</oldprice>
            <address>Jl. Laksda Adisutjipto Km. 5 , Mantrijeron, Yogyakarta</address>
            <wifi>Wi-Fi Tersedia</wifi>
            <promo_name></promo_name>
            <price>900000.00</price>
            <total_price>900000.00</total_price>
            <regional>Suryodiningratan - Mantrijeron - Daerah Istimewa Yogyakarta</regional>
            <name>The Victoria Hotel Yogyakarta</name>
            <hotel_id>3031</hotel_id>
        </result>
        <result>
            <province_name>Daerah Istimewa Yogyakarta</province_name>
            <kecamatan_name>Gedong Tengen</kecamatan_name>
            <kelurahan_name>Sosromenduran</kelurahan_name>
            <business_uri>https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/malioboro/hotel-dafam-fortuna-malioboro-yogyakarta?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;is_partner=0&amp;star_rating=0&amp;hotel_chain=0&amp;facilities=0&amp;latitude=0&amp;longitude=0&amp;distance=0&amp;uid=business%3A20087773</business_uri>
            <photo_primary>https://sandbox.tiket.com/img/business/r/o/business-rooftop_pool2.sq2.jpg</photo_primary>
            <star_rating>3</star_rating>
            <id>48285920160811</id>
            <room_available>217</room_available>
            <latitude>-7.79369329999999900000</latitude>
            <longitude>110.36283040000000000000</longitude>
            <room_max_occupancies>2</room_max_occupancies>
            <rating></rating>
            <tripadvisor_avg_rating>
                <avg_rating>4.0</avg_rating>
                <image_url>http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif</image_url>
                <review_count>210</review_count>
                <url>http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=4876648&amp;lang=en_US&amp;partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&amp;isTA=true&amp;format=html&amp;display=true</url>
            </tripadvisor_avg_rating>
            <room_facility_name>%25hotel_in_room_safe%25%7C%25hotel_ac%25%7C%25hotel_inet_wifi%25%7C%25hotel_sat_cable%25%7C%25hotel_desk%25%7C%25hotel_shower%25%7C%25hotel_free_toiletries%25</room_facility_name>
            <oldprice>729379.00</oldprice>
            <address>Dagen Street No  60, Yogyakarta, Gedong Tengen, Yogyakarta</address>
            <wifi>Wi-Fi Tersedia</wifi>
            <promo_name></promo_name>
            <price>466000.00</price>
            <total_price>466000.00</total_price>
            <regional>Sosromenduran - Gedong Tengen - Daerah Istimewa Yogyakarta</regional>
            <name>Hotel Dafam Fortuna Malioboro Yogyakarta</name>
            <hotel_id>20087773</hotel_id>
        </result>
        <result>
            <province_name>Daerah Istimewa Yogyakarta</province_name>
            <kecamatan_name>Jetis</kecamatan_name>
            <kelurahan_name>Gowongan</kelurahan_name>
            <business_uri>https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/tugu-jogja/the-101-yogyakarta-tugu?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;is_partner=0&amp;star_rating=0&amp;hotel_chain=0&amp;facilities=0&amp;latitude=0&amp;longitude=0&amp;distance=0&amp;uid=business%3A20426620</business_uri>
            <photo_primary>https://sandbox.tiket.com/img/business/i/m/business-img_2590.sq2.jpg</photo_primary>
            <star_rating>4</star_rating>
            <id>46702820160811</id>
            <room_available>5</room_available>
            <latitude>-7.78507033179146600000</latitude>
            <longitude>110.36680161952972000000</longitude>
            <room_max_occupancies>2</room_max_occupancies>
            <rating></rating>
            <tripadvisor_avg_rating>
                <avg_rating>4.0</avg_rating>
                <image_url>http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif</image_url>
                <review_count>253</review_count>
                <url>http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=6739367&amp;lang=en_US&amp;partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&amp;isTA=true&amp;format=html&amp;display=true</url>
            </tripadvisor_avg_rating>
            <room_facility_name>%25hotel_in_room_safe%25%7C%25hotel_ac%25%7C%25hotel_sat_cable%25%7C%25hotel_shower%25%7C%25hotel_hair_dryer%25%7C%25hotel_slipper%25%7C%25hotel_mirror%25%7C%25hotel_Hot_Cold_Shower%25</room_facility_name>
            <oldprice>1089358.00</oldprice>
            <address>Jalan Margoutomo No. 103 ( Mangkubumi), Yogyakarta , Jetis, Yogyakarta</address>
            <wifi></wifi>
            <promo_name></promo_name>
            <price>782990.00</price>
            <total_price>782990.00</total_price>
            <regional>Gowongan - Jetis - Daerah Istimewa Yogyakarta</regional>
            <name>THE 1O1 Yogyakarta Tugu</name>
            <hotel_id>20426620</hotel_id>
        </result>
        <result>
            <province_name>Daerah Istimewa Yogyakarta</province_name>
            <kecamatan_name> </kecamatan_name>
            <kelurahan_name> </kelurahan_name>
            <business_uri>https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/yogyakarta-airport/the-jayakarta-jogjakarta-hotel-spa?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;is_partner=0&amp;star_rating=0&amp;hotel_chain=0&amp;facilities=0&amp;latitude=0&amp;longitude=0&amp;distance=0&amp;uid=business%3A3786</business_uri>
            <photo_primary>https://sandbox.tiket.com/img/business/y/a/business-yajjarh.sq2.jpg</photo_primary>
            <star_rating>4</star_rating>
            <id>48065120160811</id>
            <room_available>12</room_available>
            <latitude>-7.78343729999999900000</latitude>
            <longitude>110.41959930000007000000</longitude>
            <room_max_occupancies>2</room_max_occupancies>
            <rating>7.9</rating>
            <tripadvisor_avg_rating>
                <avg_rating>3.5</avg_rating>
                <image_url>http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.5-18379-4.gif</image_url>
                <review_count>113</review_count>
                <url>http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=307834&amp;lang=en_US&amp;partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&amp;isTA=true&amp;format=html&amp;display=true</url>
            </tripadvisor_avg_rating>
            <room_facility_name>%25hotel_nonsmoking_rooms%25%7C%25hotel_ac%25%7C%25hotel_sat_cable%25%7C%25hotel_separate_shower_tub%25%7C%25hotel_mini_bar%25%7C%25hotel_coffee_tea+maker%25%7C%25hotel_complimentary_bottled_water%25%7C%25hotel_television%25%7C%25hotel_telephone%25%7C%25hotel_mirror%25%7C%25hotel_hair_dryer_on_request%25%7C%25hotel_balcony%25%7C%25hotel_Hot_Cold_Shower%25</room_facility_name>
            <oldprice>1363454.00</oldprice>
            <address>Jl. Laksda Adisucipto KM.8, Yogyakarta</address>
            <wifi></wifi>
            <promo_name></promo_name>
            <price>980000.00</price>
            <total_price>980000.00</total_price>
            <regional>  -   - Daerah Istimewa Yogyakarta</regional>
            <name>The Jayakarta Jogjakarta Hotel &amp;amp; Spa</name>
            <hotel_id>3786</hotel_id>
        </result>
        <result>
            <province_name>Daerah Istimewa Yogyakarta</province_name>
            <kecamatan_name>Jetis</kecamatan_name>
            <kelurahan_name>Bumijo</kelurahan_name>
            <business_uri>https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/sinduadi/hotel-tentrem-yogyakarta?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;is_partner=0&amp;star_rating=0&amp;hotel_chain=0&amp;facilities=0&amp;latitude=0&amp;longitude=0&amp;distance=0&amp;uid=business%3A19569414</business_uri>
            <photo_primary>https://sandbox.tiket.com/img/business/h/o/business-hoteltentrem_guest_r1.sq2.jpg</photo_primary>
            <star_rating>5</star_rating>
            <id>591620160811</id>
            <room_available>10</room_available>
            <latitude>-7.77713830000000000000</latitude>
            <longitude>110.36772680000001000000</longitude>
            <room_max_occupancies>2</room_max_occupancies>
            <rating>9.0</rating>
            <tripadvisor_avg_rating>
                <avg_rating>4.5</avg_rating>
                <image_url>http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.5-18379-4.gif</image_url>
                <review_count>540</review_count>
                <url>http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=3737584&amp;lang=en_US&amp;partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&amp;isTA=true&amp;format=html&amp;display=true</url>
            </tripadvisor_avg_rating>
            <room_facility_name>%25hotel_in_room_safe%25%7C%25hotel_ac%25%7C%25hotel_lcd_plasma%25%7C%25hotel_desk%25%7C%25hotel_shower%25%7C%25hotel_bathtub%25%7C%25hotel_hair_dryer%25%7C%25hotel_coffee_tea+maker%25%7C%25hotel_complimentary_bottled_water%25%7C%25hotel_television%25%7C%25hotel_telephone%25%7C%25hotel_free_toiletries%25%7C%25hotel_Cupboard%25%7C%25hotel_Hot_Cold_Shower%25%7CSatellite+TV+Service+%7CLCD+TV+%7CFree+Wi-Fi+%7CCable+TV+Service+%7CMinibar+</room_facility_name>
            <oldprice>1790143.00</oldprice>
            <address>Jl. AM Sangaji No. 72 A Yogyakarta 55233, Jetis, Yogyakarta</address>
            <wifi></wifi>
            <promo_name></promo_name>
            <price>1470500.00</price>
            <total_price>1470500.00</total_price>
            <regional>Bumijo - Jetis - Daerah Istimewa Yogyakarta</regional>
            <name>Hotel Tentrem Yogyakarta</name>
            <hotel_id>19569414</hotel_id>
        </result>
        <result>
            <province_name>Daerah Istimewa Yogyakarta</province_name>
            <kecamatan_name>Depok</kecamatan_name>
            <kelurahan_name>Condong Catur</kelurahan_name>
            <business_uri>https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/seturan/merapi-merbabu-hotels-resorts?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;is_partner=0&amp;star_rating=0&amp;hotel_chain=0&amp;facilities=0&amp;latitude=0&amp;longitude=0&amp;distance=0&amp;uid=business%3A114345</business_uri>
            <photo_primary>https://sandbox.tiket.com/img/business/m/m/business-mm-hotel-room.sq2.jpg</photo_primary>
            <star_rating>4</star_rating>
            <id>201620160811</id>
            <room_available>10</room_available>
            <latitude>-7.76510059999999900000</latitude>
            <longitude>110.41087279999999000000</longitude>
            <room_max_occupancies>2</room_max_occupancies>
            <rating>7.3</rating>
            <tripadvisor_avg_rating>
                <avg_rating>3.5</avg_rating>
                <image_url>http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.5-18379-4.gif</image_url>
                <review_count>93</review_count>
                <url>http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=2687978&amp;lang=en_US&amp;partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&amp;isTA=true&amp;format=html&amp;display=true</url>
            </tripadvisor_avg_rating>
            <room_facility_name>%25hotel_ac%25%7C%25hotel_inet_wifi_compl%25%7C%25hotel_lcd_plasma%25%7C%25hotel_sat_cable%25%7C%25hotel_desk%25%7C%25hotel_shower%25%7C%25hotel_coffee_tea+maker%25%7C%25hotel_complimentary_bottled_water%25%7C%25hotel_daily_newspaper%25%7C%25hotel_television%25%7C%25hotel_telephone%25%7C%25hotel_slipper%25%7C%25hotel_mirror%25%7C%25hotel_hair_dryer_on_request%25%7C%25hotel_refrigerator%25%7C%25hotel_free_toiletries%25%7C%25hotel_sofa_bed%25</room_facility_name>
            <oldprice>660858.00</oldprice>
            <address>Seturan Main Street, Depok, Sleman</address>
            <wifi>Wi-Fi Tersedia</wifi>
            <promo_name></promo_name>
            <price>475000.00</price>
            <total_price>475000.00</total_price>
            <regional>Condong Catur - Depok - Daerah Istimewa Yogyakarta</regional>
            <name>Merapi Merbabu Hotels and Resorts Yogyakarta</name>
            <hotel_id>114345</hotel_id>
        </result>
        <result>
            <province_name>Daerah Istimewa Yogyakarta</province_name>
            <kecamatan_name> </kecamatan_name>
            <kelurahan_name> </kelurahan_name>
            <business_uri>https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/ugm/grand-tjokro-yogyakarta?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;is_partner=0&amp;star_rating=0&amp;hotel_chain=0&amp;facilities=0&amp;latitude=0&amp;longitude=0&amp;distance=0&amp;uid=business%3A184120</business_uri>
            <photo_primary>https://sandbox.tiket.com/img/business/s/u/business-superior_twin16.sq2.jpg</photo_primary>
            <star_rating>4</star_rating>
            <id>333820160811</id>
            <room_available>25</room_available>
            <latitude>-7.78128440000000000000</latitude>
            <longitude>110.38808280000000000000</longitude>
            <room_max_occupancies>2</room_max_occupancies>
            <rating>8.0</rating>
            <tripadvisor_avg_rating>
                <avg_rating>4.0</avg_rating>
                <image_url>http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif</image_url>
                <review_count>36</review_count>
                <url>http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=3545399&amp;lang=en_US&amp;partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&amp;isTA=true&amp;format=html&amp;display=true</url>
            </tripadvisor_avg_rating>
            <room_facility_name>%25hotel_ac%25%7C%25hotel_inet_wifi_compl%25%7C%25hotel_lcd_plasma%25%7C%25hotel_sat_cable%25%7C%25hotel_shower%25%7C%25hotel_coffee_tea+maker%25%7C%25hotel_complimentary_bottled_water%25%7C%25hotel_telephone%25%7C%25hotel_slipper%25%7C%25hotel_mirror%25%7C%25hotel_refrigerator%25%7C%25hotel_free_toiletries%25%7C%25hotel_Cupboard%25%7C%25hotel_Hot_Cold_Shower%25</room_facility_name>
            <oldprice>1182588.00</oldprice>
            <address>Gejayan Street Number 37, Yogyakarta, Yogyakarta</address>
            <wifi>Wi-Fi Tersedia</wifi>
            <promo_name></promo_name>
            <price>850000.00</price>
            <total_price>850000.00</total_price>
            <regional>  -   - Daerah Istimewa Yogyakarta</regional>
            <name>Grand Tjokro Yogyakarta</name>
            <hotel_id>184120</hotel_id>
        </result>
        <result>
            <province_name>Daerah Istimewa Yogyakarta</province_name>
            <kecamatan_name> </kecamatan_name>
            <kelurahan_name> </kelurahan_name>
            <business_uri>https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/yogyakarta/the-sahid-rich-jogja-hotel?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;is_partner=0&amp;star_rating=0&amp;hotel_chain=0&amp;facilities=0&amp;latitude=0&amp;longitude=0&amp;distance=0&amp;uid=business%3A115544</business_uri>
            <photo_primary>https://sandbox.tiket.com/img/business/t/h/business-the-rich-main.sq2.jpg</photo_primary>
            <star_rating>4</star_rating>
            <id>210220160811</id>
            <room_available>298</room_available>
            <latitude>-7.75262970000000000000</latitude>
            <longitude>110.36215519999996000000</longitude>
            <room_max_occupancies>2</room_max_occupancies>
            <rating></rating>
            <tripadvisor_avg_rating>
                <avg_rating>3.5</avg_rating>
                <image_url>http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.5-18379-4.gif</image_url>
                <review_count>175</review_count>
                <url>http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=3317684&amp;lang=en_US&amp;partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&amp;isTA=true&amp;format=html&amp;display=true</url>
            </tripadvisor_avg_rating>
            <room_facility_name>%25hotel_in_room_safe%25%7C%25hotel_ac%25%7C%25hotel_lcd_plasma%25%7C%25hotel_sat_cable%25%7C%25hotel_shower%25%7C%25hotel_coffee_tea+maker%25%7C%25hotel_complimentary_bottled_water%25%7C%25hotel_telephone%25%7C%25hotel_refrigerator%25%7C%25hotel_free_toiletries%25</room_facility_name>
            <oldprice>1321716.00</oldprice>
            <address>Jl. Magelang KM.6, No 18, Yogyakarta</address>
            <wifi></wifi>
            <promo_name></promo_name>
            <price>950000.00</price>
            <total_price>950000.00</total_price>
            <regional>  -   - Daerah Istimewa Yogyakarta</regional>
            <name>The Sahid Rich Jogja Hotel</name>
            <hotel_id>115544</hotel_id>
        </result>
        <result>
            <province_name>Daerah Istimewa Yogyakarta</province_name>
            <kecamatan_name> </kecamatan_name>
            <kelurahan_name> </kelurahan_name>
            <business_uri>https://api-sandbox.tiket.com/de-laxston-hotel-jogja-by-quins?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;is_partner=0&amp;star_rating=0&amp;hotel_chain=0&amp;facilities=0&amp;latitude=0&amp;longitude=0&amp;distance=0&amp;uid=business%3A21626059</business_uri>
            <photo_primary>https://sandbox.tiket.com/img/default/d/e/default-default.sq2.jpg</photo_primary>
            <star_rating>3</star_rating>
            <id>71620320160811</id>
            <room_available>3</room_available>
            <latitude>-7.78301280000000000000</latitude>
            <longitude>110.38749610000002000000</longitude>
            <room_max_occupancies>2</room_max_occupancies>
            <rating></rating>
            <tripadvisor_avg_rating>
                <avg_rating>4.0</avg_rating>
                <image_url>http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif</image_url>
                <review_count>33</review_count>
                <url>http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=8608038&amp;lang=en_US&amp;partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&amp;isTA=true&amp;format=html&amp;display=true</url>
            </tripadvisor_avg_rating>
            <oldprice>970418.00</oldprice>
            <room_facility_name></room_facility_name>
            <address></address>
            <wifi></wifi>
            <promo_name></promo_name>
            <price>620000.00</price>
            <total_price>620000.00</total_price>
            <regional>  -   - Daerah Istimewa Yogyakarta</regional>
            <name></name>
            <hotel_id>21626059</hotel_id>
        </result>
        <result>
            <province_name>Daerah Istimewa Yogyakarta</province_name>
            <kecamatan_name> </kecamatan_name>
            <kelurahan_name> </kelurahan_name>
            <business_uri>https://api-sandbox.tiket.com/the-alana-yogyakarta-hotel-and-convention-center?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;is_partner=0&amp;star_rating=0&amp;hotel_chain=0&amp;facilities=0&amp;latitude=0&amp;longitude=0&amp;distance=0&amp;uid=business%3A21227380</business_uri>
            <photo_primary>https://sandbox.tiket.com/img/default/d/e/default-default.sq2.jpg</photo_primary>
            <star_rating>4</star_rating>
            <id>71998220160811</id>
            <room_available>219</room_available>
            <latitude>-7.72104340000000000000</latitude>
            <longitude>110.38274189999993000000</longitude>
            <room_max_occupancies>2</room_max_occupancies>
            <rating></rating>
            <tripadvisor_avg_rating>
                <avg_rating>4.0</avg_rating>
                <image_url>http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif</image_url>
                <review_count>143</review_count>
                <url>http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=7745637&amp;lang=en_US&amp;partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&amp;isTA=true&amp;format=html&amp;display=true</url>
            </tripadvisor_avg_rating>
            <oldprice>1013159.00</oldprice>
            <room_facility_name></room_facility_name>
            <address></address>
            <wifi></wifi>
            <promo_name></promo_name>
            <price>711480.00</price>
            <total_price>711480.00</total_price>
            <regional>  -   - Daerah Istimewa Yogyakarta</regional>
            <name></name>
            <hotel_id>21227380</hotel_id>
        </result>
        <result>
            <province_name>Daerah Istimewa Yogyakarta</province_name>
            <kecamatan_name>Mergangsan</kecamatan_name>
            <kelurahan_name>Brontokusuman</kelurahan_name>
            <business_uri>https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/janti/hotel-new-saphir-yogyakarta?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;is_partner=0&amp;star_rating=0&amp;hotel_chain=0&amp;facilities=0&amp;latitude=0&amp;longitude=0&amp;distance=0&amp;uid=business%3A20162398</business_uri>
            <photo_primary>https://sandbox.tiket.com/img/business/s/a/business-saphir61.sq2.jpg</photo_primary>
            <star_rating>4</star_rating>
            <id>45651120160811</id>
            <room_available>5</room_available>
            <latitude>-7.78010430000000100000</latitude>
            <longitude>110.39122980000002000000</longitude>
            <room_max_occupancies>2</room_max_occupancies>
            <rating>8.3</rating>
            <tripadvisor_avg_rating>
                <avg_rating>3.5</avg_rating>
                <image_url>http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.5-18379-4.gif</image_url>
                <review_count>132</review_count>
                <url>http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=307067&amp;lang=en_US&amp;partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&amp;isTA=true&amp;format=html&amp;display=true</url>
            </tripadvisor_avg_rating>
            <room_facility_name>%25hotel_ac%25%7C%25hotel_lcd_plasma%25%7C%25hotel_desk%25%7C%25hotel_shower%25%7C%25hotel_bathtub%25%7C%25hotel_mini_bar%25%7C%25hotel_coffee_tea+maker%25%7C%25hotel_complimentary_bottled_water%25%7C%25hotel_television%25%7C%25hotel_refrigerator%25</room_facility_name>
            <oldprice>695640.00</oldprice>
            <address>Jl. Laksda Adisucipto No. 38, Mergangsan, Yogyakarta</address>
            <wifi></wifi>
            <promo_name></promo_name>
            <price>500000.00</price>
            <total_price>500000.00</total_price>
            <regional>Brontokusuman - Mergangsan - Daerah Istimewa Yogyakarta</regional>
            <name>Hotel New Saphir Yogyakarta</name>
            <hotel_id>20162398</hotel_id>
        </result>
        <result>
            <province_name>Daerah Istimewa Yogyakarta</province_name>
            <kecamatan_name> </kecamatan_name>
            <kelurahan_name> </kelurahan_name>
            <business_uri>https://api-sandbox.tiket.com/neo-awana-yogyakarta?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;is_partner=0&amp;star_rating=0&amp;hotel_chain=0&amp;facilities=0&amp;latitude=0&amp;longitude=0&amp;distance=0&amp;uid=business%3A21171272</business_uri>
            <photo_primary>https://sandbox.tiket.com/img/default/d/e/default-default.sq2.jpg</photo_primary>
            <star_rating>3</star_rating>
            <id>55167120160811</id>
            <room_available>195</room_available>
            <latitude>-7.82049380000000000000</latitude>
            <longitude>110.36539080000000000000</longitude>
            <room_max_occupancies>2</room_max_occupancies>
            <rating></rating>
            <tripadvisor_avg_rating>
                <avg_rating>4.0</avg_rating>
                <image_url>http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif</image_url>
                <review_count>140</review_count>
                <url>http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=7751603&amp;lang=en_US&amp;partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&amp;isTA=true&amp;format=html&amp;display=true</url>
            </tripadvisor_avg_rating>
            <oldprice>635809.00</oldprice>
            <room_facility_name></room_facility_name>
            <address></address>
            <wifi></wifi>
            <promo_name></promo_name>
            <price>396880.00</price>
            <total_price>396880.00</total_price>
            <regional>  -   - Daerah Istimewa Yogyakarta</regional>
            <name></name>
            <hotel_id>21171272</hotel_id>
        </result>
    </results>
    <pagination>
        <total_found>134</total_found>
        <current_page>1</current_page>
        <offset>20</offset>
        <lastPage>7</lastPage>
    </pagination>
    <login_status>true</login_status>
    <guest_id>22691145</guest_id>
    <login_email>wida.skydev@gmail.com</login_email>
    <token>f9b29ac359ca5d77755e7588751c089bf96f0dc9</token>
</tiket>
```

```json
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "1.9093",
    "memoryusage": "22.76MB",
    "unix_timestamp": 1470370447,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "search_queries": {
    "q": "Yogyakarta",
    "uid": "",
    "startdate": "2016-08-11",
    "enddate": "2016-08-12",
    "night": "1",
    "room": 1,
    "adult": "2",
    "child": 0,
    "sort": false,
    "minstar": 0,
    "maxstar": 5,
    "minprice": "118000.00",
    "maxprice": "1000000000.00",
    "distance": 100000
  },
  "results": {
    "result": [
      {
        "province_name": "Daerah Istimewa Yogyakarta",
        "kecamatan_name": " ",
        "kelurahan_name": " ",
        "business_uri": "https://api-sandbox.tiket.com/wwwh-boutiquehotelcom?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A21298812",
        "photo_primary": "https://sandbox.tiket.com/img/default/d/e/default-default.sq2.jpg",
        "star_rating": "3",
        "id": "76233820160811",
        "room_available": "4",
        "latitude": "-7.77923380000000000000",
        "longitude": "110.37961110000003000000",
        "room_max_occupancies": "2",
        "rating": "",
        "oldprice": "539991.00",
        "room_facility_name": "",
        "address": "",
        "wifi": "",
        "promo_name": "",
        "price": "345000.00",
        "total_price": "345000.00",
        "regional": "  -   - Daerah Istimewa Yogyakarta",
        "name": "",
        "hotel_id": "21298812"
      },
      {
        "province_name": "Daerah Istimewa Yogyakarta",
        "kecamatan_name": " ",
        "kelurahan_name": " ",
        "business_uri": "https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/gejayan/the-edelweis-hotel-yogyakarta?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A15810",
        "photo_primary": "https://sandbox.tiket.com/img/business/t/w/business-twice_room_2_-312x234-.sq2.jpg",
        "star_rating": "3",
        "id": "62897320160811",
        "room_available": "10",
        "latitude": "-7.78165320000000000000",
        "longitude": "110.38783779999994000000",
        "room_max_occupancies": "2",
        "rating": "8.1",
        "tripadvisor_avg_rating": {
          "avg_rating": "3.5",
          "image_url": "http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.5-18379-4.gif",
          "review_count": "108",
          "url": "http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=2545466&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true"
        },
        "oldprice": "586946.00",
        "room_facility_name": "",
        "address": "Jl. Gejayan 17C, Gondokusuman, Yogyakarta",
        "wifi": "",
        "promo_name": "",
        "price": "375000.00",
        "total_price": "375000.00",
        "regional": "  -   - Daerah Istimewa Yogyakarta",
        "name": "The Edelweis Yogyakarta",
        "hotel_id": "15810"
      },
      {
        "province_name": "Daerah Istimewa Yogyakarta",
        "kecamatan_name": "Sleman",
        "kelurahan_name": " ",
        "business_uri": "https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/yogyakarta/fortune-fest-hotel-yogyakarta?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A20585137",
        "photo_primary": "https://sandbox.tiket.com/img/business/i/m/business-img_9741.sq2.jpg",
        "star_rating": "3",
        "id": "74956320160811",
        "room_available": "222",
        "latitude": "-7.76572909999999900000",
        "longitude": "110.41054290000000000000",
        "room_max_occupancies": "2",
        "rating": "",
        "tripadvisor_avg_rating": {
          "avg_rating": "3.5",
          "image_url": "http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.5-18379-4.gif",
          "review_count": "106",
          "url": "http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=2687978&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true"
        },
        "oldprice": "591642.00",
        "room_facility_name": "",
        "address": "Jl. Raya Seturan , Depok, Sleman",
        "wifi": "",
        "promo_name": "",
        "price": "378000.00",
        "total_price": "378000.00",
        "regional": "  - Sleman - Daerah Istimewa Yogyakarta",
        "name": "Fortune Fest Hotel Yogyakarta",
        "hotel_id": "20585137"
      },
      {
        "province_name": "Daerah Istimewa Yogyakarta",
        "kecamatan_name": " ",
        "kelurahan_name": " ",
        "business_uri": "https://api-sandbox.tiket.com/hotel/indonesia/bandung/kebon-kawung/mutiara-hotel-bandung?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A18",
        "photo_primary": "https://sandbox.tiket.com/img/business/y/u/business-yufgfyu.sq2.jpg",
        "star_rating": "3",
        "id": "56912220160811",
        "room_available": "10",
        "latitude": "-6.91237020000000100000",
        "longitude": "107.59834820000003000000",
        "room_max_occupancies": "2",
        "rating": "7.0",
        "tripadvisor_avg_rating": {
          "avg_rating": "3.0",
          "image_url": "http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.0-18379-4.gif",
          "review_count": "89",
          "url": "http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=1016088&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true"
        },
        "oldprice": "499296.00",
        "room_facility_name": "",
        "address": "Kebon Kawung Street 60, Cicendo, Bandung",
        "wifi": "",
        "promo_name": "",
        "price": "319000.00",
        "total_price": "319000.00",
        "regional": "  -   - Daerah Istimewa Yogyakarta",
        "name": "Hotel Mutiara",
        "hotel_id": "18"
      },
      {
        "province_name": "Daerah Istimewa Yogyakarta",
        "kecamatan_name": " ",
        "kelurahan_name": " ",
        "business_uri": "https://api-sandbox.tiket.com/student-park-hotel-apartment-yogyakarta?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A21307287",
        "photo_primary": "https://sandbox.tiket.com/img/default/d/e/default-default.sq2.jpg",
        "star_rating": "3",
        "id": "57184620160811",
        "room_available": "1",
        "latitude": "-7.76962580000000000000",
        "longitude": "110.40610650000008000000",
        "room_max_occupancies": "2",
        "rating": "",
        "tripadvisor_avg_rating": {
          "avg_rating": "4.5",
          "image_url": "http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.5-18379-4.gif",
          "review_count": "33",
          "url": "http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=8037466&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true"
        },
        "oldprice": "766943.00",
        "room_facility_name": "",
        "address": "",
        "wifi": "",
        "promo_name": "",
        "price": "490000.00",
        "total_price": "490000.00",
        "regional": "  -   - Daerah Istimewa Yogyakarta",
        "name": "",
        "hotel_id": "21307287"
      },
      {
        "province_name": "Daerah Istimewa Yogyakarta",
        "kecamatan_name": "Sleman",
        "kelurahan_name": " ",
        "business_uri": "https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/sinduadi/crystal-lotus-hotel-yogyakarta-managed-by-prabu?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A20087341",
        "photo_primary": "https://sandbox.tiket.com/img/business/c/r/business-crystal-lotus-exterior1.sq2.jpg",
        "star_rating": "4",
        "id": "48240320160811",
        "room_available": "30",
        "latitude": "-7.76306949999999900000",
        "longitude": "110.36527960000001000000",
        "room_max_occupancies": "2",
        "rating": "",
        "tripadvisor_avg_rating": {
          "avg_rating": "3.5",
          "image_url": "http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.5-18379-4.gif",
          "review_count": "83",
          "url": "http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=6557803&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true"
        },
        "room_facility_name": "Kamar bebas rokok ada tergantung ketersediaan|Brankas|AC|Internet - Wifi|Internet - Wifi (gratis)|Televisi LCD/layar plasma|Satelit/TV kabel|Meja|Shower|Baju Handuk|Bathtub|Pengering Rambut|Bar kecil|Mesin pembuat kopi/teh|Air mineral botol gratis|Televisi|Telepon|Sandal|Cermin|Papan setrika dengan permintaan|Kulkas|Teras|Gratis Perlengkapan Mandi|Shower Panas and Dingin",
        "oldprice": "617002.00",
        "address": "Magelang Street KM.  5,2 Yogyakarta, Sleman, Sleman",
        "wifi": "Wi-Fi Tersedia",
        "promo_name": "",
        "price": "443478.00",
        "total_price": "443478.00",
        "regional": "  - Sleman - Daerah Istimewa Yogyakarta",
        "name": "Crystal Lotus Hotel Yogyakarta Managed By Prabu",
        "hotel_id": "20087341"
      },
      {
        "province_name": "Daerah Istimewa Yogyakarta",
        "kecamatan_name": " ",
        "kelurahan_name": " ",
        "business_uri": "https://api-sandbox.tiket.com/pandanaran-hotel-yogyakarta?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A21222561",
        "photo_primary": "https://sandbox.tiket.com/img/default/d/e/default-default.sq2.jpg",
        "star_rating": "3",
        "id": "55003720160811",
        "room_available": "12",
        "latitude": "-7.81918940000000100000",
        "longitude": "110.37059939999995000000",
        "room_max_occupancies": "2",
        "rating": "",
        "tripadvisor_avg_rating": {
          "avg_rating": "4.0",
          "image_url": "http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif",
          "review_count": "79",
          "url": "http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=7808044&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true"
        },
        "oldprice": "513382.00",
        "room_facility_name": "",
        "address": "",
        "wifi": "",
        "promo_name": "",
        "price": "328000.00",
        "total_price": "328000.00",
        "regional": "  -   - Daerah Istimewa Yogyakarta",
        "name": "",
        "hotel_id": "21222561"
      },
      {
        "province_name": "Daerah Istimewa Yogyakarta",
        "kecamatan_name": " ",
        "kelurahan_name": " ",
        "business_uri": "https://api-sandbox.tiket.com/hotel-neo-malioboro?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A21402180",
        "photo_primary": "https://sandbox.tiket.com/img/default/d/e/default-default.sq2.jpg",
        "star_rating": "3",
        "id": "62897720160811",
        "room_available": "112",
        "latitude": "-7.79001630000000000000",
        "longitude": "110.36312539999994000000",
        "room_max_occupancies": "2",
        "rating": "",
        "tripadvisor_avg_rating": {
          "avg_rating": "4.0",
          "image_url": "http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif",
          "review_count": "399",
          "url": "http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=8092831&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true"
        },
        "oldprice": "771500.00",
        "room_facility_name": "",
        "address": "",
        "wifi": "",
        "promo_name": "",
        "price": "481580.00",
        "total_price": "481580.00",
        "regional": "  -   - Daerah Istimewa Yogyakarta",
        "name": "",
        "hotel_id": "21402180"
      },
      {
        "province_name": "Daerah Istimewa Yogyakarta",
        "kecamatan_name": "Mantrijeron",
        "kelurahan_name": "Suryodiningratan",
        "business_uri": "https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/seturan/the-victoria-hotel?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A3031",
        "photo_primary": "https://sandbox.tiket.com/img/business/v/i/business-victoria-yogya-pool.sq2.jpg",
        "star_rating": "3",
        "id": "31420160811",
        "room_available": "3",
        "latitude": "-7.78319030000000000000",
        "longitude": "110.40225609999993000000",
        "room_max_occupancies": "2",
        "rating": "7.6",
        "tripadvisor_avg_rating": {
          "avg_rating": "4.0",
          "image_url": "http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif",
          "review_count": "55",
          "url": "http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=2348889&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true"
        },
        "room_facility_name": "AC|Internet - Wifi|Televisi LCD/layar plasma|Satelit/TV kabel|Meja|Shower|Bar kecil|Mesin pembuat kopi/teh|Air mineral botol gratis",
        "oldprice": "1408671.00",
        "address": "Jl. Laksda Adisutjipto Km. 5 , Mantrijeron, Yogyakarta",
        "wifi": "Wi-Fi Tersedia",
        "promo_name": "",
        "price": "900000.00",
        "total_price": "900000.00",
        "regional": "Suryodiningratan - Mantrijeron - Daerah Istimewa Yogyakarta",
        "name": "The Victoria Hotel Yogyakarta",
        "hotel_id": "3031"
      },
      {
        "province_name": "Daerah Istimewa Yogyakarta",
        "kecamatan_name": "Gedong Tengen",
        "kelurahan_name": "Sosromenduran",
        "business_uri": "https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/malioboro/hotel-dafam-fortuna-malioboro-yogyakarta?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A20087773",
        "photo_primary": "https://sandbox.tiket.com/img/business/r/o/business-rooftop_pool2.sq2.jpg",
        "star_rating": "3",
        "id": "48285920160811",
        "room_available": "217",
        "latitude": "-7.79369329999999900000",
        "longitude": "110.36283040000000000000",
        "room_max_occupancies": "2",
        "rating": "",
        "tripadvisor_avg_rating": {
          "avg_rating": "4.0",
          "image_url": "http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif",
          "review_count": "210",
          "url": "http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=4876648&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true"
        },
        "room_facility_name": "Brankas|AC|Internet - Wifi|Satelit/TV kabel|Meja|Shower|Gratis Perlengkapan Mandi",
        "oldprice": "729379.00",
        "address": "Dagen Street No  60, Yogyakarta, Gedong Tengen, Yogyakarta",
        "wifi": "Wi-Fi Tersedia",
        "promo_name": "",
        "price": "466000.00",
        "total_price": "466000.00",
        "regional": "Sosromenduran - Gedong Tengen - Daerah Istimewa Yogyakarta",
        "name": "Hotel Dafam Fortuna Malioboro Yogyakarta",
        "hotel_id": "20087773"
      },
      {
        "province_name": "Daerah Istimewa Yogyakarta",
        "kecamatan_name": "Jetis",
        "kelurahan_name": "Gowongan",
        "business_uri": "https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/tugu-jogja/the-101-yogyakarta-tugu?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A20426620",
        "photo_primary": "https://sandbox.tiket.com/img/business/i/m/business-img_2590.sq2.jpg",
        "star_rating": "4",
        "id": "46702820160811",
        "room_available": "5",
        "latitude": "-7.78507033179146600000",
        "longitude": "110.36680161952972000000",
        "room_max_occupancies": "2",
        "rating": "",
        "tripadvisor_avg_rating": {
          "avg_rating": "4.0",
          "image_url": "http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif",
          "review_count": "253",
          "url": "http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=6739367&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true"
        },
        "room_facility_name": "Brankas|AC|Satelit/TV kabel|Shower|Pengering Rambut|Sandal|Cermin|Shower Panas and Dingin",
        "oldprice": "1089358.00",
        "address": "Jalan Margoutomo No. 103 ( Mangkubumi), Yogyakarta , Jetis, Yogyakarta",
        "wifi": "",
        "promo_name": "",
        "price": "782990.00",
        "total_price": "782990.00",
        "regional": "Gowongan - Jetis - Daerah Istimewa Yogyakarta",
        "name": "THE 1O1 Yogyakarta Tugu",
        "hotel_id": "20426620"
      },
      {
        "province_name": "Daerah Istimewa Yogyakarta",
        "kecamatan_name": " ",
        "kelurahan_name": " ",
        "business_uri": "https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/yogyakarta-airport/the-jayakarta-jogjakarta-hotel-spa?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A3786",
        "photo_primary": "https://sandbox.tiket.com/img/business/y/a/business-yajjarh.sq2.jpg",
        "star_rating": "4",
        "id": "48065120160811",
        "room_available": "12",
        "latitude": "-7.78343729999999900000",
        "longitude": "110.41959930000007000000",
        "room_max_occupancies": "2",
        "rating": "7.9",
        "tripadvisor_avg_rating": {
          "avg_rating": "3.5",
          "image_url": "http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.5-18379-4.gif",
          "review_count": "113",
          "url": "http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=307834&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true"
        },
        "room_facility_name": "Kamar bebas rokok ada tergantung ketersediaan|AC|Satelit/TV kabel|Shower dan bak terpisah|Bar kecil|Mesin pembuat kopi/teh|Air mineral botol gratis|Televisi|Telepon|Cermin|Pengering rambut dengan permintaan|Teras|Shower Panas and Dingin",
        "oldprice": "1363454.00",
        "address": "Jl. Laksda Adisucipto KM.8, Yogyakarta",
        "wifi": "",
        "promo_name": "",
        "price": "980000.00",
        "total_price": "980000.00",
        "regional": "  -   - Daerah Istimewa Yogyakarta",
        "name": "The Jayakarta Jogjakarta Hotel &amp; Spa",
        "hotel_id": "3786"
      },
      {
        "province_name": "Daerah Istimewa Yogyakarta",
        "kecamatan_name": "Jetis",
        "kelurahan_name": "Bumijo",
        "business_uri": "https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/sinduadi/hotel-tentrem-yogyakarta?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A19569414",
        "photo_primary": "https://sandbox.tiket.com/img/business/h/o/business-hoteltentrem_guest_r1.sq2.jpg",
        "star_rating": "5",
        "id": "591620160811",
        "room_available": "10",
        "latitude": "-7.77713830000000000000",
        "longitude": "110.36772680000001000000",
        "room_max_occupancies": "2",
        "rating": "9.0",
        "tripadvisor_avg_rating": {
          "avg_rating": "4.5",
          "image_url": "http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.5-18379-4.gif",
          "review_count": "540",
          "url": "http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=3737584&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true"
        },
        "room_facility_name": "Brankas|AC|Televisi LCD/layar plasma|Meja|Shower|Bathtub|Pengering Rambut|Mesin pembuat kopi/teh|Air mineral botol gratis|Televisi|Telepon|Gratis Perlengkapan Mandi|Lemari|Shower Panas and Dingin|Satellite TV Service |LCD TV |Free Wi-Fi |Cable TV Service |Minibar ",
        "oldprice": "1790143.00",
        "address": "Jl. AM Sangaji No. 72 A Yogyakarta 55233, Jetis, Yogyakarta",
        "wifi": "",
        "promo_name": "",
        "price": "1470500.00",
        "total_price": "1470500.00",
        "regional": "Bumijo - Jetis - Daerah Istimewa Yogyakarta",
        "name": "Hotel Tentrem Yogyakarta",
        "hotel_id": "19569414"
      },
      {
        "province_name": "Daerah Istimewa Yogyakarta",
        "kecamatan_name": "Depok",
        "kelurahan_name": "Condong Catur",
        "business_uri": "https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/seturan/merapi-merbabu-hotels-resorts?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A114345",
        "photo_primary": "https://sandbox.tiket.com/img/business/m/m/business-mm-hotel-room.sq2.jpg",
        "star_rating": "4",
        "id": "201620160811",
        "room_available": "10",
        "latitude": "-7.76510059999999900000",
        "longitude": "110.41087279999999000000",
        "room_max_occupancies": "2",
        "rating": "7.3",
        "tripadvisor_avg_rating": {
          "avg_rating": "3.5",
          "image_url": "http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.5-18379-4.gif",
          "review_count": "93",
          "url": "http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=2687978&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true"
        },
        "room_facility_name": "AC|Internet - Wifi (gratis)|Televisi LCD/layar plasma|Satelit/TV kabel|Meja|Shower|Mesin pembuat kopi/teh|Air mineral botol gratis|Surat kabar harian|Televisi|Telepon|Sandal|Cermin|Pengering rambut dengan permintaan|Kulkas|Gratis Perlengkapan Mandi|Sofa Bed",
        "oldprice": "660858.00",
        "address": "Seturan Main Street, Depok, Sleman",
        "wifi": "Wi-Fi Tersedia",
        "promo_name": "",
        "price": "475000.00",
        "total_price": "475000.00",
        "regional": "Condong Catur - Depok - Daerah Istimewa Yogyakarta",
        "name": "Merapi Merbabu Hotels and Resorts Yogyakarta",
        "hotel_id": "114345"
      },
      {
        "province_name": "Daerah Istimewa Yogyakarta",
        "kecamatan_name": " ",
        "kelurahan_name": " ",
        "business_uri": "https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/ugm/grand-tjokro-yogyakarta?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A184120",
        "photo_primary": "https://sandbox.tiket.com/img/business/s/u/business-superior_twin16.sq2.jpg",
        "star_rating": "4",
        "id": "333820160811",
        "room_available": "25",
        "latitude": "-7.78128440000000000000",
        "longitude": "110.38808280000000000000",
        "room_max_occupancies": "2",
        "rating": "8.0",
        "tripadvisor_avg_rating": {
          "avg_rating": "4.0",
          "image_url": "http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif",
          "review_count": "36",
          "url": "http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=3545399&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true"
        },
        "room_facility_name": "AC|Internet - Wifi (gratis)|Televisi LCD/layar plasma|Satelit/TV kabel|Shower|Mesin pembuat kopi/teh|Air mineral botol gratis|Telepon|Sandal|Cermin|Kulkas|Gratis Perlengkapan Mandi|Lemari|Shower Panas and Dingin",
        "oldprice": "1182588.00",
        "address": "Gejayan Street Number 37, Yogyakarta, Yogyakarta",
        "wifi": "Wi-Fi Tersedia",
        "promo_name": "",
        "price": "850000.00",
        "total_price": "850000.00",
        "regional": "  -   - Daerah Istimewa Yogyakarta",
        "name": "Grand Tjokro Yogyakarta",
        "hotel_id": "184120"
      },
      {
        "province_name": "Daerah Istimewa Yogyakarta",
        "kecamatan_name": " ",
        "kelurahan_name": " ",
        "business_uri": "https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/yogyakarta/the-sahid-rich-jogja-hotel?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A115544",
        "photo_primary": "https://sandbox.tiket.com/img/business/t/h/business-the-rich-main.sq2.jpg",
        "star_rating": "4",
        "id": "210220160811",
        "room_available": "298",
        "latitude": "-7.75262970000000000000",
        "longitude": "110.36215519999996000000",
        "room_max_occupancies": "2",
        "rating": "",
        "tripadvisor_avg_rating": {
          "avg_rating": "3.5",
          "image_url": "http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.5-18379-4.gif",
          "review_count": "175",
          "url": "http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=3317684&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true"
        },
        "room_facility_name": "Brankas|AC|Televisi LCD/layar plasma|Satelit/TV kabel|Shower|Mesin pembuat kopi/teh|Air mineral botol gratis|Telepon|Kulkas|Gratis Perlengkapan Mandi",
        "oldprice": "1321716.00",
        "address": "Jl. Magelang KM.6, No 18, Yogyakarta",
        "wifi": "",
        "promo_name": "",
        "price": "950000.00",
        "total_price": "950000.00",
        "regional": "  -   - Daerah Istimewa Yogyakarta",
        "name": "The Sahid Rich Jogja Hotel",
        "hotel_id": "115544"
      },
      {
        "province_name": "Daerah Istimewa Yogyakarta",
        "kecamatan_name": " ",
        "kelurahan_name": " ",
        "business_uri": "https://api-sandbox.tiket.com/de-laxston-hotel-jogja-by-quins?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A21626059",
        "photo_primary": "https://sandbox.tiket.com/img/default/d/e/default-default.sq2.jpg",
        "star_rating": "3",
        "id": "71620320160811",
        "room_available": "3",
        "latitude": "-7.78301280000000000000",
        "longitude": "110.38749610000002000000",
        "room_max_occupancies": "2",
        "rating": "",
        "tripadvisor_avg_rating": {
          "avg_rating": "4.0",
          "image_url": "http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif",
          "review_count": "33",
          "url": "http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=8608038&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true"
        },
        "oldprice": "970418.00",
        "room_facility_name": "",
        "address": "",
        "wifi": "",
        "promo_name": "",
        "price": "620000.00",
        "total_price": "620000.00",
        "regional": "  -   - Daerah Istimewa Yogyakarta",
        "name": "",
        "hotel_id": "21626059"
      },
      {
        "province_name": "Daerah Istimewa Yogyakarta",
        "kecamatan_name": " ",
        "kelurahan_name": " ",
        "business_uri": "https://api-sandbox.tiket.com/the-alana-yogyakarta-hotel-and-convention-center?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A21227380",
        "photo_primary": "https://sandbox.tiket.com/img/default/d/e/default-default.sq2.jpg",
        "star_rating": "4",
        "id": "71998220160811",
        "room_available": "219",
        "latitude": "-7.72104340000000000000",
        "longitude": "110.38274189999993000000",
        "room_max_occupancies": "2",
        "rating": "",
        "tripadvisor_avg_rating": {
          "avg_rating": "4.0",
          "image_url": "http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif",
          "review_count": "143",
          "url": "http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=7745637&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true"
        },
        "oldprice": "1013159.00",
        "room_facility_name": "",
        "address": "",
        "wifi": "",
        "promo_name": "",
        "price": "711480.00",
        "total_price": "711480.00",
        "regional": "  -   - Daerah Istimewa Yogyakarta",
        "name": "",
        "hotel_id": "21227380"
      },
      {
        "province_name": "Daerah Istimewa Yogyakarta",
        "kecamatan_name": "Mergangsan",
        "kelurahan_name": "Brontokusuman",
        "business_uri": "https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/janti/hotel-new-saphir-yogyakarta?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A20162398",
        "photo_primary": "https://sandbox.tiket.com/img/business/s/a/business-saphir61.sq2.jpg",
        "star_rating": "4",
        "id": "45651120160811",
        "room_available": "5",
        "latitude": "-7.78010430000000100000",
        "longitude": "110.39122980000002000000",
        "room_max_occupancies": "2",
        "rating": "8.3",
        "tripadvisor_avg_rating": {
          "avg_rating": "3.5",
          "image_url": "http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.5-18379-4.gif",
          "review_count": "132",
          "url": "http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=307067&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true"
        },
        "room_facility_name": "AC|Televisi LCD/layar plasma|Meja|Shower|Bathtub|Bar kecil|Mesin pembuat kopi/teh|Air mineral botol gratis|Televisi|Kulkas",
        "oldprice": "695640.00",
        "address": "Jl. Laksda Adisucipto No. 38, Mergangsan, Yogyakarta",
        "wifi": "",
        "promo_name": "",
        "price": "500000.00",
        "total_price": "500000.00",
        "regional": "Brontokusuman - Mergangsan - Daerah Istimewa Yogyakarta",
        "name": "Hotel New Saphir Yogyakarta",
        "hotel_id": "20162398"
      },
      {
        "province_name": "Daerah Istimewa Yogyakarta",
        "kecamatan_name": " ",
        "kelurahan_name": " ",
        "business_uri": "https://api-sandbox.tiket.com/neo-awana-yogyakarta?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A21171272",
        "photo_primary": "https://sandbox.tiket.com/img/default/d/e/default-default.sq2.jpg",
        "star_rating": "3",
        "id": "55167120160811",
        "room_available": "195",
        "latitude": "-7.82049380000000000000",
        "longitude": "110.36539080000000000000",
        "room_max_occupancies": "2",
        "rating": "",
        "tripadvisor_avg_rating": {
          "avg_rating": "4.0",
          "image_url": "http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif",
          "review_count": "140",
          "url": "http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=7751603&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true"
        },
        "oldprice": "635809.00",
        "room_facility_name": "",
        "address": "",
        "wifi": "",
        "promo_name": "",
        "price": "396880.00",
        "total_price": "396880.00",
        "regional": "  -   - Daerah Istimewa Yogyakarta",
        "name": "",
        "hotel_id": "21171272"
      }
    ]
  },
  "pagination": {
    "total_found": 134,
    "current_page": 1,
    "offset": "20",
    "lastPage": 7
  },
  "login_status": "true",
  "guest_id": "22691145",
  "login_email": "wida.skydev@gmail.com",
  "token": "f9b29ac359ca5d77755e7588751c089bf96f0dc9"
}
```

```matlab
a:9:{s:10:"diagnostic";a:7:{s:6:"status";i:200;s:10:"elapsetime";s:14:"1.8807";s:11:"memoryusage";s:14:"22.77MB";s:14:"unix_timestamp";i:1470370504;s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:11:"output_type";s:9:"serialize";s:14:"search_queries";a:14:{s:1:"q";s:10:"Yogyakarta";s:3:"uid";s:0:"";s:9:"startdate";s:10:"2016-08-11";s:7:"enddate";s:10:"2016-08-12";s:5:"night";s:1:"1";s:4:"room";i:1;s:5:"adult";s:1:"2";s:5:"child";i:0;s:4:"sort";b:0;s:7:"minstar";i:0;s:7:"maxstar";i:5;s:8:"minprice";s:9:"118000.00";s:8:"maxprice";s:13:"1000000000.00";s:8:"distance";i:100000;}s:7:"results";a:1:{s:6:"result";a:20:{i:0;a:22:{s:13:"province_name";s:26:"Daerah Istimewa Yogyakarta";s:14:"kecamatan_name";s:1:" ";s:14:"kelurahan_name";s:1:" ";s:12:"business_uri";s:215:"https://api-sandbox.tiket.com/wwwh-boutiquehotelcom?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A21298812";s:13:"photo_primary";s:65:"https://sandbox.tiket.com/img/default/d/e/default-default.sq2.jpg";s:11:"star_rating";s:1:"3";s:2:"id";s:14:"76233820160811";s:14:"room_available";s:1:"4";s:8:"latitude";s:23:"-7.77923380000000000000";s:9:"longitude";s:24:"110.37961110000003000000";s:20:"room_max_occupancies";s:1:"2";s:6:"rating";s:0:"";s:8:"oldprice";s:9:"539991.00";s:18:"room_facility_name";s:0:"";s:7:"address";s:0:"";s:4:"wifi";s:0:"";s:10:"promo_name";s:0:"";s:5:"price";s:9:"345000.00";s:11:"total_price";s:9:"345000.00";s:8:"regional";s:34:"  -   - Daerah Istimewa Yogyakarta";s:4:"name";s:0:"";s:8:"hotel_id";s:8:"21298812";}i:1;a:23:{s:13:"province_name";s:26:"Daerah Istimewa Yogyakarta";s:14:"kecamatan_name";s:1:" ";s:14:"kelurahan_name";s:1:" ";s:12:"business_uri";s:255:"https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/gejayan/the-edelweis-hotel-yogyakarta?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A15810";s:13:"photo_primary";s:82:"https://sandbox.tiket.com/img/business/t/w/business-twice_room_2_-312x234-.sq2.jpg";s:11:"star_rating";s:1:"3";s:2:"id";s:14:"62897320160811";s:14:"room_available";s:2:"10";s:8:"latitude";s:23:"-7.78165320000000000000";s:9:"longitude";s:24:"110.38783779999994000000";s:20:"room_max_occupancies";s:1:"2";s:6:"rating";s:3:"8.1";s:22:"tripadvisor_avg_rating";a:4:{s:10:"avg_rating";s:3:"3.5";s:9:"image_url";s:75:"http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.5-18379-4.gif";s:12:"review_count";s:3:"108";s:3:"url";s:164:"http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=2545466&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true";}s:8:"oldprice";s:9:"586946.00";s:18:"room_facility_name";s:0:"";s:7:"address";s:41:"Jl. Gejayan 17C, Gondokusuman, Yogyakarta";s:4:"wifi";s:0:"";s:10:"promo_name";s:0:"";s:5:"price";s:9:"375000.00";s:11:"total_price";s:9:"375000.00";s:8:"regional";s:34:"  -   - Daerah Istimewa Yogyakarta";s:4:"name";s:23:"The Edelweis Yogyakarta";s:8:"hotel_id";s:5:"15810";}i:2;a:23:{s:13:"province_name";s:26:"Daerah Istimewa Yogyakarta";s:14:"kecamatan_name";s:6:"Sleman";s:14:"kelurahan_name";s:1:" ";s:12:"business_uri";s:261:"https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/yogyakarta/fortune-fest-hotel-yogyakarta?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A20585137";s:13:"photo_primary";s:68:"https://sandbox.tiket.com/img/business/i/m/business-img_9741.sq2.jpg";s:11:"star_rating";s:1:"3";s:2:"id";s:14:"74956320160811";s:14:"room_available";s:3:"222";s:8:"latitude";s:23:"-7.76572909999999900000";s:9:"longitude";s:24:"110.41054290000000000000";s:20:"room_max_occupancies";s:1:"2";s:6:"rating";s:0:"";s:22:"tripadvisor_avg_rating";a:4:{s:10:"avg_rating";s:3:"3.5";s:9:"image_url";s:75:"http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.5-18379-4.gif";s:12:"review_count";s:3:"106";s:3:"url";s:164:"http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=2687978&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true";}s:8:"oldprice";s:9:"591642.00";s:18:"room_facility_name";s:0:"";s:7:"address";s:32:"Jl. Raya Seturan , Depok, Sleman";s:4:"wifi";s:0:"";s:10:"promo_name";s:0:"";s:5:"price";s:9:"378000.00";s:11:"total_price";s:9:"378000.00";s:8:"regional";s:39:"  - Sleman - Daerah Istimewa Yogyakarta";s:4:"name";s:29:"Fortune Fest Hotel Yogyakarta";s:8:"hotel_id";s:8:"20585137";}i:3;a:23:{s:13:"province_name";s:26:"Daerah Istimewa Yogyakarta";s:14:"kecamatan_name";s:1:" ";s:14:"kelurahan_name";s:1:" ";s:12:"business_uri";s:246:"https://api-sandbox.tiket.com/hotel/indonesia/bandung/kebon-kawung/mutiara-hotel-bandung?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A18";s:13:"photo_primary";s:67:"https://sandbox.tiket.com/img/business/y/u/business-yufgfyu.sq2.jpg";s:11:"star_rating";s:1:"3";s:2:"id";s:14:"56912220160811";s:14:"room_available";s:2:"10";s:8:"latitude";s:23:"-6.91237020000000100000";s:9:"longitude";s:24:"107.59834820000003000000";s:20:"room_max_occupancies";s:1:"2";s:6:"rating";s:3:"7.0";s:22:"tripadvisor_avg_rating";a:4:{s:10:"avg_rating";s:3:"3.0";s:9:"image_url";s:75:"http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.0-18379-4.gif";s:12:"review_count";s:2:"89";s:3:"url";s:164:"http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=1016088&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true";}s:8:"oldprice";s:9:"499296.00";s:18:"room_facility_name";s:0:"";s:7:"address";s:40:"Kebon Kawung Street 60, Cicendo, Bandung";s:4:"wifi";s:0:"";s:10:"promo_name";s:0:"";s:5:"price";s:9:"319000.00";s:11:"total_price";s:9:"319000.00";s:8:"regional";s:34:"  -   - Daerah Istimewa Yogyakarta";s:4:"name";s:13:"Hotel Mutiara";s:8:"hotel_id";s:2:"18";}i:4;a:23:{s:13:"province_name";s:26:"Daerah Istimewa Yogyakarta";s:14:"kecamatan_name";s:1:" ";s:14:"kelurahan_name";s:1:" ";s:12:"business_uri";s:233:"https://api-sandbox.tiket.com/student-park-hotel-apartment-yogyakarta?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A21307287";s:13:"photo_primary";s:65:"https://sandbox.tiket.com/img/default/d/e/default-default.sq2.jpg";s:11:"star_rating";s:1:"3";s:2:"id";s:14:"57184620160811";s:14:"room_available";s:1:"1";s:8:"latitude";s:23:"-7.76962580000000000000";s:9:"longitude";s:24:"110.40610650000008000000";s:20:"room_max_occupancies";s:1:"2";s:6:"rating";s:0:"";s:22:"tripadvisor_avg_rating";a:4:{s:10:"avg_rating";s:3:"4.5";s:9:"image_url";s:75:"http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.5-18379-4.gif";s:12:"review_count";s:2:"33";s:3:"url";s:164:"http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=8037466&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true";}s:8:"oldprice";s:9:"766943.00";s:18:"room_facility_name";s:0:"";s:7:"address";s:0:"";s:4:"wifi";s:0:"";s:10:"promo_name";s:0:"";s:5:"price";s:9:"490000.00";s:11:"total_price";s:9:"490000.00";s:8:"regional";s:34:"  -   - Daerah Istimewa Yogyakarta";s:4:"name";s:0:"";s:8:"hotel_id";s:8:"21307287";}i:5;a:23:{s:13:"province_name";s:26:"Daerah Istimewa Yogyakarta";s:14:"kecamatan_name";s:6:"Sleman";s:14:"kelurahan_name";s:1:" ";s:12:"business_uri";s:277:"https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/sinduadi/crystal-lotus-hotel-yogyakarta-managed-by-prabu?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A20087341";s:13:"photo_primary";s:83:"https://sandbox.tiket.com/img/business/c/r/business-crystal-lotus-exterior1.sq2.jpg";s:11:"star_rating";s:1:"4";s:2:"id";s:14:"48240320160811";s:14:"room_available";s:2:"30";s:8:"latitude";s:23:"-7.76306949999999900000";s:9:"longitude";s:24:"110.36527960000001000000";s:20:"room_max_occupancies";s:1:"2";s:6:"rating";s:0:"";s:22:"tripadvisor_avg_rating";a:4:{s:10:"avg_rating";s:3:"3.5";s:9:"image_url";s:75:"http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.5-18379-4.gif";s:12:"review_count";s:2:"83";s:3:"url";s:164:"http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=6557803&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true";}s:18:"room_facility_name";s:477:"Kamar bebas rokok ada tergantung ketersediaan|Brankas|AC|Internet - Wifi|Internet - Wifi (gratis)|Televisi LCD/layar plasma|Satelit/TV kabel|Meja|Shower|Baju Handuk|Bathtub|Pengering Rambut|Bar kecil|Mesin pembuat kopi/teh|Air mineral botol gratis|Televisi|Telepon|Sandal|Cermin|Papan setrika dengan permintaan|Kulkas|Teras|Gratis Perlengkapan Mandi|Shower Panas and Dingin";s:8:"oldprice";s:9:"617002.00";s:7:"address";s:51:"Magelang Street KM.  5,2 Yogyakarta, Sleman, Sleman";s:4:"wifi";s:23:"Wi-Fi Tersedia";s:10:"promo_name";s:0:"";s:5:"price";s:9:"443478.00";s:11:"total_price";s:9:"443478.00";s:8:"regional";s:39:"  - Sleman - Daerah Istimewa Yogyakarta";s:4:"name";s:47:"Crystal Lotus Hotel Yogyakarta Managed By Prabu";s:8:"hotel_id";s:8:"20087341";}i:6;a:23:{s:13:"province_name";s:26:"Daerah Istimewa Yogyakarta";s:14:"kecamatan_name";s:1:" ";s:14:"kelurahan_name";s:1:" ";s:12:"business_uri";s:221:"https://api-sandbox.tiket.com/pandanaran-hotel-yogyakarta?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A21222561";s:13:"photo_primary";s:65:"https://sandbox.tiket.com/img/default/d/e/default-default.sq2.jpg";s:11:"star_rating";s:1:"3";s:2:"id";s:14:"55003720160811";s:14:"room_available";s:2:"12";s:8:"latitude";s:23:"-7.81918940000000100000";s:9:"longitude";s:24:"110.37059939999995000000";s:20:"room_max_occupancies";s:1:"2";s:6:"rating";s:0:"";s:22:"tripadvisor_avg_rating";a:4:{s:10:"avg_rating";s:3:"4.0";s:9:"image_url";s:75:"http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif";s:12:"review_count";s:2:"79";s:3:"url";s:164:"http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=7808044&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true";}s:8:"oldprice";s:9:"513382.00";s:18:"room_facility_name";s:0:"";s:7:"address";s:0:"";s:4:"wifi";s:0:"";s:10:"promo_name";s:0:"";s:5:"price";s:9:"328000.00";s:11:"total_price";s:9:"328000.00";s:8:"regional";s:34:"  -   - Daerah Istimewa Yogyakarta";s:4:"name";s:0:"";s:8:"hotel_id";s:8:"21222561";}i:7;a:23:{s:13:"province_name";s:26:"Daerah Istimewa Yogyakarta";s:14:"kecamatan_name";s:1:" ";s:14:"kelurahan_name";s:1:" ";s:12:"business_uri";s:213:"https://api-sandbox.tiket.com/hotel-neo-malioboro?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A21402180";s:13:"photo_primary";s:65:"https://sandbox.tiket.com/img/default/d/e/default-default.sq2.jpg";s:11:"star_rating";s:1:"3";s:2:"id";s:14:"62897720160811";s:14:"room_available";s:3:"112";s:8:"latitude";s:23:"-7.79001630000000000000";s:9:"longitude";s:24:"110.36312539999994000000";s:20:"room_max_occupancies";s:1:"2";s:6:"rating";s:0:"";s:22:"tripadvisor_avg_rating";a:4:{s:10:"avg_rating";s:3:"4.0";s:9:"image_url";s:75:"http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif";s:12:"review_count";s:3:"399";s:3:"url";s:164:"http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=8092831&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true";}s:8:"oldprice";s:9:"771500.00";s:18:"room_facility_name";s:0:"";s:7:"address";s:0:"";s:4:"wifi";s:0:"";s:10:"promo_name";s:0:"";s:5:"price";s:9:"481580.00";s:11:"total_price";s:9:"481580.00";s:8:"regional";s:34:"  -   - Daerah Istimewa Yogyakarta";s:4:"name";s:0:"";s:8:"hotel_id";s:8:"21402180";}i:8;a:23:{s:13:"province_name";s:26:"Daerah Istimewa Yogyakarta";s:14:"kecamatan_name";s:11:"Mantrijeron";s:14:"kelurahan_name";s:16:"Suryodiningratan";s:12:"business_uri";s:243:"https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/seturan/the-victoria-hotel?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A3031";s:13:"photo_primary";s:79:"https://sandbox.tiket.com/img/business/v/i/business-victoria-yogya-pool.sq2.jpg";s:11:"star_rating";s:1:"3";s:2:"id";s:11:"31420160811";s:14:"room_available";s:1:"3";s:8:"latitude";s:23:"-7.78319030000000000000";s:9:"longitude";s:24:"110.40225609999993000000";s:20:"room_max_occupancies";s:1:"2";s:6:"rating";s:3:"7.6";s:22:"tripadvisor_avg_rating";a:4:{s:10:"avg_rating";s:3:"4.0";s:9:"image_url";s:75:"http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif";s:12:"review_count";s:2:"55";s:3:"url";s:164:"http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=2348889&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true";}s:18:"room_facility_name";s:171:"AC|Internet - Wifi|Televisi LCD/layar plasma|Satelit/TV kabel|Meja|Shower|Bar kecil|Mesin pembuat kopi/teh|Air mineral botol gratis";s:8:"oldprice";s:10:"1408671.00";s:7:"address";s:54:"Jl. Laksda Adisutjipto Km. 5 , Mantrijeron, Yogyakarta";s:4:"wifi";s:23:"Wi-Fi Tersedia";s:10:"promo_name";s:0:"";s:5:"price";s:9:"900000.00";s:11:"total_price";s:9:"900000.00";s:8:"regional";s:59:"Suryodiningratan - Mantrijeron - Daerah Istimewa Yogyakarta";s:4:"name";s:29:"The Victoria Hotel Yogyakarta";s:8:"hotel_id";s:4:"3031";}i:9;a:23:{s:13:"province_name";s:26:"Daerah Istimewa Yogyakarta";s:14:"kecamatan_name";s:13:"Gedong Tengen";s:14:"kelurahan_name";s:13:"Sosromenduran";s:12:"business_uri";s:271:"https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/malioboro/hotel-dafam-fortuna-malioboro-yogyakarta?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A20087773";s:13:"photo_primary";s:73:"https://sandbox.tiket.com/img/business/r/o/business-rooftop_pool2.sq2.jpg";s:11:"star_rating";s:1:"3";s:2:"id";s:14:"48285920160811";s:14:"room_available";s:3:"217";s:8:"latitude";s:23:"-7.79369329999999900000";s:9:"longitude";s:24:"110.36283040000000000000";s:20:"room_max_occupancies";s:1:"2";s:6:"rating";s:0:"";s:22:"tripadvisor_avg_rating";a:4:{s:10:"avg_rating";s:3:"4.0";s:9:"image_url";s:75:"http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif";s:12:"review_count";s:3:"210";s:3:"url";s:164:"http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=4876648&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true";}s:18:"room_facility_name";s:119:"Brankas|AC|Internet - Wifi|Satelit/TV kabel|Meja|Shower|Gratis Perlengkapan Mandi";s:8:"oldprice";s:9:"729379.00";s:7:"address";s:58:"Dagen Street No  60, Yogyakarta, Gedong Tengen, Yogyakarta";s:4:"wifi";s:23:"Wi-Fi Tersedia";s:10:"promo_name";s:0:"";s:5:"price";s:9:"466000.00";s:11:"total_price";s:9:"466000.00";s:8:"regional";s:58:"Sosromenduran - Gedong Tengen - Daerah Istimewa Yogyakarta";s:4:"name";s:40:"Hotel Dafam Fortuna Malioboro Yogyakarta";s:8:"hotel_id";s:8:"20087773";}i:10;a:23:{s:13:"province_name";s:26:"Daerah Istimewa Yogyakarta";s:14:"kecamatan_name";s:5:"Jetis";s:14:"kelurahan_name";s:8:"Gowongan";s:12:"business_uri";s:255:"https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/tugu-jogja/the-101-yogyakarta-tugu?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A20426620";s:13:"photo_primary";s:68:"https://sandbox.tiket.com/img/business/i/m/business-img_2590.sq2.jpg";s:11:"star_rating";s:1:"4";s:2:"id";s:14:"46702820160811";s:14:"room_available";s:1:"5";s:8:"latitude";s:23:"-7.78507033179146600000";s:9:"longitude";s:24:"110.36680161952972000000";s:20:"room_max_occupancies";s:1:"2";s:6:"rating";s:0:"";s:22:"tripadvisor_avg_rating";a:4:{s:10:"avg_rating";s:3:"4.0";s:9:"image_url";s:75:"http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif";s:12:"review_count";s:3:"253";s:3:"url";s:164:"http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=6739367&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true";}s:18:"room_facility_name";s:138:"Brankas|AC|Satelit/TV kabel|Shower|Pengering Rambut|Sandal|Cermin|Shower Panas and Dingin";s:8:"oldprice";s:10:"1089358.00";s:7:"address";s:70:"Jalan Margoutomo No. 103 ( Mangkubumi), Yogyakarta , Jetis, Yogyakarta";s:4:"wifi";s:0:"";s:10:"promo_name";s:0:"";s:5:"price";s:9:"782990.00";s:11:"total_price";s:9:"782990.00";s:8:"regional";s:45:"Gowongan - Jetis - Daerah Istimewa Yogyakarta";s:4:"name";s:23:"THE 1O1 Yogyakarta Tugu";s:8:"hotel_id";s:8:"20426620";}i:11;a:23:{s:13:"province_name";s:26:"Daerah Istimewa Yogyakarta";s:14:"kecamatan_name";s:1:" ";s:14:"kelurahan_name";s:1:" ";s:12:"business_uri";s:270:"https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/yogyakarta-airport/the-jayakarta-jogjakarta-hotel-spa?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A3786";s:13:"photo_primary";s:67:"https://sandbox.tiket.com/img/business/y/a/business-yajjarh.sq2.jpg";s:11:"star_rating";s:1:"4";s:2:"id";s:14:"48065120160811";s:14:"room_available";s:2:"12";s:8:"latitude";s:23:"-7.78343729999999900000";s:9:"longitude";s:24:"110.41959930000007000000";s:20:"room_max_occupancies";s:1:"2";s:6:"rating";s:3:"7.9";s:22:"tripadvisor_avg_rating";a:4:{s:10:"avg_rating";s:3:"3.5";s:9:"image_url";s:75:"http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.5-18379-4.gif";s:12:"review_count";s:3:"113";s:3:"url";s:163:"http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=307834&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true";}s:18:"room_facility_name";s:281:"Kamar bebas rokok ada tergantung ketersediaan|AC|Satelit/TV kabel|Shower dan bak terpisah|Bar kecil|Mesin pembuat kopi/teh|Air mineral botol gratis|Televisi|Telepon|Cermin|Pengering rambut dengan permintaan|Teras|Shower Panas and Dingin";s:8:"oldprice";s:10:"1363454.00";s:7:"address";s:38:"Jl. Laksda Adisucipto KM.8, Yogyakarta";s:4:"wifi";s:0:"";s:10:"promo_name";s:0:"";s:5:"price";s:9:"980000.00";s:11:"total_price";s:9:"980000.00";s:8:"regional";s:34:"  -   - Daerah Istimewa Yogyakarta";s:4:"name";s:40:"The Jayakarta Jogjakarta Hotel &amp; Spa";s:8:"hotel_id";s:4:"3786";}i:12;a:23:{s:13:"province_name";s:26:"Daerah Istimewa Yogyakarta";s:14:"kecamatan_name";s:5:"Jetis";s:14:"kelurahan_name";s:6:"Bumijo";s:12:"business_uri";s:254:"https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/sinduadi/hotel-tentrem-yogyakarta?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A19569414";s:13:"photo_primary";s:81:"https://sandbox.tiket.com/img/business/h/o/business-hoteltentrem_guest_r1.sq2.jpg";s:11:"star_rating";s:1:"5";s:2:"id";s:12:"591620160811";s:14:"room_available";s:2:"10";s:8:"latitude";s:23:"-7.77713830000000000000";s:9:"longitude";s:24:"110.36772680000001000000";s:20:"room_max_occupancies";s:1:"2";s:6:"rating";s:3:"9.0";s:22:"tripadvisor_avg_rating";a:4:{s:10:"avg_rating";s:3:"4.5";s:9:"image_url";s:75:"http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.5-18379-4.gif";s:12:"review_count";s:3:"540";s:3:"url";s:164:"http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=3737584&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true";}s:18:"room_facility_name";s:345:"Brankas|AC|Televisi LCD/layar plasma|Meja|Shower|Bathtub|Pengering Rambut|Mesin pembuat kopi/teh|Air mineral botol gratis|Televisi|Telepon|Gratis Perlengkapan Mandi|Lemari|Shower Panas and Dingin|Satellite TV Service |LCD TV |Free Wi-Fi |Cable TV Service |Minibar ";s:8:"oldprice";s:10:"1790143.00";s:7:"address";s:59:"Jl. AM Sangaji No. 72 A Yogyakarta 55233, Jetis, Yogyakarta";s:4:"wifi";s:0:"";s:10:"promo_name";s:0:"";s:5:"price";s:10:"1470500.00";s:11:"total_price";s:10:"1470500.00";s:8:"regional";s:43:"Bumijo - Jetis - Daerah Istimewa Yogyakarta";s:4:"name";s:24:"Hotel Tentrem Yogyakarta";s:8:"hotel_id";s:8:"19569414";}i:13;a:23:{s:13:"province_name";s:26:"Daerah Istimewa Yogyakarta";s:14:"kecamatan_name";s:5:"Depok";s:14:"kelurahan_name";s:13:"Condong Catur";s:12:"business_uri";s:256:"https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/seturan/merapi-merbabu-hotels-resorts?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A114345";s:13:"photo_primary";s:73:"https://sandbox.tiket.com/img/business/m/m/business-mm-hotel-room.sq2.jpg";s:11:"star_rating";s:1:"4";s:2:"id";s:12:"201620160811";s:14:"room_available";s:2:"10";s:8:"latitude";s:23:"-7.76510059999999900000";s:9:"longitude";s:24:"110.41087279999999000000";s:20:"room_max_occupancies";s:1:"2";s:6:"rating";s:3:"7.3";s:22:"tripadvisor_avg_rating";a:4:{s:10:"avg_rating";s:3:"3.5";s:9:"image_url";s:75:"http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.5-18379-4.gif";s:12:"review_count";s:2:"93";s:3:"url";s:164:"http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=2687978&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true";}s:18:"room_facility_name";s:344:"AC|Internet - Wifi (gratis)|Televisi LCD/layar plasma|Satelit/TV kabel|Meja|Shower|Mesin pembuat kopi/teh|Air mineral botol gratis|Surat kabar harian|Televisi|Telepon|Sandal|Cermin|Pengering rambut dengan permintaan|Kulkas|Gratis Perlengkapan Mandi|Sofa Bed";s:8:"oldprice";s:9:"660858.00";s:7:"address";s:34:"Seturan Main Street, Depok, Sleman";s:4:"wifi";s:23:"Wi-Fi Tersedia";s:10:"promo_name";s:0:"";s:5:"price";s:9:"475000.00";s:11:"total_price";s:9:"475000.00";s:8:"regional";s:50:"Condong Catur - Depok - Daerah Istimewa Yogyakarta";s:4:"name";s:44:"Merapi Merbabu Hotels and Resorts Yogyakarta";s:8:"hotel_id";s:6:"114345";}i:14;a:23:{s:13:"province_name";s:26:"Daerah Istimewa Yogyakarta";s:14:"kecamatan_name";s:1:" ";s:14:"kelurahan_name";s:1:" ";s:12:"business_uri";s:246:"https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/ugm/grand-tjokro-yogyakarta?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A184120";s:13:"photo_primary";s:75:"https://sandbox.tiket.com/img/business/s/u/business-superior_twin16.sq2.jpg";s:11:"star_rating";s:1:"4";s:2:"id";s:12:"333820160811";s:14:"room_available";s:2:"25";s:8:"latitude";s:23:"-7.78128440000000000000";s:9:"longitude";s:24:"110.38808280000000000000";s:20:"room_max_occupancies";s:1:"2";s:6:"rating";s:3:"8.0";s:22:"tripadvisor_avg_rating";a:4:{s:10:"avg_rating";s:3:"4.0";s:9:"image_url";s:75:"http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif";s:12:"review_count";s:2:"36";s:3:"url";s:164:"http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=3545399&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true";}s:18:"room_facility_name";s:282:"AC|Internet - Wifi (gratis)|Televisi LCD/layar plasma|Satelit/TV kabel|Shower|Mesin pembuat kopi/teh|Air mineral botol gratis|Telepon|Sandal|Cermin|Kulkas|Gratis Perlengkapan Mandi|Lemari|Shower Panas and Dingin";s:8:"oldprice";s:10:"1182588.00";s:7:"address";s:48:"Gejayan Street Number 37, Yogyakarta, Yogyakarta";s:4:"wifi";s:23:"Wi-Fi Tersedia";s:10:"promo_name";s:0:"";s:5:"price";s:9:"850000.00";s:11:"total_price";s:9:"850000.00";s:8:"regional";s:34:"  -   - Daerah Istimewa Yogyakarta";s:4:"name";s:23:"Grand Tjokro Yogyakarta";s:8:"hotel_id";s:6:"184120";}i:15;a:23:{s:13:"province_name";s:26:"Daerah Istimewa Yogyakarta";s:14:"kecamatan_name";s:1:" ";s:14:"kelurahan_name";s:1:" ";s:12:"business_uri";s:256:"https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/yogyakarta/the-sahid-rich-jogja-hotel?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A115544";s:13:"photo_primary";s:73:"https://sandbox.tiket.com/img/business/t/h/business-the-rich-main.sq2.jpg";s:11:"star_rating";s:1:"4";s:2:"id";s:12:"210220160811";s:14:"room_available";s:3:"298";s:8:"latitude";s:23:"-7.75262970000000000000";s:9:"longitude";s:24:"110.36215519999996000000";s:20:"room_max_occupancies";s:1:"2";s:6:"rating";s:0:"";s:22:"tripadvisor_avg_rating";a:4:{s:10:"avg_rating";s:3:"3.5";s:9:"image_url";s:75:"http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.5-18379-4.gif";s:12:"review_count";s:3:"175";s:3:"url";s:164:"http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=3317684&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true";}s:18:"room_facility_name";s:207:"Brankas|AC|Televisi LCD/layar plasma|Satelit/TV kabel|Shower|Mesin pembuat kopi/teh|Air mineral botol gratis|Telepon|Kulkas|Gratis Perlengkapan Mandi";s:8:"oldprice";s:10:"1321716.00";s:7:"address";s:36:"Jl. Magelang KM.6, No 18, Yogyakarta";s:4:"wifi";s:0:"";s:10:"promo_name";s:0:"";s:5:"price";s:9:"950000.00";s:11:"total_price";s:9:"950000.00";s:8:"regional";s:34:"  -   - Daerah Istimewa Yogyakarta";s:4:"name";s:26:"The Sahid Rich Jogja Hotel";s:8:"hotel_id";s:6:"115544";}i:16;a:23:{s:13:"province_name";s:26:"Daerah Istimewa Yogyakarta";s:14:"kecamatan_name";s:1:" ";s:14:"kelurahan_name";s:1:" ";s:12:"business_uri";s:225:"https://api-sandbox.tiket.com/de-laxston-hotel-jogja-by-quins?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A21626059";s:13:"photo_primary";s:65:"https://sandbox.tiket.com/img/default/d/e/default-default.sq2.jpg";s:11:"star_rating";s:1:"3";s:2:"id";s:14:"71620320160811";s:14:"room_available";s:1:"3";s:8:"latitude";s:23:"-7.78301280000000000000";s:9:"longitude";s:24:"110.38749610000002000000";s:20:"room_max_occupancies";s:1:"2";s:6:"rating";s:0:"";s:22:"tripadvisor_avg_rating";a:4:{s:10:"avg_rating";s:3:"4.0";s:9:"image_url";s:75:"http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif";s:12:"review_count";s:2:"33";s:3:"url";s:164:"http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=8608038&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true";}s:8:"oldprice";s:9:"970418.00";s:18:"room_facility_name";s:0:"";s:7:"address";s:0:"";s:4:"wifi";s:0:"";s:10:"promo_name";s:0:"";s:5:"price";s:9:"620000.00";s:11:"total_price";s:9:"620000.00";s:8:"regional";s:34:"  -   - Daerah Istimewa Yogyakarta";s:4:"name";s:0:"";s:8:"hotel_id";s:8:"21626059";}i:17;a:23:{s:13:"province_name";s:26:"Daerah Istimewa Yogyakarta";s:14:"kecamatan_name";s:1:" ";s:14:"kelurahan_name";s:1:" ";s:12:"business_uri";s:242:"https://api-sandbox.tiket.com/the-alana-yogyakarta-hotel-and-convention-center?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A21227380";s:13:"photo_primary";s:65:"https://sandbox.tiket.com/img/default/d/e/default-default.sq2.jpg";s:11:"star_rating";s:1:"4";s:2:"id";s:14:"71998220160811";s:14:"room_available";s:3:"219";s:8:"latitude";s:23:"-7.72104340000000000000";s:9:"longitude";s:24:"110.38274189999993000000";s:20:"room_max_occupancies";s:1:"2";s:6:"rating";s:0:"";s:22:"tripadvisor_avg_rating";a:4:{s:10:"avg_rating";s:3:"4.0";s:9:"image_url";s:75:"http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif";s:12:"review_count";s:3:"143";s:3:"url";s:164:"http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=7745637&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true";}s:8:"oldprice";s:10:"1013159.00";s:18:"room_facility_name";s:0:"";s:7:"address";s:0:"";s:4:"wifi";s:0:"";s:10:"promo_name";s:0:"";s:5:"price";s:9:"711480.00";s:11:"total_price";s:9:"711480.00";s:8:"regional";s:34:"  -   - Daerah Istimewa Yogyakarta";s:4:"name";s:0:"";s:8:"hotel_id";s:8:"21227380";}i:18;a:23:{s:13:"province_name";s:26:"Daerah Istimewa Yogyakarta";s:14:"kecamatan_name";s:10:"Mergangsan";s:14:"kelurahan_name";s:13:"Brontokusuman";s:12:"business_uri";s:254:"https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/janti/hotel-new-saphir-yogyakarta?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A20162398";s:13:"photo_primary";s:68:"https://sandbox.tiket.com/img/business/s/a/business-saphir61.sq2.jpg";s:11:"star_rating";s:1:"4";s:2:"id";s:14:"45651120160811";s:14:"room_available";s:1:"5";s:8:"latitude";s:23:"-7.78010430000000100000";s:9:"longitude";s:24:"110.39122980000002000000";s:20:"room_max_occupancies";s:1:"2";s:6:"rating";s:3:"8.3";s:22:"tripadvisor_avg_rating";a:4:{s:10:"avg_rating";s:3:"3.5";s:9:"image_url";s:75:"http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/3.5-18379-4.gif";s:12:"review_count";s:3:"132";s:3:"url";s:163:"http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=307067&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true";}s:18:"room_facility_name";s:191:"AC|Televisi LCD/layar plasma|Meja|Shower|Bathtub|Bar kecil|Mesin pembuat kopi/teh|Air mineral botol gratis|Televisi|Kulkas";s:8:"oldprice";s:9:"695640.00";s:7:"address";s:52:"Jl. Laksda Adisucipto No. 38, Mergangsan, Yogyakarta";s:4:"wifi";s:0:"";s:10:"promo_name";s:0:"";s:5:"price";s:9:"500000.00";s:11:"total_price";s:9:"500000.00";s:8:"regional";s:55:"Brontokusuman - Mergangsan - Daerah Istimewa Yogyakarta";s:4:"name";s:27:"Hotel New Saphir Yogyakarta";s:8:"hotel_id";s:8:"20162398";}i:19;a:23:{s:13:"province_name";s:26:"Daerah Istimewa Yogyakarta";s:14:"kecamatan_name";s:1:" ";s:14:"kelurahan_name";s:1:" ";s:12:"business_uri";s:214:"https://api-sandbox.tiket.com/neo-awana-yogyakarta?startdate=2016-08-11&night=1&room=1&adult=2&child=0&is_partner=0&star_rating=0&hotel_chain=0&facilities=0&latitude=0&longitude=0&distance=0&uid=business%3A21171272";s:13:"photo_primary";s:65:"https://sandbox.tiket.com/img/default/d/e/default-default.sq2.jpg";s:11:"star_rating";s:1:"3";s:2:"id";s:14:"55167120160811";s:14:"room_available";s:3:"195";s:8:"latitude";s:23:"-7.82049380000000000000";s:9:"longitude";s:24:"110.36539080000000000000";s:20:"room_max_occupancies";s:1:"2";s:6:"rating";s:0:"";s:22:"tripadvisor_avg_rating";a:4:{s:10:"avg_rating";s:3:"4.0";s:9:"image_url";s:75:"http://www.tripadvisor.co.id/img/cdsi/img2/ratings/traveler/4.0-18379-4.gif";s:12:"review_count";s:3:"140";s:3:"url";s:164:"http://www.tripadvisor.com/WidgetEmbed-cdspropertydetail?locationId=7751603&lang=en_US&partnerId=176DD3B47F374A79ACF1E7E5AC852AC0&isTA=true&format=html&display=true";}s:8:"oldprice";s:9:"635809.00";s:18:"room_facility_name";s:0:"";s:7:"address";s:0:"";s:4:"wifi";s:0:"";s:10:"promo_name";s:0:"";s:5:"price";s:9:"396880.00";s:11:"total_price";s:9:"396880.00";s:8:"regional";s:34:"  -   - Daerah Istimewa Yogyakarta";s:4:"name";s:0:"";s:8:"hotel_id";s:8:"21171272";}}}s:10:"pagination";a:4:{s:11:"total_found";i:134;s:12:"current_page";i:1;s:6:"offset";s:2:"20";s:8:"lastPage";d:7;}s:12:"login_status";s:4:"true";s:8:"guest_id";s:8:"22691145";s:11:"login_email";s:21:"wida.skydev@gmail.com";s:5:"token";s:40:"f9b29ac359ca5d77755e7588751c089bf96f0dc9";}
```

#### Http Request

    `GET https://api-sandbox.tiket.com/search/hotel?q=Yogyakarta&startdate=2016-08-11&night=1&enddate=2016-08-12&room=1&adult=2&child=0&token=f9b29ac359ca5d77755e7588751c089bf96f0dc9&output=json`




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


## Search by Area

```xml
<?xml version="1.0" encoding="utf-8"?>
<tiket>
    <diagnostic>
        <status>200</status>
        <elapsetime>15.1109</elapsetime>
        <memoryusage>5.64MB</memoryusage>
        <unix_timestamp>1470371037</unix_timestamp>
        <confirm>success</confirm>
        <lang>id</lang>
        <currency>IDR</currency>
    </diagnostic>
    <output_type>xml</output_type>
    <results>
        <result>
            <uid>area:168</uid>
            <value>Jakarta Timur</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:168</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:21658</uid>
            <value>Matraman</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:21658</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:21659</uid>
            <value>Pulo Gadung</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:21659</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:21670</uid>
            <value>Jatinegara</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:21670</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:21671</uid>
            <value>Duren Sawit</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:21671</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:21672</uid>
            <value>Kramat Jati</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:21672</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:21673</uid>
            <value>Pasar Rebo</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:21673</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:21674</uid>
            <value>Ciracas</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:21674</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:21675</uid>
            <value>Cipayung</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:21675</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:21676</uid>
            <value>Cakung</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:21676</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:21677</uid>
            <value>Makasar</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:21677</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31724</uid>
            <value>Kayu Manis</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31724</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31725</uid>
            <value>Pisangan Baru</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31725</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31730</uid>
            <value>Kayu Putih</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31730</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31731</uid>
            <value>Rawamangun</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31731</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31732</uid>
            <value>Pisangan Timur</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31732</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31733</uid>
            <value>Kebon Manggis</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31733</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31734</uid>
            <value>Utan Kayu Utara</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31734</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31735</uid>
            <value>Utan Kayu Selatan</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31735</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31742</uid>
            <value>Cipinang</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31742</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31743</uid>
            <value>Jatinegara Kaum</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31743</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31747</uid>
            <value>Pal Meriam</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31747</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31753</uid>
            <value>Bali Mester</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31753</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31756</uid>
            <value>Bidaracina</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31756</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31758</uid>
            <value>Kampung Melayu</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31758</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31759</uid>
            <value>Rawa Bunga</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31759</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31760</uid>
            <value>Cipinang Besar Utara</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31760</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31761</uid>
            <value>Cipinang Besar Selatan</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31761</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31762</uid>
            <value>Cipinang Muara</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31762</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31763</uid>
            <value>Cipinang Cempedak</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31763</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31766</uid>
            <value>Pinang Ranti</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31766</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31767</uid>
            <value>Halim Perdanakusuma</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31767</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31770</uid>
            <value>Cipinang Melayu</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31770</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31772</uid>
            <value>Kebon Pala</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31772</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31776</uid>
            <value>Cakung Barat</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31776</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31777</uid>
            <value>Cakung Timur</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31777</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31778</uid>
            <value>Rawa Terate</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31778</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31779</uid>
            <value>Penggilingan</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31779</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31781</uid>
            <value>Pulogebang</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31781</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31784</uid>
            <value>Ujung Menteng</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31784</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31790</uid>
            <value>Lubang Buaya</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31790</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31792</uid>
            <value>Ceger</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31792</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31794</uid>
            <value>Munjul</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31794</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31798</uid>
            <value>Pondok Ranggon</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31798</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31801</uid>
            <value>Cilangkap</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31801</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31804</uid>
            <value>Setu</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31804</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31807</uid>
            <value>Bambu Apus</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31807</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31814</uid>
            <value>Cibubur</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31814</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31816</uid>
            <value>Kelapa Dua Wetan</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31816</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31820</uid>
            <value>Susukan</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31820</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31821</uid>
            <value>Rambutan</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31821</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31823</uid>
            <value>Pekayon</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31823</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31825</uid>
            <value>Kampung Gedong</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31825</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31829</uid>
            <value>Cijantung</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31829</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31831</uid>
            <value>Kampung Baru</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31831</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31833</uid>
            <value>Kalisari</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31833</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31841</uid>
            <value>Batuampar</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31841</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31844</uid>
            <value>Balekambang</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31844</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31846</uid>
            <value>Kampung Tengah</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31846</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31847</uid>
            <value>Dukuh</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31847</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31849</uid>
            <value>Cawang</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31849</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31850</uid>
            <value>Cililitan</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31850</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31855</uid>
            <value>Pondok Bambu</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31855</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31860</uid>
            <value>Pondok Kelapa</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31860</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31863</uid>
            <value>Pondok Kopi</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31863</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31865</uid>
            <value>Malaka Jaya</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31865</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31866</uid>
            <value>Malaka Sari</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31866</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:31867</uid>
            <value>Klender</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:31867</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:67889</uid>
            <value>Halim Perdana Kusumah</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:67889</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:87342</uid>
            <value>Pramuka</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:87342</uri>
            <category>Area</category>
        </result>
        <result>
            <uid>area:87348</uid>
            <value>Taman Mini</value>
            <uri>https://api-sandbox.tiket.com/search/hotel?uid=area:87348</uri>
            <category>Area</category>
        </result>
    </results>
    <login_status>true</login_status>
    <guest_id>22691145</guest_id>
    <login_email>wida.skydev@gmail.com</login_email>
    <token>f9b29ac359ca5d77755e7588751c089bf96f0dc9</token>
</tiket>
```

```json
{
  "diagnostic": {
    "status": "200",
    "elapsetime": "15.1024",
    "memoryusage": "5.63MB",
    "unix_timestamp": 1470371205,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "results": {
    "result": [
      {
        "uid": "area:168",
        "value": "Jakarta Timur",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:168",
        "category": "Area"
      },
      {
        "uid": "area:21658",
        "value": "Matraman",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:21658",
        "category": "Area"
      },
      {
        "uid": "area:21659",
        "value": "Pulo Gadung",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:21659",
        "category": "Area"
      },
      {
        "uid": "area:21670",
        "value": "Jatinegara",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:21670",
        "category": "Area"
      },
      {
        "uid": "area:21671",
        "value": "Duren Sawit",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:21671",
        "category": "Area"
      },
      {
        "uid": "area:21672",
        "value": "Kramat Jati",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:21672",
        "category": "Area"
      },
      {
        "uid": "area:21673",
        "value": "Pasar Rebo",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:21673",
        "category": "Area"
      },
      {
        "uid": "area:21674",
        "value": "Ciracas",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:21674",
        "category": "Area"
      },
      {
        "uid": "area:21675",
        "value": "Cipayung",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:21675",
        "category": "Area"
      },
      {
        "uid": "area:21676",
        "value": "Cakung",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:21676",
        "category": "Area"
      },
      {
        "uid": "area:21677",
        "value": "Makasar",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:21677",
        "category": "Area"
      },
      {
        "uid": "area:31724",
        "value": "Kayu Manis",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31724",
        "category": "Area"
      },
      {
        "uid": "area:31725",
        "value": "Pisangan Baru",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31725",
        "category": "Area"
      },
      {
        "uid": "area:31730",
        "value": "Kayu Putih",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31730",
        "category": "Area"
      },
      {
        "uid": "area:31731",
        "value": "Rawamangun",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31731",
        "category": "Area"
      },
      {
        "uid": "area:31732",
        "value": "Pisangan Timur",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31732",
        "category": "Area"
      },
      {
        "uid": "area:31733",
        "value": "Kebon Manggis",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31733",
        "category": "Area"
      },
      {
        "uid": "area:31734",
        "value": "Utan Kayu Utara",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31734",
        "category": "Area"
      },
      {
        "uid": "area:31735",
        "value": "Utan Kayu Selatan",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31735",
        "category": "Area"
      },
      {
        "uid": "area:31742",
        "value": "Cipinang",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31742",
        "category": "Area"
      },
      {
        "uid": "area:31743",
        "value": "Jatinegara Kaum",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31743",
        "category": "Area"
      },
      {
        "uid": "area:31747",
        "value": "Pal Meriam",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31747",
        "category": "Area"
      },
      {
        "uid": "area:31753",
        "value": "Bali Mester",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31753",
        "category": "Area"
      },
      {
        "uid": "area:31756",
        "value": "Bidaracina",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31756",
        "category": "Area"
      },
      {
        "uid": "area:31758",
        "value": "Kampung Melayu",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31758",
        "category": "Area"
      },
      {
        "uid": "area:31759",
        "value": "Rawa Bunga",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31759",
        "category": "Area"
      },
      {
        "uid": "area:31760",
        "value": "Cipinang Besar Utara",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31760",
        "category": "Area"
      },
      {
        "uid": "area:31761",
        "value": "Cipinang Besar Selatan",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31761",
        "category": "Area"
      },
      {
        "uid": "area:31762",
        "value": "Cipinang Muara",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31762",
        "category": "Area"
      },
      {
        "uid": "area:31763",
        "value": "Cipinang Cempedak",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31763",
        "category": "Area"
      },
      {
        "uid": "area:31766",
        "value": "Pinang Ranti",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31766",
        "category": "Area"
      },
      {
        "uid": "area:31767",
        "value": "Halim Perdanakusuma",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31767",
        "category": "Area"
      },
      {
        "uid": "area:31770",
        "value": "Cipinang Melayu",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31770",
        "category": "Area"
      },
      {
        "uid": "area:31772",
        "value": "Kebon Pala",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31772",
        "category": "Area"
      },
      {
        "uid": "area:31776",
        "value": "Cakung Barat",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31776",
        "category": "Area"
      },
      {
        "uid": "area:31777",
        "value": "Cakung Timur",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31777",
        "category": "Area"
      },
      {
        "uid": "area:31778",
        "value": "Rawa Terate",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31778",
        "category": "Area"
      },
      {
        "uid": "area:31779",
        "value": "Penggilingan",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31779",
        "category": "Area"
      },
      {
        "uid": "area:31781",
        "value": "Pulogebang",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31781",
        "category": "Area"
      },
      {
        "uid": "area:31784",
        "value": "Ujung Menteng",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31784",
        "category": "Area"
      },
      {
        "uid": "area:31790",
        "value": "Lubang Buaya",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31790",
        "category": "Area"
      },
      {
        "uid": "area:31792",
        "value": "Ceger",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31792",
        "category": "Area"
      },
      {
        "uid": "area:31794",
        "value": "Munjul",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31794",
        "category": "Area"
      },
      {
        "uid": "area:31798",
        "value": "Pondok Ranggon",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31798",
        "category": "Area"
      },
      {
        "uid": "area:31801",
        "value": "Cilangkap",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31801",
        "category": "Area"
      },
      {
        "uid": "area:31804",
        "value": "Setu",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31804",
        "category": "Area"
      },
      {
        "uid": "area:31807",
        "value": "Bambu Apus",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31807",
        "category": "Area"
      },
      {
        "uid": "area:31814",
        "value": "Cibubur",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31814",
        "category": "Area"
      },
      {
        "uid": "area:31816",
        "value": "Kelapa Dua Wetan",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31816",
        "category": "Area"
      },
      {
        "uid": "area:31820",
        "value": "Susukan",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31820",
        "category": "Area"
      },
      {
        "uid": "area:31821",
        "value": "Rambutan",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31821",
        "category": "Area"
      },
      {
        "uid": "area:31823",
        "value": "Pekayon",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31823",
        "category": "Area"
      },
      {
        "uid": "area:31825",
        "value": "Kampung Gedong",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31825",
        "category": "Area"
      },
      {
        "uid": "area:31829",
        "value": "Cijantung",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31829",
        "category": "Area"
      },
      {
        "uid": "area:31831",
        "value": "Kampung Baru",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31831",
        "category": "Area"
      },
      {
        "uid": "area:31833",
        "value": "Kalisari",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31833",
        "category": "Area"
      },
      {
        "uid": "area:31841",
        "value": "Batuampar",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31841",
        "category": "Area"
      },
      {
        "uid": "area:31844",
        "value": "Balekambang",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31844",
        "category": "Area"
      },
      {
        "uid": "area:31846",
        "value": "Kampung Tengah",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31846",
        "category": "Area"
      },
      {
        "uid": "area:31847",
        "value": "Dukuh",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31847",
        "category": "Area"
      },
      {
        "uid": "area:31849",
        "value": "Cawang",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31849",
        "category": "Area"
      },
      {
        "uid": "area:31850",
        "value": "Cililitan",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31850",
        "category": "Area"
      },
      {
        "uid": "area:31855",
        "value": "Pondok Bambu",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31855",
        "category": "Area"
      },
      {
        "uid": "area:31860",
        "value": "Pondok Kelapa",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31860",
        "category": "Area"
      },
      {
        "uid": "area:31863",
        "value": "Pondok Kopi",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31863",
        "category": "Area"
      },
      {
        "uid": "area:31865",
        "value": "Malaka Jaya",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31865",
        "category": "Area"
      },
      {
        "uid": "area:31866",
        "value": "Malaka Sari",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31866",
        "category": "Area"
      },
      {
        "uid": "area:31867",
        "value": "Klender",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:31867",
        "category": "Area"
      },
      {
        "uid": "area:67889",
        "value": "Halim Perdana Kusumah",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:67889",
        "category": "Area"
      },
      {
        "uid": "area:87342",
        "value": "Pramuka",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:87342",
        "category": "Area"
      },
      {
        "uid": "area:87348",
        "value": "Taman Mini",
        "uri": "https://api-sandbox.tiket.com/search/hotel?uid=area:87348",
        "category": "Area"
      }
    ]
  },
  "login_status": "true",
  "guest_id": "22691145",
  "login_email": "wida.skydev@gmail.com",
  "token": "f9b29ac359ca5d77755e7588751c089bf96f0dc9"
}
```

```matlab
a:7:{s:10:"diagnostic";a:7:{s:6:"status";s:3:"200";s:10:"elapsetime";s:14:"15.1130";s:11:"memoryusage";s:14:"5.63MB";s:14:"unix_timestamp";i:1470371254;s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:11:"output_type";s:9:"serialize";s:7:"results";a:1:{s:6:"result";a:71:{i:0;a:4:{s:3:"uid";s:8:"area:168";s:5:"value";s:13:"Jakarta Timur";s:3:"uri";s:55:"https://api-sandbox.tiket.com/search/hotel?uid=area:168";s:8:"category";s:13:"Area";}i:1;a:4:{s:3:"uid";s:10:"area:21658";s:5:"value";s:8:"Matraman";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:21658";s:8:"category";s:13:"Area";}i:2;a:4:{s:3:"uid";s:10:"area:21659";s:5:"value";s:11:"Pulo Gadung";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:21659";s:8:"category";s:13:"Area";}i:3;a:4:{s:3:"uid";s:10:"area:21670";s:5:"value";s:10:"Jatinegara";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:21670";s:8:"category";s:13:"Area";}i:4;a:4:{s:3:"uid";s:10:"area:21671";s:5:"value";s:11:"Duren Sawit";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:21671";s:8:"category";s:13:"Area";}i:5;a:4:{s:3:"uid";s:10:"area:21672";s:5:"value";s:11:"Kramat Jati";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:21672";s:8:"category";s:13:"Area";}i:6;a:4:{s:3:"uid";s:10:"area:21673";s:5:"value";s:10:"Pasar Rebo";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:21673";s:8:"category";s:13:"Area";}i:7;a:4:{s:3:"uid";s:10:"area:21674";s:5:"value";s:7:"Ciracas";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:21674";s:8:"category";s:13:"Area";}i:8;a:4:{s:3:"uid";s:10:"area:21675";s:5:"value";s:8:"Cipayung";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:21675";s:8:"category";s:13:"Area";}i:9;a:4:{s:3:"uid";s:10:"area:21676";s:5:"value";s:6:"Cakung";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:21676";s:8:"category";s:13:"Area";}i:10;a:4:{s:3:"uid";s:10:"area:21677";s:5:"value";s:7:"Makasar";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:21677";s:8:"category";s:13:"Area";}i:11;a:4:{s:3:"uid";s:10:"area:31724";s:5:"value";s:10:"Kayu Manis";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31724";s:8:"category";s:13:"Area";}i:12;a:4:{s:3:"uid";s:10:"area:31725";s:5:"value";s:13:"Pisangan Baru";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31725";s:8:"category";s:13:"Area";}i:13;a:4:{s:3:"uid";s:10:"area:31730";s:5:"value";s:10:"Kayu Putih";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31730";s:8:"category";s:13:"Area";}i:14;a:4:{s:3:"uid";s:10:"area:31731";s:5:"value";s:10:"Rawamangun";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31731";s:8:"category";s:13:"Area";}i:15;a:4:{s:3:"uid";s:10:"area:31732";s:5:"value";s:14:"Pisangan Timur";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31732";s:8:"category";s:13:"Area";}i:16;a:4:{s:3:"uid";s:10:"area:31733";s:5:"value";s:13:"Kebon Manggis";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31733";s:8:"category";s:13:"Area";}i:17;a:4:{s:3:"uid";s:10:"area:31734";s:5:"value";s:15:"Utan Kayu Utara";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31734";s:8:"category";s:13:"Area";}i:18;a:4:{s:3:"uid";s:10:"area:31735";s:5:"value";s:17:"Utan Kayu Selatan";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31735";s:8:"category";s:13:"Area";}i:19;a:4:{s:3:"uid";s:10:"area:31742";s:5:"value";s:8:"Cipinang";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31742";s:8:"category";s:13:"Area";}i:20;a:4:{s:3:"uid";s:10:"area:31743";s:5:"value";s:15:"Jatinegara Kaum";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31743";s:8:"category";s:13:"Area";}i:21;a:4:{s:3:"uid";s:10:"area:31747";s:5:"value";s:10:"Pal Meriam";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31747";s:8:"category";s:13:"Area";}i:22;a:4:{s:3:"uid";s:10:"area:31753";s:5:"value";s:11:"Bali Mester";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31753";s:8:"category";s:13:"Area";}i:23;a:4:{s:3:"uid";s:10:"area:31756";s:5:"value";s:10:"Bidaracina";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31756";s:8:"category";s:13:"Area";}i:24;a:4:{s:3:"uid";s:10:"area:31758";s:5:"value";s:14:"Kampung Melayu";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31758";s:8:"category";s:13:"Area";}i:25;a:4:{s:3:"uid";s:10:"area:31759";s:5:"value";s:10:"Rawa Bunga";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31759";s:8:"category";s:13:"Area";}i:26;a:4:{s:3:"uid";s:10:"area:31760";s:5:"value";s:20:"Cipinang Besar Utara";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31760";s:8:"category";s:13:"Area";}i:27;a:4:{s:3:"uid";s:10:"area:31761";s:5:"value";s:22:"Cipinang Besar Selatan";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31761";s:8:"category";s:13:"Area";}i:28;a:4:{s:3:"uid";s:10:"area:31762";s:5:"value";s:14:"Cipinang Muara";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31762";s:8:"category";s:13:"Area";}i:29;a:4:{s:3:"uid";s:10:"area:31763";s:5:"value";s:17:"Cipinang Cempedak";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31763";s:8:"category";s:13:"Area";}i:30;a:4:{s:3:"uid";s:10:"area:31766";s:5:"value";s:12:"Pinang Ranti";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31766";s:8:"category";s:13:"Area";}i:31;a:4:{s:3:"uid";s:10:"area:31767";s:5:"value";s:19:"Halim Perdanakusuma";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31767";s:8:"category";s:13:"Area";}i:32;a:4:{s:3:"uid";s:10:"area:31770";s:5:"value";s:15:"Cipinang Melayu";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31770";s:8:"category";s:13:"Area";}i:33;a:4:{s:3:"uid";s:10:"area:31772";s:5:"value";s:10:"Kebon Pala";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31772";s:8:"category";s:13:"Area";}i:34;a:4:{s:3:"uid";s:10:"area:31776";s:5:"value";s:12:"Cakung Barat";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31776";s:8:"category";s:13:"Area";}i:35;a:4:{s:3:"uid";s:10:"area:31777";s:5:"value";s:12:"Cakung Timur";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31777";s:8:"category";s:13:"Area";}i:36;a:4:{s:3:"uid";s:10:"area:31778";s:5:"value";s:11:"Rawa Terate";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31778";s:8:"category";s:13:"Area";}i:37;a:4:{s:3:"uid";s:10:"area:31779";s:5:"value";s:12:"Penggilingan";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31779";s:8:"category";s:13:"Area";}i:38;a:4:{s:3:"uid";s:10:"area:31781";s:5:"value";s:10:"Pulogebang";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31781";s:8:"category";s:13:"Area";}i:39;a:4:{s:3:"uid";s:10:"area:31784";s:5:"value";s:13:"Ujung Menteng";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31784";s:8:"category";s:13:"Area";}i:40;a:4:{s:3:"uid";s:10:"area:31790";s:5:"value";s:12:"Lubang Buaya";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31790";s:8:"category";s:13:"Area";}i:41;a:4:{s:3:"uid";s:10:"area:31792";s:5:"value";s:5:"Ceger";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31792";s:8:"category";s:13:"Area";}i:42;a:4:{s:3:"uid";s:10:"area:31794";s:5:"value";s:6:"Munjul";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31794";s:8:"category";s:13:"Area";}i:43;a:4:{s:3:"uid";s:10:"area:31798";s:5:"value";s:14:"Pondok Ranggon";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31798";s:8:"category";s:13:"Area";}i:44;a:4:{s:3:"uid";s:10:"area:31801";s:5:"value";s:9:"Cilangkap";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31801";s:8:"category";s:13:"Area";}i:45;a:4:{s:3:"uid";s:10:"area:31804";s:5:"value";s:4:"Setu";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31804";s:8:"category";s:13:"Area";}i:46;a:4:{s:3:"uid";s:10:"area:31807";s:5:"value";s:10:"Bambu Apus";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31807";s:8:"category";s:13:"Area";}i:47;a:4:{s:3:"uid";s:10:"area:31814";s:5:"value";s:7:"Cibubur";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31814";s:8:"category";s:13:"Area";}i:48;a:4:{s:3:"uid";s:10:"area:31816";s:5:"value";s:16:"Kelapa Dua Wetan";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31816";s:8:"category";s:13:"Area";}i:49;a:4:{s:3:"uid";s:10:"area:31820";s:5:"value";s:7:"Susukan";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31820";s:8:"category";s:13:"Area";}i:50;a:4:{s:3:"uid";s:10:"area:31821";s:5:"value";s:8:"Rambutan";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31821";s:8:"category";s:13:"Area";}i:51;a:4:{s:3:"uid";s:10:"area:31823";s:5:"value";s:7:"Pekayon";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31823";s:8:"category";s:13:"Area";}i:52;a:4:{s:3:"uid";s:10:"area:31825";s:5:"value";s:14:"Kampung Gedong";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31825";s:8:"category";s:13:"Area";}i:53;a:4:{s:3:"uid";s:10:"area:31829";s:5:"value";s:9:"Cijantung";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31829";s:8:"category";s:13:"Area";}i:54;a:4:{s:3:"uid";s:10:"area:31831";s:5:"value";s:12:"Kampung Baru";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31831";s:8:"category";s:13:"Area";}i:55;a:4:{s:3:"uid";s:10:"area:31833";s:5:"value";s:8:"Kalisari";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31833";s:8:"category";s:13:"Area";}i:56;a:4:{s:3:"uid";s:10:"area:31841";s:5:"value";s:9:"Batuampar";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31841";s:8:"category";s:13:"Area";}i:57;a:4:{s:3:"uid";s:10:"area:31844";s:5:"value";s:11:"Balekambang";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31844";s:8:"category";s:13:"Area";}i:58;a:4:{s:3:"uid";s:10:"area:31846";s:5:"value";s:14:"Kampung Tengah";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31846";s:8:"category";s:13:"Area";}i:59;a:4:{s:3:"uid";s:10:"area:31847";s:5:"value";s:5:"Dukuh";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31847";s:8:"category";s:13:"Area";}i:60;a:4:{s:3:"uid";s:10:"area:31849";s:5:"value";s:6:"Cawang";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31849";s:8:"category";s:13:"Area";}i:61;a:4:{s:3:"uid";s:10:"area:31850";s:5:"value";s:9:"Cililitan";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31850";s:8:"category";s:13:"Area";}i:62;a:4:{s:3:"uid";s:10:"area:31855";s:5:"value";s:12:"Pondok Bambu";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31855";s:8:"category";s:13:"Area";}i:63;a:4:{s:3:"uid";s:10:"area:31860";s:5:"value";s:13:"Pondok Kelapa";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31860";s:8:"category";s:13:"Area";}i:64;a:4:{s:3:"uid";s:10:"area:31863";s:5:"value";s:11:"Pondok Kopi";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31863";s:8:"category";s:13:"Area";}i:65;a:4:{s:3:"uid";s:10:"area:31865";s:5:"value";s:11:"Malaka Jaya";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31865";s:8:"category";s:13:"Area";}i:66;a:4:{s:3:"uid";s:10:"area:31866";s:5:"value";s:11:"Malaka Sari";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31866";s:8:"category";s:13:"Area";}i:67;a:4:{s:3:"uid";s:10:"area:31867";s:5:"value";s:7:"Klender";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:31867";s:8:"category";s:13:"Area";}i:68;a:4:{s:3:"uid";s:10:"area:67889";s:5:"value";s:21:"Halim Perdana Kusumah";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:67889";s:8:"category";s:13:"Area";}i:69;a:4:{s:3:"uid";s:10:"area:87342";s:5:"value";s:7:"Pramuka";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:87342";s:8:"category";s:13:"Area";}i:70;a:4:{s:3:"uid";s:10:"area:87348";s:5:"value";s:10:"Taman Mini";s:3:"uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=area:87348";s:8:"category";s:13:"Area";}}}s:12:"login_status";s:4:"true";s:8:"guest_id";s:8:"22691145";s:11:"login_email";s:21:"wida.skydev@gmail.com";s:5:"token";s:40:"f9b29ac359ca5d77755e7588751c089bf96f0dc9";}
```

This API is used to get the UID number for searching specific place. You can put country ID parameter to list the province, and then put province ID to list the city, and then on area search you can get URL of area searching to be hit.

#### Http Request
    `GET http://api-sandbox.tiket.com/search/search_area?uid=city:178&token=f9b29ac359ca5d77755e7588751c089bf96f0dc9`

#### Parameters

Name | Description | Example  
---- | ----------  | -------   
UID | Id |  country |  province |  city |  kecamatan | Country:id |  Province:17 | Jika diberikan country:id maka akan menampilkan semua province di country indonesia  
Type | Tipe yang mau dicari |  Province |  city |  kecamatan |  Jika diberikan value province akan memberikan list province dengan keyword yang diberikan  
Q |  Keyword |  Jakarta |  Akan kenampilkan list city yang mengandung kata jakarta


## Search Autocomplete

```xml
<?xml version="1.0" encoding="utf-8"?>
<tiket>
    <diagnostic>
        <status>200</status>
        <elapsetime>15.1124</elapsetime>
        <memoryusage>5.6MB</memoryusage>
        <unix_timestamp>1470378201</unix_timestamp>
        <confirm>success</confirm>
        <lang>id</lang>
        <currency>IDR</currency>
    </diagnostic>
    <output_type>xml</output_type>
    <results>
        <result>
            <id>city:18119</id>
            <weight>7000535</weight>
            <distance>17910874.000000</distance>
            <skey>2.558501</skey>
            <country_id>mx</country_id>
            <label>Mahahual, Mexico  (1 Hotels)</label>
            <value>Mahahual</value>
            <category>Kota</category>
            <tipe>city_id</tipe>
            <business_uri>https://api-sandbox.tiket.com/hotel/indonesia/dki-jakarta/dki-jakarta/starbuck-coffee-40?uid=business%3A18119</business_uri>
        </result>
        <result>
            <id>city:17218</id>
            <weight>7000535</weight>
            <distance>16103025.000000</distance>
            <skey>2.300256</skey>
            <country_id>us</country_id>
            <label>Mahopac, United States  (1 Hotels)</label>
            <value>Mahopac</value>
            <category>Kota</category>
            <tipe>city_id</tipe>
            <business_uri></business_uri>
        </result>
        <result>
            <id>city:4414</id>
            <weight>7000535</weight>
            <distance>16131202.000000</distance>
            <skey>2.304281</skey>
            <country_id>us</country_id>
            <label>Mahwah, United States  (6 Hotels)</label>
            <value>Mahwah</value>
            <category>Kota</category>
            <tipe>city_id</tipe>
            <business_uri></business_uri>
        </result>
        <result>
            <id>city:18507</id>
            <weight>7000535</weight>
            <distance>15938149.000000</distance>
            <skey>2.276704</skey>
            <country_id>us</country_id>
            <label>Mahomet, United States  (1 Hotels)</label>
            <value>Mahomet</value>
            <category>Kota</category>
            <tipe>city_id</tipe>
            <business_uri>https://api-sandbox.tiket.com/hotel/indonesia/bali/bali/tepi-sawah-restaurant?uid=business%3A18507</business_uri>
        </result>
        <result>
            <id>province:10527</id>
            <weight>70527</weight>
            <distance>3609785.250000</distance>
            <skey>51.183025</skey>
            <country_id>in</country_id>
            <label>Mahabalipuram, India  (11 Hotels)</label>
            <value>Mahabalipuram</value>
            <category>Propinsi</category>
            <tipe>province_id</tipe>
            <business_uri>https://api-sandbox.tiket.com/?uid=business%3A10527</business_uri>
        </result>
        <result>
            <id>business:3874</id>
            <weight>40527</weight>
            <distance>7285.838867</distance>
            <skey>0.179777</skey>
            <country_id>id</country_id>
            <label>Maharadja Hotel (Jakarta Selatan, Mampang)</label>
            <value>Maharadja Hotel</value>
            <category>Recomended Hotel</category>
            <tipe>business_id</tipe>
            <business_uri>https://api-sandbox.tiket.com/hotel/indonesia/jakarta-selatan/mampang/maharadja-hotel?uid=business%3A3874</business_uri>
        </result>
        <result>
            <id>business:3852</id>
            <weight>40527</weight>
            <distance>7546.383301</distance>
            <skey>0.186206</skey>
            <country_id>id</country_id>
            <label>Maharani Hotel Jakarta (Jakarta Selatan, Mampang)</label>
            <value>Maharani Hotel Jakarta</value>
            <category>Recomended Hotel</category>
            <tipe>business_id</tipe>
            <business_uri>https://api-sandbox.tiket.com/hotel/indonesia/jakarta-selatan/mampang/maharani-hotel-jakarta?uid=business%3A3852</business_uri>
        </result>
        <result>
            <id>business:21058704</id>
            <weight>40527</weight>
            <distance>844112.437500</distance>
            <skey>20.828398</skey>
            <country_id>id</country_id>
            <label>Mahkota Hotel (Banyuwangi, Genteng)</label>
            <value>Mahkota Hotel</value>
            <category>Recomended Hotel</category>
            <tipe>business_id</tipe>
            <business_uri>https://api-sandbox.tiket.com/hotel/indonesia/banyuwangi/genteng/mahkota-hotel?uid=business%3A21058704</business_uri>
        </result>
        <result>
            <id>business:19935917</id>
            <weight>40527</weight>
            <distance>959587.812500</distance>
            <skey>23.677742</skey>
            <country_id>id</country_id>
            <label>Mahala Hasa Villas Seminyak (Bali, Seminyak)</label>
            <value>Mahala Hasa Villas Seminyak</value>
            <category>Recomended Hotel</category>
            <tipe>business_id</tipe>
            <business_uri>https://api-sandbox.tiket.com/hotel/indonesia/bali/seminyak/mahala-hasa-villas-seminyak?uid=business%3A19935917</business_uri>
        </result>
    </results>
    <login_status>true</login_status>
    <guest_id>22691145</guest_id>
    <login_email>wida.skydev@gmail.com</login_email>
    <token>f9b29ac359ca5d77755e7588751c089bf96f0dc9</token>
</tiket>

```

```json
{
  "diagnostic": {
    "status": "200",
    "elapsetime": "15.1152",
    "memoryusage": "5.59MB",
    "unix_timestamp": 1470378057,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "results": {
    "result": [
      {
        "id": "city:18119",
        "weight": "7000535",
        "distance": "17910874.000000",
        "skey": "2.558501",
        "country_id": "mx",
        "label": "Mahahual, Mexico  (1 Hotels)",
        "value": "Mahahual",
        "category": "Kota",
        "tipe": "city_id",
        "business_uri": "https://api-sandbox.tiket.com/hotel/indonesia/dki-jakarta/dki-jakarta/starbuck-coffee-40?uid=business%3A18119"
      },
      {
        "id": "city:17218",
        "weight": "7000535",
        "distance": "16103025.000000",
        "skey": "2.300256",
        "country_id": "us",
        "label": "Mahopac, United States  (1 Hotels)",
        "value": "Mahopac",
        "category": "Kota",
        "tipe": "city_id",
        "business_uri": ""
      },
      {
        "id": "city:4414",
        "weight": "7000535",
        "distance": "16131202.000000",
        "skey": "2.304281",
        "country_id": "us",
        "label": "Mahwah, United States  (6 Hotels)",
        "value": "Mahwah",
        "category": "Kota",
        "tipe": "city_id",
        "business_uri": ""
      },
      {
        "id": "city:18507",
        "weight": "7000535",
        "distance": "15938149.000000",
        "skey": "2.276704",
        "country_id": "us",
        "label": "Mahomet, United States  (1 Hotels)",
        "value": "Mahomet",
        "category": "Kota",
        "tipe": "city_id",
        "business_uri": "https://api-sandbox.tiket.com/hotel/indonesia/bali/bali/tepi-sawah-restaurant?uid=business%3A18507"
      },
      {
        "id": "province:10527",
        "weight": "70527",
        "distance": "3609785.250000",
        "skey": "51.183025",
        "country_id": "in",
        "label": "Mahabalipuram, India  (11 Hotels)",
        "value": "Mahabalipuram",
        "category": "Propinsi",
        "tipe": "province_id",
        "business_uri": "https://api-sandbox.tiket.com/?uid=business%3A10527"
      },
      {
        "id": "business:3874",
        "weight": "40527",
        "distance": "7285.838867",
        "skey": "0.179777",
        "country_id": "id",
        "label": "Maharadja Hotel (Jakarta Selatan, Mampang)",
        "value": "Maharadja Hotel",
        "category": "Recomended Hotel",
        "tipe": "business_id",
        "business_uri": "https://api-sandbox.tiket.com/hotel/indonesia/jakarta-selatan/mampang/maharadja-hotel?uid=business%3A3874"
      },
      {
        "id": "business:3852",
        "weight": "40527",
        "distance": "7546.383301",
        "skey": "0.186206",
        "country_id": "id",
        "label": "Maharani Hotel Jakarta (Jakarta Selatan, Mampang)",
        "value": "Maharani Hotel Jakarta",
        "category": "Recomended Hotel",
        "tipe": "business_id",
        "business_uri": "https://api-sandbox.tiket.com/hotel/indonesia/jakarta-selatan/mampang/maharani-hotel-jakarta?uid=business%3A3852"
      },
      {
        "id": "business:21058704",
        "weight": "40527",
        "distance": "844112.437500",
        "skey": "20.828398",
        "country_id": "id",
        "label": "Mahkota Hotel (Banyuwangi, Genteng)",
        "value": "Mahkota Hotel",
        "category": "Recomended Hotel",
        "tipe": "business_id",
        "business_uri": "https://api-sandbox.tiket.com/hotel/indonesia/banyuwangi/genteng/mahkota-hotel?uid=business%3A21058704"
      },
      {
        "id": "business:19935917",
        "weight": "40527",
        "distance": "959587.812500",
        "skey": "23.677742",
        "country_id": "id",
        "label": "Mahala Hasa Villas Seminyak (Bali, Seminyak)",
        "value": "Mahala Hasa Villas Seminyak",
        "category": "Recomended Hotel",
        "tipe": "business_id",
        "business_uri": "https://api-sandbox.tiket.com/hotel/indonesia/bali/seminyak/mahala-hasa-villas-seminyak?uid=business%3A19935917"
      }
    ]
  },
  "login_status": "true",
  "guest_id": "22691145",
  "login_email": "wida.skydev@gmail.com",
  "token": "f9b29ac359ca5d77755e7588751c089bf96f0dc9"
}

```

```matlab
a:7:{s:10:"diagnostic";a:7:{s:6:"status";s:3:"200";s:10:"elapsetime";s:14:"15.1610";s:11:"memoryusage";s:14:"5.59MB";s:14:"unix_timestamp";i:1470378239;s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:11:"output_type";s:9:"serialize";s:7:"results";a:1:{s:6:"result";a:9:{i:0;a:10:{s:2:"id";s:10:"city:18119";s:6:"weight";s:7:"7000535";s:8:"distance";s:15:"17910874.000000";s:4:"skey";s:8:"2.558501";s:10:"country_id";s:2:"mx";s:5:"label";s:28:"Mahahual, Mexico  (1 Hotels)";s:5:"value";s:8:"Mahahual";s:8:"category";s:13:"Kota";s:4:"tipe";s:7:"city_id";s:12:"business_uri";s:109:"https://api-sandbox.tiket.com/hotel/indonesia/dki-jakarta/dki-jakarta/starbuck-coffee-40?uid=business%3A18119";}i:1;a:10:{s:2:"id";s:10:"city:17218";s:6:"weight";s:7:"7000535";s:8:"distance";s:15:"16103025.000000";s:4:"skey";s:8:"2.300256";s:10:"country_id";s:2:"us";s:5:"label";s:34:"Mahopac, United States  (1 Hotels)";s:5:"value";s:7:"Mahopac";s:8:"category";s:13:"Kota";s:4:"tipe";s:7:"city_id";s:12:"business_uri";s:0:"";}i:2;a:10:{s:2:"id";s:9:"city:4414";s:6:"weight";s:7:"7000535";s:8:"distance";s:15:"16131202.000000";s:4:"skey";s:8:"2.304281";s:10:"country_id";s:2:"us";s:5:"label";s:33:"Mahwah, United States  (6 Hotels)";s:5:"value";s:6:"Mahwah";s:8:"category";s:13:"Kota";s:4:"tipe";s:7:"city_id";s:12:"business_uri";s:0:"";}i:3;a:10:{s:2:"id";s:10:"city:18507";s:6:"weight";s:7:"7000535";s:8:"distance";s:15:"15938149.000000";s:4:"skey";s:8:"2.276704";s:10:"country_id";s:2:"us";s:5:"label";s:34:"Mahomet, United States  (1 Hotels)";s:5:"value";s:7:"Mahomet";s:8:"category";s:13:"Kota";s:4:"tipe";s:7:"city_id";s:12:"business_uri";s:98:"https://api-sandbox.tiket.com/hotel/indonesia/bali/bali/tepi-sawah-restaurant?uid=business%3A18507";}i:4;a:10:{s:2:"id";s:14:"province:10527";s:6:"weight";s:5:"70527";s:8:"distance";s:14:"3609785.250000";s:4:"skey";s:9:"51.183025";s:10:"country_id";s:2:"in";s:5:"label";s:33:"Mahabalipuram, India  (11 Hotels)";s:5:"value";s:13:"Mahabalipuram";s:8:"category";s:17:"Propinsi";s:4:"tipe";s:11:"province_id";s:12:"business_uri";s:51:"https://api-sandbox.tiket.com/?uid=business%3A10527";}i:5;a:10:{s:2:"id";s:13:"business:3874";s:6:"weight";s:5:"40527";s:8:"distance";s:11:"7285.838867";s:4:"skey";s:8:"0.179777";s:10:"country_id";s:2:"id";s:5:"label";s:42:"Maharadja Hotel (Jakarta Selatan, Mampang)";s:5:"value";s:15:"Maharadja Hotel";s:8:"category";s:25:"Recomended Hotel";s:4:"tipe";s:11:"business_id";s:12:"business_uri";s:105:"https://api-sandbox.tiket.com/hotel/indonesia/jakarta-selatan/mampang/maharadja-hotel?uid=business%3A3874";}i:6;a:10:{s:2:"id";s:13:"business:3852";s:6:"weight";s:5:"40527";s:8:"distance";s:11:"7546.383301";s:4:"skey";s:8:"0.186206";s:10:"country_id";s:2:"id";s:5:"label";s:49:"Maharani Hotel Jakarta (Jakarta Selatan, Mampang)";s:5:"value";s:22:"Maharani Hotel Jakarta";s:8:"category";s:25:"Recomended Hotel";s:4:"tipe";s:11:"business_id";s:12:"business_uri";s:112:"https://api-sandbox.tiket.com/hotel/indonesia/jakarta-selatan/mampang/maharani-hotel-jakarta?uid=business%3A3852";}i:7;a:10:{s:2:"id";s:17:"business:21058704";s:6:"weight";s:5:"40527";s:8:"distance";s:13:"844112.437500";s:4:"skey";s:9:"20.828398";s:10:"country_id";s:2:"id";s:5:"label";s:35:"Mahkota Hotel (Banyuwangi, Genteng)";s:5:"value";s:13:"Mahkota Hotel";s:8:"category";s:25:"Recomended Hotel";s:4:"tipe";s:11:"business_id";s:12:"business_uri";s:102:"https://api-sandbox.tiket.com/hotel/indonesia/banyuwangi/genteng/mahkota-hotel?uid=business%3A21058704";}i:8;a:10:{s:2:"id";s:17:"business:19935917";s:6:"weight";s:5:"40527";s:8:"distance";s:13:"959587.812500";s:4:"skey";s:9:"23.677742";s:10:"country_id";s:2:"id";s:5:"label";s:44:"Mahala Hasa Villas Seminyak (Bali, Seminyak)";s:5:"value";s:27:"Mahala Hasa Villas Seminyak";s:8:"category";s:25:"Recomended Hotel";s:4:"tipe";s:11:"business_id";s:12:"business_uri";s:111:"https://api-sandbox.tiket.com/hotel/indonesia/bali/seminyak/mahala-hasa-villas-seminyak?uid=business%3A19935917";}}}s:12:"login_status";s:4:"true";s:8:"guest_id";s:8:"22691145";s:11:"login_email";s:21:"wida.skydev@gmail.com";s:5:"token";s:40:"f9b29ac359ca5d77755e7588751c089bf96f0dc9";}

```

#### HTTP Request

    `GET https://api-sandbox.tiket.com/search/autocomplete/hotel?q=mah&token=90d2fad44172390b11527557e6250e50&output=json`

#### Parameters

REMINDER : In development environment, please use "The Sunset Hotel and Restaurant" on Legian-Bali, as test bed hotel to search and order since it's almost always have an room allotment this respective year. Ordering another hotel may produce more error in development server.
  
Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------  
q | Keyword (hotel name / location ) | CHAR (50) |  | TRUE  
token | for saving transaction that done by user | CHAR(128) |  | TRUE
 

## View Detail Hotel

```xml
<?xml version="1.0" encoding="utf-8"?>
<tiket>
    <diagnostic>
        <status>200</status>
        <elapsetime>15.9417</elapsetime>
        <memoryusage>8MB</memoryusage>
        <unix_timestamp>1470379580</unix_timestamp>
        <confirm>success</confirm>
        <lang>id</lang>
        <currency>IDR</currency>
    </diagnostic>
    <output_type>xml</output_type>
    <primaryPhotos>http://api-sandbox.tiket.com/img/business/s/i/business-single-room-12.s.jpg</primaryPhotos>
    <breadcrumb>
        <business_id>15810</business_id>
        <business_uri>https://api-sandbox.tiket.com/the-edelweis-hotel-yogyakarta</business_uri>
        <business_name>The Edelweiss Hotel Yogyakarta</business_name>
        <area_id>87277</area_id>
        <area_name>Gejayan</area_name>
        <kelurahan_id>0</kelurahan_id>
        <kelurahan_name> </kelurahan_name>
        <kecamatan_id>317</kecamatan_id>
        <kecamatan_name>Gondokusuman</kecamatan_name>
        <city_id>257</city_id>
        <city_name>Yogyakarta</city_name>
        <province_id>16</province_id>
        <province_name>Daerah Istimewa Yogyakarta</province_name>
        <country_id>id</country_id>
        <country_name>Indonesia</country_name>
        <continent_id>1</continent_id>
        <continent_name>Asia</continent_name>
        <kelurahan_uri>https://api-sandbox.tiket.com/search/hotel?uid=city:257</kelurahan_uri>
        <kecamatan_uri>https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:317</kecamatan_uri>
        <province_uri>https://api-sandbox.tiket.com/search/hotel?uid=province:16</province_uri>
        <country_uri>https://api-sandbox.tiket.com/search/hotel?uid=country:id</country_uri>
        <continent_uri>https://api-sandbox.tiket.com/search/hotel?uid=continent:1</continent_uri>
        <star_rating>3</star_rating>
    </breadcrumb>
    <results>
        <result>
            <id>62897320160811</id>
            <room_available>10</room_available>
            <ext_source>native</ext_source>
            <room_id>628973</room_id>
            <currency>IDR</currency>
            <minimum_stays>1</minimum_stays>
            <with_breakfasts>0</with_breakfasts>
            <all_photo_room>http://api-sandbox.tiket.com/img/default/d/e/default-default.room.jpg</all_photo_room>
            <photo_url>http://api-sandbox.tiket.com/img/default/d/e/default-default.s.jpg</photo_url>
            <room_name>Superior Room Only</room_name>
            <oldprice>690525.00</oldprice>
            <price>375000.00</price>
            <bookUri>https://api-sandbox.tiket.com/order/add/hotel?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;minstar=0&amp;maxstar=0&amp;minprice=0&amp;maxprice=0&amp;facilities=0&amp;locations=0&amp;hotelname=0&amp;is_partner=0&amp;room_id=628973&amp;hasPromo=0&amp;enddate=2016-08-12&amp;room_max_occupancy=2</bookUri>
            <room_description></room_description>
            <additional_surcharge_currency></additional_surcharge_currency>
        </result>
        <result>
            <id>107720160811</id>
            <room_available>20</room_available>
            <ext_source>native</ext_source>
            <room_id>1077</room_id>
            <currency>IDR</currency>
            <minimum_stays>1</minimum_stays>
            <with_breakfasts>1</with_breakfasts>
            <all_photo_room>http://api-sandbox.tiket.com/img/business/s/i/business-single-room-1.room.jpg</all_photo_room>
            <all_photo_room>http://api-sandbox.tiket.com/img/business/s/u/business-suites_1_copy.room.jpg</all_photo_room>
            <all_photo_room>http://api-sandbox.tiket.com/img/business/s/u/business-suites_2a.room.jpg</all_photo_room>
            <all_photo_room>http://api-sandbox.tiket.com/img/business/t/w/business-twice_room_2.room.jpg</all_photo_room>
            <all_photo_room>http://api-sandbox.tiket.com/img/business/t/w/business-twice-room-1.room.jpg</all_photo_room>
            <photo_url>http://api-sandbox.tiket.com/img/business/s/i/business-single-room-1.s.jpg</photo_url>
            <room_name>Superior Room</room_name>
            <oldprice>782595.00</oldprice>
            <price>425000.00</price>
            <bookUri>https://api-sandbox.tiket.com/order/add/hotel?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;minstar=0&amp;maxstar=0&amp;minprice=0&amp;maxprice=0&amp;facilities=0&amp;locations=0&amp;hotelname=0&amp;is_partner=0&amp;room_id=1077&amp;hasPromo=0&amp;enddate=2016-08-12&amp;room_max_occupancy=2</bookUri>
            <room_facility>AC</room_facility>
            <room_facility>Mesin pembuat kopi/teh</room_facility>
            <room_facility>Air mineral botol gratis</room_facility>
            <room_facility>Internet - Wifi (gratis)</room_facility>
            <room_facility>Televisi LCD/layar plasma</room_facility>
            <room_facility>Cermin</room_facility>
            <room_facility>Kulkas</room_facility>
            <room_facility>Satelit/TV kabel</room_facility>
            <room_facility>Shower</room_facility>
            <room_facility>Sandal</room_facility>
            <room_facility>Telepon</room_facility>
            <room_description></room_description>
            <additional_surcharge_currency></additional_surcharge_currency>
        </result>
        <result>
            <id>WSMA0511003520160811</id>
            <room_available>1</room_available>
            <room_id>498707</room_id>
            <currency>IDR</currency>
            <minimum_stays>1</minimum_stays>
            <with_breakfasts>1</with_breakfasts>
            <ext_source>mgholiday</ext_source>
            <refund_policy>You have to cancel 4 day(s) prior to the arrival date. Otherwise 100 % cancellation charge for the entire stay will be applied.</refund_policy>
            <all_photo_room>http://api-sandbox.tiket.com/img/default/d/e/default-default.room.jpg</all_photo_room>
            <photo_url>http://api-sandbox.tiket.com/img/default/d/e/default-default.s.jpg</photo_url>
            <room_name>Superior (Twin) </room_name>
            <promo_title>Hanya untuk KTP/KITAS</promo_title>
            <value_added></value_added>
            <price>534483.00</price>
            <bookUri>https://api-sandbox.tiket.com/order/add/hotel?startdate=2016-08-11&amp;night=1&amp;room=1&amp;adult=2&amp;child=0&amp;minstar=0&amp;maxstar=0&amp;minprice=0&amp;maxprice=0&amp;facilities=0&amp;locations=0&amp;hotelname=0&amp;is_partner=0&amp;room_id=498707&amp;hasPromo=1&amp;enddate=2016-08-12&amp;room_max_occupancy=2&amp;breakfast=BABF</bookUri>
            <room_description>SUPERIOR</room_description>
            <additional_surcharge_currency></additional_surcharge_currency>
        </result>
    </results>
    <addinfos>
        <addinfo>Biaya makan pagi (jika tidak temasuk dalam harga kamar) : IDR 48.400,00</addinfo>
        <addinfo>Checkout : 12:00</addinfo>
        <addinfo>Jumlah Restoran : 1</addinfo>
        <addinfo>Voltase ruangan : 220 V</addinfo>
        <addinfo>Waktu untuk sampai di bandara : 20 menit</addinfo>
        <addinfo>Tahun hotel dibangun : 2011</addinfo>
    </addinfos>
    <all_photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/2/0/business-2014-04-29_16.25-.00-.s.jpg</file_name>
            <photo_type>Kolam Renang</photo_type>
        </photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/r/o/business-room_queen_-312x234-1.s.jpg</file_name>
            <photo_type>Kamar Tamu</photo_type>
        </photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/r/o/business-room_queena.s.jpg</file_name>
            <photo_type>Kamar Tamu</photo_type>
        </photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/s/i/business-single_room_1_-312x234-.s.jpg</file_name>
            <photo_type>Kamar Tamu</photo_type>
        </photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/s/i/business-single_room_1_-312x234-1.s.jpg</file_name>
            <photo_type>Kamar Tamu</photo_type>
        </photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/s/i/business-single-room-12.s.jpg</file_name>
            <photo_type>Kamar Tamu</photo_type>
        </photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/s/u/business-sup111.s.jpg</file_name>
            <photo_type>Kamar Tamu</photo_type>
        </photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/t/h/business-the_edelweiss_hotel-16.s.jpg</file_name>
            <photo_type>Interior</photo_type>
        </photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/t/t/business-ttwice_room_1.s.jpg</file_name>
            <photo_type>Kamar Tamu</photo_type>
        </photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/t/w/business-twice_room_1_-312x234-.s.jpg</file_name>
            <photo_type>Interior</photo_type>
        </photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/r/o/business-room_queen_-312x234-.s.jpg</file_name>
            <photo_type>Kamar Tamu</photo_type>
        </photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/r/e/business-resto78.s.jpg</file_name>
            <photo_type>Rumah Makan</photo_type>
        </photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/q/u/business-queen_staff_2_-312x234-2.s.jpg</file_name>
            <photo_type>Kamar Tamu</photo_type>
        </photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/3/1/business-312x234.s.jpg</file_name>
            <photo_type>Kamar Tamu</photo_type>
        </photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/9/3/business-93.s.jpg</file_name>
            <photo_type>Makanan</photo_type>
        </photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/9/3/business-931.s.jpg</file_name>
            <photo_type>Makanan</photo_type>
        </photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/b/u/business-business_center_a1.s.jpg</file_name>
            <photo_type>Pusat Bisnis</photo_type>
        </photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/e/i/business-eight_bar_-312x234-1.s.jpg</file_name>
            <photo_type>Kolam Renang</photo_type>
        </photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/f/a/business-facade_31.s.jpg</file_name>
            <photo_type>Pintu Masuk</photo_type>
        </photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/f/o/business-food_-312x234-.s.jpg</file_name>
            <photo_type>Makanan</photo_type>
        </photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/j/u/business-junior_suite_lr.s.jpg</file_name>
            <photo_type>Kamar Tamu</photo_type>
        </photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/k/u/business-kursi_-312x234-.s.jpg</file_name>
            <photo_type>Interior</photo_type>
        </photo>
        <photo>
            <file_name>http://api-sandbox.tiket.com/img/business/t/w/business-twice_room_2_-312x234-.s.jpg</file_name>
            <photo_type>Kamar Tamu</photo_type>
        </photo>
    </all_photo>
    <primaryPhotos_large>http://api-sandbox.tiket.com/img/business/s/i/business-single-room-12.crop.jpg</primaryPhotos_large>
    <avail_facilities>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Layanan Kamar 24 Jam</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Antar Jemput Bandara Dikenakan Biaya</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Bar</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Pusat Bisnis</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Tempat Parkir</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Kedai Kopi</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Staf Pribadi</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Penjaga Pintu</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Kotak Penyimpanan Barang Berharga</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Layanan Dokter 24 Jam</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Lift</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Gratis Wifi di lounge</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Gratis Wifi di kamar</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Lounge</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Bagasi Penyimpanan</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Fasilitas Rapat</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Bar Disamping Kolam Renang</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Rumah Makan</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Bar di atas gedung</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Layanan Kamar</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Kamar merokok ada tergantung ketersediaan</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Informasi Tour</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Layanan Parkir oleh Pelayan</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Wi-Fi area umum</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Wifi di Kamar</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>24-hour Front Desk </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Air-conditioned Public Areas </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Banquet Facilities </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Bar/lounge </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Complimentary Newspapers In Lobby  </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Elevator/lift </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Express Check- In </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Express Check-out </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Laundry Facilities </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Luggage Storage </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Poolside Bar </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Restaurant(s) In Hotel </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Room Service </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>hotel</facility_type>
            <facility_name>Room Service (24 Hours) </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>AC</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Mesin pembuat kopi/teh</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Air mineral botol gratis</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Shower Panas and Dingin</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Brankas</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Internet - Wifi (gratis)</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Televisi LCD/layar plasma</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Bar kecil</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Cermin</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Kamar bebas rokok ada tergantung ketersediaan</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Kulkas</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Satelit/TV kabel</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Shower</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Sandal</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Telepon</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Televisi</facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Air Conditioning </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Cable TV Service </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>City View </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Coffee/tea Maker </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Complimentary Bottled Water </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Complimentary Toiletries </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Connecting / Adjoining Rooms Available </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Daily Housekeeping </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Desk </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Free Wi-Fi </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Hair Dryer (on Request) </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>In-room Safe </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Makeup/shaving Mirror </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Minibar </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Satellite TV Service </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Slippers </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Wake-up Calls </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>room</facility_type>
            <facility_name>Wireless Internet Access </facility_name>
        </avail_facilitiy>
        <avail_facilitiy>
            <facility_type>sport</facility_type>
            <facility_name>Kolam Renang di Luar Ruangan</facility_name>
        </avail_facilitiy>
    </avail_facilities>
    <nearby_attractions>
        <nearby_attraction>
            <distance>220</distance>
            <business_primary_photo>http://api-sandbox.tiket.com/img/business/p/a/business-pancake-tiramisu-topping-ice-cream-vanilla-dixie2.s.jpg</business_primary_photo>
            <business_name>Dixie Easy Dinning</business_name>
            <business_uri>https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-dixie-easy-dinning-2</business_uri>
        </nearby_attraction>
        <nearby_attraction>
            <distance>608</distance>
            <business_primary_photo>http://api-sandbox.tiket.com/img/business/l/a/business-lana.s.jpg</business_primary_photo>
            <business_name>Lana Gallery</business_name>
            <business_uri>https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-lana-gallery</business_uri>
        </nearby_attraction>
        <nearby_attraction>
            <distance>955</distance>
            <business_primary_photo>http://api-sandbox.tiket.com/img/business/a/f/business-affandi_galeri_1.s.jpg</business_primary_photo>
            <business_name>Museum Affandi</business_name>
            <business_uri>https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-museum-affandi</business_uri>
        </nearby_attraction>
        <nearby_attraction>
            <distance>1560</distance>
            <business_primary_photo>http://api-sandbox.tiket.com/img/business/t/1/business-t144.s.jpg</business_primary_photo>
            <business_name>Telkom Office</business_name>
            <business_uri>https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-telkom-office</business_uri>
        </nearby_attraction>
        <nearby_attraction>
            <distance>1594</distance>
            <business_primary_photo>http://api-sandbox.tiket.com/img/business/4/4/business-44737073.s.jpg</business_primary_photo>
            <business_name>Kridosono Stadium</business_name>
            <business_uri>https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-kridosono-stadium</business_uri>
        </nearby_attraction>
        <nearby_attraction>
            <distance>1674</distance>
            <business_primary_photo>http://api-sandbox.tiket.com/img/business/t/2/business-t242.s.jpg</business_primary_photo>
            <business_name>Kotabaru</business_name>
            <business_uri>https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-kotabaru-poi</business_uri>
        </nearby_attraction>
        <nearby_attraction>
            <distance>1694</distance>
            <business_primary_photo>http://api-sandbox.tiket.com/img/business/l/e/business-lempuyangan.s.jpg</business_primary_photo>
            <business_name>Lempuyangan Railway station</business_name>
            <business_uri>https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-lempuyangan-railway-station</business_uri>
        </nearby_attraction>
        <nearby_attraction>
            <distance>1839</distance>
            <business_primary_photo>http://api-sandbox.tiket.com/img/business/r/a/business-raminten-21.s.jpg</business_primary_photo>
            <business_name>Raminten</business_name>
            <business_uri>https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-raminten</business_uri>
        </nearby_attraction>
        <nearby_attraction>
            <distance>1879</distance>
            <business_primary_photo>http://api-sandbox.tiket.com/img/business/t/1/business-t160.s.jpg</business_primary_photo>
            <business_name>Rumah Sakit Soedirman</business_name>
            <business_uri>https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-rumah-sakit-soedirman</business_uri>
        </nearby_attraction>
        <nearby_attraction>
            <distance>1945</distance>
            <business_primary_photo>http://api-sandbox.tiket.com/img/business/t/3/business-t337.s.jpg</business_primary_photo>
            <business_name>Museum Batik</business_name>
            <business_uri>https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-museum-batik</business_uri>
        </nearby_attraction>
        <nearby_attraction>
            <distance>2222</distance>
            <business_primary_photo>http://api-sandbox.tiket.com/img/business/u/s/business-usd.s.jpg</business_primary_photo>
            <business_name>Sanata Darma University</business_name>
            <business_uri>https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-sanata-darma-university</business_uri>
        </nearby_attraction>
    </nearby_attractions>
    <general>
        <address>Jl. Gejayan 17C, Gondokusuman, Yogyakarta</address>
        <description>The+Edelweiss+Hotel+Yogyakarta+berada+di+dalam+pusat+bisnis+dikota+Yogyakarta%2C+dekat+dengan+lingkungan+universitas+dan+distrik+perbelanjaan+di+sepanjang+jalan-jalan+yang+ramai+Jalan+Gejayan.+Lokasi+ini+menempatkan+pusat+perbelanjaan+besar+hanya+menit+dan+juga+15+menit+berkendara+ke+Bandara+Internasional+Yogyakarta.%3Cbr+%2F%3E%0A%3Cbr+%2F%3E%0A+Hotel+ini+menawarkan+95+kamar+dengan+desain+minimalis+modern+untuk+memperbaharui+dan+menginspirasi+Anda.+Akses+internet+berkecepatan+tinggi%2C+baik+kamar+yang+berkualitas+baik%2C+matrass+delightly+disediakan+untuk+layanan+bagi+para+pengunjung+yang+datang+ketempat+ini.%3Cbr+%2F%3E%0A%3Cbr+%2F%3E%0AFasilitas+terbaik+hotel+ini+termasuk+wi-fi+di+tempat-tempat+umum%2C+tempat+parkir+mobil%2C+layanan+laundry%2Fdry+cleaning%2C+restoran%2C+and+concierge.+Suasana+The+Edelweiss+Hotel+tercerminkan+dari+setiap+kamar+tamu.+kulkas%2C+kotak+penyimpanan+dalam-kamar%2C+TV+satelit%2Fkabel%2C+internet+wireless+%28gratis%29%2C+AC.</description>
        <latitude>-7.7816262945693</latitude>
        <longitude>110.38782497907</longitude>
    </general>
    <login_status>true</login_status>
    <guest_id>22691145</guest_id>
    <login_email>wida.skydev@gmail.com</login_email>
    <token>f9b29ac359ca5d77755e7588751c089bf96f0dc9</token>
</tiket>
```

```json
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "15.8781",
    "memoryusage": "7.98MB",
    "unix_timestamp": 1470379403,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "primaryPhotos": "http://api-sandbox.tiket.com/img/business/s/i/business-single-room-12.s.jpg",
  "breadcrumb": {
    "business_id": "15810",
    "business_uri": "https://api-sandbox.tiket.com/the-edelweis-hotel-yogyakarta",
    "business_name": "The Edelweiss Hotel Yogyakarta",
    "area_id": "87277",
    "area_name": "Gejayan",
    "kelurahan_id": "0",
    "kelurahan_name": " ",
    "kecamatan_id": "317",
    "kecamatan_name": "Gondokusuman",
    "city_id": "257",
    "city_name": "Yogyakarta",
    "province_id": "16",
    "province_name": "Daerah Istimewa Yogyakarta",
    "country_id": "id",
    "country_name": "Indonesia",
    "continent_id": "1",
    "continent_name": "Asia",
    "kelurahan_uri": "https://api-sandbox.tiket.com/search/hotel?uid=city:257",
    "kecamatan_uri": "https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:317",
    "province_uri": "https://api-sandbox.tiket.com/search/hotel?uid=province:16",
    "country_uri": "https://api-sandbox.tiket.com/search/hotel?uid=country:id",
    "continent_uri": "https://api-sandbox.tiket.com/search/hotel?uid=continent:1",
    "star_rating": "3"
  },
  "results": {
    "result": [
      {
        "id": "62897320160811",
        "room_available": "10",
        "ext_source": "native",
        "room_id": "628973",
        "currency": "IDR",
        "minimum_stays": "1",
        "with_breakfasts": "0",
        "all_photo_room": [
          "http://api-sandbox.tiket.com/img/default/d/e/default-default.room.jpg"
        ],
        "photo_url": "http://api-sandbox.tiket.com/img/default/d/e/default-default.s.jpg",
        "room_name": "Superior Room Only",
        "oldprice": "690525.00",
        "price": "375000.00",
        "bookUri": "https://api-sandbox.tiket.com/order/add/hotel?startdate=2016-08-11&night=1&room=1&adult=2&child=0&minstar=0&maxstar=0&minprice=0&maxprice=0&facilities=0&locations=0&hotelname=0&is_partner=0&room_id=628973&hasPromo=0&enddate=2016-08-12&room_max_occupancy=2",
        "room_facility": [],
        "room_description": false,
        "additional_surcharge_currency": ""
      },
      {
        "id": "107720160811",
        "room_available": "20",
        "ext_source": "native",
        "room_id": "1077",
        "currency": "IDR",
        "minimum_stays": "1",
        "with_breakfasts": "1",
        "all_photo_room": [
          "http://api-sandbox.tiket.com/img/business/s/i/business-single-room-1.room.jpg",
          "http://api-sandbox.tiket.com/img/business/s/u/business-suites_1_copy.room.jpg",
          "http://api-sandbox.tiket.com/img/business/s/u/business-suites_2a.room.jpg",
          "http://api-sandbox.tiket.com/img/business/t/w/business-twice_room_2.room.jpg",
          "http://api-sandbox.tiket.com/img/business/t/w/business-twice-room-1.room.jpg"
        ],
        "photo_url": "http://api-sandbox.tiket.com/img/business/s/i/business-single-room-1.s.jpg",
        "room_name": "Superior Room",
        "oldprice": "782595.00",
        "price": "425000.00",
        "bookUri": "https://api-sandbox.tiket.com/order/add/hotel?startdate=2016-08-11&night=1&room=1&adult=2&child=0&minstar=0&maxstar=0&minprice=0&maxprice=0&facilities=0&locations=0&hotelname=0&is_partner=0&room_id=1077&hasPromo=0&enddate=2016-08-12&room_max_occupancy=2",
        "room_facility": [
          "AC",
          "Mesin pembuat kopi/teh",
          "Air mineral botol gratis",
          "Internet - Wifi (gratis)",
          "Televisi LCD/layar plasma",
          "Cermin",
          "Kulkas",
          "Satelit/TV kabel",
          "Shower",
          "Sandal",
          "Telepon"
        ],
        "room_description": false,
        "additional_surcharge_currency": ""
      },
      {
        "id": "WSMA0511003520160811",
        "room_available": "1",
        "room_id": "498707",
        "currency": "IDR",
        "minimum_stays": 1,
        "with_breakfasts": 1,
        "ext_source": "mgholiday",
        "refund_policy": "You have to cancel 4 day(s) prior to the arrival date. Otherwise 100 % cancellation charge for the entire stay will be applied.",
        "all_photo_room": [
          "http://api-sandbox.tiket.com/img/default/d/e/default-default.room.jpg"
        ],
        "photo_url": "http://api-sandbox.tiket.com/img/default/d/e/default-default.s.jpg",
        "room_name": "Superior (Twin) ",
        "promo_title": "Hanya untuk KTP/KITAS",
        "value_added": "",
        "price": "534483.00",
        "bookUri": "https://api-sandbox.tiket.com/order/add/hotel?startdate=2016-08-11&night=1&room=1&adult=2&child=0&minstar=0&maxstar=0&minprice=0&maxprice=0&facilities=0&locations=0&hotelname=0&is_partner=0&room_id=498707&hasPromo=1&enddate=2016-08-12&room_max_occupancy=2&breakfast=BABF",
        "room_facility": [],
        "room_description": "SUPERIOR",
        "additional_surcharge_currency": ""
      }
    ]
  },
  "addinfos": {
    "addinfo": [
      "Biaya makan pagi (jika tidak temasuk dalam harga kamar) : IDR 48.400,00",
      "Checkout : 12:00",
      "Jumlah Restoran : 1",
      "Voltase ruangan : 220 V",
      "Waktu untuk sampai di bandara : 20 menit",
      "Tahun hotel dibangun : 2011"
    ]
  },
  "all_photo": {
    "photo": [
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/2/0/business-2014-04-29_16.25-.00-.s.jpg",
        "photo_type": "Kolam Renang"
      },
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/r/o/business-room_queen_-312x234-1.s.jpg",
        "photo_type": "Kamar Tamu"
      },
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/r/o/business-room_queena.s.jpg",
        "photo_type": "Kamar Tamu"
      },
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/s/i/business-single_room_1_-312x234-.s.jpg",
        "photo_type": "Kamar Tamu"
      },
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/s/i/business-single_room_1_-312x234-1.s.jpg",
        "photo_type": "Kamar Tamu"
      },
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/s/i/business-single-room-12.s.jpg",
        "photo_type": "Kamar Tamu"
      },
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/s/u/business-sup111.s.jpg",
        "photo_type": "Kamar Tamu"
      },
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/t/h/business-the_edelweiss_hotel-16.s.jpg",
        "photo_type": "Interior"
      },
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/t/t/business-ttwice_room_1.s.jpg",
        "photo_type": "Kamar Tamu"
      },
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/t/w/business-twice_room_1_-312x234-.s.jpg",
        "photo_type": "Interior"
      },
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/r/o/business-room_queen_-312x234-.s.jpg",
        "photo_type": "Kamar Tamu"
      },
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/r/e/business-resto78.s.jpg",
        "photo_type": "Rumah Makan"
      },
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/q/u/business-queen_staff_2_-312x234-2.s.jpg",
        "photo_type": "Kamar Tamu"
      },
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/3/1/business-312x234.s.jpg",
        "photo_type": "Kamar Tamu"
      },
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/9/3/business-93.s.jpg",
        "photo_type": "Makanan"
      },
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/9/3/business-931.s.jpg",
        "photo_type": "Makanan"
      },
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/b/u/business-business_center_a1.s.jpg",
        "photo_type": "Pusat Bisnis"
      },
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/e/i/business-eight_bar_-312x234-1.s.jpg",
        "photo_type": "Kolam Renang"
      },
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/f/a/business-facade_31.s.jpg",
        "photo_type": "Pintu Masuk"
      },
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/f/o/business-food_-312x234-.s.jpg",
        "photo_type": "Makanan"
      },
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/j/u/business-junior_suite_lr.s.jpg",
        "photo_type": "Kamar Tamu"
      },
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/k/u/business-kursi_-312x234-.s.jpg",
        "photo_type": "Interior"
      },
      {
        "file_name": "http://api-sandbox.tiket.com/img/business/t/w/business-twice_room_2_-312x234-.s.jpg",
        "photo_type": "Kamar Tamu"
      }
    ]
  },
  "primaryPhotos_large": "http://api-sandbox.tiket.com/img/business/s/i/business-single-room-12.crop.jpg",
  "avail_facilities": {
    "avail_facilitiy": [
      {
        "facility_type": "hotel",
        "facility_name": "Layanan Kamar 24 Jam"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Antar Jemput Bandara Dikenakan Biaya"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Bar"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Pusat Bisnis"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Tempat Parkir"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Kedai Kopi"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Staf Pribadi"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Penjaga Pintu"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Kotak Penyimpanan Barang Berharga"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Layanan Dokter 24 Jam"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Lift"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Gratis Wifi di lounge"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Gratis Wifi di kamar"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Lounge"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Bagasi Penyimpanan"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Fasilitas Rapat"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Bar Disamping Kolam Renang"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Rumah Makan"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Bar di atas gedung"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Layanan Kamar"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Kamar merokok ada tergantung ketersediaan"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Informasi Tour"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Layanan Parkir oleh Pelayan"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Wi-Fi area umum"
      },
      {
        "facility_type": "hotel",
        "facility_name": "Wifi di Kamar"
      },
      {
        "facility_type": "hotel",
        "facility_name": "24-hour Front Desk "
      },
      {
        "facility_type": "hotel",
        "facility_name": "Air-conditioned Public Areas "
      },
      {
        "facility_type": "hotel",
        "facility_name": "Banquet Facilities "
      },
      {
        "facility_type": "hotel",
        "facility_name": "Bar/lounge "
      },
      {
        "facility_type": "hotel",
        "facility_name": "Complimentary Newspapers In Lobby  "
      },
      {
        "facility_type": "hotel",
        "facility_name": "Elevator/lift "
      },
      {
        "facility_type": "hotel",
        "facility_name": "Express Check- In "
      },
      {
        "facility_type": "hotel",
        "facility_name": "Express Check-out "
      },
      {
        "facility_type": "hotel",
        "facility_name": "Laundry Facilities "
      },
      {
        "facility_type": "hotel",
        "facility_name": "Luggage Storage "
      },
      {
        "facility_type": "hotel",
        "facility_name": "Poolside Bar "
      },
      {
        "facility_type": "hotel",
        "facility_name": "Restaurant(s) In Hotel "
      },
      {
        "facility_type": "hotel",
        "facility_name": "Room Service "
      },
      {
        "facility_type": "hotel",
        "facility_name": "Room Service (24 Hours) "
      },
      {
        "facility_type": "room",
        "facility_name": "AC"
      },
      {
        "facility_type": "room",
        "facility_name": "Mesin pembuat kopi/teh"
      },
      {
        "facility_type": "room",
        "facility_name": "Air mineral botol gratis"
      },
      {
        "facility_type": "room",
        "facility_name": "Shower Panas and Dingin"
      },
      {
        "facility_type": "room",
        "facility_name": "Brankas"
      },
      {
        "facility_type": "room",
        "facility_name": "Internet - Wifi (gratis)"
      },
      {
        "facility_type": "room",
        "facility_name": "Televisi LCD/layar plasma"
      },
      {
        "facility_type": "room",
        "facility_name": "Bar kecil"
      },
      {
        "facility_type": "room",
        "facility_name": "Cermin"
      },
      {
        "facility_type": "room",
        "facility_name": "Kamar bebas rokok ada tergantung ketersediaan"
      },
      {
        "facility_type": "room",
        "facility_name": "Kulkas"
      },
      {
        "facility_type": "room",
        "facility_name": "Satelit/TV kabel"
      },
      {
        "facility_type": "room",
        "facility_name": "Shower"
      },
      {
        "facility_type": "room",
        "facility_name": "Sandal"
      },
      {
        "facility_type": "room",
        "facility_name": "Telepon"
      },
      {
        "facility_type": "room",
        "facility_name": "Televisi"
      },
      {
        "facility_type": "room",
        "facility_name": "Air Conditioning "
      },
      {
        "facility_type": "room",
        "facility_name": "Cable TV Service "
      },
      {
        "facility_type": "room",
        "facility_name": "City View "
      },
      {
        "facility_type": "room",
        "facility_name": "Coffee/tea Maker "
      },
      {
        "facility_type": "room",
        "facility_name": "Complimentary Bottled Water "
      },
      {
        "facility_type": "room",
        "facility_name": "Complimentary Toiletries "
      },
      {
        "facility_type": "room",
        "facility_name": "Connecting / Adjoining Rooms Available "
      },
      {
        "facility_type": "room",
        "facility_name": "Daily Housekeeping "
      },
      {
        "facility_type": "room",
        "facility_name": "Desk "
      },
      {
        "facility_type": "room",
        "facility_name": "Free Wi-Fi "
      },
      {
        "facility_type": "room",
        "facility_name": "Hair Dryer (on Request) "
      },
      {
        "facility_type": "room",
        "facility_name": "In-room Safe "
      },
      {
        "facility_type": "room",
        "facility_name": "Makeup/shaving Mirror "
      },
      {
        "facility_type": "room",
        "facility_name": "Minibar "
      },
      {
        "facility_type": "room",
        "facility_name": "Satellite TV Service "
      },
      {
        "facility_type": "room",
        "facility_name": "Slippers "
      },
      {
        "facility_type": "room",
        "facility_name": "Wake-up Calls "
      },
      {
        "facility_type": "room",
        "facility_name": "Wireless Internet Access "
      },
      {
        "facility_type": "sport",
        "facility_name": "Kolam Renang di Luar Ruangan"
      }
    ]
  },
  "nearby_attractions": {
    "nearby_attraction": [
      {
        "distance": 220,
        "business_primary_photo": "http://api-sandbox.tiket.com/img/business/p/a/business-pancake-tiramisu-topping-ice-cream-vanilla-dixie2.s.jpg",
        "business_name": "Dixie Easy Dinning",
        "business_uri": "https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-dixie-easy-dinning-2"
      },
      {
        "distance": 608,
        "business_primary_photo": "http://api-sandbox.tiket.com/img/business/l/a/business-lana.s.jpg",
        "business_name": "Lana Gallery",
        "business_uri": "https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-lana-gallery"
      },
      {
        "distance": 955,
        "business_primary_photo": "http://api-sandbox.tiket.com/img/business/a/f/business-affandi_galeri_1.s.jpg",
        "business_name": "Museum Affandi",
        "business_uri": "https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-museum-affandi"
      },
      {
        "distance": 1560,
        "business_primary_photo": "http://api-sandbox.tiket.com/img/business/t/1/business-t144.s.jpg",
        "business_name": "Telkom Office",
        "business_uri": "https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-telkom-office"
      },
      {
        "distance": 1594,
        "business_primary_photo": "http://api-sandbox.tiket.com/img/business/4/4/business-44737073.s.jpg",
        "business_name": "Kridosono Stadium",
        "business_uri": "https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-kridosono-stadium"
      },
      {
        "distance": 1674,
        "business_primary_photo": "http://api-sandbox.tiket.com/img/business/t/2/business-t242.s.jpg",
        "business_name": "Kotabaru",
        "business_uri": "https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-kotabaru-poi"
      },
      {
        "distance": 1694,
        "business_primary_photo": "http://api-sandbox.tiket.com/img/business/l/e/business-lempuyangan.s.jpg",
        "business_name": "Lempuyangan Railway station",
        "business_uri": "https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-lempuyangan-railway-station"
      },
      {
        "distance": 1839,
        "business_primary_photo": "http://api-sandbox.tiket.com/img/business/r/a/business-raminten-21.s.jpg",
        "business_name": "Raminten",
        "business_uri": "https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-raminten"
      },
      {
        "distance": 1879,
        "business_primary_photo": "http://api-sandbox.tiket.com/img/business/t/1/business-t160.s.jpg",
        "business_name": "Rumah Sakit Soedirman",
        "business_uri": "https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-rumah-sakit-soedirman"
      },
      {
        "distance": 1945,
        "business_primary_photo": "http://api-sandbox.tiket.com/img/business/t/3/business-t337.s.jpg",
        "business_name": "Museum Batik",
        "business_uri": "https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-museum-batik"
      },
      {
        "distance": 2222,
        "business_primary_photo": "http://api-sandbox.tiket.com/img/business/u/s/business-usd.s.jpg",
        "business_name": "Sanata Darma University",
        "business_uri": "https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-sanata-darma-university"
      }
    ]
  },
  "general": {
    "address": "Jl. Gejayan 17C, Gondokusuman, Yogyakarta",
    "description": "The+Edelweiss+Hotel+Yogyakarta+berada+di+dalam+pusat+bisnis+dikota+Yogyakarta%2C+dekat+dengan+lingkungan+universitas+dan+distrik+perbelanjaan+di+sepanjang+jalan-jalan+yang+ramai+Jalan+Gejayan.+Lokasi+ini+menempatkan+pusat+perbelanjaan+besar+hanya+menit+dan+juga+15+menit+berkendara+ke+Bandara+Internasional+Yogyakarta.%3Cbr+%2F%3E%0A%3Cbr+%2F%3E%0A+Hotel+ini+menawarkan+95+kamar+dengan+desain+minimalis+modern+untuk+memperbaharui+dan+menginspirasi+Anda.+Akses+internet+berkecepatan+tinggi%2C+baik+kamar+yang+berkualitas+baik%2C+matrass+delightly+disediakan+untuk+layanan+bagi+para+pengunjung+yang+datang+ketempat+ini.%3Cbr+%2F%3E%0A%3Cbr+%2F%3E%0AFasilitas+terbaik+hotel+ini+termasuk+wi-fi+di+tempat-tempat+umum%2C+tempat+parkir+mobil%2C+layanan+laundry%2Fdry+cleaning%2C+restoran%2C+and+concierge.+Suasana+The+Edelweiss+Hotel+tercerminkan+dari+setiap+kamar+tamu.+kulkas%2C+kotak+penyimpanan+dalam-kamar%2C+TV+satelit%2Fkabel%2C+internet+wireless+%28gratis%29%2C+AC.",
    "latitude": -7.7816262945693,
    "longitude": 110.38782497907
  },
  "login_status": "true",
  "guest_id": "22691145",
  "login_email": "wida.skydev@gmail.com",
  "token": "f9b29ac359ca5d77755e7588751c089bf96f0dc9"
}
```

```matlab
a:15:{s:10:"diagnostic";a:7:{s:6:"status";i:200;s:10:"elapsetime";s:14:"16.3294";s:11:"memoryusage";s:14:"7.99MB";s:14:"unix_timestamp";i:1470379640;s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:11:"output_type";s:9:"serialize";s:13:"primaryPhotos";s:75:"http://api-sandbox.tiket.com/img/business/s/i/business-single-room-12.s.jpg";s:10:"breadcrumb";a:23:{s:11:"business_id";s:5:"15810";s:12:"business_uri";s:59:"https://api-sandbox.tiket.com/the-edelweis-hotel-yogyakarta";s:13:"business_name";s:30:"The Edelweiss Hotel Yogyakarta";s:7:"area_id";s:5:"87277";s:9:"area_name";s:7:"Gejayan";s:12:"kelurahan_id";s:1:"0";s:14:"kelurahan_name";s:1:" ";s:12:"kecamatan_id";s:3:"317";s:14:"kecamatan_name";s:12:"Gondokusuman";s:7:"city_id";s:3:"257";s:9:"city_name";s:10:"Yogyakarta";s:11:"province_id";s:2:"16";s:13:"province_name";s:26:"Daerah Istimewa Yogyakarta";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";s:12:"continent_id";s:1:"1";s:14:"continent_name";s:4:"Asia";s:13:"kelurahan_uri";s:55:"https://api-sandbox.tiket.com/search/hotel?uid=city:257";s:13:"kecamatan_uri";s:60:"https://api-sandbox.tiket.com/search/hotel?uid=kecamatan:317";s:12:"province_uri";s:58:"https://api-sandbox.tiket.com/search/hotel?uid=province:16";s:11:"country_uri";s:57:"https://api-sandbox.tiket.com/search/hotel?uid=country:id";s:13:"continent_uri";s:58:"https://api-sandbox.tiket.com/search/hotel?uid=continent:1";s:11:"star_rating";s:1:"3";}s:7:"results";a:1:{s:6:"result";a:3:{i:0;a:16:{s:2:"id";s:14:"62897320160811";s:14:"room_available";s:2:"10";s:10:"ext_source";s:6:"native";s:7:"room_id";s:6:"628973";s:8:"currency";s:3:"IDR";s:13:"minimum_stays";s:1:"1";s:15:"with_breakfasts";s:1:"0";s:14:"all_photo_room";a:1:{i:0;s:69:"http://api-sandbox.tiket.com/img/default/d/e/default-default.room.jpg";}s:9:"photo_url";s:66:"http://api-sandbox.tiket.com/img/default/d/e/default-default.s.jpg";s:9:"room_name";s:18:"Superior Room Only";s:8:"oldprice";s:9:"690525.00";s:5:"price";s:9:"375000.00";s:7:"bookUri";s:255:"https://api-sandbox.tiket.com/order/add/hotel?startdate=2016-08-11&night=1&room=1&adult=2&child=0&minstar=0&maxstar=0&minprice=0&maxprice=0&facilities=0&locations=0&hotelname=0&is_partner=0&room_id=628973&hasPromo=0&enddate=2016-08-12&room_max_occupancy=2";s:13:"room_facility";a:0:{}s:16:"room_description";b:0;s:29:"additional_surcharge_currency";s:0:"";}i:1;a:16:{s:2:"id";s:12:"107720160811";s:14:"room_available";s:2:"20";s:10:"ext_source";s:6:"native";s:7:"room_id";s:4:"1077";s:8:"currency";s:3:"IDR";s:13:"minimum_stays";s:1:"1";s:15:"with_breakfasts";s:1:"1";s:14:"all_photo_room";a:5:{i:0;s:77:"http://api-sandbox.tiket.com/img/business/s/i/business-single-room-1.room.jpg";i:1;s:77:"http://api-sandbox.tiket.com/img/business/s/u/business-suites_1_copy.room.jpg";i:2;s:73:"http://api-sandbox.tiket.com/img/business/s/u/business-suites_2a.room.jpg";i:3;s:76:"http://api-sandbox.tiket.com/img/business/t/w/business-twice_room_2.room.jpg";i:4;s:76:"http://api-sandbox.tiket.com/img/business/t/w/business-twice-room-1.room.jpg";}s:9:"photo_url";s:74:"http://api-sandbox.tiket.com/img/business/s/i/business-single-room-1.s.jpg";s:9:"room_name";s:13:"Superior Room";s:8:"oldprice";s:9:"782595.00";s:5:"price";s:9:"425000.00";s:7:"bookUri";s:253:"https://api-sandbox.tiket.com/order/add/hotel?startdate=2016-08-11&night=1&room=1&adult=2&child=0&minstar=0&maxstar=0&minprice=0&maxprice=0&facilities=0&locations=0&hotelname=0&is_partner=0&room_id=1077&hasPromo=0&enddate=2016-08-12&room_max_occupancy=2";s:13:"room_facility";a:11:{i:0;s:10:"AC";i:1;s:24:"Mesin pembuat kopi/teh";i:2;s:35:"Air mineral botol gratis";i:3;s:23:"Internet - Wifi (gratis)";i:4;s:18:"Televisi LCD/layar plasma";i:5;s:14:"Cermin";i:6;s:20:"Kulkas";i:7;s:17:"Satelit/TV kabel";i:8;s:14:"Shower";i:9;s:15:"Sandal";i:10;s:17:"Telepon";}s:16:"room_description";b:0;s:29:"additional_surcharge_currency";s:0:"";}i:2;a:18:{s:2:"id";s:20:"WSMA0511003520160811";s:14:"room_available";s:1:"1";s:7:"room_id";s:6:"498707";s:8:"currency";s:3:"IDR";s:13:"minimum_stays";i:1;s:15:"with_breakfasts";i:1;s:10:"ext_source";s:9:"mgholiday";s:13:"refund_policy";s:127:"You have to cancel 4 day(s) prior to the arrival date. Otherwise 100 % cancellation charge for the entire stay will be applied.";s:14:"all_photo_room";a:1:{i:0;s:69:"http://api-sandbox.tiket.com/img/default/d/e/default-default.room.jpg";}s:9:"photo_url";s:66:"http://api-sandbox.tiket.com/img/default/d/e/default-default.s.jpg";s:9:"room_name";s:16:"Superior (Twin) ";s:11:"promo_title";s:21:"Hanya untuk KTP/KITAS";s:11:"value_added";s:0:"";s:5:"price";s:9:"534483.00";s:7:"bookUri";s:270:"https://api-sandbox.tiket.com/order/add/hotel?startdate=2016-08-11&night=1&room=1&adult=2&child=0&minstar=0&maxstar=0&minprice=0&maxprice=0&facilities=0&locations=0&hotelname=0&is_partner=0&room_id=498707&hasPromo=1&enddate=2016-08-12&room_max_occupancy=2&breakfast=BABF";s:13:"room_facility";a:0:{}s:16:"room_description";s:8:"SUPERIOR";s:29:"additional_surcharge_currency";s:0:"";}}}s:8:"addinfos";a:1:{s:7:"addinfo";a:6:{i:0;s:40:"Biaya makan pagi (jika tidak temasuk dalam harga kamar) : IDR 48.400,00";i:1;s:24:"Checkout : 12:00";i:2;s:32:"Jumlah Restoran : 1";i:3;s:28:"Voltase ruangan : 220 V";i:4;s:45:"Waktu untuk sampai di bandara : 20 menit";i:5;s:31:"Tahun hotel dibangun : 2011";}}s:9:"all_photo";a:1:{s:5:"photo";a:23:{i:0;a:2:{s:9:"file_name";s:82:"http://api-sandbox.tiket.com/img/business/2/0/business-2014-04-29_16.25-.00-.s.jpg";s:10:"photo_type";s:21:"Kolam Renang";}i:1;a:2:{s:9:"file_name";s:82:"http://api-sandbox.tiket.com/img/business/r/o/business-room_queen_-312x234-1.s.jpg";s:10:"photo_type";s:18:"Kamar Tamu";}i:2;a:2:{s:9:"file_name";s:72:"http://api-sandbox.tiket.com/img/business/r/o/business-room_queena.s.jpg";s:10:"photo_type";s:18:"Kamar Tamu";}i:3;a:2:{s:9:"file_name";s:84:"http://api-sandbox.tiket.com/img/business/s/i/business-single_room_1_-312x234-.s.jpg";s:10:"photo_type";s:18:"Kamar Tamu";}i:4;a:2:{s:9:"file_name";s:85:"http://api-sandbox.tiket.com/img/business/s/i/business-single_room_1_-312x234-1.s.jpg";s:10:"photo_type";s:18:"Kamar Tamu";}i:5;a:2:{s:9:"file_name";s:75:"http://api-sandbox.tiket.com/img/business/s/i/business-single-room-12.s.jpg";s:10:"photo_type";s:18:"Kamar Tamu";}i:6;a:2:{s:9:"file_name";s:67:"http://api-sandbox.tiket.com/img/business/s/u/business-sup111.s.jpg";s:10:"photo_type";s:18:"Kamar Tamu";}i:7;a:2:{s:9:"file_name";s:83:"http://api-sandbox.tiket.com/img/business/t/h/business-the_edelweiss_hotel-16.s.jpg";s:10:"photo_type";s:16:"Interior";}i:8;a:2:{s:9:"file_name";s:74:"http://api-sandbox.tiket.com/img/business/t/t/business-ttwice_room_1.s.jpg";s:10:"photo_type";s:18:"Kamar Tamu";}i:9;a:2:{s:9:"file_name";s:83:"http://api-sandbox.tiket.com/img/business/t/w/business-twice_room_1_-312x234-.s.jpg";s:10:"photo_type";s:16:"Interior";}i:10;a:2:{s:9:"file_name";s:81:"http://api-sandbox.tiket.com/img/business/r/o/business-room_queen_-312x234-.s.jpg";s:10:"photo_type";s:18:"Kamar Tamu";}i:11;a:2:{s:9:"file_name";s:68:"http://api-sandbox.tiket.com/img/business/r/e/business-resto78.s.jpg";s:10:"photo_type";s:18:"Rumah Makan";}i:12;a:2:{s:9:"file_name";s:85:"http://api-sandbox.tiket.com/img/business/q/u/business-queen_staff_2_-312x234-2.s.jpg";s:10:"photo_type";s:18:"Kamar Tamu";}i:13;a:2:{s:9:"file_name";s:68:"http://api-sandbox.tiket.com/img/business/3/1/business-312x234.s.jpg";s:10:"photo_type";s:18:"Kamar Tamu";}i:14;a:2:{s:9:"file_name";s:63:"http://api-sandbox.tiket.com/img/business/9/3/business-93.s.jpg";s:10:"photo_type";s:12:"Makanan";}i:15;a:2:{s:9:"file_name";s:64:"http://api-sandbox.tiket.com/img/business/9/3/business-931.s.jpg";s:10:"photo_type";s:12:"Makanan";}i:16;a:2:{s:9:"file_name";s:79:"http://api-sandbox.tiket.com/img/business/b/u/business-business_center_a1.s.jpg";s:10:"photo_type";s:23:"Pusat Bisnis";}i:17;a:2:{s:9:"file_name";s:81:"http://api-sandbox.tiket.com/img/business/e/i/business-eight_bar_-312x234-1.s.jpg";s:10:"photo_type";s:21:"Kolam Renang";}i:18;a:2:{s:9:"file_name";s:70:"http://api-sandbox.tiket.com/img/business/f/a/business-facade_31.s.jpg";s:10:"photo_type";s:16:"Pintu Masuk";}i:19;a:2:{s:9:"file_name";s:75:"http://api-sandbox.tiket.com/img/business/f/o/business-food_-312x234-.s.jpg";s:10:"photo_type";s:12:"Makanan";}i:20;a:2:{s:9:"file_name";s:76:"http://api-sandbox.tiket.com/img/business/j/u/business-junior_suite_lr.s.jpg";s:10:"photo_type";s:18:"Kamar Tamu";}i:21;a:2:{s:9:"file_name";s:76:"http://api-sandbox.tiket.com/img/business/k/u/business-kursi_-312x234-.s.jpg";s:10:"photo_type";s:16:"Interior";}i:22;a:2:{s:9:"file_name";s:83:"http://api-sandbox.tiket.com/img/business/t/w/business-twice_room_2_-312x234-.s.jpg";s:10:"photo_type";s:18:"Kamar Tamu";}}}s:19:"primaryPhotos_large";s:78:"http://api-sandbox.tiket.com/img/business/s/i/business-single-room-12.crop.jpg";s:16:"avail_facilities";a:1:{s:15:"avail_facilitiy";a:74:{i:0;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:22:"Layanan Kamar 24 Jam";}i:1;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:35:"Antar Jemput Bandara Dikenakan Biaya";}i:2;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:11:"Bar";}i:3;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:23:"Pusat Bisnis";}i:4;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:16:"Tempat Parkir";}i:5;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:19:"Kedai Kopi";}i:6;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:17:"Staf Pribadi";}i:7;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:17:"Penjaga Pintu";}i:8;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:19:"Kotak Penyimpanan Barang Berharga";}i:9;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:30:"Layanan Dokter 24 Jam";}i:10;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:16:"Lift";}i:11;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:27:"Gratis Wifi di lounge";}i:12;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:25:"Gratis Wifi di kamar";}i:13;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:14:"Lounge";}i:14;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:23:"Bagasi Penyimpanan";}i:15;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:26:"Fasilitas Rapat";}i:16;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:20:"Bar Disamping Kolam Renang";}i:17;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:18:"Rumah Makan";}i:18;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:19:"Bar di atas gedung";}i:19;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:20:"Layanan Kamar";}i:20;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:20:"Kamar merokok ada tergantung ketersediaan";}i:21;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:34:"Informasi Tour";}i:22;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:21:"Layanan Parkir oleh Pelayan";}i:23;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:19:"Wi-Fi area umum";}i:24;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:17:"Wifi di Kamar";}i:25;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:19:"24-hour Front Desk ";}i:26;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:29:"Air-conditioned Public Areas ";}i:27;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:19:"Banquet Facilities ";}i:28;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:11:"Bar/lounge ";}i:29;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:35:"Complimentary Newspapers In Lobby  ";}i:30;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:14:"Elevator/lift ";}i:31;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:18:"Express Check- In ";}i:32;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:18:"Express Check-out ";}i:33;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:19:"Laundry Facilities ";}i:34;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:16:"Luggage Storage ";}i:35;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:13:"Poolside Bar ";}i:36;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:23:"Restaurant(s) In Hotel ";}i:37;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:13:"Room Service ";}i:38;a:2:{s:13:"facility_type";s:5:"hotel";s:13:"facility_name";s:24:"Room Service (24 Hours) ";}i:39;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:10:"AC";}i:40;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:24:"Mesin pembuat kopi/teh";}i:41;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:35:"Air mineral botol gratis";}i:42;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:23:"Shower Panas and Dingin";}i:43;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:20:"Brankas";}i:44;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:23:"Internet - Wifi (gratis)";}i:45;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:18:"Televisi LCD/layar plasma";}i:46;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:16:"Bar kecil";}i:47;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:14:"Cermin";}i:48;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:24:"Kamar bebas rokok ada tergantung ketersediaan";}i:49;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:20:"Kulkas";}i:50;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:17:"Satelit/TV kabel";}i:51;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:14:"Shower";}i:52;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:15:"Sandal";}i:53;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:17:"Telepon";}i:54;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:18:"Televisi";}i:55;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:17:"Air Conditioning ";}i:56;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:17:"Cable TV Service ";}i:57;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:10:"City View ";}i:58;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:17:"Coffee/tea Maker ";}i:59;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:28:"Complimentary Bottled Water ";}i:60;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:25:"Complimentary Toiletries ";}i:61;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:39:"Connecting / Adjoining Rooms Available ";}i:62;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:19:"Daily Housekeeping ";}i:63;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:5:"Desk ";}i:64;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:11:"Free Wi-Fi ";}i:65;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:24:"Hair Dryer (on Request) ";}i:66;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:13:"In-room Safe ";}i:67;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:22:"Makeup/shaving Mirror ";}i:68;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:8:"Minibar ";}i:69;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:21:"Satellite TV Service ";}i:70;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:9:"Slippers ";}i:71;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:14:"Wake-up Calls ";}i:72;a:2:{s:13:"facility_type";s:4:"room";s:13:"facility_name";s:25:"Wireless Internet Access ";}i:73;a:2:{s:13:"facility_type";s:5:"sport";s:13:"facility_name";s:20:"Kolam Renang di Luar Ruangan";}}}s:18:"nearby_attractions";a:1:{s:17:"nearby_attraction";a:11:{i:0;a:4:{s:8:"distance";d:220;s:22:"business_primary_photo";s:110:"http://api-sandbox.tiket.com/img/business/p/a/business-pancake-tiramisu-topping-ice-cream-vanilla-dixie2.s.jpg";s:13:"business_name";s:18:"Dixie Easy Dinning";s:12:"business_uri";s:111:"https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-dixie-easy-dinning-2";}i:1;a:4:{s:8:"distance";d:608;s:22:"business_primary_photo";s:65:"http://api-sandbox.tiket.com/img/business/l/a/business-lana.s.jpg";s:13:"business_name";s:12:"Lana Gallery";s:12:"business_uri";s:103:"https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-lana-gallery";}i:2;a:4:{s:8:"distance";d:955;s:22:"business_primary_photo";s:77:"http://api-sandbox.tiket.com/img/business/a/f/business-affandi_galeri_1.s.jpg";s:13:"business_name";s:14:"Museum Affandi";s:12:"business_uri";s:105:"https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-museum-affandi";}i:3;a:4:{s:8:"distance";d:1560;s:22:"business_primary_photo";s:65:"http://api-sandbox.tiket.com/img/business/t/1/business-t144.s.jpg";s:13:"business_name";s:13:"Telkom Office";s:12:"business_uri";s:104:"https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-telkom-office";}i:4;a:4:{s:8:"distance";d:1594;s:22:"business_primary_photo";s:69:"http://api-sandbox.tiket.com/img/business/4/4/business-44737073.s.jpg";s:13:"business_name";s:17:"Kridosono Stadium";s:12:"business_uri";s:108:"https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-kridosono-stadium";}i:5;a:4:{s:8:"distance";d:1674;s:22:"business_primary_photo";s:65:"http://api-sandbox.tiket.com/img/business/t/2/business-t242.s.jpg";s:13:"business_name";s:8:"Kotabaru";s:12:"business_uri";s:103:"https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-kotabaru-poi";}i:6;a:4:{s:8:"distance";d:1694;s:22:"business_primary_photo";s:72:"http://api-sandbox.tiket.com/img/business/l/e/business-lempuyangan.s.jpg";s:13:"business_name";s:27:"Lempuyangan Railway station";s:12:"business_uri";s:118:"https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-lempuyangan-railway-station";}i:7;a:4:{s:8:"distance";d:1839;s:22:"business_primary_photo";s:72:"http://api-sandbox.tiket.com/img/business/r/a/business-raminten-21.s.jpg";s:13:"business_name";s:8:"Raminten";s:12:"business_uri";s:99:"https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-raminten";}i:8;a:4:{s:8:"distance";d:1879;s:22:"business_primary_photo";s:65:"http://api-sandbox.tiket.com/img/business/t/1/business-t160.s.jpg";s:13:"business_name";s:21:"Rumah Sakit Soedirman";s:12:"business_uri";s:112:"https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-rumah-sakit-soedirman";}i:9;a:4:{s:8:"distance";d:1945;s:22:"business_primary_photo";s:65:"http://api-sandbox.tiket.com/img/business/t/3/business-t337.s.jpg";s:13:"business_name";s:12:"Museum Batik";s:12:"business_uri";s:103:"https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-museum-batik";}i:10;a:4:{s:8:"distance";d:2222;s:22:"business_primary_photo";s:64:"http://api-sandbox.tiket.com/img/business/u/s/business-usd.s.jpg";s:13:"business_name";s:23:"Sanata Darma University";s:12:"business_uri";s:114:"https://api-sandbox.tiket.com/attractions/indonesia/daerah-istimewa-yogyakarta/hotel-dekat-sanata-darma-university";}}}s:7:"general";a:4:{s:7:"address";s:41:"Jl. Gejayan 17C, Gondokusuman, Yogyakarta";s:11:"description";s:966:"The+Edelweiss+Hotel+Yogyakarta+berada+di+dalam+pusat+bisnis+dikota+Yogyakarta%2C+dekat+dengan+lingkungan+universitas+dan+distrik+perbelanjaan+di+sepanjang+jalan-jalan+yang+ramai+Jalan+Gejayan.+Lokasi+ini+menempatkan+pusat+perbelanjaan+besar+hanya+menit+dan+juga+15+menit+berkendara+ke+Bandara+Internasional+Yogyakarta.%3Cbr+%2F%3E%0A%3Cbr+%2F%3E%0A+Hotel+ini+menawarkan+95+kamar+dengan+desain+minimalis+modern+untuk+memperbaharui+dan+menginspirasi+Anda.+Akses+internet+berkecepatan+tinggi%2C+baik+kamar+yang+berkualitas+baik%2C+matrass+delightly+disediakan+untuk+layanan+bagi+para+pengunjung+yang+datang+ketempat+ini.%3Cbr+%2F%3E%0A%3Cbr+%2F%3E%0AFasilitas+terbaik+hotel+ini+termasuk+wi-fi+di+tempat-tempat+umum%2C+tempat+parkir+mobil%2C+layanan+laundry%2Fdry+cleaning%2C+restoran%2C+and+concierge.+Suasana+The+Edelweiss+Hotel+tercerminkan+dari+setiap+kamar+tamu.+kulkas%2C+kotak+penyimpanan+dalam-kamar%2C+TV+satelit%2Fkabel%2C+internet+wireless+%28gratis%29%2C+AC.";s:8:"latitude";d:-7.78162629456927579241209969040937721729278564453125;s:9:"longitude";d:110.3878249790693217846637708134949207305908203125;}s:12:"login_status";s:4:"true";s:8:"guest_id";s:8:"22691145";s:11:"login_email";s:21:"wida.skydev@gmail.com";s:5:"token";s:40:"f9b29ac359ca5d77755e7588751c089bf96f0dc9";}
```

#### HTTP Request

    `GET https://api-sandbox.tiket.com/hotel/indonesia/yogyakarta/gejayan/the-edelweis-hotel-yogyakarta?startdate=2016-08-11&night=1&enddate&room=1&adult=2&child=0&uid=business%3A15810&token=f9b29ac359ca5d77755e7588751c089bf96f0dc9&output=json`


#### Parameters

link url to view detail can be get from search hotel, variable business_uri  
user just need to add token in the parameter.

  
Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------  
startdate | Check in date | DATE | date of today | TRUE  
night | Total night to stay | INT(5) | 1 | TRUE  
enddate | Check out date | DATE | date of tomorrow | TRUE  
room | Total room that will booked by customer | INT(5) | 1 | TRUE  
adult | Total adult | INT(5) | 2 | TRUE  
child | Total child | INT(5) | 0 |   
token | for saving transaction that done by user | CHAR(128) |  | TRUE

    
## Add Order

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
{
  "output_type": "json",
  "error": "0",
  "diagnostic": {
    "elapstime": "9.5301",
    "memoryusage": "12.15MB",
    "status": "200",
    "lang": "en",
    "currency": "IDR"
  },
  "status": "success booking train",
  "token": "1c78d7bc29690cd96dfce9e0350cfc51"
}
```

```matlab
a: 5: {
  s: 11: "output_type";s: 9: "serialize";s: 5: "error";s: 1: "0";s: 10: "diagnostic";a: 5: {
    s: 9: "elapstime";s: 14: "5.9200";s: 11: "memoryusage";s: 14: "12.15MB";s: 6: "status";s: 3: "200";s: 4: "lang";s: 2: "en";s: 8: "currency";s: 3: "IDR";
  }
  s: 6: "status";s: 21: "success booking train";s: 5: "token";s: 32: "1c78d7bc29690cd96dfce9e0350cfc51";
}

```

Add hotel order to shopping cart.

#### HTTP Request

    `GET https://api-sandbox.tiket.com/order/add/hotel?startdate=2012-06-11&enddate=2012-06-12&night=1&room=1&adult=2&child=0&minstar=0&maxstar=5&minprice=0&maxprice=1000&hotelname=0&room_id=666&hasPromo=0&token=1c78d7bc29690cd96dfce9e0350cfc51&output=json`

#### Parameters

Plink url to view detail can be get from view detail hotel, variable book_uri  
user just need to add token in the parameter.

  
Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------  
startdate | check-in date | YYYY-MM-DD | date of today | TRUE  
enddate | check-out date | YYYY-MM-DD | date of tomorrow | TRUE  
night | number of night | INT(5) | 1 | TRUE  
room | Total room that will booked by customer | INT(5) | 1 | TRUE  
adult | number of adult | INT(5) | 2 | TRUE  
child | number of child | INT(5) | 0 | FALSE  
minstar | hotel star | INT(5) |  |   
minprice | cheapest hotel price | INT(5) |  |   
hotelname | hotel name | CHAR(50) |  |   
room_id | room id that will ordered | CHAR(10) |  |   
hasPromo | if the room has promo between 1 or 0 | INT(5) |  |   
token | for saving transaction that done by user | CHAR(128) |  | TRUE
  


## Order

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
{
  "output_type": "json",
  "myorder": {
    "order_id": "120152",
    "data": [{
      "expire": 60,
      "order_detail_id": "31406",
      "order_type": "hotel",
      "order_name": "The 101 Legian",
      "order_name_detail": "Superior (Room Only)",
      "tenor": "0",
      "detail": {
        "order_detail_id": "31406",
        "room_id": "1185",
        "rooms": "1",
        "adult": "2",
        "child": "0",
        "startdate": "11 Jun 2012",
        "enddate": "12 Jun 2012",
        "nights": "1",
        "price": 517920
      },
      "order_photo": "http:\/\/www.sandbox.tiket.com\/img\/business\/1\/0\/business-10211.s.jpg",
      "tax": 106080,
      "item_charge": 0,
      "subtotal_and_charge": "624000.00",
      "delete_uri": "https:\/\/api-sandbox.tiket.com\/order\/delete_order?order_detail_id=31406"
    }],
    "total": 624000,
    "total_tax": 106080,
    "total_without_tax": 517920,
    "count_installment": 0
  },
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.2683",
    "memoryusage": "17.85MB",
    "confirm": "success",
    "lang": "en",
    "currency": "IDR"
  },
  "checkout": "https:\/\/api-sandbox.tiket.com\/order\/checkout\/120152\/IDR",
  "login_status": "false",
  "token": "8f683005261f872fe5c044f9b7085162"
}
```

```matlab
a: 6: {
  s: 11: "output_type";s: 9: "serialize";s: 7: "myorder";a: 6: {
    s: 8: "order_id";s: 6: "120152";s: 4: "data";a: 1: {
      i: 0;a: 12: {
        s: 6: "expire";i: 60;s: 15: "order_detail_id";s: 5: "31406";s: 10: "order_type";s: 5: "hotel";s: 10: "order_name";s: 14: "The 101 Legian";s: 17: "order_name_detail";s: 20: "Superior (Room Only)";s: 5: "tenor";s: 1: "0";s: 6: "detail";a: 9: {
          s: 15: "order_detail_id";s: 5: "31406";s: 7: "room_id";s: 4: "1185";s: 5: "rooms";s: 1: "1";s: 5: "adult";s: 1: "2";s: 5: "child";s: 1: "0";s: 9: "startdate";s: 11: "11 Jun 2012";s: 7: "enddate";s: 11: "12 Jun 2012";s: 6: "nights";s: 1: "1";s: 5: "price";d: 517920;
        }
        s: 11: "order_photo";s: 67: "http://www.sandbox.tiket.com/img/business/1/0/business-10211.s.jpg";s: 3: "tax";d: 106080;s: 11: "item_charge";i: 0;s: 19: "subtotal_and_charge";s: 9: "624000.00";s: 10: "delete_uri";s: 71: "https://api-sandbox.tiket.com/order/delete_order?order_detail_id=31406";
      }
    }
    s: 5: "total";d: 624000;s: 9: "total_tax";d: 106080;s: 17: "total_without_tax";d: 517920;s: 17: "count_installment";i: 0;
  }
  s: 10: "diagnostic";a: 6: {
    s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.3174";s: 11: "memoryusage";s: 14: "17.85MB";s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "en";s: 8: "currency";s: 3: "IDR";
  }
  s: 8: "checkout";s: 56: "https://api-sandbox.tiket.com/order/checkout/120152/IDR";s: 12: "login_status";s: 5: "false";s: 5: "token";s: 32: "8f683005261f872fe5c044f9b7085162";
}
```

#### HTTP Request

    `GET https://api-sandbox.tiket.com/order?token=8f683005261f872fe5c044f9b7085162&output=json`


#### Parameters

  
Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------   
token | for saving transaction that done by user | CHAR(128) |  | TRUE
 
    
## Checkout Page Request

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
{
  "output_type": "json",
  "next_checkout_uri": "httpss:\/\/api-sandbox.tiket.com\/checkout\/checkout_customer",
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.1157",
    "memoryusage": "6.43MB",
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "login_status": "false",
  "token": "9991e3092aea96042964220181374b60"
}
```

```matlab
a: 5: {
  s: 11: "output_type";s: 9: "serialize";s: 17: "next_checkout_uri";s: 57: "httpss://api-sandbox.tiket.com/checkout/checkout_customer";s: 10: "diagnostic";a: 7: {
    s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.1132";s: 11: "memoryusage";s: 14: "6.43MB";s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "id";s: 8: "currency";s: 3: "IDR";
  }
  s: 12: "login_status";s: 5: "false";s: 5: "token";s: 32: "9991e3092aea96042964220181374b60";
}
```


Early stage to access checkout.

#### HTTP Request

    `GET https://api-sandbox.tiket.com/order/checkout/119978/IDR?token=9991e3092aea96042964220181374b60&output=json`


#### Parameters

  
Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------  
token | for saving transaction that done by user | CHAR(128) |  | TRUE    


Get from order page in checkout variable.
    
    
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
[a: 5: {
  s: 11: "output_type";s: 9: "serialize";s: 10: "diagnostic";a: 7: {
    s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.1628";s: 11: "memoryusage";s: 14: "7.77MB";s: 7: "confirm";s: 7: "success";s: 10: "error_msgs";s: 0: "";s: 4: "lang";s: 2: "en";s: 8: "currency";s: 3: "IDR";
  }
  s: 12: "login_status";s: 4: "true";s: 8: "guest_id";s: 5: "21688";s: 5: "token";s: 32: "9d4ccf0c966e37a4c112c59ac2bc2e97";
}
```

#### HTTP Request

    `GET https://api-sandbox.tiket.com/checkout/checkout_customer?token=87da88eaaa429d5513a3a3658b01701e&salutation=Ms&firstName=ba&lastName=ca&emailAddress=testing@yahoocom&phone=%2B62878434343&saveContinue=2&output=json`


#### Parameters

  
Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------  
salutation | your title( ex: Mr. | Mrs. | Ms.) | CHAR(5) |  | TRUE  
firstName | your first name | CHAR(50) |  | TRUE  
lastName | your last name | CHAR(50) |  | TRUE  
emailAddress | your email | CHAR(50) |  | TRUE  
phone | your phone |  ex: 081232323343 or +62324324234234. Don't forget to urlencode + into %2B in the GET parameter | CHAR(20) |  | TRUE  
saveContinue | Flag for save unregistered user data (value=2) |  |  | TRUE
  


Setelah merequest link tersebut maka user akan dibuatkan account di tiket.com  
user akan dikirimkan email untuk mengubah password loginnya.

    
## Checkout Customer

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
{
  "output_type": "json",
  "diagnostic": {
    "status": 201,
    "elapsetime": "0.3014",
    "memoryusage": "19.19MB",
    "error_msgs": "Your Contact Person details has been saved.",
    "lang": "en",
    "currency": "IDR"
  },
  "currProfileArr": {
    "account_id": "106238",
    "account_first_name": "a",
    "account_last_name": "a",
    "account_mobile": "+62811123123",
    "account_salutation_name": "Mrs.",
    "account_phone": "+628888843",
    "account_username": "you.jul.in@gmail.com",
    "profile_id": "15774",
    "Name": "a a",
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
    "account_profile_modified": "2012-06-11 17:10:53",
    "account_birthdate": null,
    "account_gender": "F",
    "account_id_card": null
  },
  "currProfileId": "15774",
  "travellerProfileArr": {
    "account_salutation_name": "Mrs.",
    "account_first_name": "ba",
    "account_last_name": "ca",
    "account_phone": "+628888843"
  },
  "contactProfileArr": {
    "account_salutation_name": "Mrs.",
    "account_first_name": "a",
    "account_last_name": "a",
    "account_username": "bibi@ads.com",
    "account_phone": "+628888843"
  },
  "statusClass": "ok",
  "next": "http:\/\/api-sandbox.tiket.com\/checkout\/checkout_payment",
  "SideArr": {
    "currBookingArr": {
      "detail_id": "31406",
      "type": "hotel",
      "master_name": "The 101 Legian",
      "detail_name": "Superior (Room Only)",
      "contact_person": "15774",
      "last_update_contact_person": "0",
      "order_type": "hotel",
      "hotel_name": "The 101 Legian",
      "nights": "1",
      "check_in_first": "11 Jun 2012",
      "check_in_last": "12 Jun 2012",
      "adult": "2",
      "child": "0",
      "rooms": "1",
      "file_name": null,
      "last_update_cp": "0",
      "master_id": "4108",
      "room_id": "1185",
      "need_process": 1
    }
  },
  "login_status": "true",
  "id": "106238",
  "token": "8f683005261f872fe5c044f9b7085162"
}
```

```matlab
a: 11: {
  s: 11: "output_type";s: 9: "serialize";s: 10: "diagnostic";a: 6: {
    s: 6: "status";i: 201;s: 10: "elapsetime";s: 14: "0.2899";s: 11: "memoryusage";s: 14: "19.2MB";s: 10: "error_msgs";s: 42: "Your Contact Person details has been saved.";s: 4: "lang";s: 2: "en";s: 8: "currency";s: 3: "IDR";
  }
  s: 14: "currProfileArr";a: 23: {
    s: 10: "account_id";s: 6: "106238";s: 18: "account_first_name";s: 1: "a";s: 17: "account_last_name";s: 1: "a";s: 14: "account_mobile";s: 6: "021343";s: 23: "account_salutation_name";s: 4: "Mrs.";s: 13: "account_phone";s: 8: "+628888843";s: 16: "account_username";s: 20: "you.jul.in@gmail.com";s: 10: "profile_id";s: 5: "15775";s: 4: "Name";s: 3: "a a";s: 15: "address_country";N;s: 16: "address_address1";N;s: 16: "address_address2";N;s: 17: "address_kabupaten";N;s: 16: "address_province";N;s: 15: "address_zipcode";N;s: 15: "account_created";s: 19: "2012-06-11 11:24:28";s: 16: "account_password";s: 32: "021768c0b31cd2ad68b201213ff0e102";s: 14: "account_source";s: 5: "tiket";s: 5: "photo";s: 19: "default-default.jpg";s: 24: "account_profile_modified";s: 19: "2012-06-11 17:12:43";s: 17: "account_birthdate";N;s: 14: "account_gender";s: 1: "F";s: 15: "account_id_card";N;
  }
  s: 13: "currProfileId";s: 5: "15775";s: 19: "travellerProfileArr";a: 4: {
    s: 23: "account_salutation_name";s: 4: "Mrs.";s: 18: "account_first_name";s: 2: "ba";s: 17: "account_last_name";s: 2: "ca";s: 13: "account_phone";s: 8: "+628888843";
  }
  s: 17: "contactProfileArr";a: 5: {
    s: 23: "account_salutation_name";s: 4: "Mrs.";s: 18: "account_first_name";s: 1: "a";s: 17: "account_last_name";s: 1: "a";s: 16: "account_username";s: 12: "bibi@ads.com";s: 13: "account_phone";s: 8: "+628888843";
  }
  s: 11: "statusClass";s: 2: "ok";s: 7: "SideArr";a: 1: {
    s: 14: "currBookingArr";a: 19: {
      s: 9: "detail_id";s: 5: "31406";s: 4: "type";s: 5: "hotel";s: 11: "master_name";s: 14: "The 101 Legian";s: 11: "detail_name";s: 20: "Superior (Room Only)";s: 14: "contact_person";s: 5: "15775";s: 26: "last_update_contact_person";s: 1: "0";s: 10: "order_type";s: 5: "hotel";s: 10: "hotel_name";s: 14: "The 101 Legian";s: 6: "nights";s: 1: "1";s: 14: "check_in_first";s: 11: "11 Jun 2012";s: 13: "check_in_last";s: 11: "12 Jun 2012";s: 5: "adult";s: 1: "2";s: 5: "child";s: 1: "0";s: 5: "rooms";s: 1: "1";s: 9: "file_name";N;s: 14: "last_update_cp";s: 1: "0";s: 9: "master_id";s: 4: "4108";s: 7: "room_id";s: 4: "1185";s: 12: "need_process";i: 1;
    }
  }
  s: 12: "login_status";s: 4: "true";s: 2: "id";s: 6: "106238";s: 5: "token";s: 32: "8f683005261f872fe5c044f9b7085162";
}
```

#### HTTP Request

    `GET https://api-sandbox.tiket.com/checkout/checkout_customer?token=8f683005261f872fe5c044f9b7085162&salutation=Mrs&firstName=ba&lastName=ca&emailAddress=bibi@yahoocom&phone=%2B628888843&conSalutation=Mrs&conFirstName=a&conLastName=a&conEmailAddress=bibi@yahoocom&conPhone=%2B628888843&detailId=31406&country=id&output=json`


#### Parameters

  
Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------    
token | for saving transaction that done by user | CHAR(128) |  | TRUE  
salutation | your title( ex: Mr. | Mrs. | Ms.) | CHAR(5) |  | TRUE  
firstName | your first name | CHAR(50) |  | TRUE  
lastName | your last name CHAR(50) |  | TRUE  
phone | your phone |  ex: 081232323343 or +62324324234234. Don't forget to urlencode + into %2B in the GET parameter | CHAR(20) |  | TRUE  
conSalutation | contact person title ( ex: Mr. | Mrs. | Ms.) | CHAR(5) |  | TRUE  
conFirstName | contact person first name | CHAR(50) |  | TRUE  
conLastName | contact person last name | CHAR(50) |  | TRUE  
conEmailAddress | contact person email address | CHAR(50) |  | TRUE  
conPhone | contact person phone |  ex: 081232323343 or +62324324234234. Don't forget to urlencode + into %2B in the GET parameter | CHAR(20) |  | TRUE  
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

    `GET https://api-sandbox.tiket.com/checkout/checkout_payment?token=87da88eaaa429d5513a3a3658b01701e`

#### Parameters

Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------  
token | for saving transaction that done by user | CHAR(128) |  | TRUE  


## Checkout Payment

Please see [Checkout Payment](http://docs.tiket.com/#checkout-payment-309) in General API

























