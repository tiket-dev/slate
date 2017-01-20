# Flight API

<aside class="notice">Data that is provided for development stage is different from the production stage</aside>

These are the API commands for flight

Diagram flow for Flight API:  

![Flight API](https://raw.githubusercontent.com/tiket-dev/slate/master/source/images/Diagram-Flow-API-Flight.png)

## Search Flight

```xml
<?xml version="1.0" encoding="utf-8"?>
<tiket>
    <diagnostic>
        <status>200</status>
        <elapsetime>0.4048</elapsetime>
        <memoryusage>8.41MB</memoryusage>
        <unix_timestamp>1470285416</unix_timestamp>
        <confirm>success</confirm>
        <lang>id</lang>
        <currency>IDR</currency>
    </diagnostic>
    <output_type>xml</output_type>
    <round_trip>1</round_trip>
    <search_queries>
        <from>SUB</from>
        <to>LOP</to>
        <date>2016-08-04</date>
        <ret_date>2016-08-05</ret_date>
        <adult>1</adult>
        <child>0</child>
        <infant>0</infant>
        <sort></sort>
    </search_queries>
    <go_det>
        <dep_airport>
            <airport_code>SUB</airport_code>
            <international>1</international>
            <trans_name_id>7595</trans_name_id>
            <banner_image></banner_image>
            <short_name_trans_id>1193620</short_name_trans_id>
            <business_name>Juanda</business_name>
            <business_name_trans_id>5963</business_name_trans_id>
            <business_country>id</business_country>
            <business_id>20389</business_id>
            <country_name>Indonesia</country_name>
            <city_name>Surabaya</city_name>
            <province_name>Jawa Timur</province_name>
            <short_name>Surabaya</short_name>
            <location_name>Surabaya</location_name>
        </dep_airport>
        <arr_airport>
            <airport_code>LOP</airport_code>
            <international>1</international>
            <trans_name_id>7583</trans_name_id>
            <banner_image></banner_image>
            <short_name_trans_id>1193670</short_name_trans_id>
            <business_name>Lombok</business_name>
            <business_name_trans_id>5947</business_name_trans_id>
            <business_country>id</business_country>
            <business_id>20373</business_id>
            <country_name>Indonesia</country_name>
            <city_name>Mataram</city_name>
            <province_name>Nusa Tenggara Barat</province_name>
            <short_name>Lombok</short_name>
            <location_name>Lombok, Mataram</location_name>
        </arr_airport>
        <date>2016-08-04</date>
        <formatted_date>04 Agustus 2016</formatted_date>
    </go_det>
    <ret_det>
        <dep_airport>
            <airport_code>LOP</airport_code>
            <international>1</international>
            <trans_name_id>7583</trans_name_id>
            <banner_image></banner_image>
            <short_name_trans_id>1193670</short_name_trans_id>
            <business_name>Lombok</business_name>
            <business_name_trans_id>5947</business_name_trans_id>
            <business_country>id</business_country>
            <business_id>20373</business_id>
            <country_name>Indonesia</country_name>
            <city_name>Mataram</city_name>
            <province_name>Nusa Tenggara Barat</province_name>
            <short_name>Lombok</short_name>
            <location_name>Lombok, Mataram</location_name>
        </dep_airport>
        <arr_airport>
            <airport_code>SUB</airport_code>
            <international>1</international>
            <trans_name_id>7595</trans_name_id>
            <banner_image></banner_image>
            <short_name_trans_id>1193620</short_name_trans_id>
            <business_name>Juanda</business_name>
            <business_name_trans_id>5963</business_name_trans_id>
            <business_country>id</business_country>
            <business_id>20389</business_id>
            <country_name>Indonesia</country_name>
            <city_name>Surabaya</city_name>
            <province_name>Jawa Timur</province_name>
            <short_name>Surabaya</short_name>
            <location_name>Surabaya</location_name>
        </arr_airport>
        <date>2016-08-05</date>
        <formatted_date>05 Agustus 2016</formatted_date>
    </ret_det>
    <departures>
        <result>
            <flight_id>2490729</flight_id>
            <airlines_name>CITILINK</airlines_name>
            <flight_number>QG-660</flight_number>
            <departure_city>SUB</departure_city>
            <arrival_city>LOP</arrival_city>
            <stop>Langsung</stop>
            <price_value>936900.00</price_value>
            <price_adult>936900.00</price_adult>
            <price_child>0.00</price_child>
            <price_infant>0.00</price_infant>
            <timestamp>2016-08-04 11:23:25</timestamp>
            <has_food>0</has_food>
            <check_in_baggage>20</check_in_baggage>
            <is_promo>0</is_promo>
            <airport_tax>1</airport_tax>
            <simple_departure_time>15:25</simple_departure_time>
            <simple_arrival_time>17:35</simple_arrival_time>
            <long_via></long_via>
            <departure_city_name>Surabaya</departure_city_name>
            <arrival_city_name>Lombok</arrival_city_name>
            <full_via>SUB - LOP (15:25 - 17:35)</full_via>
            <markup_price_string></markup_price_string>
            <need_baggage>0</need_baggage>
            <best_deal></best_deal>
            <duration>1 j 10 m</duration>
            <image>http://api-sandbox.tiket.com/images/tiket2/icon_citilink_2.jpg</image>
            <flight_infos>
                <flight_info>
                    <flight_number>QG-660</flight_number>
                    <airlines_name>CITILINK</airlines_name>
                    <airlines_short_real_name>Citilink</airlines_short_real_name>
                    <airlines_short_real_name_ucwords>Citilink</airlines_short_real_name_ucwords>
                    <departure_city>SUB</departure_city>
                    <arrival_city>LOP</arrival_city>
                    <simple_departure_time>15:25</simple_departure_time>
                    <simple_arrival_time>17:35</simple_arrival_time>
                    <img>&lt;img width="52" height="45" src="http://api-sandbox.tiket.com/images/flight/logo/icon_citilink.png" title="Citilink" alt="QG-660 SUB LOP 15:25" /&gt;</img>
                    <img_src>http://api-sandbox.tiket.com/images/flight/logo/icon_citilink.png</img_src>
                    <check_in_baggage>20</check_in_baggage>
                    <terminal></terminal>
                    <departure_city_name>Surabaya</departure_city_name>
                    <arrival_city_name>Lombok</arrival_city_name>
                    <duration>
                        <hour>0</hour>
                        <minute>0</minute>
                        <arrival_time>2016-08-04 17:35:00</arrival_time>
                        <arrival_city>LOP</arrival_city>
                        <text_city></text_city>
                        <text_time></text_time>
                    </duration>
                    <duration_time>4200</duration_time>
                    <duration_hour>1j</duration_hour>
                    <duration_minute>10m</duration_minute>
                </flight_info>
            </flight_infos>
            <sss_key></sss_key>
        </result>
    </departures>
    <returns>
        <result>
            <flight_id>2490731</flight_id>
            <airlines_name>CITILINK</airlines_name>
            <flight_number>QG-665</flight_number>
            <departure_city>LOP</departure_city>
            <arrival_city>SUB</arrival_city>
            <stop>Langsung</stop>
            <price_value>693720.00</price_value>
            <price_adult>693720.00</price_adult>
            <price_child>0.00</price_child>
            <price_infant>0.00</price_infant>
            <timestamp>2016-08-04 11:28:03</timestamp>
            <has_food>0</has_food>
            <check_in_baggage>20</check_in_baggage>
            <is_promo>0</is_promo>
            <airport_tax>1</airport_tax>
            <simple_departure_time>12:00</simple_departure_time>
            <simple_arrival_time>12:15</simple_arrival_time>
            <long_via></long_via>
            <departure_city_name>Lombok</departure_city_name>
            <arrival_city_name>Surabaya</arrival_city_name>
            <full_via>LOP - SUB (12:00 - 12:15)</full_via>
            <markup_price_string></markup_price_string>
            <need_baggage>0</need_baggage>
            <best_deal></best_deal>
            <duration>1 j 15 m</duration>
            <image>http://api-sandbox.tiket.com/images/tiket2/icon_citilink_2.jpg</image>
            <flight_infos>
                <flight_info>
                    <flight_number>QG-665</flight_number>
                    <airlines_name>CITILINK</airlines_name>
                    <airlines_short_real_name>Citilink</airlines_short_real_name>
                    <airlines_short_real_name_ucwords>Citilink</airlines_short_real_name_ucwords>
                    <departure_city>LOP</departure_city>
                    <arrival_city>SUB</arrival_city>
                    <simple_departure_time>12:00</simple_departure_time>
                    <simple_arrival_time>12:15</simple_arrival_time>
                    <img>&lt;img width="52" height="45" src="http://api-sandbox.tiket.com/images/flight/logo/icon_citilink.png" title="Citilink" alt="QG-665 LOP SUB 12:00" /&gt;</img>
                    <img_src>http://api-sandbox.tiket.com/images/flight/logo/icon_citilink.png</img_src>
                    <check_in_baggage>20</check_in_baggage>
                    <terminal></terminal>
                    <departure_city_name>Lombok</departure_city_name>
                    <arrival_city_name>Surabaya</arrival_city_name>
                    <duration>
                        <hour>0</hour>
                        <minute>0</minute>
                        <arrival_time>2016-08-05 12:15:00</arrival_time>
                        <arrival_city>SUB</arrival_city>
                        <text_city></text_city>
                        <text_time></text_time>
                    </duration>
                    <duration_time>4500</duration_time>
                    <duration_hour>1j</duration_hour>
                    <duration_minute>15m</duration_minute>
                </flight_info>
            </flight_infos>
            <sss_key></sss_key>
        </result>
        <result>
            <flight_id>2490733</flight_id>
            <airlines_name>CITILINK</airlines_name>
            <flight_number>QG-661</flight_number>
            <departure_city>LOP</departure_city>
            <arrival_city>SUB</arrival_city>
            <stop>Langsung</stop>
            <price_value>693720.00</price_value>
            <price_adult>693720.00</price_adult>
            <price_child>0.00</price_child>
            <price_infant>0.00</price_infant>
            <timestamp>2016-08-04 11:28:03</timestamp>
            <has_food>0</has_food>
            <check_in_baggage>20</check_in_baggage>
            <is_promo>0</is_promo>
            <airport_tax>1</airport_tax>
            <simple_departure_time>18:05</simple_departure_time>
            <simple_arrival_time>18:10</simple_arrival_time>
            <long_via></long_via>
            <departure_city_name>Lombok</departure_city_name>
            <arrival_city_name>Surabaya</arrival_city_name>
            <full_via>LOP - SUB (18:05 - 18:10)</full_via>
            <markup_price_string></markup_price_string>
            <need_baggage>0</need_baggage>
            <best_deal></best_deal>
            <duration>1 j 5 m</duration>
            <image>http://api-sandbox.tiket.com/images/tiket2/icon_citilink_2.jpg</image>
            <flight_infos>
                <flight_info>
                    <flight_number>QG-661</flight_number>
                    <airlines_name>CITILINK</airlines_name>
                    <airlines_short_real_name>Citilink</airlines_short_real_name>
                    <airlines_short_real_name_ucwords>Citilink</airlines_short_real_name_ucwords>
                    <departure_city>LOP</departure_city>
                    <arrival_city>SUB</arrival_city>
                    <simple_departure_time>18:05</simple_departure_time>
                    <simple_arrival_time>18:10</simple_arrival_time>
                    <img>&lt;img width="52" height="45" src="http://api-sandbox.tiket.com/images/flight/logo/icon_citilink.png" title="Citilink" alt="QG-661 LOP SUB 18:05" /&gt;</img>
                    <img_src>http://api-sandbox.tiket.com/images/flight/logo/icon_citilink.png</img_src>
                    <check_in_baggage>20</check_in_baggage>
                    <terminal></terminal>
                    <departure_city_name>Lombok</departure_city_name>
                    <arrival_city_name>Surabaya</arrival_city_name>
                    <duration>
                        <hour>0</hour>
                        <minute>0</minute>
                        <arrival_time>2016-08-05 18:10:00</arrival_time>
                        <arrival_city>SUB</arrival_city>
                        <text_city></text_city>
                        <text_time></text_time>
                    </duration>
                    <duration_time>3900</duration_time>
                    <duration_hour>1j</duration_hour>
                    <duration_minute>5m</duration_minute>
                </flight_info>
            </flight_infos>
            <sss_key></sss_key>
        </result>
        <result>
            <flight_id>2490735</flight_id>
            <airlines_name>GARUDA</airlines_name>
            <flight_number>GA-365</flight_number>
            <departure_city>LOP</departure_city>
            <arrival_city>SUB</arrival_city>
            <stop>Langsung</stop>
            <price_value>930000.00</price_value>
            <price_adult>930000.00</price_adult>
            <price_child>0.00</price_child>
            <price_infant>0.00</price_infant>
            <timestamp>2016-08-04 11:28:06</timestamp>
            <has_food>1</has_food>
            <check_in_baggage>20</check_in_baggage>
            <is_promo>0</is_promo>
            <airport_tax>1</airport_tax>
            <simple_departure_time>14:25</simple_departure_time>
            <simple_arrival_time>14:30</simple_arrival_time>
            <long_via></long_via>
            <departure_city_name>Lombok</departure_city_name>
            <arrival_city_name>Surabaya</arrival_city_name>
            <full_via>LOP - SUB (14:25 - 14:30)</full_via>
            <markup_price_string></markup_price_string>
            <need_baggage>0</need_baggage>
            <best_deal></best_deal>
            <duration>1 j 5 m</duration>
            <image>http://api-sandbox.tiket.com/images/tiket2/icon_garuda_2.jpg</image>
            <flight_infos>
                <flight_info>
                    <flight_number>GA-365</flight_number>
                    <airlines_name>GARUDA</airlines_name>
                    <airlines_short_real_name>Garuda</airlines_short_real_name>
                    <airlines_short_real_name_ucwords>Garuda</airlines_short_real_name_ucwords>
                    <departure_city>LOP</departure_city>
                    <arrival_city>SUB</arrival_city>
                    <simple_departure_time>14:25</simple_departure_time>
                    <simple_arrival_time>14:30</simple_arrival_time>
                    <img>&lt;img width="52" height="45" src="http://api-sandbox.tiket.com/images/flight/logo/icon_garuda.png" title="Garuda Indonesia" alt="GA-365 LOP SUB 14:25" /&gt;</img>
                    <img_src>http://api-sandbox.tiket.com/images/flight/logo/icon_garuda.png</img_src>
                    <check_in_baggage>20</check_in_baggage>
                    <terminal></terminal>
                    <departure_city_name>Lombok</departure_city_name>
                    <arrival_city_name>Surabaya</arrival_city_name>
                    <duration>
                        <hour>0</hour>
                        <minute>0</minute>
                        <arrival_time>2016-08-05 14:30:00</arrival_time>
                        <arrival_city>SUB</arrival_city>
                        <text_city></text_city>
                        <text_time></text_time>
                    </duration>
                    <duration_time>3900</duration_time>
                    <duration_hour>1j</duration_hour>
                    <duration_minute>5m</duration_minute>
                </flight_info>
            </flight_infos>
            <sss_key></sss_key>
        </result>
        <result>
            <flight_id>2490737</flight_id>
            <airlines_name>LION</airlines_name>
            <flight_number>JT-823</flight_number>
            <departure_city>LOP</departure_city>
            <arrival_city>SUB</arrival_city>
            <stop>Langsung</stop>
            <price_value>501000.00</price_value>
            <price_adult>501000.00</price_adult>
            <price_child>0.00</price_child>
            <price_infant>0.00</price_infant>
            <timestamp>2016-08-04 11:28:07</timestamp>
            <has_food>0</has_food>
            <check_in_baggage>20</check_in_baggage>
            <is_promo>0</is_promo>
            <airport_tax>1</airport_tax>
            <simple_departure_time>07:00</simple_departure_time>
            <simple_arrival_time>07:00</simple_arrival_time>
            <long_via></long_via>
            <departure_city_name>Lombok</departure_city_name>
            <arrival_city_name>Surabaya</arrival_city_name>
            <full_via>LOP - SUB (07:00 - 07:00)</full_via>
            <markup_price_string></markup_price_string>
            <need_baggage>0</need_baggage>
            <best_deal></best_deal>
            <duration>1 j 0 m</duration>
            <image>http://api-sandbox.tiket.com/images/tiket2/icon_lion_2.jpg</image>
            <flight_infos>
                <flight_info>
                    <flight_number>JT-823</flight_number>
                    <airlines_name>LION</airlines_name>
                    <airlines_short_real_name>Lion</airlines_short_real_name>
                    <airlines_short_real_name_ucwords>Lion</airlines_short_real_name_ucwords>
                    <departure_city>LOP</departure_city>
                    <arrival_city>SUB</arrival_city>
                    <simple_departure_time>07:00</simple_departure_time>
                    <simple_arrival_time>07:00</simple_arrival_time>
                    <img>&lt;img width="52" height="45" src="http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png" title="Lion Air" alt="JT-823 LOP SUB 07:00" /&gt;</img>
                    <img_src>http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png</img_src>
                    <check_in_baggage>20</check_in_baggage>
                    <terminal></terminal>
                    <departure_city_name>Lombok</departure_city_name>
                    <arrival_city_name>Surabaya</arrival_city_name>
                    <duration>
                        <hour>0</hour>
                        <minute>0</minute>
                        <arrival_time>2016-08-05 07:00:00</arrival_time>
                        <arrival_city>SUB</arrival_city>
                        <text_city></text_city>
                        <text_time></text_time>
                    </duration>
                    <duration_time>3600</duration_time>
                    <duration_hour>1j</duration_hour>
                    <duration_minute></duration_minute>
                </flight_info>
            </flight_infos>
            <sss_key></sss_key>
        </result>
        <result>
            <flight_id>2490739</flight_id>
            <airlines_name>LION</airlines_name>
            <flight_number>JT-645</flight_number>
            <departure_city>LOP</departure_city>
            <arrival_city>SUB</arrival_city>
            <stop>Langsung</stop>
            <price_value>501000.00</price_value>
            <price_adult>501000.00</price_adult>
            <price_child>0.00</price_child>
            <price_infant>0.00</price_infant>
            <timestamp>2016-08-04 11:28:07</timestamp>
            <has_food>0</has_food>
            <check_in_baggage>20</check_in_baggage>
            <is_promo>0</is_promo>
            <airport_tax>1</airport_tax>
            <simple_departure_time>08:40</simple_departure_time>
            <simple_arrival_time>08:35</simple_arrival_time>
            <long_via></long_via>
            <departure_city_name>Lombok</departure_city_name>
            <arrival_city_name>Surabaya</arrival_city_name>
            <full_via>LOP - SUB (08:40 - 08:35)</full_via>
            <markup_price_string></markup_price_string>
            <need_baggage>0</need_baggage>
            <best_deal></best_deal>
            <duration>0 j 55 m</duration>
            <image>http://api-sandbox.tiket.com/images/tiket2/icon_lion_2.jpg</image>
            <flight_infos>
                <flight_info>
                    <flight_number>JT-645</flight_number>
                    <airlines_name>LION</airlines_name>
                    <airlines_short_real_name>Lion</airlines_short_real_name>
                    <airlines_short_real_name_ucwords>Lion</airlines_short_real_name_ucwords>
                    <departure_city>LOP</departure_city>
                    <arrival_city>SUB</arrival_city>
                    <simple_departure_time>08:40</simple_departure_time>
                    <simple_arrival_time>08:35</simple_arrival_time>
                    <img>&lt;img width="52" height="45" src="http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png" title="Lion Air" alt="JT-645 LOP SUB 08:40" /&gt;</img>
                    <img_src>http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png</img_src>
                    <check_in_baggage>20</check_in_baggage>
                    <terminal></terminal>
                    <departure_city_name>Lombok</departure_city_name>
                    <arrival_city_name>Surabaya</arrival_city_name>
                    <duration>
                        <hour>0</hour>
                        <minute>0</minute>
                        <arrival_time>2016-08-05 08:35:00</arrival_time>
                        <arrival_city>SUB</arrival_city>
                        <text_city></text_city>
                        <text_time></text_time>
                    </duration>
                    <duration_time>3300</duration_time>
                    <duration_hour></duration_hour>
                    <duration_minute>55m</duration_minute>
                </flight_info>
            </flight_infos>
            <sss_key></sss_key>
        </result>
        <result>
            <flight_id>2490741</flight_id>
            <airlines_name>LION</airlines_name>
            <flight_number>JT-865</flight_number>
            <departure_city>LOP</departure_city>
            <arrival_city>SUB</arrival_city>
            <stop>Langsung</stop>
            <price_value>501000.00</price_value>
            <price_adult>501000.00</price_adult>
            <price_child>0.00</price_child>
            <price_infant>0.00</price_infant>
            <timestamp>2016-08-04 11:28:07</timestamp>
            <has_food>0</has_food>
            <check_in_baggage>20</check_in_baggage>
            <is_promo>0</is_promo>
            <airport_tax>1</airport_tax>
            <simple_departure_time>09:40</simple_departure_time>
            <simple_arrival_time>09:35</simple_arrival_time>
            <long_via></long_via>
            <departure_city_name>Lombok</departure_city_name>
            <arrival_city_name>Surabaya</arrival_city_name>
            <full_via>LOP - SUB (09:40 - 09:35)</full_via>
            <markup_price_string></markup_price_string>
            <need_baggage>0</need_baggage>
            <best_deal></best_deal>
            <duration>0 j 55 m</duration>
            <image>http://api-sandbox.tiket.com/images/tiket2/icon_lion_2.jpg</image>
            <flight_infos>
                <flight_info>
                    <flight_number>JT-865</flight_number>
                    <airlines_name>LION</airlines_name>
                    <airlines_short_real_name>Lion</airlines_short_real_name>
                    <airlines_short_real_name_ucwords>Lion</airlines_short_real_name_ucwords>
                    <departure_city>LOP</departure_city>
                    <arrival_city>SUB</arrival_city>
                    <simple_departure_time>09:40</simple_departure_time>
                    <simple_arrival_time>09:35</simple_arrival_time>
                    <img>&lt;img width="52" height="45" src="http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png" title="Lion Air" alt="JT-865 LOP SUB 09:40" /&gt;</img>
                    <img_src>http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png</img_src>
                    <check_in_baggage>20</check_in_baggage>
                    <terminal></terminal>
                    <departure_city_name>Lombok</departure_city_name>
                    <arrival_city_name>Surabaya</arrival_city_name>
                    <duration>
                        <hour>0</hour>
                        <minute>0</minute>
                        <arrival_time>2016-08-05 09:35:00</arrival_time>
                        <arrival_city>SUB</arrival_city>
                        <text_city></text_city>
                        <text_time></text_time>
                    </duration>
                    <duration_time>3300</duration_time>
                    <duration_hour></duration_hour>
                    <duration_minute>55m</duration_minute>
                </flight_info>
            </flight_infos>
            <sss_key></sss_key>
        </result>
        <result>
            <flight_id>2490743</flight_id>
            <airlines_name>LION</airlines_name>
            <flight_number>JT-177</flight_number>
            <departure_city>LOP</departure_city>
            <arrival_city>SUB</arrival_city>
            <stop>Langsung</stop>
            <price_value>501000.00</price_value>
            <price_adult>501000.00</price_adult>
            <price_child>0.00</price_child>
            <price_infant>0.00</price_infant>
            <timestamp>2016-08-04 11:28:07</timestamp>
            <has_food>0</has_food>
            <check_in_baggage>20</check_in_baggage>
            <is_promo>0</is_promo>
            <airport_tax>1</airport_tax>
            <simple_departure_time>12:15</simple_departure_time>
            <simple_arrival_time>12:10</simple_arrival_time>
            <long_via></long_via>
            <departure_city_name>Lombok</departure_city_name>
            <arrival_city_name>Surabaya</arrival_city_name>
            <full_via>LOP - SUB (12:15 - 12:10)</full_via>
            <markup_price_string></markup_price_string>
            <need_baggage>0</need_baggage>
            <best_deal></best_deal>
            <duration>0 j 55 m</duration>
            <image>http://api-sandbox.tiket.com/images/tiket2/icon_lion_2.jpg</image>
            <flight_infos>
                <flight_info>
                    <flight_number>JT-177</flight_number>
                    <airlines_name>LION</airlines_name>
                    <airlines_short_real_name>Lion</airlines_short_real_name>
                    <airlines_short_real_name_ucwords>Lion</airlines_short_real_name_ucwords>
                    <departure_city>LOP</departure_city>
                    <arrival_city>SUB</arrival_city>
                    <simple_departure_time>12:15</simple_departure_time>
                    <simple_arrival_time>12:10</simple_arrival_time>
                    <img>&lt;img width="52" height="45" src="http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png" title="Lion Air" alt="JT-177 LOP SUB 12:15" /&gt;</img>
                    <img_src>http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png</img_src>
                    <check_in_baggage>20</check_in_baggage>
                    <terminal></terminal>
                    <departure_city_name>Lombok</departure_city_name>
                    <arrival_city_name>Surabaya</arrival_city_name>
                    <duration>
                        <hour>0</hour>
                        <minute>0</minute>
                        <arrival_time>2016-08-05 12:10:00</arrival_time>
                        <arrival_city>SUB</arrival_city>
                        <text_city></text_city>
                        <text_time></text_time>
                    </duration>
                    <duration_time>3300</duration_time>
                    <duration_hour></duration_hour>
                    <duration_minute>55m</duration_minute>
                </flight_info>
            </flight_infos>
            <sss_key></sss_key>
        </result>
    </returns>
    <nearby_go_date>
        <nearby>
            <date>2016-08-04</date>
            <price>936900.00</price>
        </nearby>
        <nearby>
            <date>2016-08-05</date>
        </nearby>
        <nearby>
            <date>2016-08-06</date>
        </nearby>
        <nearby>
            <date>2016-08-07</date>
        </nearby>
        <nearby>
            <date>2016-08-08</date>
        </nearby>
        <nearby>
            <date>2016-08-09</date>
        </nearby>
    </nearby_go_date>
    <nearby_ret_date>
        <nearby>
            <date>2016-08-04</date>
        </nearby>
        <nearby>
            <date>2016-08-05</date>
            <price>501000.00</price>
        </nearby>
        <nearby>
            <date>2016-08-06</date>
        </nearby>
        <nearby>
            <date>2016-08-07</date>
        </nearby>
        <nearby>
            <date>2016-08-08</date>
        </nearby>
        <nearby>
            <date>2016-08-09</date>
        </nearby>
        <nearby>
            <date>2016-08-10</date>
        </nearby>
    </nearby_ret_date>
    <login_status>false</login_status>
    <token>f9b29ac359ca5d77755e7588751c089bf96f0dc9</token>
</tiket>
```



```json
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.3525",
    "memoryusage": "8.37MB",
    "unix_timestamp": 1470285486,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "round_trip": true,
  "search_queries": {
    "from": "SUB",
    "to": "LOP",
    "date": "2016-08-04",
    "ret_date": "2016-08-05",
    "adult": 1,
    "child": 0,
    "infant": 0,
    "sort": false
  },
  "go_det": {
    "dep_airport": {
      "airport_code": "SUB",
      "international": "1",
      "trans_name_id": "7595",
      "banner_image": null,
      "short_name_trans_id": "1193620",
      "business_name": "Juanda",
      "business_name_trans_id": "5963",
      "business_country": "id",
      "business_id": "20389",
      "country_name": "Indonesia",
      "city_name": "Surabaya",
      "province_name": "Jawa Timur",
      "short_name": "Surabaya",
      "location_name": "Surabaya"
    },
    "arr_airport": {
      "airport_code": "LOP",
      "international": "1",
      "trans_name_id": "7583",
      "banner_image": null,
      "short_name_trans_id": "1193670",
      "business_name": "Lombok",
      "business_name_trans_id": "5947",
      "business_country": "id",
      "business_id": "20373",
      "country_name": "Indonesia",
      "city_name": "Mataram",
      "province_name": "Nusa Tenggara Barat",
      "short_name": "Lombok",
      "location_name": "Lombok, Mataram"
    },
    "date": "2016-08-04",
    "formatted_date": "04 Agustus 2016"
  },
  "ret_det": {
    "dep_airport": {
      "airport_code": "LOP",
      "international": "1",
      "trans_name_id": "7583",
      "banner_image": null,
      "short_name_trans_id": "1193670",
      "business_name": "Lombok",
      "business_name_trans_id": "5947",
      "business_country": "id",
      "business_id": "20373",
      "country_name": "Indonesia",
      "city_name": "Mataram",
      "province_name": "Nusa Tenggara Barat",
      "short_name": "Lombok",
      "location_name": "Lombok, Mataram"
    },
    "arr_airport": {
      "airport_code": "SUB",
      "international": "1",
      "trans_name_id": "7595",
      "banner_image": null,
      "short_name_trans_id": "1193620",
      "business_name": "Juanda",
      "business_name_trans_id": "5963",
      "business_country": "id",
      "business_id": "20389",
      "country_name": "Indonesia",
      "city_name": "Surabaya",
      "province_name": "Jawa Timur",
      "short_name": "Surabaya",
      "location_name": "Surabaya"
    },
    "date": "2016-08-05",
    "formatted_date": "05 Agustus 2016"
  },
  "departures": {
    "result": [
      {
        "flight_id": "2490729",
        "airlines_name": "CITILINK",
        "flight_number": "QG-660",
        "departure_city": "SUB",
        "arrival_city": "LOP",
        "stop": "Langsung",
        "price_value": "936900.00",
        "price_adult": "936900.00",
        "price_child": "0.00",
        "price_infant": "0.00",
        "timestamp": "2016-08-04 11:23:25",
        "has_food": "0",
        "check_in_baggage": "20",
        "is_promo": 0,
        "airport_tax": true,
        "simple_departure_time": "15:25",
        "simple_arrival_time": "17:35",
        "long_via": "",
        "departure_city_name": "Surabaya",
        "arrival_city_name": "Lombok",
        "full_via": "SUB - LOP (15:25 - 17:35)",
        "markup_price_string": "",
        "need_baggage": 0,
        "best_deal": false,
        "duration": "1 j 10 m",
        "image": "http://api-sandbox.tiket.com/images/tiket2/icon_citilink_2.jpg",
        "flight_infos": {
          "flight_info": [
            {
              "flight_number": "QG-660",
              "airlines_name": "CITILINK",
              "airlines_short_real_name": "Citilink",
              "airlines_short_real_name_ucwords": "Citilink",
              "departure_city": "SUB",
              "arrival_city": "LOP",
              "simple_departure_time": "15:25",
              "simple_arrival_time": "17:35",
              "img": "<img width=\"52\" height=\"45\" src=\"http://api-sandbox.tiket.com/images/flight/logo/icon_citilink.png\" title=\"Citilink\" alt=\"QG-660 SUB LOP 15:25\" />",
              "img_src": "http://api-sandbox.tiket.com/images/flight/logo/icon_citilink.png",
              "check_in_baggage": 20,
              "terminal": "",
              "departure_city_name": "Surabaya",
              "arrival_city_name": "Lombok",
              "duration": {
                "hour": 0,
                "minute": 0,
                "arrival_time": "2016-08-04 17:35:00",
                "arrival_city": "LOP",
                "text_city": "",
                "text_time": ""
              },
              "duration_time": 4200,
              "duration_hour": "1j",
              "duration_minute": "10m"
            }
          ]
        },
        "sss_key": null
      }
    ]
  },
  "returns": {
    "result": [
      {
        "flight_id": "2490731",
        "airlines_name": "CITILINK",
        "flight_number": "QG-665",
        "departure_city": "LOP",
        "arrival_city": "SUB",
        "stop": "Langsung",
        "price_value": "693720.00",
        "price_adult": "693720.00",
        "price_child": "0.00",
        "price_infant": "0.00",
        "timestamp": "2016-08-04 11:28:03",
        "has_food": "0",
        "check_in_baggage": "20",
        "is_promo": 0,
        "airport_tax": true,
        "simple_departure_time": "12:00",
        "simple_arrival_time": "12:15",
        "long_via": "",
        "departure_city_name": "Lombok",
        "arrival_city_name": "Surabaya",
        "full_via": "LOP - SUB (12:00 - 12:15)",
        "markup_price_string": "",
        "need_baggage": 0,
        "best_deal": false,
        "duration": "1 j 15 m",
        "image": "http://api-sandbox.tiket.com/images/tiket2/icon_citilink_2.jpg",
        "flight_infos": {
          "flight_info": [
            {
              "flight_number": "QG-665",
              "airlines_name": "CITILINK",
              "airlines_short_real_name": "Citilink",
              "airlines_short_real_name_ucwords": "Citilink",
              "departure_city": "LOP",
              "arrival_city": "SUB",
              "simple_departure_time": "12:00",
              "simple_arrival_time": "12:15",
              "img": "<img width=\"52\" height=\"45\" src=\"http://api-sandbox.tiket.com/images/flight/logo/icon_citilink.png\" title=\"Citilink\" alt=\"QG-665 LOP SUB 12:00\" />",
              "img_src": "http://api-sandbox.tiket.com/images/flight/logo/icon_citilink.png",
              "check_in_baggage": 20,
              "terminal": "",
              "departure_city_name": "Lombok",
              "arrival_city_name": "Surabaya",
              "duration": {
                "hour": 0,
                "minute": 0,
                "arrival_time": "2016-08-05 12:15:00",
                "arrival_city": "SUB",
                "text_city": "",
                "text_time": ""
              },
              "duration_time": 4500,
              "duration_hour": "1j",
              "duration_minute": "15m"
            }
          ]
        },
        "sss_key": null
      },
      {
        "flight_id": "2490733",
        "airlines_name": "CITILINK",
        "flight_number": "QG-661",
        "departure_city": "LOP",
        "arrival_city": "SUB",
        "stop": "Langsung",
        "price_value": "693720.00",
        "price_adult": "693720.00",
        "price_child": "0.00",
        "price_infant": "0.00",
        "timestamp": "2016-08-04 11:28:03",
        "has_food": "0",
        "check_in_baggage": "20",
        "is_promo": 0,
        "airport_tax": true,
        "simple_departure_time": "18:05",
        "simple_arrival_time": "18:10",
        "long_via": "",
        "departure_city_name": "Lombok",
        "arrival_city_name": "Surabaya",
        "full_via": "LOP - SUB (18:05 - 18:10)",
        "markup_price_string": "",
        "need_baggage": 0,
        "best_deal": false,
        "duration": "1 j 5 m",
        "image": "http://api-sandbox.tiket.com/images/tiket2/icon_citilink_2.jpg",
        "flight_infos": {
          "flight_info": [
            {
              "flight_number": "QG-661",
              "airlines_name": "CITILINK",
              "airlines_short_real_name": "Citilink",
              "airlines_short_real_name_ucwords": "Citilink",
              "departure_city": "LOP",
              "arrival_city": "SUB",
              "simple_departure_time": "18:05",
              "simple_arrival_time": "18:10",
              "img": "<img width=\"52\" height=\"45\" src=\"http://api-sandbox.tiket.com/images/flight/logo/icon_citilink.png\" title=\"Citilink\" alt=\"QG-661 LOP SUB 18:05\" />",
              "img_src": "http://api-sandbox.tiket.com/images/flight/logo/icon_citilink.png",
              "check_in_baggage": 20,
              "terminal": "",
              "departure_city_name": "Lombok",
              "arrival_city_name": "Surabaya",
              "duration": {
                "hour": 0,
                "minute": 0,
                "arrival_time": "2016-08-05 18:10:00",
                "arrival_city": "SUB",
                "text_city": "",
                "text_time": ""
              },
              "duration_time": 3900,
              "duration_hour": "1j",
              "duration_minute": "5m"
            }
          ]
        },
        "sss_key": null
      },
      {
        "flight_id": "2490735",
        "airlines_name": "GARUDA",
        "flight_number": "GA-365",
        "departure_city": "LOP",
        "arrival_city": "SUB",
        "stop": "Langsung",
        "price_value": "930000.00",
        "price_adult": "930000.00",
        "price_child": "0.00",
        "price_infant": "0.00",
        "timestamp": "2016-08-04 11:28:06",
        "has_food": "1",
        "check_in_baggage": "20",
        "is_promo": 0,
        "airport_tax": true,
        "simple_departure_time": "14:25",
        "simple_arrival_time": "14:30",
        "long_via": "",
        "departure_city_name": "Lombok",
        "arrival_city_name": "Surabaya",
        "full_via": "LOP - SUB (14:25 - 14:30)",
        "markup_price_string": "",
        "need_baggage": 0,
        "best_deal": false,
        "duration": "1 j 5 m",
        "image": "http://api-sandbox.tiket.com/images/tiket2/icon_garuda_2.jpg",
        "flight_infos": {
          "flight_info": [
            {
              "flight_number": "GA-365",
              "airlines_name": "GARUDA",
              "airlines_short_real_name": "Garuda",
              "airlines_short_real_name_ucwords": "Garuda",
              "departure_city": "LOP",
              "arrival_city": "SUB",
              "simple_departure_time": "14:25",
              "simple_arrival_time": "14:30",
              "img": "<img width=\"52\" height=\"45\" src=\"http://api-sandbox.tiket.com/images/flight/logo/icon_garuda.png\" title=\"Garuda Indonesia\" alt=\"GA-365 LOP SUB 14:25\" />",
              "img_src": "http://api-sandbox.tiket.com/images/flight/logo/icon_garuda.png",
              "check_in_baggage": 20,
              "terminal": "",
              "departure_city_name": "Lombok",
              "arrival_city_name": "Surabaya",
              "duration": {
                "hour": 0,
                "minute": 0,
                "arrival_time": "2016-08-05 14:30:00",
                "arrival_city": "SUB",
                "text_city": "",
                "text_time": ""
              },
              "duration_time": 3900,
              "duration_hour": "1j",
              "duration_minute": "5m"
            }
          ]
        },
        "sss_key": null
      },
      {
        "flight_id": "2490737",
        "airlines_name": "LION",
        "flight_number": "JT-823",
        "departure_city": "LOP",
        "arrival_city": "SUB",
        "stop": "Langsung",
        "price_value": "501000.00",
        "price_adult": "501000.00",
        "price_child": "0.00",
        "price_infant": "0.00",
        "timestamp": "2016-08-04 11:28:07",
        "has_food": "0",
        "check_in_baggage": "20",
        "is_promo": 0,
        "airport_tax": true,
        "simple_departure_time": "07:00",
        "simple_arrival_time": "07:00",
        "long_via": "",
        "departure_city_name": "Lombok",
        "arrival_city_name": "Surabaya",
        "full_via": "LOP - SUB (07:00 - 07:00)",
        "markup_price_string": "",
        "need_baggage": 0,
        "best_deal": false,
        "duration": "1 j 0 m",
        "image": "http://api-sandbox.tiket.com/images/tiket2/icon_lion_2.jpg",
        "flight_infos": {
          "flight_info": [
            {
              "flight_number": "JT-823",
              "airlines_name": "LION",
              "airlines_short_real_name": "Lion",
              "airlines_short_real_name_ucwords": "Lion",
              "departure_city": "LOP",
              "arrival_city": "SUB",
              "simple_departure_time": "07:00",
              "simple_arrival_time": "07:00",
              "img": "<img width=\"52\" height=\"45\" src=\"http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png\" title=\"Lion Air\" alt=\"JT-823 LOP SUB 07:00\" />",
              "img_src": "http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png",
              "check_in_baggage": 20,
              "terminal": "",
              "departure_city_name": "Lombok",
              "arrival_city_name": "Surabaya",
              "duration": {
                "hour": 0,
                "minute": 0,
                "arrival_time": "2016-08-05 07:00:00",
                "arrival_city": "SUB",
                "text_city": "",
                "text_time": ""
              },
              "duration_time": 3600,
              "duration_hour": "1j",
              "duration_minute": ""
            }
          ]
        },
        "sss_key": null
      },
      {
        "flight_id": "2490739",
        "airlines_name": "LION",
        "flight_number": "JT-645",
        "departure_city": "LOP",
        "arrival_city": "SUB",
        "stop": "Langsung",
        "price_value": "501000.00",
        "price_adult": "501000.00",
        "price_child": "0.00",
        "price_infant": "0.00",
        "timestamp": "2016-08-04 11:28:07",
        "has_food": "0",
        "check_in_baggage": "20",
        "is_promo": 0,
        "airport_tax": true,
        "simple_departure_time": "08:40",
        "simple_arrival_time": "08:35",
        "long_via": "",
        "departure_city_name": "Lombok",
        "arrival_city_name": "Surabaya",
        "full_via": "LOP - SUB (08:40 - 08:35)",
        "markup_price_string": "",
        "need_baggage": 0,
        "best_deal": false,
        "duration": "0 j 55 m",
        "image": "http://api-sandbox.tiket.com/images/tiket2/icon_lion_2.jpg",
        "flight_infos": {
          "flight_info": [
            {
              "flight_number": "JT-645",
              "airlines_name": "LION",
              "airlines_short_real_name": "Lion",
              "airlines_short_real_name_ucwords": "Lion",
              "departure_city": "LOP",
              "arrival_city": "SUB",
              "simple_departure_time": "08:40",
              "simple_arrival_time": "08:35",
              "img": "<img width=\"52\" height=\"45\" src=\"http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png\" title=\"Lion Air\" alt=\"JT-645 LOP SUB 08:40\" />",
              "img_src": "http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png",
              "check_in_baggage": 20,
              "terminal": "",
              "departure_city_name": "Lombok",
              "arrival_city_name": "Surabaya",
              "duration": {
                "hour": 0,
                "minute": 0,
                "arrival_time": "2016-08-05 08:35:00",
                "arrival_city": "SUB",
                "text_city": "",
                "text_time": ""
              },
              "duration_time": 3300,
              "duration_hour": "",
              "duration_minute": "55m"
            }
          ]
        },
        "sss_key": null
      },
      {
        "flight_id": "2490741",
        "airlines_name": "LION",
        "flight_number": "JT-865",
        "departure_city": "LOP",
        "arrival_city": "SUB",
        "stop": "Langsung",
        "price_value": "501000.00",
        "price_adult": "501000.00",
        "price_child": "0.00",
        "price_infant": "0.00",
        "timestamp": "2016-08-04 11:28:07",
        "has_food": "0",
        "check_in_baggage": "20",
        "is_promo": 0,
        "airport_tax": true,
        "simple_departure_time": "09:40",
        "simple_arrival_time": "09:35",
        "long_via": "",
        "departure_city_name": "Lombok",
        "arrival_city_name": "Surabaya",
        "full_via": "LOP - SUB (09:40 - 09:35)",
        "markup_price_string": "",
        "need_baggage": 0,
        "best_deal": false,
        "duration": "0 j 55 m",
        "image": "http://api-sandbox.tiket.com/images/tiket2/icon_lion_2.jpg",
        "flight_infos": {
          "flight_info": [
            {
              "flight_number": "JT-865",
              "airlines_name": "LION",
              "airlines_short_real_name": "Lion",
              "airlines_short_real_name_ucwords": "Lion",
              "departure_city": "LOP",
              "arrival_city": "SUB",
              "simple_departure_time": "09:40",
              "simple_arrival_time": "09:35",
              "img": "<img width=\"52\" height=\"45\" src=\"http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png\" title=\"Lion Air\" alt=\"JT-865 LOP SUB 09:40\" />",
              "img_src": "http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png",
              "check_in_baggage": 20,
              "terminal": "",
              "departure_city_name": "Lombok",
              "arrival_city_name": "Surabaya",
              "duration": {
                "hour": 0,
                "minute": 0,
                "arrival_time": "2016-08-05 09:35:00",
                "arrival_city": "SUB",
                "text_city": "",
                "text_time": ""
              },
              "duration_time": 3300,
              "duration_hour": "",
              "duration_minute": "55m"
            }
          ]
        },
        "sss_key": null
      },
      {
        "flight_id": "2490743",
        "airlines_name": "LION",
        "flight_number": "JT-177",
        "departure_city": "LOP",
        "arrival_city": "SUB",
        "stop": "Langsung",
        "price_value": "501000.00",
        "price_adult": "501000.00",
        "price_child": "0.00",
        "price_infant": "0.00",
        "timestamp": "2016-08-04 11:28:07",
        "has_food": "0",
        "check_in_baggage": "20",
        "is_promo": 0,
        "airport_tax": true,
        "simple_departure_time": "12:15",
        "simple_arrival_time": "12:10",
        "long_via": "",
        "departure_city_name": "Lombok",
        "arrival_city_name": "Surabaya",
        "full_via": "LOP - SUB (12:15 - 12:10)",
        "markup_price_string": "",
        "need_baggage": 0,
        "best_deal": false,
        "duration": "0 j 55 m",
        "image": "http://api-sandbox.tiket.com/images/tiket2/icon_lion_2.jpg",
        "flight_infos": {
          "flight_info": [
            {
              "flight_number": "JT-177",
              "airlines_name": "LION",
              "airlines_short_real_name": "Lion",
              "airlines_short_real_name_ucwords": "Lion",
              "departure_city": "LOP",
              "arrival_city": "SUB",
              "simple_departure_time": "12:15",
              "simple_arrival_time": "12:10",
              "img": "<img width=\"52\" height=\"45\" src=\"http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png\" title=\"Lion Air\" alt=\"JT-177 LOP SUB 12:15\" />",
              "img_src": "http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png",
              "check_in_baggage": 20,
              "terminal": "",
              "departure_city_name": "Lombok",
              "arrival_city_name": "Surabaya",
              "duration": {
                "hour": 0,
                "minute": 0,
                "arrival_time": "2016-08-05 12:10:00",
                "arrival_city": "SUB",
                "text_city": "",
                "text_time": ""
              },
              "duration_time": 3300,
              "duration_hour": "",
              "duration_minute": "55m"
            }
          ]
        },
        "sss_key": null
      }
    ]
  },
  "nearby_go_date": {
    "nearby": [
      {
        "date": "2016-08-04",
        "price": "936900.00"
      },
      {
        "date": "2016-08-05"
      },
      {
        "date": "2016-08-06"
      },
      {
        "date": "2016-08-07"
      },
      {
        "date": "2016-08-08"
      },
      {
        "date": "2016-08-09"
      }
    ]
  },
  "nearby_ret_date": {
    "nearby": [
      {
        "date": "2016-08-04"
      },
      {
        "date": "2016-08-05",
        "price": "501000.00"
      },
      {
        "date": "2016-08-06"
      },
      {
        "date": "2016-08-07"
      },
      {
        "date": "2016-08-08"
      },
      {
        "date": "2016-08-09"
      },
      {
        "date": "2016-08-10"
      }
    ]
  },
  "login_status": "false",
  "token": "f9b29ac359ca5d77755e7588751c089bf96f0dc9"
}
```



```matlab
a:12:{s:10:"diagnostic";a:7:{s:6:"status";i:200;s:10:"elapsetime";s:14:"0.3891";s:11:"memoryusage";s:14:"8.42MB";s:14:"unix_timestamp";i:1470285575;s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:11:"output_type";s:9:"serialize";s:10:"round_trip";b:1;s:14:"search_queries";a:8:{s:4:"from";s:3:"SUB";s:2:"to";s:3:"LOP";s:4:"date";s:10:"2016-08-04";s:8:"ret_date";s:10:"2016-08-05";s:5:"adult";i:1;s:5:"child";i:0;s:6:"infant";i:0;s:4:"sort";b:0;}s:6:"go_det";a:4:{s:11:"dep_airport";a:14:{s:12:"airport_code";s:3:"SUB";s:13:"international";s:1:"1";s:13:"trans_name_id";s:4:"7595";s:12:"banner_image";N;s:19:"short_name_trans_id";s:7:"1193620";s:13:"business_name";s:6:"Juanda";s:22:"business_name_trans_id";s:4:"5963";s:16:"business_country";s:2:"id";s:11:"business_id";s:5:"20389";s:12:"country_name";s:9:"Indonesia";s:9:"city_name";s:8:"Surabaya";s:13:"province_name";s:10:"Jawa Timur";s:10:"short_name";s:8:"Surabaya";s:13:"location_name";s:8:"Surabaya";}s:11:"arr_airport";a:14:{s:12:"airport_code";s:3:"LOP";s:13:"international";s:1:"1";s:13:"trans_name_id";s:4:"7583";s:12:"banner_image";N;s:19:"short_name_trans_id";s:7:"1193670";s:13:"business_name";s:6:"Lombok";s:22:"business_name_trans_id";s:4:"5947";s:16:"business_country";s:2:"id";s:11:"business_id";s:5:"20373";s:12:"country_name";s:9:"Indonesia";s:9:"city_name";s:7:"Mataram";s:13:"province_name";s:19:"Nusa Tenggara Barat";s:10:"short_name";s:6:"Lombok";s:13:"location_name";s:15:"Lombok, Mataram";}s:4:"date";s:10:"2016-08-04";s:14:"formatted_date";s:15:"04 Agustus 2016";}s:7:"ret_det";a:4:{s:11:"dep_airport";a:14:{s:12:"airport_code";s:3:"LOP";s:13:"international";s:1:"1";s:13:"trans_name_id";s:4:"7583";s:12:"banner_image";N;s:19:"short_name_trans_id";s:7:"1193670";s:13:"business_name";s:6:"Lombok";s:22:"business_name_trans_id";s:4:"5947";s:16:"business_country";s:2:"id";s:11:"business_id";s:5:"20373";s:12:"country_name";s:9:"Indonesia";s:9:"city_name";s:7:"Mataram";s:13:"province_name";s:19:"Nusa Tenggara Barat";s:10:"short_name";s:6:"Lombok";s:13:"location_name";s:15:"Lombok, Mataram";}s:11:"arr_airport";a:14:{s:12:"airport_code";s:3:"SUB";s:13:"international";s:1:"1";s:13:"trans_name_id";s:4:"7595";s:12:"banner_image";N;s:19:"short_name_trans_id";s:7:"1193620";s:13:"business_name";s:6:"Juanda";s:22:"business_name_trans_id";s:4:"5963";s:16:"business_country";s:2:"id";s:11:"business_id";s:5:"20389";s:12:"country_name";s:9:"Indonesia";s:9:"city_name";s:8:"Surabaya";s:13:"province_name";s:10:"Jawa Timur";s:10:"short_name";s:8:"Surabaya";s:13:"location_name";s:8:"Surabaya";}s:4:"date";s:10:"2016-08-05";s:14:"formatted_date";s:15:"05 Agustus 2016";}s:10:"departures";a:1:{s:6:"result";a:1:{i:0;a:28:{s:9:"flight_id";s:7:"2490729";s:13:"airlines_name";s:8:"CITILINK";s:13:"flight_number";s:6:"QG-660";s:14:"departure_city";s:3:"SUB";s:12:"arrival_city";s:3:"LOP";s:4:"stop";s:8:"Langsung";s:11:"price_value";s:9:"936900.00";s:11:"price_adult";s:9:"936900.00";s:11:"price_child";s:4:"0.00";s:12:"price_infant";s:4:"0.00";s:9:"timestamp";s:19:"2016-08-04 11:23:25";s:8:"has_food";s:1:"0";s:16:"check_in_baggage";s:2:"20";s:8:"is_promo";i:0;s:11:"airport_tax";b:1;s:21:"simple_departure_time";s:5:"15:25";s:19:"simple_arrival_time";s:5:"17:35";s:8:"long_via";s:0:"";s:19:"departure_city_name";s:8:"Surabaya";s:17:"arrival_city_name";s:6:"Lombok";s:8:"full_via";s:25:"SUB - LOP (15:25 - 17:35)";s:19:"markup_price_string";s:0:"";s:12:"need_baggage";i:0;s:9:"best_deal";b:0;s:8:"duration";s:26:"1 j 10 m";s:5:"image";s:62:"http://api-sandbox.tiket.com/images/tiket2/icon_citilink_2.jpg";s:12:"flight_infos";a:1:{s:11:"flight_info";a:1:{i:0;a:18:{s:13:"flight_number";s:6:"QG-660";s:13:"airlines_name";s:8:"CITILINK";s:24:"airlines_short_real_name";s:8:"Citilink";s:32:"airlines_short_real_name_ucwords";s:8:"Citilink";s:14:"departure_city";s:3:"SUB";s:12:"arrival_city";s:3:"LOP";s:21:"simple_departure_time";s:5:"15:25";s:19:"simple_arrival_time";s:5:"17:35";s:3:"img";s:146:"
<img width="52" height="45" src="http://api-sandbox.tiket.com/images/flight/logo/icon_citilink.png" title="Citilink" alt="QG-660 SUB LOP 15:25" />";s:7:"img_src";s:65:"http://api-sandbox.tiket.com/images/flight/logo/icon_citilink.png";s:16:"check_in_baggage";i:20;s:8:"terminal";s:0:"";s:19:"departure_city_name";s:8:"Surabaya";s:17:"arrival_city_name";s:6:"Lombok";s:8:"duration";a:6:{s:4:"hour";i:0;s:6:"minute";i:0;s:12:"arrival_time";s:19:"2016-08-04 17:35:00";s:12:"arrival_city";s:3:"LOP";s:9:"text_city";s:0:"";s:9:"text_time";s:0:"";}s:13:"duration_time";i:4200;s:13:"duration_hour";s:2:"1j";s:15:"duration_minute";s:3:"10m";}}}s:7:"sss_key";N;}}}s:7:"returns";a:1:{s:6:"result";a:7:{i:0;a:28:{s:9:"flight_id";s:7:"2490731";s:13:"airlines_name";s:8:"CITILINK";s:13:"flight_number";s:6:"QG-665";s:14:"departure_city";s:3:"LOP";s:12:"arrival_city";s:3:"SUB";s:4:"stop";s:8:"Langsung";s:11:"price_value";s:9:"693720.00";s:11:"price_adult";s:9:"693720.00";s:11:"price_child";s:4:"0.00";s:12:"price_infant";s:4:"0.00";s:9:"timestamp";s:19:"2016-08-04 11:28:03";s:8:"has_food";s:1:"0";s:16:"check_in_baggage";s:2:"20";s:8:"is_promo";i:0;s:11:"airport_tax";b:1;s:21:"simple_departure_time";s:5:"12:00";s:19:"simple_arrival_time";s:5:"12:15";s:8:"long_via";s:0:"";s:19:"departure_city_name";s:6:"Lombok";s:17:"arrival_city_name";s:8:"Surabaya";s:8:"full_via";s:25:"LOP - SUB (12:00 - 12:15)";s:19:"markup_price_string";s:0:"";s:12:"need_baggage";i:0;s:9:"best_deal";b:0;s:8:"duration";s:26:"1 j 15 m";s:5:"image";s:62:"http://api-sandbox.tiket.com/images/tiket2/icon_citilink_2.jpg";s:12:"flight_infos";a:1:{s:11:"flight_info";a:1:{i:0;a:18:{s:13:"flight_number";s:6:"QG-665";s:13:"airlines_name";s:8:"CITILINK";s:24:"airlines_short_real_name";s:8:"Citilink";s:32:"airlines_short_real_name_ucwords";s:8:"Citilink";s:14:"departure_city";s:3:"LOP";s:12:"arrival_city";s:3:"SUB";s:21:"simple_departure_time";s:5:"12:00";s:19:"simple_arrival_time";s:5:"12:15";s:3:"img";s:146:"
<img width="52" height="45" src="http://api-sandbox.tiket.com/images/flight/logo/icon_citilink.png" title="Citilink" alt="QG-665 LOP SUB 12:00" />";s:7:"img_src";s:65:"http://api-sandbox.tiket.com/images/flight/logo/icon_citilink.png";s:16:"check_in_baggage";i:20;s:8:"terminal";s:0:"";s:19:"departure_city_name";s:6:"Lombok";s:17:"arrival_city_name";s:8:"Surabaya";s:8:"duration";a:6:{s:4:"hour";i:0;s:6:"minute";i:0;s:12:"arrival_time";s:19:"2016-08-05 12:15:00";s:12:"arrival_city";s:3:"SUB";s:9:"text_city";s:0:"";s:9:"text_time";s:0:"";}s:13:"duration_time";i:4500;s:13:"duration_hour";s:2:"1j";s:15:"duration_minute";s:3:"15m";}}}s:7:"sss_key";N;}i:1;a:28:{s:9:"flight_id";s:7:"2490733";s:13:"airlines_name";s:8:"CITILINK";s:13:"flight_number";s:6:"QG-661";s:14:"departure_city";s:3:"LOP";s:12:"arrival_city";s:3:"SUB";s:4:"stop";s:8:"Langsung";s:11:"price_value";s:9:"693720.00";s:11:"price_adult";s:9:"693720.00";s:11:"price_child";s:4:"0.00";s:12:"price_infant";s:4:"0.00";s:9:"timestamp";s:19:"2016-08-04 11:28:03";s:8:"has_food";s:1:"0";s:16:"check_in_baggage";s:2:"20";s:8:"is_promo";i:0;s:11:"airport_tax";b:1;s:21:"simple_departure_time";s:5:"18:05";s:19:"simple_arrival_time";s:5:"18:10";s:8:"long_via";s:0:"";s:19:"departure_city_name";s:6:"Lombok";s:17:"arrival_city_name";s:8:"Surabaya";s:8:"full_via";s:25:"LOP - SUB (18:05 - 18:10)";s:19:"markup_price_string";s:0:"";s:12:"need_baggage";i:0;s:9:"best_deal";b:0;s:8:"duration";s:25:"1 j 5 m";s:5:"image";s:62:"http://api-sandbox.tiket.com/images/tiket2/icon_citilink_2.jpg";s:12:"flight_infos";a:1:{s:11:"flight_info";a:1:{i:0;a:18:{s:13:"flight_number";s:6:"QG-661";s:13:"airlines_name";s:8:"CITILINK";s:24:"airlines_short_real_name";s:8:"Citilink";s:32:"airlines_short_real_name_ucwords";s:8:"Citilink";s:14:"departure_city";s:3:"LOP";s:12:"arrival_city";s:3:"SUB";s:21:"simple_departure_time";s:5:"18:05";s:19:"simple_arrival_time";s:5:"18:10";s:3:"img";s:146:"
<img width="52" height="45" src="http://api-sandbox.tiket.com/images/flight/logo/icon_citilink.png" title="Citilink" alt="QG-661 LOP SUB 18:05" />";s:7:"img_src";s:65:"http://api-sandbox.tiket.com/images/flight/logo/icon_citilink.png";s:16:"check_in_baggage";i:20;s:8:"terminal";s:0:"";s:19:"departure_city_name";s:6:"Lombok";s:17:"arrival_city_name";s:8:"Surabaya";s:8:"duration";a:6:{s:4:"hour";i:0;s:6:"minute";i:0;s:12:"arrival_time";s:19:"2016-08-05 18:10:00";s:12:"arrival_city";s:3:"SUB";s:9:"text_city";s:0:"";s:9:"text_time";s:0:"";}s:13:"duration_time";i:3900;s:13:"duration_hour";s:2:"1j";s:15:"duration_minute";s:2:"5m";}}}s:7:"sss_key";N;}i:2;a:28:{s:9:"flight_id";s:7:"2490735";s:13:"airlines_name";s:6:"GARUDA";s:13:"flight_number";s:6:"GA-365";s:14:"departure_city";s:3:"LOP";s:12:"arrival_city";s:3:"SUB";s:4:"stop";s:8:"Langsung";s:11:"price_value";s:9:"930000.00";s:11:"price_adult";s:9:"930000.00";s:11:"price_child";s:4:"0.00";s:12:"price_infant";s:4:"0.00";s:9:"timestamp";s:19:"2016-08-04 11:28:06";s:8:"has_food";s:1:"1";s:16:"check_in_baggage";s:2:"20";s:8:"is_promo";i:0;s:11:"airport_tax";b:1;s:21:"simple_departure_time";s:5:"14:25";s:19:"simple_arrival_time";s:5:"14:30";s:8:"long_via";s:0:"";s:19:"departure_city_name";s:6:"Lombok";s:17:"arrival_city_name";s:8:"Surabaya";s:8:"full_via";s:25:"LOP - SUB (14:25 - 14:30)";s:19:"markup_price_string";s:0:"";s:12:"need_baggage";i:0;s:9:"best_deal";b:0;s:8:"duration";s:25:"1 j 5 m";s:5:"image";s:60:"http://api-sandbox.tiket.com/images/tiket2/icon_garuda_2.jpg";s:12:"flight_infos";a:1:{s:11:"flight_info";a:1:{i:0;a:18:{s:13:"flight_number";s:6:"GA-365";s:13:"airlines_name";s:6:"GARUDA";s:24:"airlines_short_real_name";s:6:"Garuda";s:32:"airlines_short_real_name_ucwords";s:6:"Garuda";s:14:"departure_city";s:3:"LOP";s:12:"arrival_city";s:3:"SUB";s:21:"simple_departure_time";s:5:"14:25";s:19:"simple_arrival_time";s:5:"14:30";s:3:"img";s:152:"
<img width="52" height="45" src="http://api-sandbox.tiket.com/images/flight/logo/icon_garuda.png" title="Garuda Indonesia" alt="GA-365 LOP SUB 14:25" />";s:7:"img_src";s:63:"http://api-sandbox.tiket.com/images/flight/logo/icon_garuda.png";s:16:"check_in_baggage";i:20;s:8:"terminal";s:0:"";s:19:"departure_city_name";s:6:"Lombok";s:17:"arrival_city_name";s:8:"Surabaya";s:8:"duration";a:6:{s:4:"hour";i:0;s:6:"minute";i:0;s:12:"arrival_time";s:19:"2016-08-05 14:30:00";s:12:"arrival_city";s:3:"SUB";s:9:"text_city";s:0:"";s:9:"text_time";s:0:"";}s:13:"duration_time";i:3900;s:13:"duration_hour";s:2:"1j";s:15:"duration_minute";s:2:"5m";}}}s:7:"sss_key";N;}i:3;a:28:{s:9:"flight_id";s:7:"2490737";s:13:"airlines_name";s:4:"LION";s:13:"flight_number";s:6:"JT-823";s:14:"departure_city";s:3:"LOP";s:12:"arrival_city";s:3:"SUB";s:4:"stop";s:8:"Langsung";s:11:"price_value";s:9:"501000.00";s:11:"price_adult";s:9:"501000.00";s:11:"price_child";s:4:"0.00";s:12:"price_infant";s:4:"0.00";s:9:"timestamp";s:19:"2016-08-04 11:28:07";s:8:"has_food";s:1:"0";s:16:"check_in_baggage";s:2:"20";s:8:"is_promo";i:0;s:11:"airport_tax";b:1;s:21:"simple_departure_time";s:5:"07:00";s:19:"simple_arrival_time";s:5:"07:00";s:8:"long_via";s:0:"";s:19:"departure_city_name";s:6:"Lombok";s:17:"arrival_city_name";s:8:"Surabaya";s:8:"full_via";s:25:"LOP - SUB (07:00 - 07:00)";s:19:"markup_price_string";s:0:"";s:12:"need_baggage";i:0;s:9:"best_deal";b:0;s:8:"duration";s:25:"1 j 0 m";s:5:"image";s:58:"http://api-sandbox.tiket.com/images/tiket2/icon_lion_2.jpg";s:12:"flight_infos";a:1:{s:11:"flight_info";a:1:{i:0;a:18:{s:13:"flight_number";s:6:"JT-823";s:13:"airlines_name";s:4:"LION";s:24:"airlines_short_real_name";s:4:"Lion";s:32:"airlines_short_real_name_ucwords";s:4:"Lion";s:14:"departure_city";s:3:"LOP";s:12:"arrival_city";s:3:"SUB";s:21:"simple_departure_time";s:5:"07:00";s:19:"simple_arrival_time";s:5:"07:00";s:3:"img";s:142:"
<img width="52" height="45" src="http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png" title="Lion Air" alt="JT-823 LOP SUB 07:00" />";s:7:"img_src";s:61:"http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png";s:16:"check_in_baggage";i:20;s:8:"terminal";s:0:"";s:19:"departure_city_name";s:6:"Lombok";s:17:"arrival_city_name";s:8:"Surabaya";s:8:"duration";a:6:{s:4:"hour";i:0;s:6:"minute";i:0;s:12:"arrival_time";s:19:"2016-08-05 07:00:00";s:12:"arrival_city";s:3:"SUB";s:9:"text_city";s:0:"";s:9:"text_time";s:0:"";}s:13:"duration_time";i:3600;s:13:"duration_hour";s:2:"1j";s:15:"duration_minute";s:0:"";}}}s:7:"sss_key";N;}i:4;a:28:{s:9:"flight_id";s:7:"2490739";s:13:"airlines_name";s:4:"LION";s:13:"flight_number";s:6:"JT-645";s:14:"departure_city";s:3:"LOP";s:12:"arrival_city";s:3:"SUB";s:4:"stop";s:8:"Langsung";s:11:"price_value";s:9:"501000.00";s:11:"price_adult";s:9:"501000.00";s:11:"price_child";s:4:"0.00";s:12:"price_infant";s:4:"0.00";s:9:"timestamp";s:19:"2016-08-04 11:28:07";s:8:"has_food";s:1:"0";s:16:"check_in_baggage";s:2:"20";s:8:"is_promo";i:0;s:11:"airport_tax";b:1;s:21:"simple_departure_time";s:5:"08:40";s:19:"simple_arrival_time";s:5:"08:35";s:8:"long_via";s:0:"";s:19:"departure_city_name";s:6:"Lombok";s:17:"arrival_city_name";s:8:"Surabaya";s:8:"full_via";s:25:"LOP - SUB (08:40 - 08:35)";s:19:"markup_price_string";s:0:"";s:12:"need_baggage";i:0;s:9:"best_deal";b:0;s:8:"duration";s:26:"0 j 55 m";s:5:"image";s:58:"http://api-sandbox.tiket.com/images/tiket2/icon_lion_2.jpg";s:12:"flight_infos";a:1:{s:11:"flight_info";a:1:{i:0;a:18:{s:13:"flight_number";s:6:"JT-645";s:13:"airlines_name";s:4:"LION";s:24:"airlines_short_real_name";s:4:"Lion";s:32:"airlines_short_real_name_ucwords";s:4:"Lion";s:14:"departure_city";s:3:"LOP";s:12:"arrival_city";s:3:"SUB";s:21:"simple_departure_time";s:5:"08:40";s:19:"simple_arrival_time";s:5:"08:35";s:3:"img";s:142:"
<img width="52" height="45" src="http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png" title="Lion Air" alt="JT-645 LOP SUB 08:40" />";s:7:"img_src";s:61:"http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png";s:16:"check_in_baggage";i:20;s:8:"terminal";s:0:"";s:19:"departure_city_name";s:6:"Lombok";s:17:"arrival_city_name";s:8:"Surabaya";s:8:"duration";a:6:{s:4:"hour";i:0;s:6:"minute";i:0;s:12:"arrival_time";s:19:"2016-08-05 08:35:00";s:12:"arrival_city";s:3:"SUB";s:9:"text_city";s:0:"";s:9:"text_time";s:0:"";}s:13:"duration_time";i:3300;s:13:"duration_hour";s:0:"";s:15:"duration_minute";s:3:"55m";}}}s:7:"sss_key";N;}i:5;a:28:{s:9:"flight_id";s:7:"2490741";s:13:"airlines_name";s:4:"LION";s:13:"flight_number";s:6:"JT-865";s:14:"departure_city";s:3:"LOP";s:12:"arrival_city";s:3:"SUB";s:4:"stop";s:8:"Langsung";s:11:"price_value";s:9:"501000.00";s:11:"price_adult";s:9:"501000.00";s:11:"price_child";s:4:"0.00";s:12:"price_infant";s:4:"0.00";s:9:"timestamp";s:19:"2016-08-04 11:28:07";s:8:"has_food";s:1:"0";s:16:"check_in_baggage";s:2:"20";s:8:"is_promo";i:0;s:11:"airport_tax";b:1;s:21:"simple_departure_time";s:5:"09:40";s:19:"simple_arrival_time";s:5:"09:35";s:8:"long_via";s:0:"";s:19:"departure_city_name";s:6:"Lombok";s:17:"arrival_city_name";s:8:"Surabaya";s:8:"full_via";s:25:"LOP - SUB (09:40 - 09:35)";s:19:"markup_price_string";s:0:"";s:12:"need_baggage";i:0;s:9:"best_deal";b:0;s:8:"duration";s:26:"0 j 55 m";s:5:"image";s:58:"http://api-sandbox.tiket.com/images/tiket2/icon_lion_2.jpg";s:12:"flight_infos";a:1:{s:11:"flight_info";a:1:{i:0;a:18:{s:13:"flight_number";s:6:"JT-865";s:13:"airlines_name";s:4:"LION";s:24:"airlines_short_real_name";s:4:"Lion";s:32:"airlines_short_real_name_ucwords";s:4:"Lion";s:14:"departure_city";s:3:"LOP";s:12:"arrival_city";s:3:"SUB";s:21:"simple_departure_time";s:5:"09:40";s:19:"simple_arrival_time";s:5:"09:35";s:3:"img";s:142:"
<img width="52" height="45" src="http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png" title="Lion Air" alt="JT-865 LOP SUB 09:40" />";s:7:"img_src";s:61:"http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png";s:16:"check_in_baggage";i:20;s:8:"terminal";s:0:"";s:19:"departure_city_name";s:6:"Lombok";s:17:"arrival_city_name";s:8:"Surabaya";s:8:"duration";a:6:{s:4:"hour";i:0;s:6:"minute";i:0;s:12:"arrival_time";s:19:"2016-08-05 09:35:00";s:12:"arrival_city";s:3:"SUB";s:9:"text_city";s:0:"";s:9:"text_time";s:0:"";}s:13:"duration_time";i:3300;s:13:"duration_hour";s:0:"";s:15:"duration_minute";s:3:"55m";}}}s:7:"sss_key";N;}i:6;a:28:{s:9:"flight_id";s:7:"2490743";s:13:"airlines_name";s:4:"LION";s:13:"flight_number";s:6:"JT-177";s:14:"departure_city";s:3:"LOP";s:12:"arrival_city";s:3:"SUB";s:4:"stop";s:8:"Langsung";s:11:"price_value";s:9:"501000.00";s:11:"price_adult";s:9:"501000.00";s:11:"price_child";s:4:"0.00";s:12:"price_infant";s:4:"0.00";s:9:"timestamp";s:19:"2016-08-04 11:28:07";s:8:"has_food";s:1:"0";s:16:"check_in_baggage";s:2:"20";s:8:"is_promo";i:0;s:11:"airport_tax";b:1;s:21:"simple_departure_time";s:5:"12:15";s:19:"simple_arrival_time";s:5:"12:10";s:8:"long_via";s:0:"";s:19:"departure_city_name";s:6:"Lombok";s:17:"arrival_city_name";s:8:"Surabaya";s:8:"full_via";s:25:"LOP - SUB (12:15 - 12:10)";s:19:"markup_price_string";s:0:"";s:12:"need_baggage";i:0;s:9:"best_deal";b:0;s:8:"duration";s:26:"0 j 55 m";s:5:"image";s:58:"http://api-sandbox.tiket.com/images/tiket2/icon_lion_2.jpg";s:12:"flight_infos";a:1:{s:11:"flight_info";a:1:{i:0;a:18:{s:13:"flight_number";s:6:"JT-177";s:13:"airlines_name";s:4:"LION";s:24:"airlines_short_real_name";s:4:"Lion";s:32:"airlines_short_real_name_ucwords";s:4:"Lion";s:14:"departure_city";s:3:"LOP";s:12:"arrival_city";s:3:"SUB";s:21:"simple_departure_time";s:5:"12:15";s:19:"simple_arrival_time";s:5:"12:10";s:3:"img";s:142:"
<img width="52" height="45" src="http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png" title="Lion Air" alt="JT-177 LOP SUB 12:15" />";s:7:"img_src";s:61:"http://api-sandbox.tiket.com/images/flight/logo/icon_lion.png";s:16:"check_in_baggage";i:20;s:8:"terminal";s:0:"";s:19:"departure_city_name";s:6:"Lombok";s:17:"arrival_city_name";s:8:"Surabaya";s:8:"duration";a:6:{s:4:"hour";i:0;s:6:"minute";i:0;s:12:"arrival_time";s:19:"2016-08-05 12:10:00";s:12:"arrival_city";s:3:"SUB";s:9:"text_city";s:0:"";s:9:"text_time";s:0:"";}s:13:"duration_time";i:3300;s:13:"duration_hour";s:0:"";s:15:"duration_minute";s:3:"55m";}}}s:7:"sss_key";N;}}}s:14:"nearby_go_date";a:1:{s:6:"nearby";a:6:{i:0;a:2:{s:4:"date";s:10:"2016-08-04";s:5:"price";s:9:"936900.00";}i:1;a:1:{s:4:"date";s:10:"2016-08-05";}i:2;a:1:{s:4:"date";s:10:"2016-08-06";}i:3;a:1:{s:4:"date";s:10:"2016-08-07";}i:4;a:1:{s:4:"date";s:10:"2016-08-08";}i:5;a:1:{s:4:"date";s:10:"2016-08-09";}}}s:15:"nearby_ret_date";a:1:{s:6:"nearby";a:7:{i:0;a:1:{s:4:"date";s:10:"2016-08-04";}i:1;a:2:{s:4:"date";s:10:"2016-08-05";s:5:"price";s:9:"501000.00";}i:2;a:1:{s:4:"date";s:10:"2016-08-06";}i:3;a:1:{s:4:"date";s:10:"2016-08-07";}i:4;a:1:{s:4:"date";s:10:"2016-08-08";}i:5;a:1:{s:4:"date";s:10:"2016-08-09";}i:6;a:1:{s:4:"date";s:10:"2016-08-10";}}}s:12:"login_status";s:5:"false";s:5:"token";s:40:"f9b29ac359ca5d77755e7588751c089bf96f0dc9";}
```


1. When you first call the API, it will return cache data
2. Function flow to get updated data :  
    search &rarr; Check Update &rarr; search  
    (We recommend you to call the **Check Update** function every 10 seconds)
    * Search: show last cache data  
    * Check Update: if update > 0, it means that there is an updated data available for grab  
    * Search: show updated data

Child and Infant price will be displayed if the request exists and its value is greater than 0. If there is no infant or child variable requested, then the API will not return the variable and the value.

#### HTTP Request

`GET http://api-sandbox.tiket.com/search/flight?d=SUB&a=LOP&date=2016-08-04&ret_date=2016-08-05&adult=1&child=0&infant=0&token=f9b29ac359ca5d77755e7588751c089bf96f0dc9&v=3&output=xml`
    
#### Parameters

Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------
d | Departure airport code | CHAR(3) |  | TRUE  
a | Arrival airport code | CHAR(3) |  | TRUE  
date | Depart date. Result will be in | YYYY-MM-DD |  | TRUE  
ret_date | return date. If provided, then system will return | YYYY-MM-DD |  | FALSE  
adult | number of adult passenger | INT | 1 | FALSE  
child | number of child passenger | INT | 0 | FALSE  
infant | number of infant passenger | INT | 0 | FALSE  
token | for saving transaction that done by user | CHAR(128) |  | TRUE  
v | version of the search | INT | 1 | FALSE

#### Version Info

For variable `v`, you must set to the following values depending on your time of implementation. This version information is for backward compatibility

Ver no. | Description
------ | -------
1 | Flight Sriwijaya, Lion Air, Garuda, Merpati
2 | Flight Citilink added. New variable **birthdatea1** (birthdate for adult) required for [flight Add Order](http://docs.tiket.com/#add-order-121)  
3 | Flight Mandala and Tiger added. New variable **dcheckinbaggagea1[$i]** (departure baggage for adult), **dcheckinbaggagec1[$i]** (departure baggage for child), **rcheckinbaggagea1[$i]** (return baggage for child), **rcheckinbaggagec1[$i]** (return baggage for child), required for [flight Add Order](http://docs.tiket.com/#add-order-121)  


## Flight Promo


```xml
<tiket>
  <diagnostic>...</diagnostic>
  <output_type>xml</output_type>
  <promos>
    <result>
      <flight_id>40600985</flight_id>
      <flight_date>2014-05-14</flight_date>
      <flight_number>SL 8560</flight_number>
      <airlines_name>LION</airlines_name>
      <departure_city>HDY</departure_city>
      <arrival_city>URT</arrival_city>
      <price_value>175200.00</price_value>
      <simple_departure_time>09:45</simple_departure_time>
      <simple_arrival_time>10:45</simple_arrival_time>
      <image>
        https://www.tiket.com/images/tiket2/icon_lion_2.jpg
      </image>
      <duration>1 j 0 m</duration>
      <departure_city_name>Hat Yai</departure_city_name>
      <arrival_city_name>Surat Thani</arrival_city_name>
      <price_adult>175200.00</price_adult>
      <price_child>0,00</price_child>
      <price_infant>0,00</price_infant>
    </result>
    <result>
      <flight_id>24041203</flight_id>
      <flight_date>2014-05-20</flight_date>
      <flight_number>JT 140</flight_number>
      <airlines_name>LION</airlines_name>
      <departure_city>KNO</departure_city>
      <arrival_city>PKU</arrival_city>
      <price_value>273400.00</price_value>
      <simple_departure_time>12:40</simple_departure_time>
      <simple_arrival_time>13:45</simple_arrival_time>
      <image>
        https://www.tiket.com/images/tiket2/icon_lion_2.jpg
      </image>
      <duration>1 j 5 m</duration>
      <departure_city_name>Medan (Kuala Namu)</departure_city_name>
      <arrival_city_name>Pekanbaru</arrival_city_name>
      <price_adult>273400.00</price_adult>
      <price_child>0,00</price_child>
      <price_infant>0,00</price_infant>
    </result>
    <result>
      <flight_id>33602255</flight_id>
      <flight_date>2014-05-18</flight_date>
      <flight_number>MZ 6465</flight_number>
      <airlines_name>MERPATI</airlines_name>
      <departure_city>SWQ</departure_city>
      <arrival_city>LOP</arrival_city>
      <price_value>219000.00</price_value>
      <simple_departure_time>13:05</simple_departure_time>
      <simple_arrival_time>13:45</simple_arrival_time>
      <image>
        https://www.tiket.com/images/tiket2/icon_merpati_2.jpg
      </image>
      <duration>0 j 40 m</duration>
      <departure_city_name>Sumbawa</departure_city_name>
      <arrival_city_name>Lombok, Mataram</arrival_city_name>
      <price_adult>219000.00</price_adult>
      <price_child>0,00</price_child>
      <price_infant>0,00</price_infant>
    </result>
    <result>
      <flight_id>24565043</flight_id>
      <flight_date>2014-05-14</flight_date>
      <flight_number>MZ 66</flight_number>
      <airlines_name>MERPATI</airlines_name>
      <departure_city>LOP</departure_city>
      <arrival_city>DPS</arrival_city>
      <price_value>246000.00</price_value>
      <simple_departure_time>15:25</simple_departure_time>
      <simple_arrival_time>16:10</simple_arrival_time>
      <image>
        https://www.tiket.com/images/tiket2/icon_merpati_2.jpg
      </image>
      <duration>0 j 45 m</duration>
      <departure_city_name>Lombok, Mataram</departure_city_name>
      <arrival_city_name>Denpasar, Bali</arrival_city_name>
      <price_adult>246000.00</price_adult>
      <price_child>0,00</price_child>
      <price_infant>0,00</price_infant>
    </result>
    <result>
      <flight_id>42046155</flight_id>
      <flight_date>2014-05-18</flight_date>
      <flight_number>OD 2101</flight_number>
      <airlines_name>MALINDO</airlines_name>
      <departure_city>PEN</departure_city>
      <arrival_city>KUL</arrival_city>
      <price_value>125300.00</price_value>
      <simple_departure_time>09:40</simple_departure_time>
      <simple_arrival_time>10:40</simple_arrival_time>
      <image>
        https://www.tiket.com/images/tiket2/icon_malindo_2.jpg
      </image>
      <duration>1 j 0 m</duration>
      <departure_city_name>Penang</departure_city_name>
      <arrival_city_name>Kuala Lumpur</arrival_city_name>
      <price_adult>125300.00</price_adult>
      <price_child>0,00</price_child>
      <price_infant>0,00</price_infant>
    </result>
    <result>
      <flight_id>43736391</flight_id>
      <flight_date>2014-05-19</flight_date>
      <flight_number>IW 1170</flight_number>
      <airlines_name>WINGS</airlines_name>
      <departure_city>TTE</departure_city>
      <arrival_city>WUB</arrival_city>
      <price_value>254700.00</price_value>
      <simple_departure_time>12:05</simple_departure_time>
      <simple_arrival_time>12:35</simple_arrival_time>
      <image>
        https://www.tiket.com/images/tiket2/icon_wings_2.jpg
      </image>
      <duration>0 j 30 m</duration>
      <departure_city_name>Ternate</departure_city_name>
      <arrival_city_name>Buli</arrival_city_name>
      <price_adult>254700.00</price_adult>
      <price_child>0,00</price_child>
      <price_infant>0,00</price_infant>
    </result>
    <result>
      <flight_id>36872272</flight_id>
      <flight_date>2014-05-20</flight_date>
      <flight_number>AK 392</flight_number>
      <airlines_name>AIRASIA</airlines_name>
      <departure_city>KNO</departure_city>
      <arrival_city>KUL</arrival_city>
      <price_value>193950.00</price_value>
      <simple_departure_time>17:25</simple_departure_time>
      <simple_arrival_time>19:20</simple_arrival_time>
      <image>
        https://www.tiket.com/images/tiket2/icon_airasia_2.jpg
      </image>
      <duration>0 j 55 m</duration>
      <departure_city_name>Medan (Kuala Namu)</departure_city_name>
      <arrival_city_name>Kuala Lumpur</arrival_city_name>
      <price_adult>193950.00</price_adult>
      <price_child>0,00</price_child>
      <price_infant>0,00</price_infant>
    </result>
    <result>
      <flight_id>25680777</flight_id>
      <flight_date>2014-05-17</flight_date>
      <flight_number>SJ 102</flight_number>
      <airlines_name>SRIWIJAYA</airlines_name>
      <departure_city>KNO</departure_city>
      <arrival_city>PEN</arrival_city>
      <price_value>193950.00</price_value>
      <simple_departure_time>08:50</simple_departure_time>
      <simple_arrival_time>10:35</simple_arrival_time>
      <image>
        https://www.tiket.com/images/tiket2/icon_sriwijaya_2.jpg
      </image>
      <duration>0 j 45 m</duration>
      <departure_city_name>Medan (Kuala Namu)</departure_city_name>
      <arrival_city_name>Penang</arrival_city_name>
      <price_adult>193950.00</price_adult>
      <price_child>0,00</price_child>
      <price_infant>0,00</price_infant>
    </result>
    <result>
      <flight_id>30664125</flight_id>
      <flight_date>2014-05-18</flight_date>
      <flight_number>TR2455</flight_number>
      <airlines_name>TIGER</airlines_name>
      <departure_city>KUL</departure_city>
      <arrival_city>SIN</arrival_city>
      <price_value>258500.00</price_value>
      <simple_departure_time>11:30</simple_departure_time>
      <simple_arrival_time>12:35</simple_arrival_time>
      <image>
        https://www.tiket.com/images/tiket2/icon_tiger_2.jpg
      </image>
      <duration>1 j 5 m</duration>
      <departure_city_name>Kuala Lumpur</departure_city_name>
      <arrival_city_name>Singapore</arrival_city_name>
      <price_adult>258500.00</price_adult>
      <price_child>0,00</price_child>
      <price_infant>0,00</price_infant>
    </result>
    <result>
      <flight_id>20639492</flight_id>
      <flight_date>2014-05-15</flight_date>
      <flight_number>TR2455</flight_number>
      <airlines_name>TIGER</airlines_name>
      <departure_city>KUL</departure_city>
      <arrival_city>SIN</arrival_city>
      <price_value>177600.00</price_value>
      <simple_departure_time>11:30</simple_departure_time>
      <simple_arrival_time>12:35</simple_arrival_time>
      <image>
        https://www.tiket.com/images/tiket2/icon_tiger_2.jpg
      </image>
      <duration>1 j 5 m</duration>
      <departure_city_name>Kuala Lumpur</departure_city_name>
      <arrival_city_name>Singapore</arrival_city_name>
      <price_adult>177600.00</price_adult>
      <price_child>0,00</price_child>
      <price_infant>0,00</price_infant>
    </result>
  </promos>
  <login_status>false</login_status>
  <token>b8cca7a82b3a3575948ed43422cc6310e201c154</token>
</tiket>
```



```json
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.0491",
    "memoryusage": "5.1MB",
    "unix_timestamp": 1399953198,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "promos": {
    "result": [{
      "flight_id": "36732430",
      "flight_date": "2014-05-16",
      "flight_number": "AK 392",
      "airlines_name": "AIRASIA",
      "departure_city": "KNO",
      "arrival_city": "KUL",
      "price_value": "193950.00",
      "simple_departure_time": "17:25",
      "simple_arrival_time": "19:20",
      "image": "https:\/\/www.tiket.com\/images\/tiket2\/icon_airasia_2.jpg",
      "duration": "0 j 55 m",
      "departure_city_name": "Medan (Kuala Namu)",
      "arrival_city_name": "Kuala Lumpur",
      "price_adult": "193950.00",
      "price_child": "0,00",
      "price_infant": "0,00"
    }, {
      "flight_id": "33602255",
      "flight_date": "2014-05-18",
      "flight_number": "MZ 6465",
      "airlines_name": "MERPATI",
      "departure_city": "SWQ",
      "arrival_city": "LOP",
      "price_value": "219000.00",
      "simple_departure_time": "13:05",
      "simple_arrival_time": "13:45",
      "image": "https:\/\/www.tiket.com\/images\/tiket2\/icon_merpati_2.jpg",
      "duration": "0 j 40 m",
      "departure_city_name": "Sumbawa",
      "arrival_city_name": "Lombok, Mataram",
      "price_adult": "219000.00",
      "price_child": "0,00",
      "price_infant": "0,00"
    }, {
      "flight_id": "28654470",
      "flight_date": "2014-05-19",
      "flight_number": "SJ 102",
      "airlines_name": "SRIWIJAYA",
      "departure_city": "KNO",
      "arrival_city": "PEN",
      "price_value": "193950.00",
      "simple_departure_time": "08:50",
      "simple_arrival_time": "10:35",
      "image": "https:\/\/www.tiket.com\/images\/tiket2\/icon_sriwijaya_2.jpg",
      "duration": "0 j 45 m",
      "departure_city_name": "Medan (Kuala Namu)",
      "arrival_city_name": "Penang",
      "price_adult": "193950.00",
      "price_child": "0,00",
      "price_infant": "0,00"
    }, {
      "flight_id": "43736391",
      "flight_date": "2014-05-19",
      "flight_number": "IW 1170",
      "airlines_name": "WINGS",
      "departure_city": "TTE",
      "arrival_city": "WUB",
      "price_value": "254700.00",
      "simple_departure_time": "12:05",
      "simple_arrival_time": "12:35",
      "image": "https:\/\/www.tiket.com\/images\/tiket2\/icon_wings_2.jpg",
      "duration": "0 j 30 m",
      "departure_city_name": "Ternate",
      "arrival_city_name": "Buli",
      "price_adult": "254700.00",
      "price_child": "0,00",
      "price_infant": "0,00"
    }, {
      "flight_id": "37088662",
      "flight_date": "2014-05-20",
      "flight_number": "AK 422",
      "airlines_name": "AIRASIA",
      "departure_city": "BTJ",
      "arrival_city": "KUL",
      "price_value": "258150.00",
      "simple_departure_time": "12:55",
      "simple_arrival_time": "15:20",
      "image": "https:\/\/www.tiket.com\/images\/tiket2\/icon_airasia_2.jpg",
      "duration": "1 j 25 m",
      "departure_city_name": "Banda Aceh",
      "arrival_city_name": "Kuala Lumpur",
      "price_adult": "258150.00",
      "price_child": "0,00",
      "price_infant": "0,00"
    }, {
      "flight_id": "43416394",
      "flight_date": "2014-05-16",
      "flight_number": "IW 1170",
      "airlines_name": "WINGS",
      "departure_city": "TTE",
      "arrival_city": "WUB",
      "price_value": "254700.00",
      "simple_departure_time": "12:05",
      "simple_arrival_time": "12:35",
      "image": "https:\/\/www.tiket.com\/images\/tiket2\/icon_wings_2.jpg",
      "duration": "0 j 30 m",
      "departure_city_name": "Ternate",
      "arrival_city_name": "Buli",
      "price_adult": "254700.00",
      "price_child": "0,00",
      "price_infant": "0,00"
    }, {
      "flight_id": "24565043",
      "flight_date": "2014-05-14",
      "flight_number": "MZ 66",
      "airlines_name": "MERPATI",
      "departure_city": "LOP",
      "arrival_city": "DPS",
      "price_value": "246000.00",
      "simple_departure_time": "15:25",
      "simple_arrival_time": "16:10",
      "image": "https:\/\/www.tiket.com\/images\/tiket2\/icon_merpati_2.jpg",
      "duration": "0 j 45 m",
      "departure_city_name": "Lombok, Mataram",
      "arrival_city_name": "Denpasar, Bali",
      "price_adult": "246000.00",
      "price_child": "0,00",
      "price_infant": "0,00"
    }, {
      "flight_id": "20723404",
      "flight_date": "2014-05-16",
      "flight_number": "TR2455",
      "airlines_name": "TIGER",
      "departure_city": "KUL",
      "arrival_city": "SIN",
      "price_value": "177600.00",
      "simple_departure_time": "11:30",
      "simple_arrival_time": "12:35",
      "image": "https:\/\/www.tiket.com\/images\/tiket2\/icon_tiger_2.jpg",
      "duration": "1 j 5 m",
      "departure_city_name": "Kuala Lumpur",
      "arrival_city_name": "Singapore",
      "price_adult": "177600.00",
      "price_child": "0,00",
      "price_infant": "0,00"
    }, {
      "flight_id": "30664125",
      "flight_date": "2014-05-18",
      "flight_number": "TR2455",
      "airlines_name": "TIGER",
      "departure_city": "KUL",
      "arrival_city": "SIN",
      "price_value": "258500.00",
      "simple_departure_time": "11:30",
      "simple_arrival_time": "12:35",
      "image": "https:\/\/www.tiket.com\/images\/tiket2\/icon_tiger_2.jpg",
      "duration": "1 j 5 m",
      "departure_city_name": "Kuala Lumpur",
      "arrival_city_name": "Singapore",
      "price_adult": "258500.00",
      "price_child": "0,00",
      "price_infant": "0,00"
    }, {
      "flight_id": "30073466",
      "flight_date": "2014-05-17",
      "flight_number": "TR2455",
      "airlines_name": "TIGER",
      "departure_city": "KUL",
      "arrival_city": "SIN",
      "price_value": "177600.00",
      "simple_departure_time": "11:30",
      "simple_arrival_time": "12:35",
      "image": "https:\/\/www.tiket.com\/images\/tiket2\/icon_tiger_2.jpg",
      "duration": "1 j 5 m",
      "departure_city_name": "Kuala Lumpur",
      "arrival_city_name": "Singapore",
      "price_adult": "177600.00",
      "price_child": "0,00",
      "price_infant": "0,00"
    }]
  },
  "login_status": "false",
  "token": "b8cca7a82b3a3575948ed43422cc6310e201c154"
}
```



```matlab
a: 5: {
  s: 10: "diagnostic";a: 7: {
    s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.0590";s: 11: "memoryusage";s: 14: "5.1MB";s: 14: "unix_timestamp";i: 1399953246;s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "id";s: 8: "currency";s: 3: "IDR";
  }
  s: 11: "output_type";s: 9: "serialize";s: 6: "promos";a: 1: {
    s: 6: "result";a: 10: {
      i: 0;a: 16: {
        s: 9: "flight_id";s: 8: "28782051";s: 11: "flight_date";s: 10: "2014-05-20";s: 13: "flight_number";s: 6: "TR2465";s: 13: "airlines_name";s: 5: "TIGER";s: 14: "departure_city";s: 3: "KUL";s: 12: "arrival_city";s: 3: "SIN";s: 11: "price_value";s: 9: "177600.00";s: 21: "simple_departure_time";s: 5: "18:30";s: 19: "simple_arrival_time";s: 5: "19:45";s: 5: "image";s: 52: "https://www.tiket.com/images/tiket2/icon_tiger_2.jpg";s: 8: "duration";s: 26: "1 j 15 m";s: 19: "departure_city_name";s: 12: "Kuala Lumpur";s: 17: "arrival_city_name";s: 9: "Singapore";s: 11: "price_adult";s: 9: "177600.00";s: 11: "price_child";s: 4: "0,00";s: 12: "price_infant";s: 4: "0,00";
      }
      i: 1;a: 16: {
        s: 9: "flight_id";s: 8: "30664125";s: 11: "flight_date";s: 10: "2014-05-18";s: 13: "flight_number";s: 6: "TR2455";s: 13: "airlines_name";s: 5: "TIGER";s: 14: "departure_city";s: 3: "KUL";s: 12: "arrival_city";s: 3: "SIN";s: 11: "price_value";s: 9: "258500.00";s: 21: "simple_departure_time";s: 5: "11:30";s: 19: "simple_arrival_time";s: 5: "12:35";s: 5: "image";s: 52: "https://www.tiket.com/images/tiket2/icon_tiger_2.jpg";s: 8: "duration";s: 25: "1 j 5 m";s: 19: "departure_city_name";s: 12: "Kuala Lumpur";s: 17: "arrival_city_name";s: 9: "Singapore";s: 11: "price_adult";s: 9: "258500.00";s: 11: "price_child";s: 4: "0,00";s: 12: "price_infant";s: 4: "0,00";
      }
      i: 2;a: 16: {
        s: 9: "flight_id";s: 8: "28871071";s: 11: "flight_date";s: 10: "2014-05-15";s: 13: "flight_number";s: 6: "MZ 660";s: 13: "airlines_name";s: 7: "MERPATI";s: 14: "departure_city";s: 3: "DPS";s: 12: "arrival_city";s: 3: "LOP";s: 11: "price_value";s: 9: "180000.00";s: 21: "simple_departure_time";s: 5: "12:30";s: 19: "simple_arrival_time";s: 5: "13:15";s: 5: "image";s: 54: "https://www.tiket.com/images/tiket2/icon_merpati_2.jpg";s: 8: "duration";s: 26: "0 j 45 m";s: 19: "departure_city_name";s: 14: "Denpasar, Bali";s: 17: "arrival_city_name";s: 15: "Lombok, Mataram";s: 11: "price_adult";s: 9: "180000.00";s: 11: "price_child";s: 4: "0,00";s: 12: "price_infant";s: 4: "0,00";
      }
      i: 3;a: 16: {
        s: 9: "flight_id";s: 8: "24565043";s: 11: "flight_date";s: 10: "2014-05-14";s: 13: "flight_number";s: 5: "MZ 66";s: 13: "airlines_name";s: 7: "MERPATI";s: 14: "departure_city";s: 3: "LOP";s: 12: "arrival_city";s: 3: "DPS";s: 11: "price_value";s: 9: "246000.00";s: 21: "simple_departure_time";s: 5: "15:25";s: 19: "simple_arrival_time";s: 5: "16:10";s: 5: "image";s: 54: "https://www.tiket.com/images/tiket2/icon_merpati_2.jpg";s: 8: "duration";s: 26: "0 j 45 m";s: 19: "departure_city_name";s: 15: "Lombok, Mataram";s: 17: "arrival_city_name";s: 14: "Denpasar, Bali";s: 11: "price_adult";s: 9: "246000.00";s: 11: "price_child";s: 4: "0,00";s: 12: "price_infant";s: 4: "0,00";
      }
      i: 4;a: 16: {
        s: 9: "flight_id";s: 8: "43392863";s: 11: "flight_date";s: 10: "2014-05-15";s: 13: "flight_number";s: 7: "IW 1170";s: 13: "airlines_name";s: 5: "WINGS";s: 14: "departure_city";s: 3: "TTE";s: 12: "arrival_city";s: 3: "WUB";s: 11: "price_value";s: 9: "254700.00";s: 21: "simple_departure_time";s: 5: "12:05";s: 19: "simple_arrival_time";s: 5: "12:35";s: 5: "image";s: 52: "https://www.tiket.com/images/tiket2/icon_wings_2.jpg";s: 8: "duration";s: 26: "0 j 30 m";s: 19: "departure_city_name";s: 7: "Ternate";s: 17: "arrival_city_name";s: 4: "Buli";s: 11: "price_adult";s: 9: "254700.00";s: 11: "price_child";s: 4: "0,00";s: 12: "price_infant";s: 4: "0,00";
      }
      i: 5;a: 16: {
        s: 9: "flight_id";s: 8: "30664111";s: 11: "flight_date";s: 10: "2014-05-19";s: 13: "flight_number";s: 6: "TR2455";s: 13: "airlines_name";s: 5: "TIGER";s: 14: "departure_city";s: 3: "KUL";s: 12: "arrival_city";s: 3: "SIN";s: 11: "price_value";s: 9: "258500.00";s: 21: "simple_departure_time";s: 5: "11:30";s: 19: "simple_arrival_time";s: 5: "12:35";s: 5: "image";s: 52: "https://www.tiket.com/images/tiket2/icon_tiger_2.jpg";s: 8: "duration";s: 25: "1 j 5 m";s: 19: "departure_city_name";s: 12: "Kuala Lumpur";s: 17: "arrival_city_name";s: 9: "Singapore";s: 11: "price_adult";s: 9: "258500.00";s: 11: "price_child";s: 4: "0,00";s: 12: "price_infant";s: 4: "0,00";
      }
      i: 6;a: 16: {
        s: 9: "flight_id";s: 8: "20639492";s: 11: "flight_date";s: 10: "2014-05-15";s: 13: "flight_number";s: 6: "TR2455";s: 13: "airlines_name";s: 5: "TIGER";s: 14: "departure_city";s: 3: "KUL";s: 12: "arrival_city";s: 3: "SIN";s: 11: "price_value";s: 9: "177600.00";s: 21: "simple_departure_time";s: 5: "11:30";s: 19: "simple_arrival_time";s: 5: "12:35";s: 5: "image";s: 52: "https://www.tiket.com/images/tiket2/icon_tiger_2.jpg";s: 8: "duration";s: 25: "1 j 5 m";s: 19: "departure_city_name";s: 12: "Kuala Lumpur";s: 17: "arrival_city_name";s: 9: "Singapore";s: 11: "price_adult";s: 9: "177600.00";s: 11: "price_child";s: 4: "0,00";s: 12: "price_infant";s: 4: "0,00";
      }
      i: 7;a: 16: {
        s: 9: "flight_id";s: 8: "40600985";s: 11: "flight_date";s: 10: "2014-05-14";s: 13: "flight_number";s: 7: "SL 8560";s: 13: "airlines_name";s: 4: "LION";s: 14: "departure_city";s: 3: "HDY";s: 12: "arrival_city";s: 3: "URT";s: 11: "price_value";s: 9: "175200.00";s: 21: "simple_departure_time";s: 5: "09:45";s: 19: "simple_arrival_time";s: 5: "10:45";s: 5: "image";s: 51: "https://www.tiket.com/images/tiket2/icon_lion_2.jpg";s: 8: "duration";s: 25: "1 j 0 m";s: 19: "departure_city_name";s: 7: "Hat Yai";s: 17: "arrival_city_name";s: 11: "Surat Thani";s: 11: "price_adult";s: 9: "175200.00";s: 11: "price_child";s: 4: "0,00";s: 12: "price_infant";s: 4: "0,00";
      }
      i: 8;a: 16: {
        s: 9: "flight_id";s: 8: "24565040";s: 11: "flight_date";s: 10: "2014-05-15";s: 13: "flight_number";s: 5: "MZ 66";s: 13: "airlines_name";s: 7: "MERPATI";s: 14: "departure_city";s: 3: "LOP";s: 12: "arrival_city";s: 3: "DPS";s: 11: "price_value";s: 9: "246000.00";s: 21: "simple_departure_time";s: 5: "14:45";s: 19: "simple_arrival_time";s: 5: "15:30";s: 5: "image";s: 54: "https://www.tiket.com/images/tiket2/icon_merpati_2.jpg";s: 8: "duration";s: 26: "0 j 45 m";s: 19: "departure_city_name";s: 15: "Lombok, Mataram";s: 17: "arrival_city_name";s: 14: "Denpasar, Bali";s: 11: "price_adult";s: 9: "246000.00";s: 11: "price_child";s: 4: "0,00";s: 12: "price_infant";s: 4: "0,00";
      }
      i: 9;a: 16: {
        s: 9: "flight_id";s: 8: "30073466";s: 11: "flight_date";s: 10: "2014-05-17";s: 13: "flight_number";s: 6: "TR2455";s: 13: "airlines_name";s: 5: "TIGER";s: 14: "departure_city";s: 3: "KUL";s: 12: "arrival_city";s: 3: "SIN";s: 11: "price_value";s: 9: "177600.00";s: 21: "simple_departure_time";s: 5: "11:30";s: 19: "simple_arrival_time";s: 5: "12:35";s: 5: "image";s: 52: "https://www.tiket.com/images/tiket2/icon_tiger_2.jpg";s: 8: "duration";s: 25: "1 j 5 m";s: 19: "departure_city_name";s: 12: "Kuala Lumpur";s: 17: "arrival_city_name";s: 9: "Singapore";s: 11: "price_adult";s: 9: "177600.00";s: 11: "price_child";s: 4: "0,00";s: 12: "price_infant";s: 4: "0,00";
      }
    }
  }
  s: 12: "login_status";s: 5: "false";s: 5: "token";s: 40: "b8cca7a82b3a3575948ed43422cc6310e201c154";
}
```
    
    
Get flight rute with promo price

#### HTTP Request

`GET https://api-sandbox.tiket.com/general_api/get_flight_promo?token=b8cca7a82b3a3575948ed43422cc6310e201c154`

#### Parameters

Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------
token | for saving transaction that done by user | CHAR(128) |  | TRUE  


    
## Get Nearest Airport

Retrieve the nearest airport

### By IP Address 

```xml
<tiket>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.0603</elapsetime>
    <memoryusage>5.5MB</memoryusage>
    <unix_timestamp>1399953745</unix_timestamp>
    <confirm>success</confirm>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <output_type>xml</output_type>
  <search>
    <ip>182.253.203.58</ip>
    <latitude>-6.1744</latitude>
    <longitude>106.8294</longitude>
  </search>
  <nearest_airports>
    <airport>
      <airport_code>CGK</airport_code>
      <business_name>SOEKARNO - HATTA</business_name>
      <distance>19.46 KM</distance>
    </airport>
  </nearest_airports>
  <login_status>false</login_status>
  <token>c5a32cce21b11d6e9a764ca685b5ee10378647ee</token>
</tiket>
```



```json
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.0429",
    "memoryusage": "5.49MB",
    "unix_timestamp": 1399954397,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "search": {
    "ip": "182.253.203.58",
    "latitude": "-6.1744",
    "longitude": "106.8294"
  },
  "nearest_airports": {
    "airport": [{
      "airport_code": "CGK",
      "business_name": "SOEKARNO - HATTA",
      "distance": "19.46 KM"
    }]
  },
  "login_status": "false",
  "token": "c5a32cce21b11d6e9a764ca685b5ee10378647ee"
}
```



```matlab
a: 6: {
  s: 10: "diagnostic";a: 7: {
    s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.0444";s: 11: "memoryusage";s: 14: "5.49MB";s: 14: "unix_timestamp";i: 1399954456;s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "id";s: 8: "currency";s: 3: "IDR";
  }
  s: 11: "output_type";s: 9: "serialize";s: 6: "search";a: 3: {
    s: 2: "ip";s: 14: "182.253.203.58";s: 8: "latitude";s: 7: "-6.1744";s: 9: "longitude";s: 8: "106.8294";
  }
  s: 16: "nearest_airports";a: 1: {
    s: 7: "airport";a: 1: {
      i: 0;a: 3: {
        s: 12: "airport_code";s: 3: "CGK";s: 13: "business_name";s: 16: "SOEKARNO - HATTA";s: 8: "distance";s: 8: "19.46 KM";
      }
    }
  }
  s: 12: "login_status";s: 5: "false";s: 5: "token";s: 40: "c5a32cce21b11d6e9a764ca685b5ee10378647ee";
}
```


<aside class="success">If the input is provided via IP address it will looked for the closest airport for IP address that detected.</aside>

#### HTTP Request

`GET https://api-sandbox.tiket.com/flight_api/getNearestAirport?token=c5a32cce21b11d6e9a764ca685b5ee10378647ee&ip=182.253.203.58`

#### Parameters

Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------
token | for saving transaction that done by user | CHAR(128) |  | TRUE  
ip | ip address user | CHAR(20), |  | RUE  

### By latitude & longitude

```xml
<?xml version="1.0" encoding="utf-8"?>
<tiket>
    <diagnostic>
        <status>200</status>
        <elapsetime>0.0961</elapsetime>
        <memoryusage>6.08MB</memoryusage>
        <unix_timestamp>1470221306</unix_timestamp>
        <confirm>success</confirm>
        <lang>id</lang>
        <currency>IDR</currency>
    </diagnostic>
    <output_type>xml</output_type>
    <search>
        <latitude>-6.195062</latitude>
        <longitude>106.803181</longitude>
    </search>
    <nearest_airports>
        <airport>
            <airport_code>CGK</airport_code>
            <business_name>Soekarno Hatta</business_name>
            <distance>17.57 KM</distance>
            <location_name>Jakarta - Cengkareng</location_name>
        </airport>
    </nearest_airports>
    <login_status>false</login_status>
    <token>f9b29ac359ca5d77755e7588751c089bf96f0dc9</token>
</tiket>
```

```json
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.1005",
    "memoryusage": "6.07MB",
    "unix_timestamp": 1470221465,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "search": {
    "latitude": "-6.195062",
    "longitude": "106.803181"
  },
  "nearest_airports": {
    "airport": [
      {
        "airport_code": "CGK",
        "business_name": "Soekarno Hatta",
        "distance": "17.57 KM",
        "location_name": "Jakarta - Cengkareng"
      }
    ]
  },
  "login_status": "false",
  "token": "f9b29ac359ca5d77755e7588751c089bf96f0dc9"
}
```



```matlab
a:6:{s:10:"diagnostic";a:7:{s:6:"status";i:200;s:10:"elapsetime";s:14:"0.1037";s:11:"memoryusage";s:14:"6.07MB";s:14:"unix_timestamp";i:1470221529;s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:11:"output_type";s:9:"serialize";s:6:"search";a:2:{s:8:"latitude";s:9:"-6.195062";s:9:"longitude";s:10:"106.803181";}s:16:"nearest_airports";a:1:{s:7:"airport";a:1:{i:0;a:4:{s:12:"airport_code";s:3:"CGK";s:13:"business_name";s:14:"Soekarno Hatta";s:8:"distance";s:8:"17.57 KM";s:13:"location_name";s:20:"Jakarta - Cengkareng";}}}s:12:"login_status";s:5:"false";s:5:"token";s:40:"f9b29ac359ca5d77755e7588751c089bf96f0dc9";}
```

<aside class="success">If the input is provided via coordinate (latitude and longitude), it will look for the closest airport from the coordinate.</aside>

#### HTTP Request

`GET https://api-sandbox.tiket.com/flight_api/getNearestAirport?token=905f0af68759becf520885084c42469b&latitude=-6.195062&longitude=106.803181&output=json`

#### Parameters

Name | Description | Format | Default | Mandatory 
---- | ----------  | -----  | ------- | ---------
token | for saving transaction that done by user | CHAR(128) |  | TRUE  
latitude | latitude position user | CHAR(20) |  | TRUE  
longitude | latitude position user | CHAR(20) |  | TRUE  


## Get Popular Airport Destination


```xml
<?xml version="1.0" encoding="utf-8"?>
<tiket>
    <diagnostic>
        <status>200</status>
        <elapsetime>0.1139</elapsetime>
        <memoryusage>6.05MB</memoryusage>
        <unix_timestamp>1470278207</unix_timestamp>
        <confirm>success</confirm>
        <lang>id</lang>
        <currency>IDR</currency>
    </diagnostic>
    <output_type>xml</output_type>
    <popular_destinations>
        <airport>
            <arrival_city>DPS</arrival_city>
            <business_name>Ngurah Rai</business_name>
            <province_name>Bali</province_name>
            <location_name>Denpasar, Bali</location_name>
        </airport>
        <airport>
            <arrival_city>JKT</arrival_city>
            <business_name>Jakarta</business_name>
            <province_name></province_name>
            <location_name>Jakarta</location_name>
        </airport>
        <airport>
            <arrival_city>KNO</arrival_city>
            <business_name>Kuala Namu</business_name>
            <province_name>Sumatera Utara</province_name>
            <location_name>Medan (Kuala Namu)</location_name>
        </airport>
        <airport>
            <arrival_city>JOG</arrival_city>
            <business_name>Adi Sutjipto</business_name>
            <province_name>Daerah Istimewa Yogyakarta</province_name>
            <location_name>Yogyakarta</location_name>
        </airport>
        <airport>
            <arrival_city>SUB</arrival_city>
            <business_name>Juanda</business_name>
            <province_name>Jawa Timur</province_name>
            <location_name>Surabaya</location_name>
        </airport>
        <airport>
            <arrival_city>PNK</arrival_city>
            <business_name>Supadio</business_name>
            <province_name>Kalimantan Barat</province_name>
            <location_name>Pontianak</location_name>
        </airport>
        <airport>
            <arrival_city>BPN</arrival_city>
            <business_name>Sepinggan</business_name>
            <province_name>Kalimantan Timur</province_name>
            <location_name>BalikPapan</location_name>
        </airport>
        <airport>
            <arrival_city>SRG</arrival_city>
            <business_name>Achmad Yani</business_name>
            <province_name>Jawa Tengah</province_name>
            <location_name>Semarang</location_name>
        </airport>
        <airport>
            <arrival_city>PGK</arrival_city>
            <business_name>Depati Amir</business_name>
            <province_name>Kepulauan Bangka-Belitung</province_name>
            <location_name>Pangkal pinang</location_name>
        </airport>
        <airport>
            <arrival_city>SIN</arrival_city>
            <business_name>Changi</business_name>
            <province_name></province_name>
            <location_name>Singapore</location_name>
        </airport>
        <airport>
            <arrival_city>PDG</arrival_city>
            <business_name>Minangkabau</business_name>
            <province_name>Sumatera Barat</province_name>
            <location_name>Padang</location_name>
        </airport>
        <airport>
            <arrival_city>UPG</arrival_city>
            <business_name>Sultan Hasanuddin</business_name>
            <province_name>Sulawesi Selatan</province_name>
            <location_name>Ujungpandang, Makassar</location_name>
        </airport>
        <airport>
            <arrival_city>SOC</arrival_city>
            <business_name>Adisumarmo</business_name>
            <province_name>Jawa Tengah</province_name>
            <location_name>Solo</location_name>
        </airport>
    </popular_destinations>
    <login_status>false</login_status>
    <token>f9b29ac359ca5d77755e7588751c089bf96f0dc9</token>
</tiket>
```



```json
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.1108",
    "memoryusage": "6.04MB",
    "unix_timestamp": 1470278309,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "popular_destinations": {
    "airport": [
      {
        "arrival_city": "DPS",
        "business_name": "Ngurah Rai",
        "province_name": "Bali",
        "location_name": "Denpasar, Bali"
      },
      {
        "arrival_city": "JKT",
        "business_name": "Jakarta",
        "province_name": "",
        "location_name": "Jakarta"
      },
      {
        "arrival_city": "KNO",
        "business_name": "Kuala Namu",
        "province_name": "Sumatera Utara",
        "location_name": "Medan (Kuala Namu)"
      },
      {
        "arrival_city": "JOG",
        "business_name": "Adi Sutjipto",
        "province_name": "Daerah Istimewa Yogyakarta",
        "location_name": "Yogyakarta"
      },
      {
        "arrival_city": "SUB",
        "business_name": "Juanda",
        "province_name": "Jawa Timur",
        "location_name": "Surabaya"
      },
      {
        "arrival_city": "PNK",
        "business_name": "Supadio",
        "province_name": "Kalimantan Barat",
        "location_name": "Pontianak"
      },
      {
        "arrival_city": "BPN",
        "business_name": "Sepinggan",
        "province_name": "Kalimantan Timur",
        "location_name": "BalikPapan"
      },
      {
        "arrival_city": "SRG",
        "business_name": "Achmad Yani",
        "province_name": "Jawa Tengah",
        "location_name": "Semarang"
      },
      {
        "arrival_city": "PGK",
        "business_name": "Depati Amir",
        "province_name": "Kepulauan Bangka-Belitung",
        "location_name": "Pangkal pinang"
      },
      {
        "arrival_city": "SIN",
        "business_name": "Changi",
        "province_name": "",
        "location_name": "Singapore"
      },
      {
        "arrival_city": "PDG",
        "business_name": "Minangkabau",
        "province_name": "Sumatera Barat",
        "location_name": "Padang"
      },
      {
        "arrival_city": "UPG",
        "business_name": "Sultan Hasanuddin",
        "province_name": "Sulawesi Selatan",
        "location_name": "Ujungpandang, Makassar"
      },
      {
        "arrival_city": "SOC",
        "business_name": "Adisumarmo",
        "province_name": "Jawa Tengah",
        "location_name": "Solo"
      }
    ]
  },
  "login_status": "false",
  "token": "f9b29ac359ca5d77755e7588751c089bf96f0dc9"
}
```


```matlab
a:5:{s:10:"diagnostic";a:7:{s:6:"status";i:200;s:10:"elapsetime";s:14:"0.1122";s:11:"memoryusage";s:14:"6.04MB";s:14:"unix_timestamp";i:1470278368;s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:11:"output_type";s:9:"serialize";s:20:"popular_destinations";a:1:{s:7:"airport";a:13:{i:0;a:4:{s:12:"arrival_city";s:3:"DPS";s:13:"business_name";s:10:"Ngurah Rai";s:13:"province_name";s:4:"Bali";s:13:"location_name";s:14:"Denpasar, Bali";}i:1;a:4:{s:12:"arrival_city";s:3:"JKT";s:13:"business_name";s:7:"Jakarta";s:13:"province_name";s:0:"";s:13:"location_name";s:7:"Jakarta";}i:2;a:4:{s:12:"arrival_city";s:3:"KNO";s:13:"business_name";s:10:"Kuala Namu";s:13:"province_name";s:14:"Sumatera Utara";s:13:"location_name";s:18:"Medan (Kuala Namu)";}i:3;a:4:{s:12:"arrival_city";s:3:"JOG";s:13:"business_name";s:12:"Adi Sutjipto";s:13:"province_name";s:26:"Daerah Istimewa Yogyakarta";s:13:"location_name";s:10:"Yogyakarta";}i:4;a:4:{s:12:"arrival_city";s:3:"SUB";s:13:"business_name";s:6:"Juanda";s:13:"province_name";s:10:"Jawa Timur";s:13:"location_name";s:8:"Surabaya";}i:5;a:4:{s:12:"arrival_city";s:3:"PNK";s:13:"business_name";s:7:"Supadio";s:13:"province_name";s:16:"Kalimantan Barat";s:13:"location_name";s:9:"Pontianak";}i:6;a:4:{s:12:"arrival_city";s:3:"BPN";s:13:"business_name";s:9:"Sepinggan";s:13:"province_name";s:16:"Kalimantan Timur";s:13:"location_name";s:10:"BalikPapan";}i:7;a:4:{s:12:"arrival_city";s:3:"SRG";s:13:"business_name";s:11:"Achmad Yani";s:13:"province_name";s:11:"Jawa Tengah";s:13:"location_name";s:8:"Semarang";}i:8;a:4:{s:12:"arrival_city";s:3:"PGK";s:13:"business_name";s:11:"Depati Amir";s:13:"province_name";s:25:"Kepulauan Bangka-Belitung";s:13:"location_name";s:14:"Pangkal pinang";}i:9;a:4:{s:12:"arrival_city";s:3:"SIN";s:13:"business_name";s:6:"Changi";s:13:"province_name";s:0:"";s:13:"location_name";s:9:"Singapore";}i:10;a:4:{s:12:"arrival_city";s:3:"PDG";s:13:"business_name";s:11:"Minangkabau";s:13:"province_name";s:14:"Sumatera Barat";s:13:"location_name";s:6:"Padang";}i:11;a:4:{s:12:"arrival_city";s:3:"UPG";s:13:"business_name";s:17:"Sultan Hasanuddin";s:13:"province_name";s:16:"Sulawesi Selatan";s:13:"location_name";s:22:"Ujungpandang, Makassar";}i:12;a:4:{s:12:"arrival_city";s:3:"SOC";s:13:"business_name";s:10:"Adisumarmo";s:13:"province_name";s:11:"Jawa Tengah";s:13:"location_name";s:4:"Solo";}}}s:12:"login_status";s:5:"false";s:5:"token";s:40:"f9b29ac359ca5d77755e7588751c089bf96f0dc9";}
```

List all popular airport destination based on departure airport code

#### HTTP Request

`GET https://api-sandbox.tiket.com/flight_api/getPopularDestination?token=c5a32cce21b11d6e9a764ca685b5ee10378647ee&depart=CGK`

#### Parameters

Name |Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------
token | for saving transaction that done by user | CHAR(128) |  | TRUE  
depart | depart airport code | CHAR(20) |  | TRUE  


## Search Airport

List of all airport


```xml
<?xml version="1.0" encoding="utf-8"?>
<tiket>
    <diagnostic>
        <status>200</status>
        <elapsetime>0.1005</elapsetime>
        <memoryusage>6.43MB</memoryusage>
        <unix_timestamp>1470279929</unix_timestamp>
        <confirm>success</confirm>
        <lang>id</lang>
        <currency>IDR</currency>
    </diagnostic>
    <output_type>xml</output_type>
    <all_airport>
        <airport>
            <airport_name>Pattimura</airport_name>
            <airport_code>AMQ</airport_code>
            <location_name>Ambon</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>ATAMBUA</airport_name>
            <airport_code>ABU</airport_code>
            <location_name>Atambua</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Soa</airport_name>
            <airport_code>BJW</airport_code>
            <location_name>Bajawa</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Sepinggan</airport_name>
            <airport_code>BPN</airport_code>
            <location_name>BalikPapan</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Sultan Iskandar Muda</airport_name>
            <airport_code>BTJ</airport_code>
            <location_name>Banda Aceh</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Husein Sastranegara</airport_name>
            <airport_code>BDO</airport_code>
            <location_name>Bandung</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>SYAMSUDDIN NOOR</airport_name>
            <airport_code>BDJ</airport_code>
            <location_name>Banjarmasin</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>BLIMBINGSARI</airport_name>
            <airport_code>DQJ</airport_code>
            <location_name>Banyuwangi - BLIMBINGSARI</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Hang Nadim</airport_name>
            <airport_code>BTH</airport_code>
            <location_name>Batam</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Baubau</airport_name>
            <airport_code>BUW</airport_code>
            <location_name>Baubau</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Fatmawati Soekarno</airport_name>
            <airport_code>BKS</airport_code>
            <location_name>Bengkulu</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Kalimarau</airport_name>
            <airport_code>BEJ</airport_code>
            <location_name>Berau</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Frans Kaisiepo</airport_name>
            <airport_code>BIK</airport_code>
            <location_name>Biak</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Muhammad Salahuddin</airport_name>
            <airport_code>BMU</airport_code>
            <location_name>Bima</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>BLIMBINGSARI</airport_name>
            <airport_code>BWX</airport_code>
            <location_name>BLIMBINGSARI</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Buli</airport_name>
            <airport_code>WUB</airport_code>
            <location_name>Buli</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Pogugol</airport_name>
            <airport_code>UOL</airport_code>
            <location_name>Buol</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>NGURAH RAI</airport_name>
            <airport_code>DPS</airport_code>
            <location_name>Denpasar, Bali</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>H. Hasan Aroeboesman</airport_name>
            <airport_code>ENE</airport_code>
            <location_name>Ende</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Fakfak</airport_name>
            <airport_code>FKQ</airport_code>
            <location_name>FakFak</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>GALELA</airport_name>
            <airport_code>GLX</airport_code>
            <location_name>Galela</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Jalaluddin</airport_name>
            <airport_code>GTO</airport_code>
            <location_name>Gorontalo</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Gunung Sitoli, Binaka</airport_name>
            <airport_code>GNS</airport_code>
            <location_name>GunungSitoli</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Soekarno Hatta</airport_name>
            <airport_code>CGK</airport_code>
            <location_name>Jakarta - Cengkareng</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>HALIM PERDANAKUSUMA</airport_name>
            <airport_code>HLP</airport_code>
            <location_name>Jakarta - Halim</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Sultan Thaha Syaifuddin</airport_name>
            <airport_code>DJB</airport_code>
            <location_name>Jambi</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Sentani</airport_name>
            <airport_code>DJJ</airport_code>
            <location_name>Jayapura</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Kaimana, Utarom</airport_name>
            <airport_code>KNG</airport_code>
            <location_name>Kaimana</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Haluoleo</airport_name>
            <airport_code>KDI</airport_code>
            <location_name>Kendari</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>RAHADI OESMAN</airport_name>
            <airport_code>KTG</airport_code>
            <location_name>Ketapang</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Kotabaru</airport_name>
            <airport_code>KBU</airport_code>
            <location_name>Kotabaru</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>El Tari</airport_name>
            <airport_code>KOE</airport_code>
            <location_name>Kupang</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Labuanbajo, Komodo</airport_name>
            <airport_code>LBJ</airport_code>
            <location_name>LabuanBajo</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Labuha, Oesman Sadik</airport_name>
            <airport_code>LAH</airport_code>
            <location_name>Labuha</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Radin Inten II</airport_name>
            <airport_code>TKG</airport_code>
            <location_name>Lampung</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Lhokseumawe, Malikussaleh</airport_name>
            <airport_code>LSW</airport_code>
            <location_name>Lhokseumawe</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Lombok</airport_name>
            <airport_code>LOP</airport_code>
            <location_name>Lombok, Mataram</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Syukuran Aminuddin Amir</airport_name>
            <airport_code>LUW</airport_code>
            <location_name>Luwuk</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Abdul Rachman Saleh</airport_name>
            <airport_code>MLG</airport_code>
            <location_name>Malang</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>ROBERT ATTY BESSING</airport_name>
            <airport_code>MLN</airport_code>
            <location_name>Malinau</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Mamuju</airport_name>
            <airport_code>MJU</airport_code>
            <location_name>Mamuju</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Sam Ratulangi</airport_name>
            <airport_code>MDC</airport_code>
            <location_name>Manado</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Rendani</airport_name>
            <airport_code>MKW</airport_code>
            <location_name>Manokwari</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Wai Oti</airport_name>
            <airport_code>MOF</airport_code>
            <location_name>Maumere</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Kuala Namu</airport_name>
            <airport_code>KNO</airport_code>
            <location_name>Medan (Kuala Namu)</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>MELALAN</airport_name>
            <airport_code>MLK</airport_code>
            <location_name>Melak</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Melonguane</airport_name>
            <airport_code>MNA</airport_code>
            <location_name>Melanguane</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Mopah</airport_name>
            <airport_code>MKQ</airport_code>
            <location_name>Merauke</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Meulaboh, Cut Nyak Dien</airport_name>
            <airport_code>MEQ</airport_code>
            <location_name>Meulaboh</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>MOROTAI</airport_name>
            <airport_code>OTI</airport_code>
            <location_name>MOROTAI</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>BANDAR UDARA BERINGIN</airport_name>
            <airport_code>MTW</airport_code>
            <location_name>Muara Teweh</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Nabire</airport_name>
            <airport_code>NBX</airport_code>
            <location_name>Nabire</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Natuna Ranai</airport_name>
            <airport_code>NTX</airport_code>
            <location_name>NatunaRanai</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>NUNUKAN</airport_name>
            <airport_code>NNX</airport_code>
            <location_name>Nunukan</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Minangkabau</airport_name>
            <airport_code>PDG</airport_code>
            <location_name>Padang</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Tjilik Riwut</airport_name>
            <airport_code>PKY</airport_code>
            <location_name>Palangka raya</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Sultan Mahmud Badaruddin II</airport_name>
            <airport_code>PLM</airport_code>
            <location_name>Palembang</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Mutiara</airport_name>
            <airport_code>PLW</airport_code>
            <location_name>Palu</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Depati Amir</airport_name>
            <airport_code>PGK</airport_code>
            <location_name>Pangkal pinang</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>PANGKALAN BUN</airport_name>
            <airport_code>PKN</airport_code>
            <location_name>Pangkalan Bun</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Sultan Syarif Kasim II</airport_name>
            <airport_code>PKU</airport_code>
            <location_name>Pekanbaru</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Sangia Nibandera Pomalaa</airport_name>
            <airport_code>PUM</airport_code>
            <location_name>Pomalaa</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Supadio</airport_name>
            <airport_code>PNK</airport_code>
            <location_name>Pontianak</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Poso, Kasiguncu</airport_name>
            <airport_code>PSJ</airport_code>
            <location_name>Poso</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Mali</airport_name>
            <airport_code>ARD</airport_code>
            <location_name>Pulau Alor</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>PUTUSSIBAU</airport_name>
            <airport_code>PSU</airport_code>
            <location_name>Putussibau</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>ROTE</airport_name>
            <airport_code>RTI</airport_code>
            <location_name>Rote</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Frans Sales Lega</airport_name>
            <airport_code>RTG</airport_code>
            <location_name>Ruteng</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>TEMINDUNG</airport_name>
            <airport_code>SRI</airport_code>
            <location_name>Samarinda</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>H. Asan Sampit</airport_name>
            <airport_code>SMQ</airport_code>
            <location_name>Sampit</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>BANDAR UDARA OLILIT</airport_name>
            <airport_code>SXK</airport_code>
            <location_name>Saumlaki</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>SELAYAR</airport_name>
            <airport_code>YKR</airport_code>
            <location_name>Selayar</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Achmad Yani</airport_name>
            <airport_code>SRG</airport_code>
            <location_name>Semarang</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>SIBOLGA</airport_name>
            <airport_code>RRZ</airport_code>
            <location_name>Sibolga</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Silangit</airport_name>
            <airport_code>DTB</airport_code>
            <location_name>Silangit</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Lasikin</airport_name>
            <airport_code>SNX</airport_code>
            <location_name>Sinabang</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>SUSILO</airport_name>
            <airport_code>SQG</airport_code>
            <location_name>Sintang</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Adisumarmo</airport_name>
            <airport_code>SOC</airport_code>
            <location_name>Solo</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Dominique Edward Osok</airport_name>
            <airport_code>SOQ</airport_code>
            <location_name>Sorong</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Sumbawa, Brang Biji</airport_name>
            <airport_code>SWQ</airport_code>
            <location_name>Sumbawa</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Juanda</airport_name>
            <airport_code>SUB</airport_code>
            <location_name>Surabaya</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Naha</airport_name>
            <airport_code>NAH</airport_code>
            <location_name>Tahuna</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Tampolaka</airport_name>
            <airport_code>TMC</airport_code>
            <location_name>Tambolaka</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>H.A.S Hanandjoeddin</airport_name>
            <airport_code>TJQ</airport_code>
            <location_name>Tanjung Pandan</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Raja Haji FIsabilillah</airport_name>
            <airport_code>TNJ</airport_code>
            <location_name>Tanjung Pinang</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>TANJUNG HARAPAN</airport_name>
            <airport_code>TJS</airport_code>
            <location_name>Tanjung Selor</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>WARUKIN</airport_name>
            <airport_code>TJG</airport_code>
            <location_name>Tanjung Warukin</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Juwata</airport_name>
            <airport_code>TRK</airport_code>
            <location_name>Tarakan</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Sultan Babullah</airport_name>
            <airport_code>TTE</airport_code>
            <location_name>Ternate</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Mozes Kilangin</airport_name>
            <airport_code>TIM</airport_code>
            <location_name>Timika</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Tobelo</airport_name>
            <airport_code>KAZ</airport_code>
            <location_name>Tobelo</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>TOLI TOLI</airport_name>
            <airport_code>TLI</airport_code>
            <location_name>TOLI TOLI</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Tual, Dumatubin</airport_name>
            <airport_code>LUV</airport_code>
            <location_name>Tual</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>SULTAN HASANUDDIN</airport_name>
            <airport_code>UPG</airport_code>
            <location_name>Ujungpandang, Makassar</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>WAINGAPU</airport_name>
            <airport_code>WGP</airport_code>
            <location_name>Waingapu</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Matahora</airport_name>
            <airport_code>WNI</airport_code>
            <location_name>Wakatobi</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>WAMENA</airport_name>
            <airport_code>WMX</airport_code>
            <location_name>Wamena</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Wangi wangi, Matahora</airport_name>
            <airport_code>WGI</airport_code>
            <location_name>Wangi wangi</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>Adi Sutjipto</airport_name>
            <airport_code>JOG</airport_code>
            <location_name>Yogyakarta</location_name>
            <country_id>id</country_id>
            <country_name>Indonesia</country_name>
        </airport>
        <airport>
            <airport_name>ADELAIDE</airport_name>
            <airport_code>ADL</airport_code>
            <location_name>Adelaide</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>Alice Springs</airport_name>
            <airport_code>ASP</airport_code>
            <location_name>Alice Springs</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>AVALON</airport_name>
            <airport_code>AVV</airport_code>
            <location_name>AVALON</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>BALLINA BYRON</airport_name>
            <airport_code>BNK</airport_code>
            <location_name>BALLINA BYRON</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>BRISBANE</airport_name>
            <airport_code>BNE</airport_code>
            <location_name>Brisbane</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>CAIRNS</airport_name>
            <airport_code>CNS</airport_code>
            <location_name>Cairns</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>CANBERRA</airport_name>
            <airport_code>CBR</airport_code>
            <location_name>CANBERRA</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>Coffs Harbour</airport_name>
            <airport_code>CFS</airport_code>
            <location_name>Coffs Harbour</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>DARWIN</airport_name>
            <airport_code>DRW</airport_code>
            <location_name>Darwin</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>GOLD COAST</airport_name>
            <airport_code>OOL</airport_code>
            <location_name>Gold Coast</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>HAMILTON ISLAND</airport_name>
            <airport_code>HTI</airport_code>
            <location_name>HAMILTON ISLAND</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>HAYMAN ISLAND</airport_name>
            <airport_code>HIS</airport_code>
            <location_name>HAYMAN ISLAND</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>HOBART</airport_name>
            <airport_code>HBA</airport_code>
            <location_name>Hobart</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>LAUNCESTON</airport_name>
            <airport_code>LST</airport_code>
            <location_name>Launceston</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>MACKAY</airport_name>
            <airport_code>MKY</airport_code>
            <location_name>Mackay (Whitsundays)</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>MELBOURNE</airport_name>
            <airport_code>MEL</airport_code>
            <location_name>Melbourne</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>MELBOURNE (ALL AIRPORTS)</airport_name>
            <airport_code>VIZ</airport_code>
            <location_name>Melbourne (all airports)</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>NEWCASTLE - PORT STEPHENS</airport_name>
            <airport_code>NTL</airport_code>
            <location_name>NEWCASTLE - PORT STEPHENS</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>PERTH</airport_name>
            <airport_code>PER</airport_code>
            <location_name>Perth</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>SUNSHINE COAST</airport_name>
            <airport_code>MCY</airport_code>
            <location_name>Sunshine Coast</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>SYDNEY (KINGSFORD-SMITH)</airport_name>
            <airport_code>SYD</airport_code>
            <location_name>Sydney</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>TOWNSVILLE</airport_name>
            <airport_code>TSV</airport_code>
            <location_name>TOWNSVILLE</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>ULURU</airport_name>
            <airport_code>AYQ</airport_code>
            <location_name>Uluru</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>WHITSUNDAY COAST - PROSERPINE</airport_name>
            <airport_code>PPP</airport_code>
            <location_name>WHITSUNDAY COAST - PROSERPINE</location_name>
            <country_id>au</country_id>
            <country_name>Australia </country_name>
        </airport>
        <airport>
            <airport_name>SHAH AMANAT</airport_name>
            <airport_code>CGP</airport_code>
            <location_name>Chittagong</location_name>
            <country_id>bd</country_id>
            <country_name>Bangladesh </country_name>
        </airport>
        <airport>
            <airport_name>INDIRA GANDHI</airport_name>
            <airport_code>DEL</airport_code>
            <location_name>Delhi</location_name>
            <country_id>bd</country_id>
            <country_name>Bangladesh </country_name>
        </airport>
        <airport>
            <airport_name>Dhaka</airport_name>
            <airport_code>DAC</airport_code>
            <location_name>Dhaka</location_name>
            <country_id>bd</country_id>
            <country_name>Bangladesh </country_name>
        </airport>
        <airport>
            <airport_name>BRUNEI</airport_name>
            <airport_code>BWN</airport_code>
            <location_name>Brunei</location_name>
            <country_id>bn</country_id>
            <country_name>Brunei Darussalam </country_name>
        </airport>
        <airport>
            <airport_name>PHNOM PENH</airport_name>
            <airport_code>PNH</airport_code>
            <location_name>Phnom Penh</location_name>
            <country_id>kh</country_id>
            <country_name>Cambodia </country_name>
        </airport>
        <airport>
            <airport_name>SIEM REAP</airport_name>
            <airport_code>REP</airport_code>
            <location_name>Siem Reap</location_name>
            <country_id>kh</country_id>
            <country_name>Cambodia </country_name>
        </airport>
        <airport>
            <airport_name>Beijing Capital</airport_name>
            <airport_code>PEK</airport_code>
            <location_name>Beijing</location_name>
            <country_id>cn</country_id>
            <country_name>China </country_name>
        </airport>
        <airport>
            <airport_name>Chengdu Shuangliu</airport_name>
            <airport_code>CTU</airport_code>
            <location_name>Chengdu</location_name>
            <country_id>cn</country_id>
            <country_name>China </country_name>
        </airport>
        <airport>
            <airport_name>Chongqing Jiangbei</airport_name>
            <airport_code>CKG</airport_code>
            <location_name>Chongqing</location_name>
            <country_id>cn</country_id>
            <country_name>China </country_name>
        </airport>
        <airport>
            <airport_name>Guangzhou Baiyun</airport_name>
            <airport_code>CAN</airport_code>
            <location_name>Guangzhou</location_name>
            <country_id>cn</country_id>
            <country_name>China </country_name>
        </airport>
        <airport>
            <airport_name>Guilin Liangjiang</airport_name>
            <airport_code>KWL</airport_code>
            <location_name>Guilin</location_name>
            <country_id>cn</country_id>
            <country_name>China </country_name>
        </airport>
        <airport>
            <airport_name>HAIKOU</airport_name>
            <airport_code>HAK</airport_code>
            <location_name>Haikou</location_name>
            <country_id>cn</country_id>
            <country_name>China </country_name>
        </airport>
        <airport>
            <airport_name>HANGZHOU XIAOSHAN</airport_name>
            <airport_code>HGH</airport_code>
            <location_name>Hangzhou</location_name>
            <country_id>cn</country_id>
            <country_name>China </country_name>
        </airport>
        <airport>
            <airport_name>Kunming Wujiaba</airport_name>
            <airport_code>KMG</airport_code>
            <location_name>Kunming</location_name>
            <country_id>cn</country_id>
            <country_name>China </country_name>
        </airport>
        <airport>
            <airport_name>Nanning Wuxu</airport_name>
            <airport_code>NNG</airport_code>
            <location_name>Nanning</location_name>
            <country_id>cn</country_id>
            <country_name>China </country_name>
        </airport>
        <airport>
            <airport_name>Ningbo Lishe</airport_name>
            <airport_code>NGB</airport_code>
            <location_name>Ningbo</location_name>
            <country_id>cn</country_id>
            <country_name>China </country_name>
        </airport>
        <airport>
            <airport_name>Qingdao</airport_name>
            <airport_code>TAO</airport_code>
            <location_name>Qingdao</location_name>
            <country_id>cn</country_id>
            <country_name>China </country_name>
        </airport>
        <airport>
            <airport_name>Shanghai Pudong</airport_name>
            <airport_code>PVG</airport_code>
            <location_name>Shanghai</location_name>
            <country_id>cn</country_id>
            <country_name>China </country_name>
        </airport>
        <airport>
            <airport_name>SHANTOU / JIEYANG</airport_name>
            <airport_code>SWA</airport_code>
            <location_name>SHANTOU / JIEYANG</location_name>
            <country_id>cn</country_id>
            <country_name>China </country_name>
        </airport>
        <airport>
            <airport_name>Shenyang</airport_name>
            <airport_code>SHE</airport_code>
            <location_name>Shenyang</location_name>
            <country_id>cn</country_id>
            <country_name>China </country_name>
        </airport>
        <airport>
            <airport_name>Shenzhen</airport_name>
            <airport_code>SZX</airport_code>
            <location_name>Shenzhen</location_name>
            <country_id>cn</country_id>
            <country_name>China </country_name>
        </airport>
        <airport>
            <airport_name>Tianjin</airport_name>
            <airport_code>TSN</airport_code>
            <location_name>Tianjin</location_name>
            <country_id>cn</country_id>
            <country_name>China </country_name>
        </airport>
        <airport>
            <airport_name>Wuhan Tianhe</airport_name>
            <airport_code>WUH</airport_code>
            <location_name>Wuhan</location_name>
            <country_id>cn</country_id>
            <country_name>China </country_name>
        </airport>
        <airport>
            <airport_name>Xi An Xianyang</airport_name>
            <airport_code>XIY</airport_code>
            <location_name>Xi'an</location_name>
            <country_id>cn</country_id>
            <country_name>China </country_name>
        </airport>
        <airport>
            <airport_name>Naike</airport_name>
            <airport_code>CMB</airport_code>
            <location_name>Colombo</location_name>
            <country_id>co</country_id>
            <country_name>Colombia </country_name>
        </airport>
        <airport>
            <airport_name>NADI</airport_name>
            <airport_code>NAN</airport_code>
            <location_name>NADI</location_name>
            <country_id>fj</country_id>
            <country_name>Fiji </country_name>
        </airport>
        <airport>
            <airport_name>HONG KONG</airport_name>
            <airport_code>HKG</airport_code>
            <location_name>Hong Kong</location_name>
            <country_id>hk</country_id>
            <country_name>Hong Kong </country_name>
        </airport>
        <airport>
            <airport_name>SARDAR VALLABHBHAI PATEL</airport_name>
            <airport_code>AMD</airport_code>
            <location_name>Ahmedabad</location_name>
            <country_id>in</country_id>
            <country_name>India </country_name>
        </airport>
        <airport>
            <airport_name>Bangalore</airport_name>
            <airport_code>BLR</airport_code>
            <location_name>Bangalore</location_name>
            <country_id>in</country_id>
            <country_name>India </country_name>
        </airport>
        <airport>
            <airport_name>Chennai</airport_name>
            <airport_code>MAA</airport_code>
            <location_name>Chennai</location_name>
            <country_id>in</country_id>
            <country_name>India </country_name>
        </airport>
        <airport>
            <airport_name>Hyderabad</airport_name>
            <airport_code>HYD</airport_code>
            <location_name>Hyderabad</location_name>
            <country_id>in</country_id>
            <country_name>India </country_name>
        </airport>
        <airport>
            <airport_name>Kochi</airport_name>
            <airport_code>COK</airport_code>
            <location_name>Kochi</location_name>
            <country_id>in</country_id>
            <country_name>India </country_name>
        </airport>
        <airport>
            <airport_name>Netaji Subhas Chandra Bosen</airport_name>
            <airport_code>CCU</airport_code>
            <location_name>Kolkata</location_name>
            <country_id>in</country_id>
            <country_name>India </country_name>
        </airport>
        <airport>
            <airport_name>CHHATRAPATI SHIVAJI</airport_name>
            <airport_code>BOM</airport_code>
            <location_name>Mumbai</location_name>
            <country_id>in</country_id>
            <country_name>India </country_name>
        </airport>
        <airport>
            <airport_name>Thiruvananthapuram</airport_name>
            <airport_code>TRV</airport_code>
            <location_name>Thiruvananthapuram</location_name>
            <country_id>in</country_id>
            <country_name>India </country_name>
        </airport>
        <airport>
            <airport_name>Tiruchirapalli (Trichy)</airport_name>
            <airport_code>TRZ</airport_code>
            <location_name>Tiruchirapalli (Trichy)</location_name>
            <country_id>in</country_id>
            <country_name>India </country_name>
        </airport>
        <airport>
            <airport_name>FUKUOKA</airport_name>
            <airport_code>FUK</airport_code>
            <location_name>Fukuoka</location_name>
            <country_id>jp</country_id>
            <country_name>Japan </country_name>
        </airport>
        <airport>
            <airport_name>KAGOSHIMA</airport_name>
            <airport_code>KOJ</airport_code>
            <location_name>Kagoshima</location_name>
            <country_id>jp</country_id>
            <country_name>Japan </country_name>
        </airport>
        <airport>
            <airport_name>KUMAMOTO</airport_name>
            <airport_code>KMJ</airport_code>
            <location_name>Kumamoto</location_name>
            <country_id>jp</country_id>
            <country_name>Japan </country_name>
        </airport>
        <airport>
            <airport_name>MATSUYAMA</airport_name>
            <airport_code>MYJ</airport_code>
            <location_name>Matsuyama</location_name>
            <country_id>jp</country_id>
            <country_name>Japan </country_name>
        </airport>
        <airport>
            <airport_name>NAGOYA CHUBU CENTRAIR</airport_name>
            <airport_code>NGO</airport_code>
            <location_name>Nagoya</location_name>
            <country_id>jp</country_id>
            <country_name>Japan </country_name>
        </airport>
        <airport>
            <airport_name>OITA</airport_name>
            <airport_code>OIT</airport_code>
            <location_name>Oita</location_name>
            <country_id>jp</country_id>
            <country_name>Japan </country_name>
        </airport>
        <airport>
            <airport_name>OKINAWA, NAHA</airport_name>
            <airport_code>OKA</airport_code>
            <location_name>Okinawa - Naha</location_name>
            <country_id>jp</country_id>
            <country_name>Japan </country_name>
        </airport>
        <airport>
            <airport_name>OSAKA, KANSAI</airport_name>
            <airport_code>KIX</airport_code>
            <location_name>Osaka - Kansai</location_name>
            <country_id>jp</country_id>
            <country_name>Japan </country_name>
        </airport>
        <airport>
            <airport_name>SAPPORO, SHIN-CHITOSE</airport_name>
            <airport_code>CTS</airport_code>
            <location_name>Sapporo - Shin-Chitose</location_name>
            <country_id>jp</country_id>
            <country_name>Japan </country_name>
        </airport>
        <airport>
            <airport_name>TAKAMATSU </airport_name>
            <airport_code>TAK</airport_code>
            <location_name>Takamatsu </location_name>
            <country_id>jp</country_id>
            <country_name>Japan </country_name>
        </airport>
        <airport>
            <airport_name>Tokyo, Haneda</airport_name>
            <airport_code>HND</airport_code>
            <location_name>Tokyo - Haneda</location_name>
            <country_id>jp</country_id>
            <country_name>Japan </country_name>
        </airport>
        <airport>
            <airport_name>TOKYO, NARITA</airport_name>
            <airport_code>NRT</airport_code>
            <location_name>Tokyo - Narita</location_name>
            <country_id>jp</country_id>
            <country_name>Japan </country_name>
        </airport>
        <airport>
            <airport_name>Wattay</airport_name>
            <airport_code>VTE</airport_code>
            <location_name>Vientiane</location_name>
            <country_id>la</country_id>
            <country_name>Laos</country_name>
        </airport>
        <airport>
            <airport_name>MACAU</airport_name>
            <airport_code>MFM</airport_code>
            <location_name>Macau</location_name>
            <country_id>mo</country_id>
            <country_name>Macau </country_name>
        </airport>
        <airport>
            <airport_name>Sultan Abdul Halim</airport_name>
            <airport_code>AOR</airport_code>
            <location_name>Alor Setar</location_name>
            <country_id>my</country_id>
            <country_name>Malaysia </country_name>
        </airport>
        <airport>
            <airport_name>Bintulu</airport_name>
            <airport_code>BTU</airport_code>
            <location_name>Bintulu</location_name>
            <country_id>my</country_id>
            <country_name>Malaysia </country_name>
        </airport>
        <airport>
            <airport_name>Senai</airport_name>
            <airport_code>JHB</airport_code>
            <location_name>Johor Baru</location_name>
            <country_id>my</country_id>
            <country_name>Malaysia </country_name>
        </airport>
        <airport>
            <airport_name>Sultan Ismail Petra</airport_name>
            <airport_code>KBR</airport_code>
            <location_name>Kota Bharu</location_name>
            <country_id>my</country_id>
            <country_name>Malaysia </country_name>
        </airport>
        <airport>
            <airport_name>Kota Kinabalu</airport_name>
            <airport_code>BKI</airport_code>
            <location_name>Kota Kinabalu</location_name>
            <country_id>my</country_id>
            <country_name>Malaysia </country_name>
        </airport>
        <airport>
            <airport_name>KUALA LUMPUR</airport_name>
            <airport_code>KUL</airport_code>
            <location_name>Kuala Lumpur</location_name>
            <country_id>my</country_id>
            <country_name>Malaysia </country_name>
        </airport>
        <airport>
            <airport_name>SULTAN MAHMUD</airport_name>
            <airport_code>TGG</airport_code>
            <location_name>Kuala Terengganu</location_name>
            <country_id>my</country_id>
            <country_name>Malaysia </country_name>
        </airport>
        <airport>
            <airport_name>Kuching</airport_name>
            <airport_code>KCH</airport_code>
            <location_name>Kuching</location_name>
            <country_id>my</country_id>
            <country_name>Malaysia </country_name>
        </airport>
        <airport>
            <airport_name>Langkawi</airport_name>
            <airport_code>LGK</airport_code>
            <location_name>Langkawi</location_name>
            <country_id>my</country_id>
            <country_name>Malaysia </country_name>
        </airport>
        <airport>
            <airport_name>Malacca</airport_name>
            <airport_code>MKZ</airport_code>
            <location_name>Malacca</location_name>
            <country_id>my</country_id>
            <country_name>Malaysia </country_name>
        </airport>
        <airport>
            <airport_name>Miri</airport_name>
            <airport_code>MYY</airport_code>
            <location_name>Miri</location_name>
            <country_id>my</country_id>
            <country_name>Malaysia </country_name>
        </airport>
        <airport>
            <airport_name>PENANG</airport_name>
            <airport_code>PEN</airport_code>
            <location_name>Penang</location_name>
            <country_id>my</country_id>
            <country_name>Malaysia </country_name>
        </airport>
        <airport>
            <airport_name>Sandakan</airport_name>
            <airport_code>SDK</airport_code>
            <location_name>Sandaka</location_name>
            <country_id>my</country_id>
            <country_name>Malaysia </country_name>
        </airport>
        <airport>
            <airport_name>Sibu</airport_name>
            <airport_code>SBW</airport_code>
            <location_name>Sibu</location_name>
            <country_id>my</country_id>
            <country_name>Malaysia </country_name>
        </airport>
        <airport>
            <airport_name>Sultan Abdul Aziz Shah</airport_name>
            <airport_code>SZB</airport_code>
            <location_name>Subang</location_name>
            <country_id>my</country_id>
            <country_name>Malaysia </country_name>
        </airport>
        <airport>
            <airport_name>IPOH</airport_name>
            <airport_code>IPH</airport_code>
            <location_name>SULTAN AZLAN SHAH</location_name>
            <country_id>my</country_id>
            <country_name>Malaysia </country_name>
        </airport>
        <airport>
            <airport_name>Tawau</airport_name>
            <airport_code>TWU</airport_code>
            <location_name>Tawau</location_name>
            <country_id>my</country_id>
            <country_name>Malaysia </country_name>
        </airport>
        <airport>
            <airport_name>Mandalay</airport_name>
            <airport_code>MDL</airport_code>
            <location_name>Mandalay</location_name>
            <country_id>mm</country_id>
            <country_name>Myanmar </country_name>
        </airport>
        <airport>
            <airport_name>YANGOON</airport_name>
            <airport_code>RGN</airport_code>
            <location_name>Yangoon</location_name>
            <country_id>mm</country_id>
            <country_name>Myanmar </country_name>
        </airport>
        <airport>
            <airport_name>Tribhuvan</airport_name>
            <airport_code>KTM</airport_code>
            <location_name>Kathmandu</location_name>
            <country_id>np</country_id>
            <country_name>Nepal </country_name>
        </airport>
        <airport>
            <airport_name>SCHIPHOL</airport_name>
            <airport_code>AMS</airport_code>
            <location_name>SCHIPHOL</location_name>
            <country_id>nl</country_id>
            <country_name>Netherlands </country_name>
        </airport>
        <airport>
            <airport_name>AUCKLAND</airport_name>
            <airport_code>AKL</airport_code>
            <location_name>AUCKLAND</location_name>
            <country_id>nz</country_id>
            <country_name>New Zealand </country_name>
        </airport>
        <airport>
            <airport_name>CHRISTCHURCH</airport_name>
            <airport_code>CHC</airport_code>
            <location_name>CHRISTCHURCH</location_name>
            <country_id>nz</country_id>
            <country_name>New Zealand </country_name>
        </airport>
        <airport>
            <airport_name>DUNEDIN</airport_name>
            <airport_code>DUD</airport_code>
            <location_name>DUNEDIN</location_name>
            <country_id>nz</country_id>
            <country_name>New Zealand </country_name>
        </airport>
        <airport>
            <airport_name>QUEENSTOWN</airport_name>
            <airport_code>ZQN</airport_code>
            <location_name>QUEENSTOWN</location_name>
            <country_id>nz</country_id>
            <country_name>New Zealand </country_name>
        </airport>
        <airport>
            <airport_name>WELLINGTON</airport_name>
            <airport_code>WLG</airport_code>
            <location_name>WELLINGTON</location_name>
            <country_id>nz</country_id>
            <country_name>New Zealand </country_name>
        </airport>
        <airport>
            <airport_name>Bacolod</airport_name>
            <airport_code>BCD</airport_code>
            <location_name>Bacolod</location_name>
            <country_id>ph</country_id>
            <country_name>Philippines </country_name>
        </airport>
        <airport>
            <airport_name>Mactan-Cebu</airport_name>
            <airport_code>CEB</airport_code>
            <location_name>Cebu</location_name>
            <country_id>ph</country_id>
            <country_name>Philippines </country_name>
        </airport>
        <airport>
            <airport_name>CLARK</airport_name>
            <airport_code>CRK</airport_code>
            <location_name>Clark</location_name>
            <country_id>ph</country_id>
            <country_name>Philippines </country_name>
        </airport>
        <airport>
            <airport_name>Davao</airport_name>
            <airport_code>DVO</airport_code>
            <location_name>Davao</location_name>
            <country_id>ph</country_id>
            <country_name>Philippines </country_name>
        </airport>
        <airport>
            <airport_name>Iloilo</airport_name>
            <airport_code>ILO</airport_code>
            <location_name>Iloilo</location_name>
            <country_id>ph</country_id>
            <country_name>Philippines </country_name>
        </airport>
        <airport>
            <airport_name>NINOY AQUINO</airport_name>
            <airport_code>MNL</airport_code>
            <location_name>Manila (NAIA)</location_name>
            <country_id>ph</country_id>
            <country_name>Philippines </country_name>
        </airport>
        <airport>
            <airport_name>Puerto Princesa</airport_name>
            <airport_code>PPS</airport_code>
            <location_name>Puerto Princesa</location_name>
            <country_id>ph</country_id>
            <country_name>Philippines </country_name>
        </airport>
        <airport>
            <airport_name>Tacloban</airport_name>
            <airport_code>TAC</airport_code>
            <location_name>Tacloban</location_name>
            <country_id>ph</country_id>
            <country_name>Philippines </country_name>
        </airport>
        <airport>
            <airport_name>King Abdulaziz</airport_name>
            <airport_code>JED</airport_code>
            <location_name>Jeddah</location_name>
            <country_id>sa</country_id>
            <country_name>Saudi Arabia </country_name>
        </airport>
        <airport>
            <airport_name>Changi</airport_name>
            <airport_code>SIN</airport_code>
            <location_name>Singapore</location_name>
            <country_id>sg</country_id>
            <country_name>Singapore </country_name>
        </airport>
        <airport>
            <airport_name>Gimhae</airport_name>
            <airport_code>PUS</airport_code>
            <location_name>Busan</location_name>
            <country_id>kr</country_id>
            <country_name>South Korea</country_name>
        </airport>
        <airport>
            <airport_name>Incheon</airport_name>
            <airport_code>ICN</airport_code>
            <location_name>Seoul</location_name>
            <country_id>kr</country_id>
            <country_name>South Korea</country_name>
        </airport>
        <airport>
            <airport_name>TAIWAN TAOYUAN</airport_name>
            <airport_code>TPE</airport_code>
            <location_name>Taipei</location_name>
            <country_id>tw</country_id>
            <country_name>Taiwan</country_name>
        </airport>
        <airport>
            <airport_name>DON MUEANG</airport_name>
            <airport_code>DMK</airport_code>
            <location_name>Bangkok - Don Mueang</location_name>
            <country_id>th</country_id>
            <country_name>Thailand </country_name>
        </airport>
        <airport>
            <airport_name>SUVARNABHUMI</airport_name>
            <airport_code>BKK</airport_code>
            <location_name>Bangkok - Suvarnabhumi</location_name>
            <country_id>th</country_id>
            <country_name>Thailand </country_name>
        </airport>
        <airport>
            <airport_name>CHIANG MAI</airport_name>
            <airport_code>CNX</airport_code>
            <location_name>Chiang Mai</location_name>
            <country_id>th</country_id>
            <country_name>Thailand </country_name>
        </airport>
        <airport>
            <airport_name>Mae Fah Luang-Chiang Rai</airport_name>
            <airport_code>CEI</airport_code>
            <location_name>Chiang Rai</location_name>
            <country_id>th</country_id>
            <country_name>Thailand </country_name>
        </airport>
        <airport>
            <airport_name>Hat Yai</airport_name>
            <airport_code>HDY</airport_code>
            <location_name>Hat Yai</location_name>
            <country_id>th</country_id>
            <country_name>Thailand </country_name>
        </airport>
        <airport>
            <airport_name>Krabi</airport_name>
            <airport_code>KBV</airport_code>
            <location_name>Krabi</location_name>
            <country_id>th</country_id>
            <country_name>Thailand </country_name>
        </airport>
        <airport>
            <airport_name>Nakhon Phanom</airport_name>
            <airport_code>KOP</airport_code>
            <location_name>Nakhon Phanom</location_name>
            <country_id>th</country_id>
            <country_name>Thailand </country_name>
        </airport>
        <airport>
            <airport_name>Nakhon Si Thammarat</airport_name>
            <airport_code>NST</airport_code>
            <location_name>Nakhon Si Thammarat</location_name>
            <country_id>th</country_id>
            <country_name>Thailand </country_name>
        </airport>
        <airport>
            <airport_name>Narathiwat</airport_name>
            <airport_code>NAW</airport_code>
            <location_name>Narathiwat</location_name>
            <country_id>th</country_id>
            <country_name>Thailand </country_name>
        </airport>
        <airport>
            <airport_name>PHUKET</airport_name>
            <airport_code>HKT</airport_code>
            <location_name>Phuket</location_name>
            <country_id>th</country_id>
            <country_name>Thailand </country_name>
        </airport>
        <airport>
            <airport_name>Surat Thani</airport_name>
            <airport_code>URT</airport_code>
            <location_name>Surat Thani</location_name>
            <country_id>th</country_id>
            <country_name>Thailand </country_name>
        </airport>
        <airport>
            <airport_name>Trang</airport_name>
            <airport_code>TST</airport_code>
            <location_name>Trang</location_name>
            <country_id>th</country_id>
            <country_name>Thailand </country_name>
        </airport>
        <airport>
            <airport_name>Ubon Ratchathani</airport_name>
            <airport_code>UBP</airport_code>
            <location_name>Ubon Ratchathani</location_name>
            <country_id>th</country_id>
            <country_name>Thailand </country_name>
        </airport>
        <airport>
            <airport_name>Udonthani</airport_name>
            <airport_code>UTH</airport_code>
            <location_name>Udon Thani</location_name>
            <country_id>th</country_id>
            <country_name>Thailand </country_name>
        </airport>
        <airport>
            <airport_name>Presidente Nicolau Lobato</airport_name>
            <airport_code>DIL</airport_code>
            <location_name>Dili</location_name>
            <country_id>tl</country_id>
            <country_name>Timor-Leste </country_name>
        </airport>
        <airport>
            <airport_name>ABU DHABI</airport_name>
            <airport_code>ABU</airport_code>
            <location_name>Abu Dhabi</location_name>
            <country_id>ae</country_id>
            <country_name>United Arab Emirates </country_name>
        </airport>
        <airport>
            <airport_name>ABU DHABI</airport_name>
            <airport_code>AUH</airport_code>
            <location_name>Abu Dhabi</location_name>
            <country_id>ae</country_id>
            <country_name>United Arab Emirates </country_name>
        </airport>
        <airport>
            <airport_name>DUBAI INTERNATIONAL AIRPORT</airport_name>
            <airport_code>DXB</airport_code>
            <location_name>Dubai</location_name>
            <country_id>ae</country_id>
            <country_name>United Arab Emirates </country_name>
        </airport>
        <airport>
            <airport_name>DYCE AIRPORT</airport_name>
            <airport_code>ABZ</airport_code>
            <location_name>edinbrugh</location_name>
            <country_id>gb</country_id>
            <country_name>United Kingdom </country_name>
        </airport>
        <airport>
            <airport_name>LONDON</airport_name>
            <airport_code>LGW</airport_code>
            <location_name>London</location_name>
            <country_id>gb</country_id>
            <country_name>United Kingdom </country_name>
        </airport>
        <airport>
            <airport_name>LONDON HEATHROW</airport_name>
            <airport_code>LHR</airport_code>
            <location_name>palmers green</location_name>
            <country_id>gb</country_id>
            <country_name>United Kingdom </country_name>
        </airport>
        <airport>
            <airport_name>HONOLULU</airport_name>
            <airport_code>HNL</airport_code>
            <location_name>HONOLULU</location_name>
            <country_id>us</country_id>
            <country_name>United States </country_name>
        </airport>
        <airport>
            <airport_name>LOS ANGELES INTERNATIONAL AIRPORT</airport_name>
            <airport_code>LAX</airport_code>
            <location_name>Los Angeles</location_name>
            <country_id>us</country_id>
            <country_name>United States </country_name>
        </airport>
        <airport>
            <airport_name>SAN DIEGO INTERNATIONAL AIRPORT</airport_name>
            <airport_code>SAN</airport_code>
            <location_name>North Harbor Drive San Diego</location_name>
            <country_id>us</country_id>
            <country_name>United States </country_name>
        </airport>
        <airport>
            <airport_name>BUON MA THUOT</airport_name>
            <airport_code>BMV</airport_code>
            <location_name>Buon Ma Thuot</location_name>
            <country_id>vn</country_id>
            <country_name>Vietnam </country_name>
        </airport>
        <airport>
            <airport_name>DA NANG</airport_name>
            <airport_code>DAD</airport_code>
            <location_name>Da Nang</location_name>
            <country_id>vn</country_id>
            <country_name>Vietnam </country_name>
        </airport>
        <airport>
            <airport_name>DONG HOI</airport_name>
            <airport_code>VDH</airport_code>
            <location_name>Dong Hoi</location_name>
            <country_id>vn</country_id>
            <country_name>Vietnam </country_name>
        </airport>
        <airport>
            <airport_name>HAI PHONG</airport_name>
            <airport_code>HPH</airport_code>
            <location_name>Hai Phong</location_name>
            <country_id>vn</country_id>
            <country_name>Vietnam </country_name>
        </airport>
        <airport>
            <airport_name>TAN SON NHAT</airport_name>
            <airport_code>SGN</airport_code>
            <location_name>Ho Chi Minh City</location_name>
            <country_id>vn</country_id>
            <country_name>Vietnam </country_name>
        </airport>
        <airport>
            <airport_name>HUI</airport_name>
            <airport_code>HUI</airport_code>
            <location_name>HUI</location_name>
            <country_id>vn</country_id>
            <country_name>Vietnam </country_name>
        </airport>
        <airport>
            <airport_name>NHA TRANG</airport_name>
            <airport_code>CXR</airport_code>
            <location_name>Nha Trang</location_name>
            <country_id>vn</country_id>
            <country_name>Vietnam </country_name>
        </airport>
        <airport>
            <airport_name>NOI BAI</airport_name>
            <airport_code>HAN</airport_code>
            <location_name>Noi Bai</location_name>
            <country_id>vn</country_id>
            <country_name>Vietnam </country_name>
        </airport>
        <airport>
            <airport_name>PHU QUOC</airport_name>
            <airport_code>PQC</airport_code>
            <location_name>Phu Quoc</location_name>
            <country_id>vn</country_id>
            <country_name>Vietnam </country_name>
        </airport>
        <airport>
            <airport_name>QUY NHON</airport_name>
            <airport_code>UIH</airport_code>
            <location_name>Quy Nhon </location_name>
            <country_id>vn</country_id>
            <country_name>Vietnam </country_name>
        </airport>
        <airport>
            <airport_name>THANH HOA</airport_name>
            <airport_code>THD</airport_code>
            <location_name>Thanh Hoa</location_name>
            <country_id>vn</country_id>
            <country_name>Vietnam </country_name>
        </airport>
        <airport>
            <airport_name>TUY HOA</airport_name>
            <airport_code>TBB</airport_code>
            <location_name>Tuy Hoa</location_name>
            <country_id>vn</country_id>
            <country_name>Vietnam </country_name>
        </airport>
        <airport>
            <airport_name>VINH</airport_name>
            <airport_code>VII</airport_code>
            <location_name>Vinh</location_name>
            <country_id>vn</country_id>
            <country_name>Vietnam </country_name>
        </airport>
    </all_airport>
    <login_status>false</login_status>
    <token>f9b29ac359ca5d77755e7588751c089bf96f0dc9</token>
</tiket>
```



```json
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.1006",
    "memoryusage": "6.39MB",
    "unix_timestamp": 1470280239,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "all_airport": {
    "airport": [
      {
        "airport_name": "Mali",
        "airport_code": "ARD",
        "location_name": "Alor Island",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Pattimura",
        "airport_code": "AMQ",
        "location_name": "Ambon",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "ATAMBUA",
        "airport_code": "ABU",
        "location_name": "Atambua",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Soa",
        "airport_code": "BJW",
        "location_name": "Bajawa",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Sepinggan",
        "airport_code": "BPN",
        "location_name": "BalikPapan",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Sultan Iskandar Muda",
        "airport_code": "BTJ",
        "location_name": "Banda Aceh",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Husein Sastranegara",
        "airport_code": "BDO",
        "location_name": "Bandung",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "SYAMSUDDIN NOOR",
        "airport_code": "BDJ",
        "location_name": "Banjarmasin",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "BLIMBINGSARI",
        "airport_code": "DQJ",
        "location_name": "Banyuwangi - BLIMBINGSARI",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Hang Nadim",
        "airport_code": "BTH",
        "location_name": "Batam",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Baubau",
        "airport_code": "BUW",
        "location_name": "Baubau",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Fatmawati Soekarno",
        "airport_code": "BKS",
        "location_name": "Bengkulu",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Kalimarau",
        "airport_code": "BEJ",
        "location_name": "Berau",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "BANDAR UDARA BERINGIN",
        "airport_code": "MTW",
        "location_name": "Beringin Airport",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Frans Kaisiepo",
        "airport_code": "BIK",
        "location_name": "Biak",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Muhammad Salahuddin",
        "airport_code": "BMU",
        "location_name": "Bima",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "BLIMBINGSARI",
        "airport_code": "BWX",
        "location_name": "BLIMBINGSARI",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Buli",
        "airport_code": "WUB",
        "location_name": "Buli",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Pogugol",
        "airport_code": "UOL",
        "location_name": "Buol",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "NGURAH RAI",
        "airport_code": "DPS",
        "location_name": "Denpasar, Bali",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "H. Hasan Aroeboesman",
        "airport_code": "ENE",
        "location_name": "Ende",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Fakfak",
        "airport_code": "FKQ",
        "location_name": "FakFak",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "GALELA",
        "airport_code": "GLX",
        "location_name": "Galela",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Jalaluddin",
        "airport_code": "GTO",
        "location_name": "Gorontalo",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Gunung Sitoli, Binaka",
        "airport_code": "GNS",
        "location_name": "GunungSitoli",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Soekarno Hatta",
        "airport_code": "CGK",
        "location_name": "Jakarta - Cengkareng",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "HALIM PERDANAKUSUMA",
        "airport_code": "HLP",
        "location_name": "Jakarta - Halim",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Sultan Thaha Syaifuddin",
        "airport_code": "DJB",
        "location_name": "Jambi",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Sentani",
        "airport_code": "DJJ",
        "location_name": "Jayapura",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Kaimana, Utarom",
        "airport_code": "KNG",
        "location_name": "Kaimana",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Haluoleo",
        "airport_code": "KDI",
        "location_name": "Kendari",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "RAHADI OESMAN",
        "airport_code": "KTG",
        "location_name": "Ketapang",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Kotabaru",
        "airport_code": "KBU",
        "location_name": "Kotabaru",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "El Tari",
        "airport_code": "KOE",
        "location_name": "Kupang",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Labuanbajo, Komodo",
        "airport_code": "LBJ",
        "location_name": "LabuanBajo",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Labuha, Oesman Sadik",
        "airport_code": "LAH",
        "location_name": "Labuha",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Radin Inten II",
        "airport_code": "TKG",
        "location_name": "Lampung",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Lhokseumawe, Malikussaleh",
        "airport_code": "LSW",
        "location_name": "Lhokseumawe",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Lombok",
        "airport_code": "LOP",
        "location_name": "Lombok, Mataram",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Syukuran Aminuddin Amir",
        "airport_code": "LUW",
        "location_name": "Luwuk",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Abdul Rachman Saleh",
        "airport_code": "MLG",
        "location_name": "Malang",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "ROBERT ATTY BESSING",
        "airport_code": "MLN",
        "location_name": "Malinau",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Mamuju",
        "airport_code": "MJU",
        "location_name": "Mamuju",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Sam Ratulangi",
        "airport_code": "MDC",
        "location_name": "Manado",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Rendani",
        "airport_code": "MKW",
        "location_name": "Manokwari",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Wai Oti",
        "airport_code": "MOF",
        "location_name": "Maumere",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Kuala Namu",
        "airport_code": "KNO",
        "location_name": "Medan (Kuala Namu)",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "MELALAN",
        "airport_code": "MLK",
        "location_name": "Melak",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Melonguane",
        "airport_code": "MNA",
        "location_name": "Melanguane",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Mopah",
        "airport_code": "MKQ",
        "location_name": "Merauke",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Meulaboh, Cut Nyak Dien",
        "airport_code": "MEQ",
        "location_name": "Meulaboh",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "MOROTAI",
        "airport_code": "OTI",
        "location_name": "MOROTAI",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Nabire",
        "airport_code": "NBX",
        "location_name": "Nabire",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Natuna Ranai",
        "airport_code": "NTX",
        "location_name": "NatunaRanai",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "NUNUKAN",
        "airport_code": "NNX",
        "location_name": "Nunukan",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Minangkabau",
        "airport_code": "PDG",
        "location_name": "Padang",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Tjilik Riwut",
        "airport_code": "PKY",
        "location_name": "Palangka raya",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Sultan Mahmud Badaruddin II",
        "airport_code": "PLM",
        "location_name": "Palembang",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Mutiara",
        "airport_code": "PLW",
        "location_name": "Palu",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Depati Amir",
        "airport_code": "PGK",
        "location_name": "Pangkal pinang",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "PANGKALAN BUN",
        "airport_code": "PKN",
        "location_name": "Pangkalan Bun",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Sultan Syarif Kasim II",
        "airport_code": "PKU",
        "location_name": "Pekanbaru",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Sangia Nibandera Pomalaa",
        "airport_code": "PUM",
        "location_name": "Pomalaa",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Supadio",
        "airport_code": "PNK",
        "location_name": "Pontianak",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Poso, Kasiguncu",
        "airport_code": "PSJ",
        "location_name": "Poso",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "PUTUSSIBAU",
        "airport_code": "PSU",
        "location_name": "Putussibau",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "ROTE",
        "airport_code": "RTI",
        "location_name": "Rote",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Frans Sales Lega",
        "airport_code": "RTG",
        "location_name": "Ruteng",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "TEMINDUNG",
        "airport_code": "SRI",
        "location_name": "Samarinda",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "H. Asan Sampit",
        "airport_code": "SMQ",
        "location_name": "Sampit",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "BANDAR UDARA OLILIT",
        "airport_code": "SXK",
        "location_name": "Saumlaki",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "SELAYAR",
        "airport_code": "YKR",
        "location_name": "Selayar",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Achmad Yani",
        "airport_code": "SRG",
        "location_name": "Semarang",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "SIBOLGA",
        "airport_code": "RRZ",
        "location_name": "Sibolga",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Silangit",
        "airport_code": "DTB",
        "location_name": "Silangit",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Lasikin",
        "airport_code": "SNX",
        "location_name": "Sinabang",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "SUSILO",
        "airport_code": "SQG",
        "location_name": "Sintang",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Adisumarmo",
        "airport_code": "SOC",
        "location_name": "Solo",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Dominique Edward Osok",
        "airport_code": "SOQ",
        "location_name": "Sorong",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Sumbawa, Brang Biji",
        "airport_code": "SWQ",
        "location_name": "Sumbawa",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Juanda",
        "airport_code": "SUB",
        "location_name": "Surabaya",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Naha",
        "airport_code": "NAH",
        "location_name": "Tahuna",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Tampolaka",
        "airport_code": "TMC",
        "location_name": "Tambolaka",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "H.A.S Hanandjoeddin",
        "airport_code": "TJQ",
        "location_name": "Tanjung Pandan",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Raja Haji FIsabilillah",
        "airport_code": "TNJ",
        "location_name": "Tanjung Pinang",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "TANJUNG HARAPAN",
        "airport_code": "TJS",
        "location_name": "Tanjung Selor",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "WARUKIN",
        "airport_code": "TJG",
        "location_name": "Tanjung Warukin",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Juwata",
        "airport_code": "TRK",
        "location_name": "Tarakan",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Sultan Babullah",
        "airport_code": "TTE",
        "location_name": "Ternate",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Mozes Kilangin",
        "airport_code": "TIM",
        "location_name": "Timika",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Tobelo",
        "airport_code": "KAZ",
        "location_name": "Tobelo",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "TOLI TOLI",
        "airport_code": "TLI",
        "location_name": "TOLI TOLI",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Tual, Dumatubin",
        "airport_code": "LUV",
        "location_name": "Tual",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "SULTAN HASANUDDIN",
        "airport_code": "UPG",
        "location_name": "Ujungpandang, Makassar",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "WAINGAPU",
        "airport_code": "WGP",
        "location_name": "Waingapu",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Matahora",
        "airport_code": "WNI",
        "location_name": "Wakatobi",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "WAMENA",
        "airport_code": "WMX",
        "location_name": "Wamena",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Wangi wangi, Matahora",
        "airport_code": "WGI",
        "location_name": "Wangi wangi",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "Adi Sutjipto",
        "airport_code": "JOG",
        "location_name": "Yogyakarta",
        "country_id": "id",
        "country_name": "Indonesia"
      },
      {
        "airport_name": "ADELAIDE",
        "airport_code": "ADL",
        "location_name": "Adelaide",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "Alice Springs",
        "airport_code": "ASP",
        "location_name": "Alice Springs",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "AVALON",
        "airport_code": "AVV",
        "location_name": "AVALON",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "BALLINA BYRON",
        "airport_code": "BNK",
        "location_name": "BALLINA BYRON",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "BRISBANE",
        "airport_code": "BNE",
        "location_name": "Brisbane",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "CAIRNS",
        "airport_code": "CNS",
        "location_name": "Cairns",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "CANBERRA",
        "airport_code": "CBR",
        "location_name": "CANBERRA",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "Coffs Harbour",
        "airport_code": "CFS",
        "location_name": "Coffs Harbour",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "DARWIN",
        "airport_code": "DRW",
        "location_name": "Darwin",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "GOLD COAST",
        "airport_code": "OOL",
        "location_name": "Gold Coast",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "HAMILTON ISLAND",
        "airport_code": "HTI",
        "location_name": "HAMILTON ISLAND",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "HAYMAN ISLAND",
        "airport_code": "HIS",
        "location_name": "HAYMAN ISLAND",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "HOBART",
        "airport_code": "HBA",
        "location_name": "Hobart",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "LAUNCESTON",
        "airport_code": "LST",
        "location_name": "Launceston",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "MACKAY",
        "airport_code": "MKY",
        "location_name": "Mackay (Whitsundays)",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "MELBOURNE",
        "airport_code": "MEL",
        "location_name": "Melbourne",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "MELBOURNE (ALL AIRPORTS)",
        "airport_code": "VIZ",
        "location_name": "Melbourne (all airports)",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "NEWCASTLE - PORT STEPHENS",
        "airport_code": "NTL",
        "location_name": "NEWCASTLE - PORT STEPHENS",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "PERTH",
        "airport_code": "PER",
        "location_name": "Perth",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "SUNSHINE COAST",
        "airport_code": "MCY",
        "location_name": "Sunshine Coast",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "SYDNEY (KINGSFORD-SMITH)",
        "airport_code": "SYD",
        "location_name": "Sydney",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "TOWNSVILLE",
        "airport_code": "TSV",
        "location_name": "TOWNSVILLE",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "ULURU",
        "airport_code": "AYQ",
        "location_name": "Uluru",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "WHITSUNDAY COAST - PROSERPINE",
        "airport_code": "PPP",
        "location_name": "WHITSUNDAY COAST - PROSERPINE",
        "country_id": "au",
        "country_name": "Australia "
      },
      {
        "airport_name": "SHAH AMANAT",
        "airport_code": "CGP",
        "location_name": "Chittagong",
        "country_id": "bd",
        "country_name": "Bangladesh "
      },
      {
        "airport_name": "INDIRA GANDHI",
        "airport_code": "DEL",
        "location_name": "Delhi",
        "country_id": "bd",
        "country_name": "Bangladesh "
      },
      {
        "airport_name": "Dhaka",
        "airport_code": "DAC",
        "location_name": "Dhaka",
        "country_id": "bd",
        "country_name": "Bangladesh "
      },
      {
        "airport_name": "BRUNEI",
        "airport_code": "BWN",
        "location_name": "Brunei",
        "country_id": "bn",
        "country_name": "Brunei Darussalam "
      },
      {
        "airport_name": "PHNOM PENH",
        "airport_code": "PNH",
        "location_name": "Phnom Penh",
        "country_id": "kh",
        "country_name": "Cambodia "
      },
      {
        "airport_name": "SIEM REAP",
        "airport_code": "REP",
        "location_name": "Siem Reap",
        "country_id": "kh",
        "country_name": "Cambodia "
      },
      {
        "airport_name": "Beijing Capital",
        "airport_code": "PEK",
        "location_name": "Beijing",
        "country_id": "cn",
        "country_name": "China "
      },
      {
        "airport_name": "Chengdu Shuangliu",
        "airport_code": "CTU",
        "location_name": "Chengdu",
        "country_id": "cn",
        "country_name": "China "
      },
      {
        "airport_name": "Chongqing Jiangbei",
        "airport_code": "CKG",
        "location_name": "Chongqing",
        "country_id": "cn",
        "country_name": "China "
      },
      {
        "airport_name": "Guangzhou Baiyun",
        "airport_code": "CAN",
        "location_name": "Guangzhou",
        "country_id": "cn",
        "country_name": "China "
      },
      {
        "airport_name": "Guilin Liangjiang",
        "airport_code": "KWL",
        "location_name": "Guilin",
        "country_id": "cn",
        "country_name": "China "
      },
      {
        "airport_name": "HAIKOU",
        "airport_code": "HAK",
        "location_name": "Haikou",
        "country_id": "cn",
        "country_name": "China "
      },
      {
        "airport_name": "HANGZHOU XIAOSHAN",
        "airport_code": "HGH",
        "location_name": "Hangzhou",
        "country_id": "cn",
        "country_name": "China "
      },
      {
        "airport_name": "Kunming Wujiaba",
        "airport_code": "KMG",
        "location_name": "Kunming",
        "country_id": "cn",
        "country_name": "China "
      },
      {
        "airport_name": "Nanning Wuxu",
        "airport_code": "NNG",
        "location_name": "Nanning",
        "country_id": "cn",
        "country_name": "China "
      },
      {
        "airport_name": "Ningbo Lishe",
        "airport_code": "NGB",
        "location_name": "Ningbo",
        "country_id": "cn",
        "country_name": "China "
      },
      {
        "airport_name": "Qingdao",
        "airport_code": "TAO",
        "location_name": "Qingdao",
        "country_id": "cn",
        "country_name": "China "
      },
      {
        "airport_name": "Shanghai Pudong",
        "airport_code": "PVG",
        "location_name": "Shanghai",
        "country_id": "cn",
        "country_name": "China "
      },
      {
        "airport_name": "SHANTOU / JIEYANG",
        "airport_code": "SWA",
        "location_name": "SHANTOU / JIEYANG",
        "country_id": "cn",
        "country_name": "China "
      },
      {
        "airport_name": "Shenyang",
        "airport_code": "SHE",
        "location_name": "Shenyang",
        "country_id": "cn",
        "country_name": "China "
      },
      {
        "airport_name": "Shenzhen",
        "airport_code": "SZX",
        "location_name": "Shenzhen",
        "country_id": "cn",
        "country_name": "China "
      },
      {
        "airport_name": "Tianjin",
        "airport_code": "TSN",
        "location_name": "Tianjin",
        "country_id": "cn",
        "country_name": "China "
      },
      {
        "airport_name": "Wuhan Tianhe",
        "airport_code": "WUH",
        "location_name": "Wuhan",
        "country_id": "cn",
        "country_name": "China "
      },
      {
        "airport_name": "Xi An Xianyang",
        "airport_code": "XIY",
        "location_name": "Xi'an",
        "country_id": "cn",
        "country_name": "China "
      },
      {
        "airport_name": "Naike",
        "airport_code": "CMB",
        "location_name": "Colombo",
        "country_id": "co",
        "country_name": "Colombia "
      },
      {
        "airport_name": "NADI",
        "airport_code": "NAN",
        "location_name": "NADI",
        "country_id": "fj",
        "country_name": "Fiji "
      },
      {
        "airport_name": "HONG KONG",
        "airport_code": "HKG",
        "location_name": "Hong Kong",
        "country_id": "hk",
        "country_name": "Hong Kong "
      },
      {
        "airport_name": "SARDAR VALLABHBHAI PATEL",
        "airport_code": "AMD",
        "location_name": "Ahmedabad",
        "country_id": "in",
        "country_name": "India "
      },
      {
        "airport_name": "Bangalore",
        "airport_code": "BLR",
        "location_name": "Bangalore",
        "country_id": "in",
        "country_name": "India "
      },
      {
        "airport_name": "Chennai",
        "airport_code": "MAA",
        "location_name": "Chennai",
        "country_id": "in",
        "country_name": "India "
      },
      {
        "airport_name": "Hyderabad",
        "airport_code": "HYD",
        "location_name": "Hyderabad",
        "country_id": "in",
        "country_name": "India "
      },
      {
        "airport_name": "Kochi",
        "airport_code": "COK",
        "location_name": "Kochi",
        "country_id": "in",
        "country_name": "India "
      },
      {
        "airport_name": "Netaji Subhas Chandra Bosen",
        "airport_code": "CCU",
        "location_name": "Kolkata",
        "country_id": "in",
        "country_name": "India "
      },
      {
        "airport_name": "CHHATRAPATI SHIVAJI",
        "airport_code": "BOM",
        "location_name": "Mumbai",
        "country_id": "in",
        "country_name": "India "
      },
      {
        "airport_name": "Thiruvananthapuram",
        "airport_code": "TRV",
        "location_name": "Thiruvananthapuram",
        "country_id": "in",
        "country_name": "India "
      },
      {
        "airport_name": "Tiruchirapalli (Trichy)",
        "airport_code": "TRZ",
        "location_name": "Tiruchirapalli (Trichy)",
        "country_id": "in",
        "country_name": "India "
      },
      {
        "airport_name": "FUKUOKA",
        "airport_code": "FUK",
        "location_name": "Fukuoka",
        "country_id": "jp",
        "country_name": "Japan "
      },
      {
        "airport_name": "KAGOSHIMA",
        "airport_code": "KOJ",
        "location_name": "Kagoshima",
        "country_id": "jp",
        "country_name": "Japan "
      },
      {
        "airport_name": "KUMAMOTO",
        "airport_code": "KMJ",
        "location_name": "Kumamoto",
        "country_id": "jp",
        "country_name": "Japan "
      },
      {
        "airport_name": "MATSUYAMA",
        "airport_code": "MYJ",
        "location_name": "Matsuyama",
        "country_id": "jp",
        "country_name": "Japan "
      },
      {
        "airport_name": "NAGOYA CHUBU CENTRAIR",
        "airport_code": "NGO",
        "location_name": "Nagoya",
        "country_id": "jp",
        "country_name": "Japan "
      },
      {
        "airport_name": "OITA",
        "airport_code": "OIT",
        "location_name": "Oita",
        "country_id": "jp",
        "country_name": "Japan "
      },
      {
        "airport_name": "OKINAWA, NAHA",
        "airport_code": "OKA",
        "location_name": "Okinawa - Naha",
        "country_id": "jp",
        "country_name": "Japan "
      },
      {
        "airport_name": "OSAKA, KANSAI",
        "airport_code": "KIX",
        "location_name": "Osaka - Kansai",
        "country_id": "jp",
        "country_name": "Japan "
      },
      {
        "airport_name": "SAPPORO, SHIN-CHITOSE",
        "airport_code": "CTS",
        "location_name": "Sapporo - Shin-Chitose",
        "country_id": "jp",
        "country_name": "Japan "
      },
      {
        "airport_name": "TAKAMATSU ",
        "airport_code": "TAK",
        "location_name": "Takamatsu ",
        "country_id": "jp",
        "country_name": "Japan "
      },
      {
        "airport_name": "Tokyo, Haneda",
        "airport_code": "HND",
        "location_name": "Tokyo - Haneda",
        "country_id": "jp",
        "country_name": "Japan "
      },
      {
        "airport_name": "TOKYO, NARITA",
        "airport_code": "NRT",
        "location_name": "Tokyo - Narita",
        "country_id": "jp",
        "country_name": "Japan "
      },
      {
        "airport_name": "Wattay",
        "airport_code": "VTE",
        "location_name": "Vientiane",
        "country_id": "la",
        "country_name": "Laos"
      },
      {
        "airport_name": "MACAU",
        "airport_code": "MFM",
        "location_name": "Macau",
        "country_id": "mo",
        "country_name": "Macau "
      },
      {
        "airport_name": "Sultan Abdul Halim",
        "airport_code": "AOR",
        "location_name": "Alor Setar",
        "country_id": "my",
        "country_name": "Malaysia "
      },
      {
        "airport_name": "Bintulu",
        "airport_code": "BTU",
        "location_name": "Bintulu",
        "country_id": "my",
        "country_name": "Malaysia "
      },
      {
        "airport_name": "Senai",
        "airport_code": "JHB",
        "location_name": "Johor Baru",
        "country_id": "my",
        "country_name": "Malaysia "
      },
      {
        "airport_name": "Sultan Ismail Petra",
        "airport_code": "KBR",
        "location_name": "Kota Bharu",
        "country_id": "my",
        "country_name": "Malaysia "
      },
      {
        "airport_name": "Kota Kinabalu",
        "airport_code": "BKI",
        "location_name": "Kota Kinabalu",
        "country_id": "my",
        "country_name": "Malaysia "
      },
      {
        "airport_name": "KUALA LUMPUR",
        "airport_code": "KUL",
        "location_name": "Kuala Lumpur",
        "country_id": "my",
        "country_name": "Malaysia "
      },
      {
        "airport_name": "SULTAN MAHMUD",
        "airport_code": "TGG",
        "location_name": "Kuala Terengganu",
        "country_id": "my",
        "country_name": "Malaysia "
      },
      {
        "airport_name": "Kuching",
        "airport_code": "KCH",
        "location_name": "Kuching",
        "country_id": "my",
        "country_name": "Malaysia "
      },
      {
        "airport_name": "Langkawi",
        "airport_code": "LGK",
        "location_name": "Langkawi",
        "country_id": "my",
        "country_name": "Malaysia "
      },
      {
        "airport_name": "Malacca",
        "airport_code": "MKZ",
        "location_name": "Malacca",
        "country_id": "my",
        "country_name": "Malaysia "
      },
      {
        "airport_name": "Miri",
        "airport_code": "MYY",
        "location_name": "Miri",
        "country_id": "my",
        "country_name": "Malaysia "
      },
      {
        "airport_name": "PENANG",
        "airport_code": "PEN",
        "location_name": "Penang",
        "country_id": "my",
        "country_name": "Malaysia "
      },
      {
        "airport_name": "Sandakan",
        "airport_code": "SDK",
        "location_name": "Sandaka",
        "country_id": "my",
        "country_name": "Malaysia "
      },
      {
        "airport_name": "Sibu",
        "airport_code": "SBW",
        "location_name": "Sibu",
        "country_id": "my",
        "country_name": "Malaysia "
      },
      {
        "airport_name": "Sultan Abdul Aziz Shah",
        "airport_code": "SZB",
        "location_name": "Subang",
        "country_id": "my",
        "country_name": "Malaysia "
      },
      {
        "airport_name": "IPOH",
        "airport_code": "IPH",
        "location_name": "SULTAN AZLAN SHAH",
        "country_id": "my",
        "country_name": "Malaysia "
      },
      {
        "airport_name": "Tawau",
        "airport_code": "TWU",
        "location_name": "Tawau",
        "country_id": "my",
        "country_name": "Malaysia "
      },
      {
        "airport_name": "Mandalay",
        "airport_code": "MDL",
        "location_name": "Mandalay",
        "country_id": "mm",
        "country_name": "Myanmar "
      },
      {
        "airport_name": "YANGOON",
        "airport_code": "RGN",
        "location_name": "Yangoon",
        "country_id": "mm",
        "country_name": "Myanmar "
      },
      {
        "airport_name": "Tribhuvan",
        "airport_code": "KTM",
        "location_name": "Kathmandu",
        "country_id": "np",
        "country_name": "Nepal "
      },
      {
        "airport_name": "SCHIPHOL",
        "airport_code": "AMS",
        "location_name": "SCHIPHOL",
        "country_id": "nl",
        "country_name": "Netherlands "
      },
      {
        "airport_name": "AUCKLAND",
        "airport_code": "AKL",
        "location_name": "AUCKLAND",
        "country_id": "nz",
        "country_name": "New Zealand "
      },
      {
        "airport_name": "CHRISTCHURCH",
        "airport_code": "CHC",
        "location_name": "CHRISTCHURCH",
        "country_id": "nz",
        "country_name": "New Zealand "
      },
      {
        "airport_name": "DUNEDIN",
        "airport_code": "DUD",
        "location_name": "DUNEDIN",
        "country_id": "nz",
        "country_name": "New Zealand "
      },
      {
        "airport_name": "QUEENSTOWN",
        "airport_code": "ZQN",
        "location_name": "QUEENSTOWN",
        "country_id": "nz",
        "country_name": "New Zealand "
      },
      {
        "airport_name": "WELLINGTON",
        "airport_code": "WLG",
        "location_name": "WELLINGTON",
        "country_id": "nz",
        "country_name": "New Zealand "
      },
      {
        "airport_name": "Bacolod",
        "airport_code": "BCD",
        "location_name": "Bacolod",
        "country_id": "ph",
        "country_name": "Philippines "
      },
      {
        "airport_name": "Mactan-Cebu",
        "airport_code": "CEB",
        "location_name": "Cebu",
        "country_id": "ph",
        "country_name": "Philippines "
      },
      {
        "airport_name": "CLARK",
        "airport_code": "CRK",
        "location_name": "Clark",
        "country_id": "ph",
        "country_name": "Philippines "
      },
      {
        "airport_name": "Davao",
        "airport_code": "DVO",
        "location_name": "Davao",
        "country_id": "ph",
        "country_name": "Philippines "
      },
      {
        "airport_name": "Iloilo",
        "airport_code": "ILO",
        "location_name": "Iloilo",
        "country_id": "ph",
        "country_name": "Philippines "
      },
      {
        "airport_name": "NINOY AQUINO",
        "airport_code": "MNL",
        "location_name": "Manila (NAIA)",
        "country_id": "ph",
        "country_name": "Philippines "
      },
      {
        "airport_name": "Puerto Princesa",
        "airport_code": "PPS",
        "location_name": "Puerto Princesa",
        "country_id": "ph",
        "country_name": "Philippines "
      },
      {
        "airport_name": "Tacloban",
        "airport_code": "TAC",
        "location_name": "Tacloban",
        "country_id": "ph",
        "country_name": "Philippines "
      },
      {
        "airport_name": "King Abdulaziz",
        "airport_code": "JED",
        "location_name": "Jeddah",
        "country_id": "sa",
        "country_name": "Saudi Arabia "
      },
      {
        "airport_name": "Changi",
        "airport_code": "SIN",
        "location_name": "Singapore",
        "country_id": "sg",
        "country_name": "Singapore "
      },
      {
        "airport_name": "Gimhae",
        "airport_code": "PUS",
        "location_name": "Busan",
        "country_id": "kr",
        "country_name": "South Korea"
      },
      {
        "airport_name": "Incheon",
        "airport_code": "ICN",
        "location_name": "Seoul",
        "country_id": "kr",
        "country_name": "South Korea"
      },
      {
        "airport_name": "TAIWAN TAOYUAN",
        "airport_code": "TPE",
        "location_name": "Taipei",
        "country_id": "tw",
        "country_name": "Taiwan"
      },
      {
        "airport_name": "SUVARNABHUMI",
        "airport_code": "BKK",
        "location_name": "Bangkok",
        "country_id": "th",
        "country_name": "Thailand "
      },
      {
        "airport_name": "DON MUEANG",
        "airport_code": "DMK",
        "location_name": "Bangkok - Don Mueang",
        "country_id": "th",
        "country_name": "Thailand "
      },
      {
        "airport_name": "CHIANG MAI",
        "airport_code": "CNX",
        "location_name": "Chiang Mai",
        "country_id": "th",
        "country_name": "Thailand "
      },
      {
        "airport_name": "Mae Fah Luang-Chiang Rai",
        "airport_code": "CEI",
        "location_name": "Chiang Rai",
        "country_id": "th",
        "country_name": "Thailand "
      },
      {
        "airport_name": "Hat Yai",
        "airport_code": "HDY",
        "location_name": "Hat Yai",
        "country_id": "th",
        "country_name": "Thailand "
      },
      {
        "airport_name": "Krabi",
        "airport_code": "KBV",
        "location_name": "Krabi",
        "country_id": "th",
        "country_name": "Thailand "
      },
      {
        "airport_name": "Nakhon Phanom",
        "airport_code": "KOP",
        "location_name": "Nakhon Phanom",
        "country_id": "th",
        "country_name": "Thailand "
      },
      {
        "airport_name": "Nakhon Si Thammarat",
        "airport_code": "NST",
        "location_name": "Nakhon Si Thammarat",
        "country_id": "th",
        "country_name": "Thailand "
      },
      {
        "airport_name": "Narathiwat",
        "airport_code": "NAW",
        "location_name": "Narathiwat",
        "country_id": "th",
        "country_name": "Thailand "
      },
      {
        "airport_name": "PHUKET",
        "airport_code": "HKT",
        "location_name": "Phuket",
        "country_id": "th",
        "country_name": "Thailand "
      },
      {
        "airport_name": "Surat Thani",
        "airport_code": "URT",
        "location_name": "Surat Thani",
        "country_id": "th",
        "country_name": "Thailand "
      },
      {
        "airport_name": "Trang",
        "airport_code": "TST",
        "location_name": "Trang",
        "country_id": "th",
        "country_name": "Thailand "
      },
      {
        "airport_name": "Ubon Ratchathani",
        "airport_code": "UBP",
        "location_name": "Ubon Ratchathani",
        "country_id": "th",
        "country_name": "Thailand "
      },
      {
        "airport_name": "Udonthani",
        "airport_code": "UTH",
        "location_name": "Udon Thani",
        "country_id": "th",
        "country_name": "Thailand "
      },
      {
        "airport_name": "Presidente Nicolau Lobato",
        "airport_code": "DIL",
        "location_name": "Dili",
        "country_id": "tl",
        "country_name": "Timor-Leste "
      },
      {
        "airport_name": "ABU DHABI",
        "airport_code": "ABU",
        "location_name": "Abu Dhabi",
        "country_id": "ae",
        "country_name": "United Arab Emirates "
      },
      {
        "airport_name": "ABU DHABI",
        "airport_code": "AUH",
        "location_name": "Abu Dhabi",
        "country_id": "ae",
        "country_name": "United Arab Emirates "
      },
      {
        "airport_name": "DUBAI INTERNATIONAL AIRPORT",
        "airport_code": "DXB",
        "location_name": "Dubai",
        "country_id": "ae",
        "country_name": "United Arab Emirates "
      },
      {
        "airport_name": "DYCE AIRPORT",
        "airport_code": "ABZ",
        "location_name": "edinbrugh",
        "country_id": "gb",
        "country_name": "United Kingdom "
      },
      {
        "airport_name": "LONDON",
        "airport_code": "LGW",
        "location_name": "London",
        "country_id": "gb",
        "country_name": "United Kingdom "
      },
      {
        "airport_name": "LONDON HEATHROW",
        "airport_code": "LHR",
        "location_name": "palmers green",
        "country_id": "gb",
        "country_name": "United Kingdom "
      },
      {
        "airport_name": "HONOLULU",
        "airport_code": "HNL",
        "location_name": "HONOLULU",
        "country_id": "us",
        "country_name": "United States "
      },
      {
        "airport_name": "LOS ANGELES INTERNATIONAL AIRPORT",
        "airport_code": "LAX",
        "location_name": "Los Angeles",
        "country_id": "us",
        "country_name": "United States "
      },
      {
        "airport_name": "SAN DIEGO INTERNATIONAL AIRPORT",
        "airport_code": "SAN",
        "location_name": "San Diego International Airport",
        "country_id": "us",
        "country_name": "United States "
      },
      {
        "airport_name": "BUON MA THUOT",
        "airport_code": "BMV",
        "location_name": "Buon Ma Thuot",
        "country_id": "vn",
        "country_name": "Vietnam "
      },
      {
        "airport_name": "DA NANG",
        "airport_code": "DAD",
        "location_name": "Da Nang",
        "country_id": "vn",
        "country_name": "Vietnam "
      },
      {
        "airport_name": "DONG HOI",
        "airport_code": "VDH",
        "location_name": "Dong Hoi",
        "country_id": "vn",
        "country_name": "Vietnam "
      },
      {
        "airport_name": "HAI PHONG",
        "airport_code": "HPH",
        "location_name": "Hai Phong",
        "country_id": "vn",
        "country_name": "Vietnam "
      },
      {
        "airport_name": "TAN SON NHAT",
        "airport_code": "SGN",
        "location_name": "Ho Chi Minh City",
        "country_id": "vn",
        "country_name": "Vietnam "
      },
      {
        "airport_name": "HUI",
        "airport_code": "HUI",
        "location_name": "HUI",
        "country_id": "vn",
        "country_name": "Vietnam "
      },
      {
        "airport_name": "NHA TRANG",
        "airport_code": "CXR",
        "location_name": "Nha Trang",
        "country_id": "vn",
        "country_name": "Vietnam "
      },
      {
        "airport_name": "NOI BAI",
        "airport_code": "HAN",
        "location_name": "Noi Bai",
        "country_id": "vn",
        "country_name": "Vietnam "
      },
      {
        "airport_name": "PHU QUOC",
        "airport_code": "PQC",
        "location_name": "Phu Quoc",
        "country_id": "vn",
        "country_name": "Vietnam "
      },
      {
        "airport_name": "QUY NHON",
        "airport_code": "UIH",
        "location_name": "Quy Nhon ",
        "country_id": "vn",
        "country_name": "Vietnam "
      },
      {
        "airport_name": "THANH HOA",
        "airport_code": "THD",
        "location_name": "Thanh Hoa",
        "country_id": "vn",
        "country_name": "Vietnam "
      },
      {
        "airport_name": "TUY HOA",
        "airport_code": "TBB",
        "location_name": "Tuy Hoa",
        "country_id": "vn",
        "country_name": "Vietnam "
      },
      {
        "airport_name": "VINH",
        "airport_code": "VII",
        "location_name": "Vinh",
        "country_id": "vn",
        "country_name": "Vietnam "
      }
    ]
  },
  "login_status": "false",
  "token": "f9b29ac359ca5d77755e7588751c089bf96f0dc9"
}
```



```matlab
a:5:{s:10:"diagnostic";a:7:{s:6:"status";i:200;s:10:"elapsetime";s:14:"0.0999";s:11:"memoryusage";s:14:"6.41MB";s:14:"unix_timestamp";i:1470280404;s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:11:"output_type";s:9:"serialize";s:11:"all_airport";a:1:{s:7:"airport";a:249:{i:0;a:5:{s:12:"airport_name";s:4:"Mali";s:12:"airport_code";s:3:"ARD";s:13:"location_name";s:11:"Alor Island";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:1;a:5:{s:12:"airport_name";s:9:"Pattimura";s:12:"airport_code";s:3:"AMQ";s:13:"location_name";s:5:"Ambon";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:2;a:5:{s:12:"airport_name";s:7:"ATAMBUA";s:12:"airport_code";s:3:"ABU";s:13:"location_name";s:7:"Atambua";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:3;a:5:{s:12:"airport_name";s:3:"Soa";s:12:"airport_code";s:3:"BJW";s:13:"location_name";s:6:"Bajawa";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:4;a:5:{s:12:"airport_name";s:9:"Sepinggan";s:12:"airport_code";s:3:"BPN";s:13:"location_name";s:10:"BalikPapan";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:5;a:5:{s:12:"airport_name";s:20:"Sultan Iskandar Muda";s:12:"airport_code";s:3:"BTJ";s:13:"location_name";s:10:"Banda Aceh";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:6;a:5:{s:12:"airport_name";s:19:"Husein Sastranegara";s:12:"airport_code";s:3:"BDO";s:13:"location_name";s:7:"Bandung";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:7;a:5:{s:12:"airport_name";s:15:"SYAMSUDDIN NOOR";s:12:"airport_code";s:3:"BDJ";s:13:"location_name";s:11:"Banjarmasin";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:8;a:5:{s:12:"airport_name";s:12:"BLIMBINGSARI";s:12:"airport_code";s:3:"DQJ";s:13:"location_name";s:25:"Banyuwangi - BLIMBINGSARI";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:9;a:5:{s:12:"airport_name";s:10:"Hang Nadim";s:12:"airport_code";s:3:"BTH";s:13:"location_name";s:5:"Batam";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:10;a:5:{s:12:"airport_name";s:6:"Baubau";s:12:"airport_code";s:3:"BUW";s:13:"location_name";s:6:"Baubau";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:11;a:5:{s:12:"airport_name";s:18:"Fatmawati Soekarno";s:12:"airport_code";s:3:"BKS";s:13:"location_name";s:8:"Bengkulu";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:12;a:5:{s:12:"airport_name";s:9:"Kalimarau";s:12:"airport_code";s:3:"BEJ";s:13:"location_name";s:5:"Berau";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:13;a:5:{s:12:"airport_name";s:21:"BANDAR UDARA BERINGIN";s:12:"airport_code";s:3:"MTW";s:13:"location_name";s:16:"Beringin Airport";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:14;a:5:{s:12:"airport_name";s:14:"Frans Kaisiepo";s:12:"airport_code";s:3:"BIK";s:13:"location_name";s:4:"Biak";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:15;a:5:{s:12:"airport_name";s:19:"Muhammad Salahuddin";s:12:"airport_code";s:3:"BMU";s:13:"location_name";s:4:"Bima";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:16;a:5:{s:12:"airport_name";s:12:"BLIMBINGSARI";s:12:"airport_code";s:3:"BWX";s:13:"location_name";s:12:"BLIMBINGSARI";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:17;a:5:{s:12:"airport_name";s:4:"Buli";s:12:"airport_code";s:3:"WUB";s:13:"location_name";s:4:"Buli";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:18;a:5:{s:12:"airport_name";s:7:"Pogugol";s:12:"airport_code";s:3:"UOL";s:13:"location_name";s:4:"Buol";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:19;a:5:{s:12:"airport_name";s:10:"NGURAH RAI";s:12:"airport_code";s:3:"DPS";s:13:"location_name";s:14:"Denpasar, Bali";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:20;a:5:{s:12:"airport_name";s:20:"H. Hasan Aroeboesman";s:12:"airport_code";s:3:"ENE";s:13:"location_name";s:4:"Ende";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:21;a:5:{s:12:"airport_name";s:6:"Fakfak";s:12:"airport_code";s:3:"FKQ";s:13:"location_name";s:6:"FakFak";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:22;a:5:{s:12:"airport_name";s:6:"GALELA";s:12:"airport_code";s:3:"GLX";s:13:"location_name";s:6:"Galela";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:23;a:5:{s:12:"airport_name";s:10:"Jalaluddin";s:12:"airport_code";s:3:"GTO";s:13:"location_name";s:9:"Gorontalo";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:24;a:5:{s:12:"airport_name";s:21:"Gunung Sitoli, Binaka";s:12:"airport_code";s:3:"GNS";s:13:"location_name";s:12:"GunungSitoli";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:25;a:5:{s:12:"airport_name";s:14:"Soekarno Hatta";s:12:"airport_code";s:3:"CGK";s:13:"location_name";s:20:"Jakarta - Cengkareng";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:26;a:5:{s:12:"airport_name";s:19:"HALIM PERDANAKUSUMA";s:12:"airport_code";s:3:"HLP";s:13:"location_name";s:15:"Jakarta - Halim";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:27;a:5:{s:12:"airport_name";s:23:"Sultan Thaha Syaifuddin";s:12:"airport_code";s:3:"DJB";s:13:"location_name";s:5:"Jambi";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:28;a:5:{s:12:"airport_name";s:7:"Sentani";s:12:"airport_code";s:3:"DJJ";s:13:"location_name";s:8:"Jayapura";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:29;a:5:{s:12:"airport_name";s:15:"Kaimana, Utarom";s:12:"airport_code";s:3:"KNG";s:13:"location_name";s:7:"Kaimana";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:30;a:5:{s:12:"airport_name";s:8:"Haluoleo";s:12:"airport_code";s:3:"KDI";s:13:"location_name";s:7:"Kendari";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:31;a:5:{s:12:"airport_name";s:13:"RAHADI OESMAN";s:12:"airport_code";s:3:"KTG";s:13:"location_name";s:8:"Ketapang";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:32;a:5:{s:12:"airport_name";s:8:"Kotabaru";s:12:"airport_code";s:3:"KBU";s:13:"location_name";s:8:"Kotabaru";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:33;a:5:{s:12:"airport_name";s:7:"El Tari";s:12:"airport_code";s:3:"KOE";s:13:"location_name";s:6:"Kupang";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:34;a:5:{s:12:"airport_name";s:18:"Labuanbajo, Komodo";s:12:"airport_code";s:3:"LBJ";s:13:"location_name";s:10:"LabuanBajo";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:35;a:5:{s:12:"airport_name";s:20:"Labuha, Oesman Sadik";s:12:"airport_code";s:3:"LAH";s:13:"location_name";s:6:"Labuha";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:36;a:5:{s:12:"airport_name";s:14:"Radin Inten II";s:12:"airport_code";s:3:"TKG";s:13:"location_name";s:7:"Lampung";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:37;a:5:{s:12:"airport_name";s:25:"Lhokseumawe, Malikussaleh";s:12:"airport_code";s:3:"LSW";s:13:"location_name";s:11:"Lhokseumawe";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:38;a:5:{s:12:"airport_name";s:6:"Lombok";s:12:"airport_code";s:3:"LOP";s:13:"location_name";s:15:"Lombok, Mataram";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:39;a:5:{s:12:"airport_name";s:23:"Syukuran Aminuddin Amir";s:12:"airport_code";s:3:"LUW";s:13:"location_name";s:5:"Luwuk";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:40;a:5:{s:12:"airport_name";s:19:"Abdul Rachman Saleh";s:12:"airport_code";s:3:"MLG";s:13:"location_name";s:6:"Malang";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:41;a:5:{s:12:"airport_name";s:19:"ROBERT ATTY BESSING";s:12:"airport_code";s:3:"MLN";s:13:"location_name";s:7:"Malinau";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:42;a:5:{s:12:"airport_name";s:6:"Mamuju";s:12:"airport_code";s:3:"MJU";s:13:"location_name";s:6:"Mamuju";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:43;a:5:{s:12:"airport_name";s:13:"Sam Ratulangi";s:12:"airport_code";s:3:"MDC";s:13:"location_name";s:6:"Manado";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:44;a:5:{s:12:"airport_name";s:7:"Rendani";s:12:"airport_code";s:3:"MKW";s:13:"location_name";s:9:"Manokwari";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:45;a:5:{s:12:"airport_name";s:7:"Wai Oti";s:12:"airport_code";s:3:"MOF";s:13:"location_name";s:7:"Maumere";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:46;a:5:{s:12:"airport_name";s:10:"Kuala Namu";s:12:"airport_code";s:3:"KNO";s:13:"location_name";s:18:"Medan (Kuala Namu)";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:47;a:5:{s:12:"airport_name";s:7:"MELALAN";s:12:"airport_code";s:3:"MLK";s:13:"location_name";s:5:"Melak";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:48;a:5:{s:12:"airport_name";s:10:"Melonguane";s:12:"airport_code";s:3:"MNA";s:13:"location_name";s:10:"Melanguane";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:49;a:5:{s:12:"airport_name";s:5:"Mopah";s:12:"airport_code";s:3:"MKQ";s:13:"location_name";s:7:"Merauke";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:50;a:5:{s:12:"airport_name";s:23:"Meulaboh, Cut Nyak Dien";s:12:"airport_code";s:3:"MEQ";s:13:"location_name";s:8:"Meulaboh";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:51;a:5:{s:12:"airport_name";s:7:"MOROTAI";s:12:"airport_code";s:3:"OTI";s:13:"location_name";s:7:"MOROTAI";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:52;a:5:{s:12:"airport_name";s:6:"Nabire";s:12:"airport_code";s:3:"NBX";s:13:"location_name";s:6:"Nabire";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:53;a:5:{s:12:"airport_name";s:12:"Natuna Ranai";s:12:"airport_code";s:3:"NTX";s:13:"location_name";s:11:"NatunaRanai";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:54;a:5:{s:12:"airport_name";s:7:"NUNUKAN";s:12:"airport_code";s:3:"NNX";s:13:"location_name";s:7:"Nunukan";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:55;a:5:{s:12:"airport_name";s:11:"Minangkabau";s:12:"airport_code";s:3:"PDG";s:13:"location_name";s:6:"Padang";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:56;a:5:{s:12:"airport_name";s:12:"Tjilik Riwut";s:12:"airport_code";s:3:"PKY";s:13:"location_name";s:13:"Palangka raya";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:57;a:5:{s:12:"airport_name";s:27:"Sultan Mahmud Badaruddin II";s:12:"airport_code";s:3:"PLM";s:13:"location_name";s:9:"Palembang";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:58;a:5:{s:12:"airport_name";s:7:"Mutiara";s:12:"airport_code";s:3:"PLW";s:13:"location_name";s:4:"Palu";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:59;a:5:{s:12:"airport_name";s:11:"Depati Amir";s:12:"airport_code";s:3:"PGK";s:13:"location_name";s:14:"Pangkal pinang";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:60;a:5:{s:12:"airport_name";s:13:"PANGKALAN BUN";s:12:"airport_code";s:3:"PKN";s:13:"location_name";s:13:"Pangkalan Bun";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:61;a:5:{s:12:"airport_name";s:22:"Sultan Syarif Kasim II";s:12:"airport_code";s:3:"PKU";s:13:"location_name";s:9:"Pekanbaru";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:62;a:5:{s:12:"airport_name";s:24:"Sangia Nibandera Pomalaa";s:12:"airport_code";s:3:"PUM";s:13:"location_name";s:7:"Pomalaa";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:63;a:5:{s:12:"airport_name";s:7:"Supadio";s:12:"airport_code";s:3:"PNK";s:13:"location_name";s:9:"Pontianak";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:64;a:5:{s:12:"airport_name";s:15:"Poso, Kasiguncu";s:12:"airport_code";s:3:"PSJ";s:13:"location_name";s:4:"Poso";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:65;a:5:{s:12:"airport_name";s:10:"PUTUSSIBAU";s:12:"airport_code";s:3:"PSU";s:13:"location_name";s:10:"Putussibau";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:66;a:5:{s:12:"airport_name";s:4:"ROTE";s:12:"airport_code";s:3:"RTI";s:13:"location_name";s:4:"Rote";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:67;a:5:{s:12:"airport_name";s:16:"Frans Sales Lega";s:12:"airport_code";s:3:"RTG";s:13:"location_name";s:6:"Ruteng";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:68;a:5:{s:12:"airport_name";s:9:"TEMINDUNG";s:12:"airport_code";s:3:"SRI";s:13:"location_name";s:9:"Samarinda";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:69;a:5:{s:12:"airport_name";s:14:"H. Asan Sampit";s:12:"airport_code";s:3:"SMQ";s:13:"location_name";s:6:"Sampit";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:70;a:5:{s:12:"airport_name";s:19:"BANDAR UDARA OLILIT";s:12:"airport_code";s:3:"SXK";s:13:"location_name";s:8:"Saumlaki";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:71;a:5:{s:12:"airport_name";s:7:"SELAYAR";s:12:"airport_code";s:3:"YKR";s:13:"location_name";s:7:"Selayar";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:72;a:5:{s:12:"airport_name";s:11:"Achmad Yani";s:12:"airport_code";s:3:"SRG";s:13:"location_name";s:8:"Semarang";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:73;a:5:{s:12:"airport_name";s:7:"SIBOLGA";s:12:"airport_code";s:3:"RRZ";s:13:"location_name";s:7:"Sibolga";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:74;a:5:{s:12:"airport_name";s:8:"Silangit";s:12:"airport_code";s:3:"DTB";s:13:"location_name";s:8:"Silangit";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:75;a:5:{s:12:"airport_name";s:7:"Lasikin";s:12:"airport_code";s:3:"SNX";s:13:"location_name";s:8:"Sinabang";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:76;a:5:{s:12:"airport_name";s:6:"SUSILO";s:12:"airport_code";s:3:"SQG";s:13:"location_name";s:7:"Sintang";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:77;a:5:{s:12:"airport_name";s:10:"Adisumarmo";s:12:"airport_code";s:3:"SOC";s:13:"location_name";s:4:"Solo";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:78;a:5:{s:12:"airport_name";s:21:"Dominique Edward Osok";s:12:"airport_code";s:3:"SOQ";s:13:"location_name";s:6:"Sorong";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:79;a:5:{s:12:"airport_name";s:19:"Sumbawa, Brang Biji";s:12:"airport_code";s:3:"SWQ";s:13:"location_name";s:7:"Sumbawa";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:80;a:5:{s:12:"airport_name";s:6:"Juanda";s:12:"airport_code";s:3:"SUB";s:13:"location_name";s:8:"Surabaya";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:81;a:5:{s:12:"airport_name";s:4:"Naha";s:12:"airport_code";s:3:"NAH";s:13:"location_name";s:6:"Tahuna";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:82;a:5:{s:12:"airport_name";s:9:"Tampolaka";s:12:"airport_code";s:3:"TMC";s:13:"location_name";s:9:"Tambolaka";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:83;a:5:{s:12:"airport_name";s:19:"H.A.S Hanandjoeddin";s:12:"airport_code";s:3:"TJQ";s:13:"location_name";s:14:"Tanjung Pandan";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:84;a:5:{s:12:"airport_name";s:22:"Raja Haji FIsabilillah";s:12:"airport_code";s:3:"TNJ";s:13:"location_name";s:14:"Tanjung Pinang";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:85;a:5:{s:12:"airport_name";s:15:"TANJUNG HARAPAN";s:12:"airport_code";s:3:"TJS";s:13:"location_name";s:13:"Tanjung Selor";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:86;a:5:{s:12:"airport_name";s:7:"WARUKIN";s:12:"airport_code";s:3:"TJG";s:13:"location_name";s:15:"Tanjung Warukin";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:87;a:5:{s:12:"airport_name";s:6:"Juwata";s:12:"airport_code";s:3:"TRK";s:13:"location_name";s:7:"Tarakan";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:88;a:5:{s:12:"airport_name";s:15:"Sultan Babullah";s:12:"airport_code";s:3:"TTE";s:13:"location_name";s:7:"Ternate";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:89;a:5:{s:12:"airport_name";s:14:"Mozes Kilangin";s:12:"airport_code";s:3:"TIM";s:13:"location_name";s:6:"Timika";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:90;a:5:{s:12:"airport_name";s:6:"Tobelo";s:12:"airport_code";s:3:"KAZ";s:13:"location_name";s:6:"Tobelo";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:91;a:5:{s:12:"airport_name";s:9:"TOLI TOLI";s:12:"airport_code";s:3:"TLI";s:13:"location_name";s:9:"TOLI TOLI";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:92;a:5:{s:12:"airport_name";s:15:"Tual, Dumatubin";s:12:"airport_code";s:3:"LUV";s:13:"location_name";s:4:"Tual";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:93;a:5:{s:12:"airport_name";s:17:"SULTAN HASANUDDIN";s:12:"airport_code";s:3:"UPG";s:13:"location_name";s:22:"Ujungpandang, Makassar";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:94;a:5:{s:12:"airport_name";s:8:"WAINGAPU";s:12:"airport_code";s:3:"WGP";s:13:"location_name";s:8:"Waingapu";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:95;a:5:{s:12:"airport_name";s:8:"Matahora";s:12:"airport_code";s:3:"WNI";s:13:"location_name";s:8:"Wakatobi";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:96;a:5:{s:12:"airport_name";s:6:"WAMENA";s:12:"airport_code";s:3:"WMX";s:13:"location_name";s:6:"Wamena";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:97;a:5:{s:12:"airport_name";s:21:"Wangi wangi, Matahora";s:12:"airport_code";s:3:"WGI";s:13:"location_name";s:11:"Wangi wangi";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:98;a:5:{s:12:"airport_name";s:12:"Adi Sutjipto";s:12:"airport_code";s:3:"JOG";s:13:"location_name";s:10:"Yogyakarta";s:10:"country_id";s:2:"id";s:12:"country_name";s:9:"Indonesia";}i:99;a:5:{s:12:"airport_name";s:8:"ADELAIDE";s:12:"airport_code";s:3:"ADL";s:13:"location_name";s:8:"Adelaide";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:100;a:5:{s:12:"airport_name";s:13:"Alice Springs";s:12:"airport_code";s:3:"ASP";s:13:"location_name";s:13:"Alice Springs";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:101;a:5:{s:12:"airport_name";s:6:"AVALON";s:12:"airport_code";s:3:"AVV";s:13:"location_name";s:6:"AVALON";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:102;a:5:{s:12:"airport_name";s:13:"BALLINA BYRON";s:12:"airport_code";s:3:"BNK";s:13:"location_name";s:13:"BALLINA BYRON";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:103;a:5:{s:12:"airport_name";s:8:"BRISBANE";s:12:"airport_code";s:3:"BNE";s:13:"location_name";s:8:"Brisbane";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:104;a:5:{s:12:"airport_name";s:6:"CAIRNS";s:12:"airport_code";s:3:"CNS";s:13:"location_name";s:6:"Cairns";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:105;a:5:{s:12:"airport_name";s:8:"CANBERRA";s:12:"airport_code";s:3:"CBR";s:13:"location_name";s:8:"CANBERRA";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:106;a:5:{s:12:"airport_name";s:13:"Coffs Harbour";s:12:"airport_code";s:3:"CFS";s:13:"location_name";s:13:"Coffs Harbour";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:107;a:5:{s:12:"airport_name";s:6:"DARWIN";s:12:"airport_code";s:3:"DRW";s:13:"location_name";s:6:"Darwin";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:108;a:5:{s:12:"airport_name";s:10:"GOLD COAST";s:12:"airport_code";s:3:"OOL";s:13:"location_name";s:10:"Gold Coast";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:109;a:5:{s:12:"airport_name";s:15:"HAMILTON ISLAND";s:12:"airport_code";s:3:"HTI";s:13:"location_name";s:15:"HAMILTON ISLAND";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:110;a:5:{s:12:"airport_name";s:13:"HAYMAN ISLAND";s:12:"airport_code";s:3:"HIS";s:13:"location_name";s:13:"HAYMAN ISLAND";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:111;a:5:{s:12:"airport_name";s:6:"HOBART";s:12:"airport_code";s:3:"HBA";s:13:"location_name";s:6:"Hobart";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:112;a:5:{s:12:"airport_name";s:10:"LAUNCESTON";s:12:"airport_code";s:3:"LST";s:13:"location_name";s:10:"Launceston";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:113;a:5:{s:12:"airport_name";s:6:"MACKAY";s:12:"airport_code";s:3:"MKY";s:13:"location_name";s:20:"Mackay (Whitsundays)";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:114;a:5:{s:12:"airport_name";s:9:"MELBOURNE";s:12:"airport_code";s:3:"MEL";s:13:"location_name";s:9:"Melbourne";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:115;a:5:{s:12:"airport_name";s:24:"MELBOURNE (ALL AIRPORTS)";s:12:"airport_code";s:3:"VIZ";s:13:"location_name";s:24:"Melbourne (all airports)";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:116;a:5:{s:12:"airport_name";s:25:"NEWCASTLE - PORT STEPHENS";s:12:"airport_code";s:3:"NTL";s:13:"location_name";s:25:"NEWCASTLE - PORT STEPHENS";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:117;a:5:{s:12:"airport_name";s:5:"PERTH";s:12:"airport_code";s:3:"PER";s:13:"location_name";s:5:"Perth";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:118;a:5:{s:12:"airport_name";s:14:"SUNSHINE COAST";s:12:"airport_code";s:3:"MCY";s:13:"location_name";s:14:"Sunshine Coast";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:119;a:5:{s:12:"airport_name";s:24:"SYDNEY (KINGSFORD-SMITH)";s:12:"airport_code";s:3:"SYD";s:13:"location_name";s:6:"Sydney";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:120;a:5:{s:12:"airport_name";s:10:"TOWNSVILLE";s:12:"airport_code";s:3:"TSV";s:13:"location_name";s:10:"TOWNSVILLE";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:121;a:5:{s:12:"airport_name";s:5:"ULURU";s:12:"airport_code";s:3:"AYQ";s:13:"location_name";s:5:"Uluru";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:122;a:5:{s:12:"airport_name";s:29:"WHITSUNDAY COAST - PROSERPINE";s:12:"airport_code";s:3:"PPP";s:13:"location_name";s:29:"WHITSUNDAY COAST - PROSERPINE";s:10:"country_id";s:2:"au";s:12:"country_name";s:10:"Australia ";}i:123;a:5:{s:12:"airport_name";s:11:"SHAH AMANAT";s:12:"airport_code";s:3:"CGP";s:13:"location_name";s:10:"Chittagong";s:10:"country_id";s:2:"bd";s:12:"country_name";s:11:"Bangladesh ";}i:124;a:5:{s:12:"airport_name";s:13:"INDIRA GANDHI";s:12:"airport_code";s:3:"DEL";s:13:"location_name";s:5:"Delhi";s:10:"country_id";s:2:"bd";s:12:"country_name";s:11:"Bangladesh ";}i:125;a:5:{s:12:"airport_name";s:5:"Dhaka";s:12:"airport_code";s:3:"DAC";s:13:"location_name";s:5:"Dhaka";s:10:"country_id";s:2:"bd";s:12:"country_name";s:11:"Bangladesh ";}i:126;a:5:{s:12:"airport_name";s:6:"BRUNEI";s:12:"airport_code";s:3:"BWN";s:13:"location_name";s:6:"Brunei";s:10:"country_id";s:2:"bn";s:12:"country_name";s:18:"Brunei Darussalam ";}i:127;a:5:{s:12:"airport_name";s:10:"PHNOM PENH";s:12:"airport_code";s:3:"PNH";s:13:"location_name";s:10:"Phnom Penh";s:10:"country_id";s:2:"kh";s:12:"country_name";s:9:"Cambodia ";}i:128;a:5:{s:12:"airport_name";s:9:"SIEM REAP";s:12:"airport_code";s:3:"REP";s:13:"location_name";s:9:"Siem Reap";s:10:"country_id";s:2:"kh";s:12:"country_name";s:9:"Cambodia ";}i:129;a:5:{s:12:"airport_name";s:15:"Beijing Capital";s:12:"airport_code";s:3:"PEK";s:13:"location_name";s:7:"Beijing";s:10:"country_id";s:2:"cn";s:12:"country_name";s:6:"China ";}i:130;a:5:{s:12:"airport_name";s:17:"Chengdu Shuangliu";s:12:"airport_code";s:3:"CTU";s:13:"location_name";s:7:"Chengdu";s:10:"country_id";s:2:"cn";s:12:"country_name";s:6:"China ";}i:131;a:5:{s:12:"airport_name";s:18:"Chongqing Jiangbei";s:12:"airport_code";s:3:"CKG";s:13:"location_name";s:9:"Chongqing";s:10:"country_id";s:2:"cn";s:12:"country_name";s:6:"China ";}i:132;a:5:{s:12:"airport_name";s:16:"Guangzhou Baiyun";s:12:"airport_code";s:3:"CAN";s:13:"location_name";s:9:"Guangzhou";s:10:"country_id";s:2:"cn";s:12:"country_name";s:6:"China ";}i:133;a:5:{s:12:"airport_name";s:17:"Guilin Liangjiang";s:12:"airport_code";s:3:"KWL";s:13:"location_name";s:6:"Guilin";s:10:"country_id";s:2:"cn";s:12:"country_name";s:6:"China ";}i:134;a:5:{s:12:"airport_name";s:6:"HAIKOU";s:12:"airport_code";s:3:"HAK";s:13:"location_name";s:6:"Haikou";s:10:"country_id";s:2:"cn";s:12:"country_name";s:6:"China ";}i:135;a:5:{s:12:"airport_name";s:17:"HANGZHOU XIAOSHAN";s:12:"airport_code";s:3:"HGH";s:13:"location_name";s:8:"Hangzhou";s:10:"country_id";s:2:"cn";s:12:"country_name";s:6:"China ";}i:136;a:5:{s:12:"airport_name";s:15:"Kunming Wujiaba";s:12:"airport_code";s:3:"KMG";s:13:"location_name";s:7:"Kunming";s:10:"country_id";s:2:"cn";s:12:"country_name";s:6:"China ";}i:137;a:5:{s:12:"airport_name";s:12:"Nanning Wuxu";s:12:"airport_code";s:3:"NNG";s:13:"location_name";s:7:"Nanning";s:10:"country_id";s:2:"cn";s:12:"country_name";s:6:"China ";}i:138;a:5:{s:12:"airport_name";s:12:"Ningbo Lishe";s:12:"airport_code";s:3:"NGB";s:13:"location_name";s:6:"Ningbo";s:10:"country_id";s:2:"cn";s:12:"country_name";s:6:"China ";}i:139;a:5:{s:12:"airport_name";s:7:"Qingdao";s:12:"airport_code";s:3:"TAO";s:13:"location_name";s:7:"Qingdao";s:10:"country_id";s:2:"cn";s:12:"country_name";s:6:"China ";}i:140;a:5:{s:12:"airport_name";s:15:"Shanghai Pudong";s:12:"airport_code";s:3:"PVG";s:13:"location_name";s:8:"Shanghai";s:10:"country_id";s:2:"cn";s:12:"country_name";s:6:"China ";}i:141;a:5:{s:12:"airport_name";s:17:"SHANTOU / JIEYANG";s:12:"airport_code";s:3:"SWA";s:13:"location_name";s:17:"SHANTOU / JIEYANG";s:10:"country_id";s:2:"cn";s:12:"country_name";s:6:"China ";}i:142;a:5:{s:12:"airport_name";s:8:"Shenyang";s:12:"airport_code";s:3:"SHE";s:13:"location_name";s:8:"Shenyang";s:10:"country_id";s:2:"cn";s:12:"country_name";s:6:"China ";}i:143;a:5:{s:12:"airport_name";s:8:"Shenzhen";s:12:"airport_code";s:3:"SZX";s:13:"location_name";s:8:"Shenzhen";s:10:"country_id";s:2:"cn";s:12:"country_name";s:6:"China ";}i:144;a:5:{s:12:"airport_name";s:7:"Tianjin";s:12:"airport_code";s:3:"TSN";s:13:"location_name";s:7:"Tianjin";s:10:"country_id";s:2:"cn";s:12:"country_name";s:6:"China ";}i:145;a:5:{s:12:"airport_name";s:12:"Wuhan Tianhe";s:12:"airport_code";s:3:"WUH";s:13:"location_name";s:5:"Wuhan";s:10:"country_id";s:2:"cn";s:12:"country_name";s:6:"China ";}i:146;a:5:{s:12:"airport_name";s:14:"Xi An Xianyang";s:12:"airport_code";s:3:"XIY";s:13:"location_name";s:5:"Xi'an";s:10:"country_id";s:2:"cn";s:12:"country_name";s:6:"China ";}i:147;a:5:{s:12:"airport_name";s:5:"Naike";s:12:"airport_code";s:3:"CMB";s:13:"location_name";s:7:"Colombo";s:10:"country_id";s:2:"co";s:12:"country_name";s:9:"Colombia ";}i:148;a:5:{s:12:"airport_name";s:4:"NADI";s:12:"airport_code";s:3:"NAN";s:13:"location_name";s:4:"NADI";s:10:"country_id";s:2:"fj";s:12:"country_name";s:5:"Fiji ";}i:149;a:5:{s:12:"airport_name";s:9:"HONG KONG";s:12:"airport_code";s:3:"HKG";s:13:"location_name";s:9:"Hong Kong";s:10:"country_id";s:2:"hk";s:12:"country_name";s:10:"Hong Kong ";}i:150;a:5:{s:12:"airport_name";s:24:"SARDAR VALLABHBHAI PATEL";s:12:"airport_code";s:3:"AMD";s:13:"location_name";s:9:"Ahmedabad";s:10:"country_id";s:2:"in";s:12:"country_name";s:6:"India ";}i:151;a:5:{s:12:"airport_name";s:9:"Bangalore";s:12:"airport_code";s:3:"BLR";s:13:"location_name";s:9:"Bangalore";s:10:"country_id";s:2:"in";s:12:"country_name";s:6:"India ";}i:152;a:5:{s:12:"airport_name";s:7:"Chennai";s:12:"airport_code";s:3:"MAA";s:13:"location_name";s:7:"Chennai";s:10:"country_id";s:2:"in";s:12:"country_name";s:6:"India ";}i:153;a:5:{s:12:"airport_name";s:9:"Hyderabad";s:12:"airport_code";s:3:"HYD";s:13:"location_name";s:9:"Hyderabad";s:10:"country_id";s:2:"in";s:12:"country_name";s:6:"India ";}i:154;a:5:{s:12:"airport_name";s:5:"Kochi";s:12:"airport_code";s:3:"COK";s:13:"location_name";s:5:"Kochi";s:10:"country_id";s:2:"in";s:12:"country_name";s:6:"India ";}i:155;a:5:{s:12:"airport_name";s:27:"Netaji Subhas Chandra Bosen";s:12:"airport_code";s:3:"CCU";s:13:"location_name";s:7:"Kolkata";s:10:"country_id";s:2:"in";s:12:"country_name";s:6:"India ";}i:156;a:5:{s:12:"airport_name";s:19:"CHHATRAPATI SHIVAJI";s:12:"airport_code";s:3:"BOM";s:13:"location_name";s:6:"Mumbai";s:10:"country_id";s:2:"in";s:12:"country_name";s:6:"India ";}i:157;a:5:{s:12:"airport_name";s:18:"Thiruvananthapuram";s:12:"airport_code";s:3:"TRV";s:13:"location_name";s:18:"Thiruvananthapuram";s:10:"country_id";s:2:"in";s:12:"country_name";s:6:"India ";}i:158;a:5:{s:12:"airport_name";s:23:"Tiruchirapalli (Trichy)";s:12:"airport_code";s:3:"TRZ";s:13:"location_name";s:23:"Tiruchirapalli (Trichy)";s:10:"country_id";s:2:"in";s:12:"country_name";s:6:"India ";}i:159;a:5:{s:12:"airport_name";s:7:"FUKUOKA";s:12:"airport_code";s:3:"FUK";s:13:"location_name";s:7:"Fukuoka";s:10:"country_id";s:2:"jp";s:12:"country_name";s:6:"Japan ";}i:160;a:5:{s:12:"airport_name";s:9:"KAGOSHIMA";s:12:"airport_code";s:3:"KOJ";s:13:"location_name";s:9:"Kagoshima";s:10:"country_id";s:2:"jp";s:12:"country_name";s:6:"Japan ";}i:161;a:5:{s:12:"airport_name";s:8:"KUMAMOTO";s:12:"airport_code";s:3:"KMJ";s:13:"location_name";s:8:"Kumamoto";s:10:"country_id";s:2:"jp";s:12:"country_name";s:6:"Japan ";}i:162;a:5:{s:12:"airport_name";s:9:"MATSUYAMA";s:12:"airport_code";s:3:"MYJ";s:13:"location_name";s:9:"Matsuyama";s:10:"country_id";s:2:"jp";s:12:"country_name";s:6:"Japan ";}i:163;a:5:{s:12:"airport_name";s:21:"NAGOYA CHUBU CENTRAIR";s:12:"airport_code";s:3:"NGO";s:13:"location_name";s:6:"Nagoya";s:10:"country_id";s:2:"jp";s:12:"country_name";s:6:"Japan ";}i:164;a:5:{s:12:"airport_name";s:4:"OITA";s:12:"airport_code";s:3:"OIT";s:13:"location_name";s:4:"Oita";s:10:"country_id";s:2:"jp";s:12:"country_name";s:6:"Japan ";}i:165;a:5:{s:12:"airport_name";s:13:"OKINAWA, NAHA";s:12:"airport_code";s:3:"OKA";s:13:"location_name";s:14:"Okinawa - Naha";s:10:"country_id";s:2:"jp";s:12:"country_name";s:6:"Japan ";}i:166;a:5:{s:12:"airport_name";s:13:"OSAKA, KANSAI";s:12:"airport_code";s:3:"KIX";s:13:"location_name";s:14:"Osaka - Kansai";s:10:"country_id";s:2:"jp";s:12:"country_name";s:6:"Japan ";}i:167;a:5:{s:12:"airport_name";s:21:"SAPPORO, SHIN-CHITOSE";s:12:"airport_code";s:3:"CTS";s:13:"location_name";s:22:"Sapporo - Shin-Chitose";s:10:"country_id";s:2:"jp";s:12:"country_name";s:6:"Japan ";}i:168;a:5:{s:12:"airport_name";s:10:"TAKAMATSU ";s:12:"airport_code";s:3:"TAK";s:13:"location_name";s:10:"Takamatsu ";s:10:"country_id";s:2:"jp";s:12:"country_name";s:6:"Japan ";}i:169;a:5:{s:12:"airport_name";s:13:"Tokyo, Haneda";s:12:"airport_code";s:3:"HND";s:13:"location_name";s:14:"Tokyo - Haneda";s:10:"country_id";s:2:"jp";s:12:"country_name";s:6:"Japan ";}i:170;a:5:{s:12:"airport_name";s:13:"TOKYO, NARITA";s:12:"airport_code";s:3:"NRT";s:13:"location_name";s:14:"Tokyo - Narita";s:10:"country_id";s:2:"jp";s:12:"country_name";s:6:"Japan ";}i:171;a:5:{s:12:"airport_name";s:6:"Wattay";s:12:"airport_code";s:3:"VTE";s:13:"location_name";s:9:"Vientiane";s:10:"country_id";s:2:"la";s:12:"country_name";s:4:"Laos";}i:172;a:5:{s:12:"airport_name";s:5:"MACAU";s:12:"airport_code";s:3:"MFM";s:13:"location_name";s:5:"Macau";s:10:"country_id";s:2:"mo";s:12:"country_name";s:6:"Macau ";}i:173;a:5:{s:12:"airport_name";s:18:"Sultan Abdul Halim";s:12:"airport_code";s:3:"AOR";s:13:"location_name";s:10:"Alor Setar";s:10:"country_id";s:2:"my";s:12:"country_name";s:9:"Malaysia ";}i:174;a:5:{s:12:"airport_name";s:7:"Bintulu";s:12:"airport_code";s:3:"BTU";s:13:"location_name";s:7:"Bintulu";s:10:"country_id";s:2:"my";s:12:"country_name";s:9:"Malaysia ";}i:175;a:5:{s:12:"airport_name";s:5:"Senai";s:12:"airport_code";s:3:"JHB";s:13:"location_name";s:10:"Johor Baru";s:10:"country_id";s:2:"my";s:12:"country_name";s:9:"Malaysia ";}i:176;a:5:{s:12:"airport_name";s:19:"Sultan Ismail Petra";s:12:"airport_code";s:3:"KBR";s:13:"location_name";s:10:"Kota Bharu";s:10:"country_id";s:2:"my";s:12:"country_name";s:9:"Malaysia ";}i:177;a:5:{s:12:"airport_name";s:13:"Kota Kinabalu";s:12:"airport_code";s:3:"BKI";s:13:"location_name";s:13:"Kota Kinabalu";s:10:"country_id";s:2:"my";s:12:"country_name";s:9:"Malaysia ";}i:178;a:5:{s:12:"airport_name";s:12:"KUALA LUMPUR";s:12:"airport_code";s:3:"KUL";s:13:"location_name";s:12:"Kuala Lumpur";s:10:"country_id";s:2:"my";s:12:"country_name";s:9:"Malaysia ";}i:179;a:5:{s:12:"airport_name";s:13:"SULTAN MAHMUD";s:12:"airport_code";s:3:"TGG";s:13:"location_name";s:16:"Kuala Terengganu";s:10:"country_id";s:2:"my";s:12:"country_name";s:9:"Malaysia ";}i:180;a:5:{s:12:"airport_name";s:7:"Kuching";s:12:"airport_code";s:3:"KCH";s:13:"location_name";s:7:"Kuching";s:10:"country_id";s:2:"my";s:12:"country_name";s:9:"Malaysia ";}i:181;a:5:{s:12:"airport_name";s:8:"Langkawi";s:12:"airport_code";s:3:"LGK";s:13:"location_name";s:8:"Langkawi";s:10:"country_id";s:2:"my";s:12:"country_name";s:9:"Malaysia ";}i:182;a:5:{s:12:"airport_name";s:7:"Malacca";s:12:"airport_code";s:3:"MKZ";s:13:"location_name";s:7:"Malacca";s:10:"country_id";s:2:"my";s:12:"country_name";s:9:"Malaysia ";}i:183;a:5:{s:12:"airport_name";s:4:"Miri";s:12:"airport_code";s:3:"MYY";s:13:"location_name";s:4:"Miri";s:10:"country_id";s:2:"my";s:12:"country_name";s:9:"Malaysia ";}i:184;a:5:{s:12:"airport_name";s:6:"PENANG";s:12:"airport_code";s:3:"PEN";s:13:"location_name";s:6:"Penang";s:10:"country_id";s:2:"my";s:12:"country_name";s:9:"Malaysia ";}i:185;a:5:{s:12:"airport_name";s:8:"Sandakan";s:12:"airport_code";s:3:"SDK";s:13:"location_name";s:7:"Sandaka";s:10:"country_id";s:2:"my";s:12:"country_name";s:9:"Malaysia ";}i:186;a:5:{s:12:"airport_name";s:4:"Sibu";s:12:"airport_code";s:3:"SBW";s:13:"location_name";s:4:"Sibu";s:10:"country_id";s:2:"my";s:12:"country_name";s:9:"Malaysia ";}i:187;a:5:{s:12:"airport_name";s:22:"Sultan Abdul Aziz Shah";s:12:"airport_code";s:3:"SZB";s:13:"location_name";s:6:"Subang";s:10:"country_id";s:2:"my";s:12:"country_name";s:9:"Malaysia ";}i:188;a:5:{s:12:"airport_name";s:4:"IPOH";s:12:"airport_code";s:3:"IPH";s:13:"location_name";s:17:"SULTAN AZLAN SHAH";s:10:"country_id";s:2:"my";s:12:"country_name";s:9:"Malaysia ";}i:189;a:5:{s:12:"airport_name";s:5:"Tawau";s:12:"airport_code";s:3:"TWU";s:13:"location_name";s:5:"Tawau";s:10:"country_id";s:2:"my";s:12:"country_name";s:9:"Malaysia ";}i:190;a:5:{s:12:"airport_name";s:8:"Mandalay";s:12:"airport_code";s:3:"MDL";s:13:"location_name";s:8:"Mandalay";s:10:"country_id";s:2:"mm";s:12:"country_name";s:8:"Myanmar ";}i:191;a:5:{s:12:"airport_name";s:7:"YANGOON";s:12:"airport_code";s:3:"RGN";s:13:"location_name";s:7:"Yangoon";s:10:"country_id";s:2:"mm";s:12:"country_name";s:8:"Myanmar ";}i:192;a:5:{s:12:"airport_name";s:9:"Tribhuvan";s:12:"airport_code";s:3:"KTM";s:13:"location_name";s:9:"Kathmandu";s:10:"country_id";s:2:"np";s:12:"country_name";s:6:"Nepal ";}i:193;a:5:{s:12:"airport_name";s:8:"SCHIPHOL";s:12:"airport_code";s:3:"AMS";s:13:"location_name";s:8:"SCHIPHOL";s:10:"country_id";s:2:"nl";s:12:"country_name";s:12:"Netherlands ";}i:194;a:5:{s:12:"airport_name";s:8:"AUCKLAND";s:12:"airport_code";s:3:"AKL";s:13:"location_name";s:8:"AUCKLAND";s:10:"country_id";s:2:"nz";s:12:"country_name";s:12:"New Zealand ";}i:195;a:5:{s:12:"airport_name";s:12:"CHRISTCHURCH";s:12:"airport_code";s:3:"CHC";s:13:"location_name";s:12:"CHRISTCHURCH";s:10:"country_id";s:2:"nz";s:12:"country_name";s:12:"New Zealand ";}i:196;a:5:{s:12:"airport_name";s:7:"DUNEDIN";s:12:"airport_code";s:3:"DUD";s:13:"location_name";s:7:"DUNEDIN";s:10:"country_id";s:2:"nz";s:12:"country_name";s:12:"New Zealand ";}i:197;a:5:{s:12:"airport_name";s:10:"QUEENSTOWN";s:12:"airport_code";s:3:"ZQN";s:13:"location_name";s:10:"QUEENSTOWN";s:10:"country_id";s:2:"nz";s:12:"country_name";s:12:"New Zealand ";}i:198;a:5:{s:12:"airport_name";s:10:"WELLINGTON";s:12:"airport_code";s:3:"WLG";s:13:"location_name";s:10:"WELLINGTON";s:10:"country_id";s:2:"nz";s:12:"country_name";s:12:"New Zealand ";}i:199;a:5:{s:12:"airport_name";s:7:"Bacolod";s:12:"airport_code";s:3:"BCD";s:13:"location_name";s:7:"Bacolod";s:10:"country_id";s:2:"ph";s:12:"country_name";s:12:"Philippines ";}i:200;a:5:{s:12:"airport_name";s:11:"Mactan-Cebu";s:12:"airport_code";s:3:"CEB";s:13:"location_name";s:4:"Cebu";s:10:"country_id";s:2:"ph";s:12:"country_name";s:12:"Philippines ";}i:201;a:5:{s:12:"airport_name";s:5:"CLARK";s:12:"airport_code";s:3:"CRK";s:13:"location_name";s:5:"Clark";s:10:"country_id";s:2:"ph";s:12:"country_name";s:12:"Philippines ";}i:202;a:5:{s:12:"airport_name";s:5:"Davao";s:12:"airport_code";s:3:"DVO";s:13:"location_name";s:5:"Davao";s:10:"country_id";s:2:"ph";s:12:"country_name";s:12:"Philippines ";}i:203;a:5:{s:12:"airport_name";s:6:"Iloilo";s:12:"airport_code";s:3:"ILO";s:13:"location_name";s:6:"Iloilo";s:10:"country_id";s:2:"ph";s:12:"country_name";s:12:"Philippines ";}i:204;a:5:{s:12:"airport_name";s:12:"NINOY AQUINO";s:12:"airport_code";s:3:"MNL";s:13:"location_name";s:13:"Manila (NAIA)";s:10:"country_id";s:2:"ph";s:12:"country_name";s:12:"Philippines ";}i:205;a:5:{s:12:"airport_name";s:15:"Puerto Princesa";s:12:"airport_code";s:3:"PPS";s:13:"location_name";s:15:"Puerto Princesa";s:10:"country_id";s:2:"ph";s:12:"country_name";s:12:"Philippines ";}i:206;a:5:{s:12:"airport_name";s:8:"Tacloban";s:12:"airport_code";s:3:"TAC";s:13:"location_name";s:8:"Tacloban";s:10:"country_id";s:2:"ph";s:12:"country_name";s:12:"Philippines ";}i:207;a:5:{s:12:"airport_name";s:14:"King Abdulaziz";s:12:"airport_code";s:3:"JED";s:13:"location_name";s:6:"Jeddah";s:10:"country_id";s:2:"sa";s:12:"country_name";s:13:"Saudi Arabia ";}i:208;a:5:{s:12:"airport_name";s:6:"Changi";s:12:"airport_code";s:3:"SIN";s:13:"location_name";s:9:"Singapore";s:10:"country_id";s:2:"sg";s:12:"country_name";s:10:"Singapore ";}i:209;a:5:{s:12:"airport_name";s:6:"Gimhae";s:12:"airport_code";s:3:"PUS";s:13:"location_name";s:5:"Busan";s:10:"country_id";s:2:"kr";s:12:"country_name";s:11:"South Korea";}i:210;a:5:{s:12:"airport_name";s:7:"Incheon";s:12:"airport_code";s:3:"ICN";s:13:"location_name";s:5:"Seoul";s:10:"country_id";s:2:"kr";s:12:"country_name";s:11:"South Korea";}i:211;a:5:{s:12:"airport_name";s:14:"TAIWAN TAOYUAN";s:12:"airport_code";s:3:"TPE";s:13:"location_name";s:6:"Taipei";s:10:"country_id";s:2:"tw";s:12:"country_name";s:6:"Taiwan";}i:212;a:5:{s:12:"airport_name";s:12:"SUVARNABHUMI";s:12:"airport_code";s:3:"BKK";s:13:"location_name";s:7:"Bangkok";s:10:"country_id";s:2:"th";s:12:"country_name";s:9:"Thailand ";}i:213;a:5:{s:12:"airport_name";s:10:"DON MUEANG";s:12:"airport_code";s:3:"DMK";s:13:"location_name";s:20:"Bangkok - Don Mueang";s:10:"country_id";s:2:"th";s:12:"country_name";s:9:"Thailand ";}i:214;a:5:{s:12:"airport_name";s:10:"CHIANG MAI";s:12:"airport_code";s:3:"CNX";s:13:"location_name";s:10:"Chiang Mai";s:10:"country_id";s:2:"th";s:12:"country_name";s:9:"Thailand ";}i:215;a:5:{s:12:"airport_name";s:24:"Mae Fah Luang-Chiang Rai";s:12:"airport_code";s:3:"CEI";s:13:"location_name";s:10:"Chiang Rai";s:10:"country_id";s:2:"th";s:12:"country_name";s:9:"Thailand ";}i:216;a:5:{s:12:"airport_name";s:7:"Hat Yai";s:12:"airport_code";s:3:"HDY";s:13:"location_name";s:7:"Hat Yai";s:10:"country_id";s:2:"th";s:12:"country_name";s:9:"Thailand ";}i:217;a:5:{s:12:"airport_name";s:5:"Krabi";s:12:"airport_code";s:3:"KBV";s:13:"location_name";s:5:"Krabi";s:10:"country_id";s:2:"th";s:12:"country_name";s:9:"Thailand ";}i:218;a:5:{s:12:"airport_name";s:13:"Nakhon Phanom";s:12:"airport_code";s:3:"KOP";s:13:"location_name";s:13:"Nakhon Phanom";s:10:"country_id";s:2:"th";s:12:"country_name";s:9:"Thailand ";}i:219;a:5:{s:12:"airport_name";s:19:"Nakhon Si Thammarat";s:12:"airport_code";s:3:"NST";s:13:"location_name";s:19:"Nakhon Si Thammarat";s:10:"country_id";s:2:"th";s:12:"country_name";s:9:"Thailand ";}i:220;a:5:{s:12:"airport_name";s:10:"Narathiwat";s:12:"airport_code";s:3:"NAW";s:13:"location_name";s:10:"Narathiwat";s:10:"country_id";s:2:"th";s:12:"country_name";s:9:"Thailand ";}i:221;a:5:{s:12:"airport_name";s:6:"PHUKET";s:12:"airport_code";s:3:"HKT";s:13:"location_name";s:6:"Phuket";s:10:"country_id";s:2:"th";s:12:"country_name";s:9:"Thailand ";}i:222;a:5:{s:12:"airport_name";s:11:"Surat Thani";s:12:"airport_code";s:3:"URT";s:13:"location_name";s:11:"Surat Thani";s:10:"country_id";s:2:"th";s:12:"country_name";s:9:"Thailand ";}i:223;a:5:{s:12:"airport_name";s:5:"Trang";s:12:"airport_code";s:3:"TST";s:13:"location_name";s:5:"Trang";s:10:"country_id";s:2:"th";s:12:"country_name";s:9:"Thailand ";}i:224;a:5:{s:12:"airport_name";s:16:"Ubon Ratchathani";s:12:"airport_code";s:3:"UBP";s:13:"location_name";s:16:"Ubon Ratchathani";s:10:"country_id";s:2:"th";s:12:"country_name";s:9:"Thailand ";}i:225;a:5:{s:12:"airport_name";s:9:"Udonthani";s:12:"airport_code";s:3:"UTH";s:13:"location_name";s:10:"Udon Thani";s:10:"country_id";s:2:"th";s:12:"country_name";s:9:"Thailand ";}i:226;a:5:{s:12:"airport_name";s:25:"Presidente Nicolau Lobato";s:12:"airport_code";s:3:"DIL";s:13:"location_name";s:4:"Dili";s:10:"country_id";s:2:"tl";s:12:"country_name";s:12:"Timor-Leste ";}i:227;a:5:{s:12:"airport_name";s:9:"ABU DHABI";s:12:"airport_code";s:3:"ABU";s:13:"location_name";s:9:"Abu Dhabi";s:10:"country_id";s:2:"ae";s:12:"country_name";s:21:"United Arab Emirates ";}i:228;a:5:{s:12:"airport_name";s:9:"ABU DHABI";s:12:"airport_code";s:3:"AUH";s:13:"location_name";s:9:"Abu Dhabi";s:10:"country_id";s:2:"ae";s:12:"country_name";s:21:"United Arab Emirates ";}i:229;a:5:{s:12:"airport_name";s:27:"DUBAI INTERNATIONAL AIRPORT";s:12:"airport_code";s:3:"DXB";s:13:"location_name";s:5:"Dubai";s:10:"country_id";s:2:"ae";s:12:"country_name";s:21:"United Arab Emirates ";}i:230;a:5:{s:12:"airport_name";s:12:"DYCE AIRPORT";s:12:"airport_code";s:3:"ABZ";s:13:"location_name";s:9:"edinbrugh";s:10:"country_id";s:2:"gb";s:12:"country_name";s:15:"United Kingdom ";}i:231;a:5:{s:12:"airport_name";s:6:"LONDON";s:12:"airport_code";s:3:"LGW";s:13:"location_name";s:6:"London";s:10:"country_id";s:2:"gb";s:12:"country_name";s:15:"United Kingdom ";}i:232;a:5:{s:12:"airport_name";s:15:"LONDON HEATHROW";s:12:"airport_code";s:3:"LHR";s:13:"location_name";s:13:"palmers green";s:10:"country_id";s:2:"gb";s:12:"country_name";s:15:"United Kingdom ";}i:233;a:5:{s:12:"airport_name";s:8:"HONOLULU";s:12:"airport_code";s:3:"HNL";s:13:"location_name";s:8:"HONOLULU";s:10:"country_id";s:2:"us";s:12:"country_name";s:14:"United States ";}i:234;a:5:{s:12:"airport_name";s:33:"LOS ANGELES INTERNATIONAL AIRPORT";s:12:"airport_code";s:3:"LAX";s:13:"location_name";s:11:"Los Angeles";s:10:"country_id";s:2:"us";s:12:"country_name";s:14:"United States ";}i:235;a:5:{s:12:"airport_name";s:31:"SAN DIEGO INTERNATIONAL AIRPORT";s:12:"airport_code";s:3:"SAN";s:13:"location_name";s:31:"San Diego International Airport";s:10:"country_id";s:2:"us";s:12:"country_name";s:14:"United States ";}i:236;a:5:{s:12:"airport_name";s:13:"BUON MA THUOT";s:12:"airport_code";s:3:"BMV";s:13:"location_name";s:13:"Buon Ma Thuot";s:10:"country_id";s:2:"vn";s:12:"country_name";s:8:"Vietnam ";}i:237;a:5:{s:12:"airport_name";s:7:"DA NANG";s:12:"airport_code";s:3:"DAD";s:13:"location_name";s:7:"Da Nang";s:10:"country_id";s:2:"vn";s:12:"country_name";s:8:"Vietnam ";}i:238;a:5:{s:12:"airport_name";s:8:"DONG HOI";s:12:"airport_code";s:3:"VDH";s:13:"location_name";s:8:"Dong Hoi";s:10:"country_id";s:2:"vn";s:12:"country_name";s:8:"Vietnam ";}i:239;a:5:{s:12:"airport_name";s:9:"HAI PHONG";s:12:"airport_code";s:3:"HPH";s:13:"location_name";s:9:"Hai Phong";s:10:"country_id";s:2:"vn";s:12:"country_name";s:8:"Vietnam ";}i:240;a:5:{s:12:"airport_name";s:12:"TAN SON NHAT";s:12:"airport_code";s:3:"SGN";s:13:"location_name";s:16:"Ho Chi Minh City";s:10:"country_id";s:2:"vn";s:12:"country_name";s:8:"Vietnam ";}i:241;a:5:{s:12:"airport_name";s:3:"HUI";s:12:"airport_code";s:3:"HUI";s:13:"location_name";s:3:"HUI";s:10:"country_id";s:2:"vn";s:12:"country_name";s:8:"Vietnam ";}i:242;a:5:{s:12:"airport_name";s:9:"NHA TRANG";s:12:"airport_code";s:3:"CXR";s:13:"location_name";s:9:"Nha Trang";s:10:"country_id";s:2:"vn";s:12:"country_name";s:8:"Vietnam ";}i:243;a:5:{s:12:"airport_name";s:7:"NOI BAI";s:12:"airport_code";s:3:"HAN";s:13:"location_name";s:7:"Noi Bai";s:10:"country_id";s:2:"vn";s:12:"country_name";s:8:"Vietnam ";}i:244;a:5:{s:12:"airport_name";s:8:"PHU QUOC";s:12:"airport_code";s:3:"PQC";s:13:"location_name";s:8:"Phu Quoc";s:10:"country_id";s:2:"vn";s:12:"country_name";s:8:"Vietnam ";}i:245;a:5:{s:12:"airport_name";s:8:"QUY NHON";s:12:"airport_code";s:3:"UIH";s:13:"location_name";s:9:"Quy Nhon ";s:10:"country_id";s:2:"vn";s:12:"country_name";s:8:"Vietnam ";}i:246;a:5:{s:12:"airport_name";s:9:"THANH HOA";s:12:"airport_code";s:3:"THD";s:13:"location_name";s:9:"Thanh Hoa";s:10:"country_id";s:2:"vn";s:12:"country_name";s:8:"Vietnam ";}i:247;a:5:{s:12:"airport_name";s:7:"TUY HOA";s:12:"airport_code";s:3:"TBB";s:13:"location_name";s:7:"Tuy Hoa";s:10:"country_id";s:2:"vn";s:12:"country_name";s:8:"Vietnam ";}i:248;a:5:{s:12:"airport_name";s:4:"VINH";s:12:"airport_code";s:3:"VII";s:13:"location_name";s:4:"Vinh";s:10:"country_id";s:2:"vn";s:12:"country_name";s:8:"Vietnam ";}}}s:12:"login_status";s:5:"false";s:5:"token";s:40:"f9b29ac359ca5d77755e7588751c089bf96f0dc9";}
```

#### HTTP Request

`GET https://api-sandbox.tiket.com/flight_api/all_airport?token=2b2f462814af7c0d2e1b40f28e2d9dff5e900f24`

#### Parameters
  
Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------
token | for saving transaction that done by user | CHAR(128) |  | TRUE  


    
## Check Update


```xml
<tiket>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.0437</elapsetime>
    <memoryusage>4.36MB</memoryusage>
    <unix_timestamp>1399963263</unix_timestamp>
    <confirm>success</confirm>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <update>24</update>
  <output_type>xml</output_type>
  <timestamp>1399963263</timestamp>
  <login_status>false</login_status>
  <token>2b2f462814af7c0d2e1b40f28e2d9dff5e900f24</token>
</tiket>
```



```json
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.0557",
    "memoryusage": "4.35MB",
    "unix_timestamp": 1399963609,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "update": 24,
  "output_type": "json",
  "timestamp": 1399963609,
  "login_status": "false",
  "token": "2b2f462814af7c0d2e1b40f28e2d9dff5e900f24"
}
```



```matlab
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.0557",
    "memoryusage": "4.35MB",
    "unix_timestamp": 1399963609,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "update": 24,
  "output_type": "json",
  "timestamp": 1399963609,
  "login_status": "false",
  "token": "2b2f462814af7c0d2e1b40f28e2d9dff5e900f24"
}
```
   
   
Data given when requested is the latest data updated by the previous request, not the live data. For checking whether new or updated data exists or not, you should call `check update` function.  
If update variable is greater than 0, it means that there is new fresh data for you to grab.  
To get the latest data, search function must be called again.

#### HTTP Request

`https://api-sandbox.tiket.com/ajax/mCheckFlightUpdated?token=2b2f462814af7c0d2e1b40f28e2d9dff5e900f24&d=CGK&a=DPS&date=2014-05-30&adult=1&child=0&infant=0&time=134078435`

#### Parameters
  
Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------
d | Departure airport code | CHAR(3) |  | TRUE  
a | Arrival airport code | CHAR(3) |  | TRUE  
date | depart date | YYYY-MM-DD |  | TRUE  
adult | number of adult passenger | INT | 1 | FALSE  
child | number of child passenger | INT | 0 | FALSE  
infant | number of infant passenger | INT | 0 | FALSE  
time | Timestamp (time()) | timestamp |  | TRUE  
token | for saving transaction that done by user | CHAR(128) |  | TRUE  

    
    
## Get Lion Captcha


```xml
<tiket>
  <output_type>xml</output_type>
  <lioncaptcha>
    data:image/jpeg;base64,/9j/4AAQSkZJRgABAQEA04K0H5bmJF4Xy2+UdOCtFFAAfluYkXhfLb5R04K0UUUAf/9k=
  </lioncaptcha>
  <lionsessionid>35gds5amnkamlo55npu0z355|0</lionsessionid>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.3305</elapsetime>
    <memoryusage>3.94MB</memoryusage>
    <confirm>success</confirm>
    <lang>en</lang>
    <currency>IDR</currency>
  </diagnostic>
  <token>adcefff7d50618ff205473975adf9d64</token>
</tiket>
```



```json
{
  output_type: "json",
  lioncaptcha: "data:image/jpeg;base64,/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAgGBgcGBQgHBwcJ",
  lionsessionid: "0yjpyyahziye1u55vgdau1a3|0",
  diagnostic: {
    status: 200,
    elapsetime: "0.4400",
    memoryusage: "3.91MB",
    confirm: "success",
    lang: "en",
    currency: "IDR"
  },
  token: "adcefff7d50618ff205473975adf9d64"
}
```



```matlab
a: 5: {
  s: 11: "output_type";s: 9: "serialize";s: 12: "lioncaptcha";s: 3283: "data:image/jpeg;base64,/9j/4AAQSkZJRgABAQEAYABgAAD/AH//Z";s: 15: "lionsessionid";s: 26: "omhqis55vrnuobz3jtdtobe2|0";s: 10: "diagnostic";a: 6: {
    s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.3032";s: 11: "memoryusage";s: 14: "3.91MB";s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "en";s: 8: "currency";s: 3: "IDR";
  }
  s: 5: "token";s: 32: "adcefff7d50618ff205473975adf9d64";
}
```

This API is specific for Lion air flights whe you will have to ask customer to enter captcha so that they can continue their booking.  
If the `getLionCaptcha` return data, the captcha and sessionid must be included while calling add order.


#### HTTP Request

`GET https://api-sandbox.tiket.com/flight_api/getLionCaptcha?token=adcefff7d50618ff205473975adf9d64&output=json`

#### Parameters

Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------
token | for saving transaction that done by user | CHAR(128) |  | TRUE  


## Get Flight Data

```xml
<tiket>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.0571</elapsetime>
    <memoryusage>5.38MB</memoryusage>
    <unix_timestamp>1399967481</unix_timestamp>
    <confirm>success</confirm>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <output_type>xml</output_type>
  <required>
    <separator>
      <mandatory>1</mandatory>
      <type>text</type>
      <example/>
      <FieldText>Contact Person Information</FieldText>
      <category>separator</category>
    </separator>
    <conSalutation>
      <mandatory>1</mandatory>
      <type>combobox</type>
      <example>Mr</example>
      <FieldText>Title</FieldText>
      <category>contact</category>
      <resource>
        <id>Mr</id>
        <name>Mr</name>
      </resource>
      <resource>
        <id>Mrs</id>
        <name>Mrs</name>
      </resource>
      <resource>
        <id>Ms</id>
        <name>Ms</name>
      </resource>
    </conSalutation>
    <conFirstName>
      <mandatory>1</mandatory>
      <type>textbox</type>
      <example>Jane</example>
      <FieldText>First Name</FieldText>
      <category>contact</category>
    </conFirstName>
    <conLastName>
      <mandatory>1</mandatory>
      <type>textbox</type>
      <example>Wacob</example>
      <FieldText>Last Name</FieldText>
      <category>contact</category>
    </conLastName>
    <conPhone>
      <mandatory>1</mandatory>
      <type>textbox</type>
      <example>Jane</example>
      <FieldText>Phone Number</FieldText>
      <category>contact</category>
    </conPhone>
    <separator_adult1>
      <mandatory>1</mandatory>
      <type>text</type>
      <example/>
      <FieldText>Adult Passenger 1</FieldText>
      <category>separator</category>
    </separator_adult1>
    <firstnamea1>
      <mandatory>1</mandatory>
      <type>textbox</type>
      <example>Jane</example>
      <FieldText>First Name</FieldText>
      <category>adult1</category>
    </firstnamea1>
    <lastnamea1>
      <mandatory>1</mandatory>
      <type>textbox</type>
      <example>wacob</example>
      <FieldText>Last Name</FieldText>
      <category>adult1</category>
    </lastnamea1>
    <ida1>
      <mandatory>1</mandatory>
      <type>textbox</type>
      <example>143243434323443</example>
      <FieldText>ID Card Number (KTP/Passport/Other)</FieldText>
      <category>adult1</category>
    </ida1>
    <titlea1>
      <mandatory>1</mandatory>
      <type>combobox</type>
      <example>Mr</example>
      <FieldText>Title</FieldText>
      <category>adult1</category>
      <resource>
        <id>Mr</id>
        <name>Mr</name>
      </resource>
      <resource>
        <id>Mrs</id>
        <name>Mrs</name>
      </resource>
      <resource>
        <id>Ms</id>
        <name>Ms</name>
      </resource>
    </titlea1>
    <birthdatea1>
      <mandatory>1</mandatory>
      <type>datetime</type>
      <example>1990-01-01</example>
      <FieldText>Birth Date</FieldText>
      <category>adult1</category>
    </birthdatea1>
    <passportnationalitya1>
      <mandatory>1</mandatory>
      <type>combobox</type>
      <example>id</example>
      <FieldText>Nationality</FieldText>
      <category>adult1</category>
      <resource>http://api.tiket.com/general_api/listCountry</resource>
    </passportnationalitya1>
  </required>
  <departures>
    <flight_id>16825942</flight_id>
    <airlines_name>CITILINK</airlines_name>
    <flight_number>QG-850</flight_number>
    <price_value>1362800.00</price_value>
    <count_adult>1</count_adult>
    <count_child>0</count_child>
    <count_infant>0</count_infant>
    <timestamp>2014-05-13 11:06:21</timestamp>
    <price_adult>1362800.00</price_adult>
    <price_child>0.00</price_child>
    <price_infant>0.00</price_infant>
    <simple_departure_time>07:40</simple_departure_time>
    <simple_arrival_time>10:25</simple_arrival_time>
    <stop>Nonstop</stop>
    <long_via/>
    <full_via>CGK - DPS (07:40 - 10:25)</full_via>
    <need_baggage>0</need_baggage>
    <duration>1 h 45 m</duration>
    <image>
      http://www.tiket.com/images/tiket2/icon_citilink_2.jpg
    </image>
    <flight_infos>
      <flight_info>
        <flight_number>QG-850</flight_number>
        <departure_city>CGK</departure_city>
        <arrival_city>DPS</arrival_city>
        <simple_departure_time/>
        <simple_arrival_time/>
      </flight_info>
    </flight_infos>
  </departures>
  <login_status>false</login_status>
  <token>2b2f462814af7c0d2e1b40f28e2d9dff5e900f24</token>
</tiket>
```

```json
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.0672",
    "memoryusage": "5.37MB",
    "unix_timestamp": 1399967577,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "required": {
    "separator": {
      "mandatory": 1,
      "type": "text",
      "example": "",
      "FieldText": "Contact Person Information ",
      "category": "separator"
    },
    "conSalutation": {
      "mandatory": 1,
      "type": "combobox",
      "example": "Mr",
      "FieldText": "Title",
      "category": "contact",
      "resource": [{
        "id": "Mr",
        "name": "Mr"
      }, {
        "id": "Mrs",
        "name": "Mrs"
      }, {
        "id": "Ms",
        "name": "Ms"
      }]
    },
    "conFirstName": {
      "mandatory": 1,
      "type": "textbox",
      "example": "Jane",
      "FieldText": "First Name",
      "category": "contact"
    },
    "conLastName": {
      "mandatory": 1,
      "type": "textbox",
      "example": "Wacob",
      "FieldText": "Last Name",
      "category": "contact"
    },
    "conPhone": {
      "mandatory": 1,
      "type": "textbox",
      "example": "Jane",
      "FieldText": "Phone Number",
      "category": "contact"
    },
    "separator_adult1": {
      "mandatory": 1,
      "type": "text",
      "example": "",
      "FieldText": "Adult Passenger 1",
      "category": "separator"
    },
    "firstnamea1": {
      "mandatory": 1,
      "type": "textbox",
      "example": "Jane",
      "FieldText": "First Name",
      "category": "adult1"
    },
    "lastnamea1": {
      "mandatory": 1,
      "type": "textbox",
      "example": "wacob",
      "FieldText": "Last Name",
      "category": "adult1"
    },
    "ida1": {
      "mandatory": 1,
      "type": "textbox",
      "example": "143243434323443",
      "FieldText": "ID Card Number (KTP/Passport/Other)",
      "category": "adult1"
    },
    "titlea1": {
      "mandatory": 1,
      "type": "combobox",
      "example": "Mr",
      "FieldText": "Title",
      "category": "adult1",
      "resource": [{
        "id": "Mr",
        "name": "Mr"
      }, {
        "id": "Mrs",
        "name": "Mrs"
      }, {
        "id": "Ms",
        "name": "Ms"
      }]
    },
    "birthdatea1": {
      "mandatory": 1,
      "type": "datetime",
      "example": "1990-01-01",
      "FieldText": "Birth Date",
      "category": "adult1"
    },
    "passportnationalitya1": {
      "mandatory": 1,
      "type": "combobox",
      "example": "id",
      "FieldText": "Nationality",
      "category": "adult1",
      "resource": "http:\/\/api.tiket.com\/general_api\/listCountry"
    }
  },
  "departures": {
    "flight_id": "16825942",
    "airlines_name": "CITILINK",
    "flight_number": "QG-850",
    "price_value": "1362800.00",
    "count_adult": "1",
    "count_child": "0",
    "count_infant": "0",
    "timestamp": "2014-05-13 11:06:21",
    "price_adult": "1362800.00",
    "price_child": "0.00",
    "price_infant": "0.00",
    "simple_departure_time": "07:40",
    "simple_arrival_time": "10:25",
    "stop": "Nonstop",
    "long_via": "",
    "full_via": "CGK - DPS (07:40 - 10:25)",
    "need_baggage": 0,
    "duration": "1 h 45 m",
    "image": "http:\/\/www.tiket.com\/images\/tiket2\/icon_citilink_2.jpg",
    "flight_infos": {
      "flight_info": [{
        "flight_number": "QG-850",
        "departure_city": "CGK",
        "arrival_city": "DPS",
        "simple_departure_time": "",
        "simple_arrival_time": ""
      }]
    }
  },
  "login_status": "false",
  "token": "2b2f462814af7c0d2e1b40f28e2d9dff5e900f24"
}
```

```matlab
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.0672",
    "memoryusage": "5.37MB",
    "unix_timestamp": 1399967577,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "required": {
    "separator": {
      "mandatory": 1,
      "type": "text",
      "example": "",
      "FieldText": "Contact Person Information ",
      "category": "separator"
    },
    "conSalutation": {
      "mandatory": 1,
      "type": "combobox",
      "example": "Mr",
      "FieldText": "Title",
      "category": "contact",
      "resource": [{
        "id": "Mr",
        "name": "Mr"
      }, {
        "id": "Mrs",
        "name": "Mrs"
      }, {
        "id": "Ms",
        "name": "Ms"
      }]
    },
    "conFirstName": {
      "mandatory": 1,
      "type": "textbox",
      "example": "Jane",
      "FieldText": "First Name",
      "category": "contact"
    },
    "conLastName": {
      "mandatory": 1,
      "type": "textbox",
      "example": "Wacob",
      "FieldText": "Last Name",
      "category": "contact"
    },
    "conPhone": {
      "mandatory": 1,
      "type": "textbox",
      "example": "Jane",
      "FieldText": "Phone Number",
      "category": "contact"
    },
    "separator_adult1": {
      "mandatory": 1,
      "type": "text",
      "example": "",
      "FieldText": "Adult Passenger 1",
      "category": "separator"
    },
    "firstnamea1": {
      "mandatory": 1,
      "type": "textbox",
      "example": "Jane",
      "FieldText": "First Name",
      "category": "adult1"
    },
    "lastnamea1": {
      "mandatory": 1,
      "type": "textbox",
      "example": "wacob",
      "FieldText": "Last Name",
      "category": "adult1"
    },
    "ida1": {
      "mandatory": 1,
      "type": "textbox",
      "example": "143243434323443",
      "FieldText": "ID Card Number (KTP/Passport/Other)",
      "category": "adult1"
    },
    "titlea1": {
      "mandatory": 1,
      "type": "combobox",
      "example": "Mr",
      "FieldText": "Title",
      "category": "adult1",
      "resource": [{
        "id": "Mr",
        "name": "Mr"
      }, {
        "id": "Mrs",
        "name": "Mrs"
      }, {
        "id": "Ms",
        "name": "Ms"
      }]
    },
    "birthdatea1": {
      "mandatory": 1,
      "type": "datetime",
      "example": "1990-01-01",
      "FieldText": "Birth Date",
      "category": "adult1"
    },
    "passportnationalitya1": {
      "mandatory": 1,
      "type": "combobox",
      "example": "id",
      "FieldText": "Nationality",
      "category": "adult1",
      "resource": "http:\/\/api.tiket.com\/general_api\/listCountry"
    }
  },
  "departures": {
    "flight_id": "16825942",
    "airlines_name": "CITILINK",
    "flight_number": "QG-850",
    "price_value": "1362800.00",
    "count_adult": "1",
    "count_child": "0",
    "count_infant": "0",
    "timestamp": "2014-05-13 11:06:21",
    "price_adult": "1362800.00",
    "price_child": "0.00",
    "price_infant": "0.00",
    "simple_departure_time": "07:40",
    "simple_arrival_time": "10:25",
    "stop": "Nonstop",
    "long_via": "",
    "full_via": "CGK - DPS (07:40 - 10:25)",
    "need_baggage": 0,
    "duration": "1 h 45 m",
    "image": "http:\/\/www.tiket.com\/images\/tiket2\/icon_citilink_2.jpg",
    "flight_infos": {
      "flight_info": [{
        "flight_number": "QG-850",
        "departure_city": "CGK",
        "arrival_city": "DPS",
        "simple_departure_time": "",
        "simple_arrival_time": ""
      }]
    }
  },
  "login_status": "false",
  "token": "2b2f462814af7c0d2e1b40f28e2d9dff5e900f24"
}
```

After search, call this function when user choose the flight to ensure that the data is up to date. 

<aside class="warning">By calling this API, you will hit the airlines API directly. Use this sparingly. Do not abuse!</aside>

#### HTTP Request

`GET https://api-sandbox.tiket.com/flight_api/get_flight_data?flight_id=2490731&token=f9b29ac359ca5d77755e7588751c089bf96f0dc9&output=xml`

#### Parameters

Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------
flight_id |  flight_id want to order  |  CHAR |  | TRUE 
ret_flight_id |  ret_flight_id want to order for return flight  |  CHAR |  | TRUE/FALSE  
ret_date |  return date want to travel  |  CHAR |  | TRUE  
token |   |  CHAR |  | TRUE  


This function contains response that is **required** for the next api call `Flight Add Order`. Please ensure that every field in the required field is sent when adding order

    
    
## Add Order


```xml
<tiket>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.0447</elapsetime>
    <memoryusage>4.16MB</memoryusage>
    <unix_timestamp>1401938205</unix_timestamp>
    <confirm>success</confirm>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <output_type>xml</output_type>
  <login_status>false</login_status>
  <token>3fe6e7cd89ec0df92f102d0e12c19536972e2aa5</token>
</tiket>
```


```json
{
"diagnostic": {
  "status": 200,
  "elapsetime": "0.0449",
  "memoryusage": "4.15MB",
  "unix_timestamp": 1401938247,
  "confirm": "success",
  "lang": "id",
  "currency": "IDR"
},
"output_type": "json",
"login_status": "false",
"token": "55b2746a9c8393822d58eae15f4bc92aedbda089"
}
```



```matlab
a: 4: {
s: 10: "diagnostic";a: 7: {
  s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.0595";s: 11: "memoryusage";s: 14: "4.15MB";s: 14: "unix_timestamp";i: 1401938329;s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "id";s: 8: "currency";s: 3: "IDR";
}
s: 11: "output_type";s: 9: "serialize";s: 12: "login_status";s: 5: "false";s: 5: "token";s: 40: "bec1f8aa40aabbfeb32e0f3576a2b7fdf533505e";
}
```

Attention!  
- we hope the data that was use for testing is not an random word, use data that seems real  
true : susi , budi ext  
wrong : abcs, dsgeg, ext  
- dont book flight with same rute and same passengers data over and over again in adjacent time  
- the requirement field for add order may vary from one airlines to another, please check the variables in Get Flight Data API (one step behind)

Maximal passenger per book:  
Maximal passenger Adult : 6  
Maximal passenger Child : 6  
Maximal passenger infant : 6

#### HTTP Request

     `GET https://api-sandbox.tiket.com/order/add/flight?token=4a5ef3fb7627b9f2900f1aafa46b0f9f095f6aaf&flight_id=20203327&child=1&adult=1&infant=1&conSalutation=Mrs&conFirstName=budianto&conLastName=wijaya&conPhone=%2B6287880182218&conEmailAddress=you_julin@yahoo.com&firstnamea1=susi&lastnamea1=wijaya&ida1=1116057107900001&titlea1=Mr&conOtherPhone=%2B628521342534&titlec1=Ms&firstnamec1=carreen&lastnamec1=athalia&birthdatec1=2005-02-02&titlei1=Mr&parenti1=1&firstnamei1=wendy&lastnamei1=suprato&birthdatei1=2011-06-29&output=XML`

#### Parameters
 
Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------
token | for saving transaction that done by user | CHAR(128) |  | TRUE  
flight_id | flight id that choosen by user | CHAR(~) |  | TRUE  
ret_flight_id | return flight id that choosen by user | CHAR(~) |  | TRUE  
lioncaptcha | lioncaptcha that user input if order lion airines and function get captcha didn't return empty value | CHAR(~) |  | TRUE/FALSE  
lionsessionid | captcha session id that show to user if order lion airines and function get captcha didn't return empty value | CHAR(~) |  | TRUE/FALSE  
child | number of child passenger | INT | 0 | FALSE  
adult | number of adult passenger | INT | 1 | FALSE  
conSalutation | contact person title ( ex: Mr., Mrs., Ms.) | CHAR(5) |  | TRUE  
conFirstName | contact person first name | CHAR(50) |  | TRUE  
conLastName | contact person last name | CHAR(50) |  | TRUE  
conPhone | contact person phone , ex: 081232323343 or +62324324234234. Don't forget to urlencode + into %2B in the GET parameter | CHAR(20) |  | TRUE  
conEmailAddress | contact person email address | CHAR(50) |  | TRUE  
firstnamea1 | as an array like firstnamea1 firstnamea2 if you have adult passager | CHAR(50) |  | TRUE  
lastnamea1 | as an array like lastnamea1 lastnamea2 if you have adult passager | CHAR(50) |  | TRUE  
birthdatea1 | as an array like birthdatea1 , birthdatea2 if you have adult passenger : format YYYY-MM-DD. **Mandatory for v=2 and above** | DATE |  | FALSE/TRUE  
ida1 | as an array like ida1,  ida2 if you have adult passager | CHAR(50) |  | TRUE  
titlea1 | as an array like titlea1, titlea2 if you have adult passager : Mr., Ms., Mrs. | CHAR(5) |  | TRUE  
conOtherPhone | Other contact person phone, ex: 081232323343 or +62324324234234. Don't forget to urlencode + into %2B in the GET parameter | CHAR(20) |  | FALSE  
titlec1 | as an array like titlec1, titlec2 if you have child passager : Mstr., Miss. | CHAR(5) |  | TRUE  
firstnamec1 | as an array like firstnamec1, firstnamec2 if you have child passager | CHAR(50) |  | TRUE  
lastnamec1 | as an array like lastnamec1, lastnamec2 if you have child passager | CHAR(50) |  | TRUE  
birthdatec1 | as an array like birthdatec1, birthdatec2 if you have Child passager : format YYYY-MM-DD | DATE |  | TRUE  
idc1 | as an array like idc1, idc2 if you have child passager | CHAR(50) |  | FALSE  
titlei1 | as an array like titlei1, titlei2 if you have infant passager : Mstr., Miss. | CHAR(5) |  | TRUE  
parenti1 | as an array like parenti1, parenti2 if you have infant passager (total infant ≤ total adult). Ex : 1 (adult 1 as parent of infant),  2 (adult 2 as parent of infant) | INT | 1 | TRUE  
firstnamei1 | as an array like firstnamei1, firstnamei2 if you have infant passager | CHAR(50) |  | TRUE  
lastnamei1 | as an array like lastnamei1, lastnamei2 if you have infant passager | CHAR(50) |  | TRUE  
birthdatei1 | as an array like birthdatei1, birthdatei2 if you have infant passager : format YYYY-MM-DD | DATE |  | TRUE  
idi1 | as an array like idi1, idi2 if you have child passager | CHAR(50) |  | FALSE  


#### Additional Fields According to Airlines

Each Airlines has its specific required fields, you can use the Get Flight Data function to checks the required field.  
This is the list of field to may appears



Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------
passportnoa1 | as an array like passportnoa1, passportnoa2 if you have adult passenger | CHAR(50) |  | TRUE  
passportExpiryDatea1 | as an array like passportExpiryDatea1, passportExpiryDatea2 if you have adult passenger : format YYYY-MM-DD | DATE |  | TRUE  
passportissueddatea1 | as an array like passportissueddatea1, passportissueddatea2 if you have adult passenger : format YYYY-MM-DD | DATE |  | TRUE  
birthdatea1 | as an array like birthdatea1, birthdatea2 if you have adult passenger : format YYYY-MM-DD | DATE |  | TRUE  
passportissuinga1 | as an array like passportissuinga1, passportissuinga2 if you have adult passenger (select from list country ex id for indonesia) | CHAR(50) |  | TRUE  
passportnationalitya1 | as an array like passportnationalitya1, passportnationalitya2 if you have adult passenger (select from list country ex id for indonesia) | CHAR(50) |  | TRUE



#### Additonal Fields For Mandala, Tiger and Airasia Flight

Some airlines may required to submit the baggage fields, here is the example

  
Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------
dcheckinbaggagea11 | departure baggage code for adult passanger as an array like dcheckinbaggagea11, dcheckinbaggagea12 if you have adult passenger and array like dcheckinbaggagea11, dcheckinbaggagea21 if transit flight | CHAR(18) |  | TRUE  
dcheckinbaggagec11 | departure baggage code for child passanger as an array like dcheckinbaggagec11, dcheckinbaggagec12 if you have adult passenge and array like dcheckinbaggagec11,  dcheckinbaggagec21 if transit flight  | CHAR(18) |  | TRUE  
rcheckinbaggagea11 | return baggage code for adult passanger as an array like rcheckinbaggagea11, rcheckinbaggagea12 if you have adult passenger and array like rcheckinbaggagea11,  rcheckinbaggagea21 if transit flight | CHAR(18) |  | TRUE  
rcheckinbaggagec11 | return baggage cod for child passanger as an array like rcheckinbaggagec11, rcheckinbaggagec12 if you have adult passenger and array like rcheckinbaggagec11,  rcheckinbaggagec21 if transit flight | CHAR(18) |  | TRUE


    
    
## Order


```xml
<tiket>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.1170</elapsetime>
    <memoryusage>6.2MB</memoryusage>
    <unix_timestamp>1401938806</unix_timestamp>
    <confirm>success</confirm>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <output_type>xml</output_type>
  <myorder>
    <order_id>20604252</order_id>
    <data>
    <expire>45</expire>
    <uri/>
    <order_detail_id>8092570</order_detail_id>
    <order_type>flight</order_type>
    <customer_price>1086300.00</customer_price>
    <order_name>CGK (Jakarta - Cengkareng) - DPS (Denpasar, Bali)</order_name>
    <order_name_detail>Lion (JT-568 - Depart)</order_name_detail>
    <order_detail_status>active</order_detail_status>
    <detail>
    <order_detail_id>8092570</order_detail_id>
    <airlines_name>Lion</airlines_name>
    <flight_number>JT-568</flight_number>
    <price_adult>1086300.00</price_adult>
    <price_child>0.00</price_child>
    <price_infant>0.00</price_infant>
    <flight_date>25 Jun 2014</flight_date>
    <departure_time>19:00</departure_time>
    <arrival_time>23:00</arrival_time>
    <baggage_fee/>
    <departure_airport_name>Soekarno Hatta</departure_airport_name>
    <arrival_airport_name>Ngurah Rai</arrival_airport_name>
    <passengers>
    <adult>
    <order_passenger_id>3079516</order_passenger_id>
    <order_detail_id>8092570</order_detail_id>
    <type>adult</type>
    <first_name>susi</first_name>
    <last_name>wijaya</last_name>
    <title>Mr</title>
    <id_number>1116057107900001</id_number>
    <birth_date/>
    <adult_index/>
    <passport_no/>
    <passport_expiry/>
    <passport_issuing_country/>
    <passport_nationality/>
    <check_in_baggage/>
    <check_in_baggage_size/>
    <passport_issued_date/>
    <birth_country/>
    </adult>
    </passengers>
    <price>1086300</price>
    <breakdown_price>
    <category>price adult</category>
    <type>none</type>
    <value>1086300</value>
    <currency>IDR</currency>
    <text>Harga Dewasa</text>
    </breakdown_price>
    <breakdown_price>
    <category>total base price</category>
    <type>price</type>
    <value>1086300</value>
    <currency>IDR</currency>
    <text>Harga Total</text>
    </breakdown_price>
    <breakdown_price>
    <category>baggage fee</category>
    <type>add</type>
    <value>0</value>
    <currency>IDR</currency>
    <text>Biaya Bagasi</text>
    </breakdown_price>
    <breakdown_price>
    <category>subsidy</category>
    <type>subtract</type>
    <value>0</value>
    <currency>IDR</currency>
    <text>Subsidi</text>
    </breakdown_price>
    </detail>
    <order_photo>https://api.tiket.com/images/icon_lion.jpg</order_photo>
    <order_icon>h3b</order_icon>
    <tax_and_charge>26985.00</tax_and_charge>
    <subtotal_and_charge>1113285.00</subtotal_and_charge>
    <delete_uri>
    https://api.tiket.com/order/delete_order?order_detail_id=8092570
    </delete_uri>
    </data>
    <total>1113285</total>
    <total_tax>26985</total_tax>
    <total_without_tax>1086300</total_without_tax>
    <count_installment>0</count_installment>
    <discount>
      Dapatkan potongan hingga IDR 26.985,00 saat anda checkout . Tidak berlaku untuk Kartu Kredit.
    </discount>
    <discount_amount>26985.00</discount_amount>
  </myorder>
  <checkout>https://api.tiket.com/order/checkout/20604252/IDR</checkout>
  <login_status>false</login_status>
  <token>4a5ef3fb7627b9f2900f1aafa46b0f9f095f6aaf</token>
</tiket>
```



```json
{
"diagnostic": {
  "status": 200,
  "elapsetime": "0.1562",
  "memoryusage": "6.19MB",
  "unix_timestamp": 1401939129,
  "confirm": "success",
  "lang": "id",
  "currency": "IDR"
},
"output_type": "json",
"myorder": {
  "order_id": "20604252",
  "data": [{
    "expire": 40,
    "uri": null,
    "order_detail_id": "8092570",
    "order_type": "flight",
    "customer_price": "1086300.00",
    "order_name": "CGK (Jakarta - Cengkareng) - DPS (Denpasar, Bali)",
    "order_name_detail": "Lion (JT-568 - Depart)",
    "order_detail_status": "active",
    "detail": {
      "order_detail_id": "8092570",
      "airlines_name": "Lion",
      "flight_number": "JT-568",
      "price_adult": "1086300.00",
      "price_child": "0.00",
      "price_infant": "0.00",
      "flight_date": "25 Jun 2014",
      "departure_time": "19:00",
      "arrival_time": "23:00",
      "baggage_fee": null,
      "departure_airport_name": "Soekarno Hatta",
      "arrival_airport_name": "Ngurah Rai",
      "passengers": {
        "adult": [{
          "order_passenger_id": "3079516",
          "order_detail_id": "8092570",
          "type": "adult",
          "first_name": "susi",
          "last_name": "wijaya",
          "title": "Mr",
          "id_number": "1116057107900001",
          "birth_date": null,
          "adult_index": null,
          "passport_no": null,
          "passport_expiry": null,
          "passport_issuing_country": null,
          "passport_nationality": null,
          "check_in_baggage": null,
          "check_in_baggage_size": null,
          "passport_issued_date": null,
          "birth_country": null
        }]
      },
      "price": 1086300,
      "breakdown_price": [{
        "category": "price adult",
        "type": "none",
        "value": 1086300,
        "currency": "IDR",
        "text": "Harga Dewasa"
      }, {
        "category": "total base price",
        "type": "price",
        "value": 1086300,
        "currency": "IDR",
        "text": "Harga Total"
      }, {
        "category": "baggage fee",
        "type": "add",
        "value": 0,
        "currency": "IDR",
        "text": "Biaya Bagasi"
      }, {
        "category": "subsidy",
        "type": "subtract",
        "value": 0,
        "currency": "IDR",
        "text": "Subsidi"
      }]
    },
    "order_photo": "https:\/\/api.tiket.com\/images\/icon_lion.jpg",
    "order_icon": "h3b",
    "tax_and_charge": "26985.00",
    "subtotal_and_charge": "1113285.00",
    "delete_uri": "https:\/\/api.tiket.com\/order\/delete_order?order_detail_id=8092570"
  }],
  "total": 1113285,
  "total_tax": 26985,
  "total_without_tax": 1086300,
  "count_installment": 0,
  "promo": [],
  "discount": "Dapatkan potongan hingga IDR 26.985,00 saat anda checkout . Tidak berlaku untuk Kartu Kredit.",
  "discount_amount": "26985.00"
},
"checkout": "https:\/\/api.tiket.com\/order\/checkout\/20604252\/IDR",
"login_status": "false",
"token": "4a5ef3fb7627b9f2900f1aafa46b0f9f095f6aaf"
}
```



```matlab
a: 6: {
s: 10: "diagnostic";a: 7: {
  s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.0915";s: 11: "memoryusage";s: 14: "6.19MB";s: 14: "unix_timestamp";i: 1401939144;s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "id";s: 8: "currency";s: 3: "IDR";
}
s: 11: "output_type";s: 9: "serialize";s: 7: "myorder";a: 9: {
  s: 8: "order_id";s: 8: "20604252";s: 4: "data";a: 1: {
    i: 0;a: 14: {
      s: 6: "expire";i: 40;s: 3: "uri";N;s: 15: "order_detail_id";s: 7: "8092570";s: 10: "order_type";s: 6: "flight";s: 14: "customer_price";s: 10: "1086300.00";s: 10: "order_name";s: 49: "CGK (Jakarta - Cengkareng) - DPS (Denpasar, Bali)";s: 17: "order_name_detail";s: 22: "Lion (JT-568 - Depart)";s: 19: "order_detail_status";s: 6: "active";s: 6: "detail";a: 15: {
        s: 15: "order_detail_id";s: 7: "8092570";s: 13: "airlines_name";s: 4: "Lion";s: 13: "flight_number";s: 6: "JT-568";s: 11: "price_adult";s: 10: "1086300.00";s: 11: "price_child";s: 4: "0.00";s: 12: "price_infant";s: 4: "0.00";s: 11: "flight_date";s: 11: "25 Jun 2014";s: 14: "departure_time";s: 5: "19:00";s: 12: "arrival_time";s: 5: "23:00";s: 11: "baggage_fee";N;s: 22: "departure_airport_name";s: 14: "Soekarno Hatta";s: 20: "arrival_airport_name";s: 10: "Ngurah Rai";s: 10: "passengers";a: 1: {
          s: 5: "adult";a: 1: {
            i: 0;a: 17: {
              s: 18: "order_passenger_id";s: 7: "3079516";s: 15: "order_detail_id";s: 7: "8092570";s: 4: "type";s: 5: "adult";s: 10: "first_name";s: 4: "susi";s: 9: "last_name";s: 6: "wijaya";s: 5: "title";s: 2: "Mr";s: 9: "id_number";s: 16: "1116057107900001";s: 10: "birth_date";N;s: 11: "adult_index";N;s: 11: "passport_no";N;s: 15: "passport_expiry";N;s: 24: "passport_issuing_country";N;s: 20: "passport_nationality";N;s: 16: "check_in_baggage";N;s: 21: "check_in_baggage_size";N;s: 20: "passport_issued_date";N;s: 13: "birth_country";N;
            }
          }
        }
        s: 5: "price";d: 1086300;s: 15: "breakdown_price";a: 4: {
          i: 0;a: 5: {
            s: 8: "category";s: 11: "price adult";s: 4: "type";s: 4: "none";s: 5: "value";d: 1086300;s: 8: "currency";s: 3: "IDR";s: 4: "text";s: 29: "Harga Dewasa";
          }
          i: 1;a: 5: {
            s: 8: "category";s: 16: "total base price";s: 4: "type";s: 5: "price";s: 5: "value";d: 1086300;s: 8: "currency";s: 3: "IDR";s: 4: "text";s: 29: "Harga Total";
          }
          i: 2;a: 5: {
            s: 8: "category";s: 11: "baggage fee";s: 4: "type";s: 3: "add";s: 5: "value";i: 0;s: 8: "currency";s: 3: "IDR";s: 4: "text";s: 35: "Biaya Bagasi";
          }
          i: 3;a: 5: {
            s: 8: "category";s: 7: "subsidy";s: 4: "type";s: 8: "subtract";s: 5: "value";d: 0;s: 8: "currency";s: 3: "IDR";s: 4: "text";s: 31: "Subsidi";
          }
        }
      }
      s: 11: "order_photo";s: 42: "https://api.tiket.com/images/icon_lion.jpg";s: 10: "order_icon";s: 3: "h3b";s: 14: "tax_and_charge";s: 8: "26985.00";s: 19: "subtotal_and_charge";s: 10: "1113285.00";s: 10: "delete_uri";s: 64: "https://api.tiket.com/order/delete_order?order_detail_id=8092570";
    }
  }
  s: 5: "total";d: 1113285;s: 9: "total_tax";d: 26985;s: 17: "total_without_tax";d: 1086300;s: 17: "count_installment";i: 0;s: 5: "promo";a: 0: {}
  s: 8: "discount";s: 110: "Dapatkan potongan hingga IDR 26.985,00 saat anda checkout . Tidak berlaku untuk Kartu Kredit.";s: 15: "discount_amount";s: 8: "26985.00";
}
s: 8: "checkout";s: 49: "https://api.tiket.com/order/checkout/20604252/IDR";s: 12: "login_status";s: 5: "false";s: 5: "token";s: 40: "4a5ef3fb7627b9f2900f1aafa46b0f9f095f6aaf";
}
```

#### HTTP Request

    `GET https://api-sandbox.tiket.com/order?token=4a5ef3fb7627b9f2900f1aafa46b0f9f095f6aaf&output=xml`

#### Parameters
  
Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------
token | for saving transaction that done by user | CHAR(128) |  | TRUE  



## Delete Order

```xml
<tiket>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.2537</elapsetime>
    <memoryusage>5.5MB</memoryusage>
    <unix_timestamp>1401939501</unix_timestamp>
    <confirm>success</confirm>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <output_type>xml</output_type>
  <updateStatus>success delete order</updateStatus>
  <login_status>false</login_status>
  <token>4a5ef3fb7627b9f2900f1aafa46b0f9f095f6aaf</token>
</tiket>
```

```json
{
"diagnostic": {
  "error_msgs": "Order failed to delete",
  "status": 201,
  "elapsetime": "0.0557",
  "memoryusage": "4.58MB",
  "unix_timestamp": 1401939653,
  "lang": "id",
  "currency": "IDR"
},
"output_type": "json",
"updateStatus": "failed delete order",
"login_status": "false",
"token": "4a5ef3fb7627b9f2900f1aafa46b0f9f095f6aaf"
}
```

```matlab
a: 5: {
s: 10: "diagnostic";a: 7: {
  s: 10: "error_msgs";s: 22: "Order failed to delete";s: 6: "status";i: 201;s: 10: "elapsetime";s: 14: "0.0465";s: 11: "memoryusage";s: 14: "4.58MB";s: 14: "unix_timestamp";i: 1401939677;s: 4: "lang";s: 2: "id";s: 8: "currency";s: 3: "IDR";
}
s: 11: "output_type";s: 9: "serialize";s: 12: "updateStatus";s: 19: "failed delete order";s: 12: "login_status";s: 5: "false";s: 5: "token";s: 40: "4a5ef3fb7627b9f2900f1aafa46b0f9f095f6aaf";
}
```

link url can be get from order, variable delete_uri

#### HTTP Request

    `GET https://api-sandbox.tiket.com/order/delete_order?order_detail_id=8092570&token=4a5ef3fb7627b9f2900f1aafa46b0f9f095f6aaf&output=xml`

#### Parameters

Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------
order_detail_id | Order detail ID that want to delete from order | NUMBER |  | TRUE  
token | for saving transaction that done by user | CHAR(128) |  | TRUE  


    
## Checkout Page request

```xml
<tiket>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.0807</elapsetime>
    <memoryusage>4.6MB</memoryusage>
    <unix_timestamp>1401943234</unix_timestamp>
    <confirm>success</confirm>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <output_type>xml</output_type>
  <next_checkout_uri>https://api.tiket.com/checkout/checkout_customer</next_checkout_uri>
  <login_status>false</login_status>
  <token>4a5ef3fb7627b9f2900f1aafa46b0f9f095f6aaf</token>
</tiket>
```

```json
{
"diagnostic": {
 "status": 200,
 "elapsetime": "0.0794",
 "memoryusage": "4.59MB",
 "unix_timestamp": 1401943530,
 "confirm": "success",
 "lang": "id",
 "currency": "IDR"
},
"output_type": "json",
"next_checkout_uri": "https:\/\/api.tiket.com\/checkout\/checkout_customer",
"login_status": "false",
"token": "4a5ef3fb7627b9f2900f1aafa46b0f9f095f6aaf"
}
```

```matlab
a: 5: {
s: 10: "diagnostic";a: 7: {
  s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.0639";s: 11: "memoryusage";s: 14: "4.59MB";s: 14: "unix_timestamp";i: 1401943547;s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "id";s: 8: "currency";s: 3: "IDR";
}
s: 11: "output_type";s: 9: "serialize";s: 17: "next_checkout_uri";s: 48: "https://api.tiket.com/checkout/checkout_customer";s: 12: "login_status";s: 5: "false";s: 5: "token";s: 40: "4a5ef3fb7627b9f2900f1aafa46b0f9f095f6aaf";
}
``` 

Early stage to access checkout.

link url can be get from order, variable checkout.

#### HTTP Request

     `GET https://api-sandbox.tiket.com/order/checkout/20604252/IDR?token=4a5ef3fb7627b9f2900f1aafa46b0f9f095f6aaf`

Get from order page in checkout variable.

#### Parameters

  
Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------
token | for saving transaction that done by user | CHAR(128) |  | TRUE  



    
## Checkout Login - Checkout Costumer

```xml
<tiket>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.0897</elapsetime>
    <memoryusage>5.01MB</memoryusage>
    <unix_timestamp>1401959766</unix_timestamp>
    <confirm>success</confirm>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <output_type>xml</output_type>
  <user_account>
    <username>fatmamiharja@gmail.com</username>
  </user_account>
  <login_status>true</login_status>
  <guest_id>167023</guest_id>
  <login_email>fatmamiharja@gmail.com</login_email>
  <token>4a5ef3fb7627b9f2900f1aafa46b0f9f095f6aaf</token>
</tiket>
```



```json
{
"diagnostic": {
  "status": 200,
  "elapsetime": "0.1441",
  "memoryusage": "5MB",
  "unix_timestamp": 1401959843,
  "confirm": "success",
  "lang": "id",
  "currency": "IDR"
},
"output_type": "json",
"user_account": {
  "username": "fatmamiharja@gmail.com"
},
"login_status": "true",
"guest_id": "167023",
"login_email": "fatmamiharja@gmail.com",
"token": "4a5ef3fb7627b9f2900f1aafa46b0f9f095f6aaf"
}
```

```matlab
a: 6: {
s: 10: "diagnostic";a: 7: {
  s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.0946";s: 11: "memoryusage";s: 14: "5MB";s: 14: "unix_timestamp";i: 1401959859;s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "id";s: 8: "currency";s: 3: "IDR";
}
s: 11: "output_type";s: 9: "serialize";s: 12: "user_account";a: 1: {
  s: 8: "username";s: 22: "fatmamiharja@gmail.com";
}
s: 12: "login_status";s: 4: "true";s: 8: "guest_id";s: 6: "167023";s: 11: "login_email";s: 22: "fatmamiharja@gmail.com";s: 5: "token";s: 40: "4a5ef3fb7627b9f2900f1aafa46b0f9f095f6aaf";
}
```  

#### HTTP Request

     `GET https://api-sandbox.tiket.com/checkout/checkout_customer?token=4a5ef3fb7627b9f2900f1aafa46b0f9f095f6aaf&salutation=Ms&firstName=ba&lastName=ca&emailAddress=fatmamiharja@gmail.com&phone=%2B62878434343&saveContinue=2`

Setelah merequest link tersebut maka user akan dibuatkan account di tiket.com  
user akan dikirimkan email untuk mengubah password loginnya.

#### Parameters
  
Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------
salutation | "your title( ex: Mr. | Mrs. | Ms.)" | CHAR(5) |  | TRUE  
firstName | your first name | CHAR(50) |  | TRUE  
lastName | your last name | CHAR(50) |  | TRUE  
emailAddress | your email | CHAR(50) |  | TRUE  
phone | "your phone |  ex: 081232323343 or +62324324234234. Don't forget to urlencode + into %2B in the GET parameter" | CHAR(20) |  | TRUE  
saveContinue | "Flag for save unregistered user data (value=2)" |  |  | TRUE  



    
## Available Payment

```xml
<?xml version="1.0" encoding="utf-8"?>
<tiket>
    <diagnostic>
        <status>200</status>
        <elapsetime>15.3215</elapsetime>
        <memoryusage>7.99MB</memoryusage>
        <unix_timestamp>1470297049</unix_timestamp>
        <confirm>success</confirm>
        <lang>id</lang>
        <currency>IDR</currency>
    </diagnostic>
    <output_type>xml</output_type>
    <available_payment>
        <link>http://sandbox.tiket.com/payment/checkout_payment?payment_type=1</link>
        <text>Kartu Kredit</text>
        <message></message>
        <type>creditcard</type>
    </available_payment>
    <available_payment>
        <link>https://api-sandbox.tiket.com/checkout/checkout_payment/35</link>
        <text>ATM Transfer</text>
        <message></message>
        <type>jatis</type>
    </available_payment>
    <available_payment>
        <link>http://sandbox.tiket.com/payment/checkout_payment?payment_type=31</link>
        <text>CIMB Clicks</text>
        <message></message>
        <type>cimbclicks</type>
    </available_payment>
    <available_payment>
        <link>https://api-sandbox.tiket.com/checkout/checkout_payment/3</link>
        <text>KlikBCA</text>
        <message></message>
        <type>klikbca</type>
    </available_payment>
    <available_payment>
        <link>https://api-sandbox.tiket.com/checkout/checkout_payment/39</link>
        <text>ATM BCA</text>
        <message></message>
        <type>rintis</type>
    </available_payment>
    <available_payment>
        <link>https://api-sandbox.tiket.com/checkout/checkout_payment/34</link>
        <text>Mandiri Clickpay</text>
        <message>Butuh No. Kartu dan Token</message>
        <type>mandiri_clickpay</type>
    </available_payment>
    <available_payment>
        <link>#</link>
        <text>Transfer Online and M-Banking</text>
        <message>Metode pembayaran ini sementara tidak tersedia atau sedang mengalami gangguan</message>
        <type>banktransfer</type>
    </available_payment>
    <available_payment>
        <link>http://sandbox.tiket.com/payment/checkout_payment?payment_type=33</link>
        <text>ePay BRI</text>
        <message></message>
        <type>epaybri</type>
    </available_payment>
    <available_payment>
        <link>http://sandbox.tiket.com/payment/checkout_payment?payment_type=4</link>
        <text>BCA KlikPay</text>
        <message></message>
        <type>klikpay</type>
    </available_payment>
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
    "elapsetime": "15.3177",
    "memoryusage": "7.98MB",
    "unix_timestamp": 1470297169,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "available_payment": [
    {
      "link": "http://sandbox.tiket.com/payment/checkout_payment?payment_type=1",
      "text": "Kartu Kredit",
      "message": "",
      "type": "creditcard"
    },
    {
      "link": "https://api-sandbox.tiket.com/checkout/checkout_payment/35",
      "text": "ATM Transfer",
      "message": "",
      "type": "jatis"
    },
    {
      "link": "http://sandbox.tiket.com/payment/checkout_payment?payment_type=31",
      "text": "CIMB Clicks",
      "message": "",
      "type": "cimbclicks"
    },
    {
      "link": "https://api-sandbox.tiket.com/checkout/checkout_payment/3",
      "text": "KlikBCA",
      "message": "",
      "type": "klikbca"
    },
    {
      "link": "https://api-sandbox.tiket.com/checkout/checkout_payment/39",
      "text": "ATM BCA",
      "message": "",
      "type": "rintis"
    },
    {
      "link": "https://api-sandbox.tiket.com/checkout/checkout_payment/34",
      "text": "Mandiri Clickpay",
      "message": "Butuh No. Kartu dan Token",
      "type": "mandiri_clickpay"
    },
    {
      "link": "#",
      "text": "Transfer Online and M-Banking",
      "message": "Metode pembayaran ini sementara tidak tersedia atau sedang mengalami gangguan",
      "type": "banktransfer"
    },
    {
      "link": "http://sandbox.tiket.com/payment/checkout_payment?payment_type=33",
      "text": "ePay BRI",
      "message": "",
      "type": "epaybri"
    },
    {
      "link": "http://sandbox.tiket.com/payment/checkout_payment?payment_type=4",
      "text": "BCA KlikPay",
      "message": "",
      "type": "klikpay"
    }
  ],
  "login_status": "true",
  "guest_id": "22691145",
  "login_email": "wida.skydev@gmail.com",
  "token": "f9b29ac359ca5d77755e7588751c089bf96f0dc9"
}
```

```matlab
a:7:{s:10:"diagnostic";a:7:{s:6:"status";i:200;s:10:"elapsetime";s:14:"15.3094";s:11:"memoryusage";s:14:"7.98MB";s:14:"unix_timestamp";i:1470297257;s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:11:"output_type";s:9:"serialize";s:17:"available_payment";a:9:{i:0;a:4:{s:4:"link";s:64:"http://sandbox.tiket.com/payment/checkout_payment?payment_type=1";s:4:"text";s:22:"Kartu Kredit";s:7:"message";s:0:"";s:4:"type";s:10:"creditcard";}i:1;a:4:{s:4:"link";s:58:"https://api-sandbox.tiket.com/checkout/checkout_payment/35";s:4:"text";s:12:"ATM Transfer";s:7:"message";s:0:"";s:4:"type";s:5:"jatis";}i:2;a:4:{s:4:"link";s:65:"http://sandbox.tiket.com/payment/checkout_payment?payment_type=31";s:4:"text";s:11:"CIMB Clicks";s:7:"message";s:0:"";s:4:"type";s:10:"cimbclicks";}i:3;a:4:{s:4:"link";s:57:"https://api-sandbox.tiket.com/checkout/checkout_payment/3";s:4:"text";s:7:"KlikBCA";s:7:"message";s:0:"";s:4:"type";s:7:"klikbca";}i:4;a:4:{s:4:"link";s:58:"https://api-sandbox.tiket.com/checkout/checkout_payment/39";s:4:"text";s:7:"ATM BCA";s:7:"message";s:0:"";s:4:"type";s:6:"rintis";}i:5;a:4:{s:4:"link";s:58:"https://api-sandbox.tiket.com/checkout/checkout_payment/34";s:4:"text";s:16:"Mandiri Clickpay";s:7:"message";s:39:"Butuh No. Kartu dan Token";s:4:"type";s:16:"mandiri_clickpay";}i:6;a:4:{s:4:"link";s:1:"#";s:4:"text";s:24:"Transfer Online and M-Banking";s:7:"message";s:29:"Metode pembayaran ini sementara tidak tersedia atau sedang mengalami gangguan";s:4:"type";s:12:"banktransfer";}i:7;a:4:{s:4:"link";s:65:"http://sandbox.tiket.com/payment/checkout_payment?payment_type=33";s:4:"text";s:8:"ePay BRI";s:7:"message";s:0:"";s:4:"type";s:7:"epaybri";}i:8;a:4:{s:4:"link";s:64:"http://sandbox.tiket.com/payment/checkout_payment?payment_type=4";s:4:"text";s:11:"BCA KlikPay";s:7:"message";s:0:"";s:4:"type";s:7:"klikpay";}}s:12:"login_status";s:4:"true";s:8:"guest_id";s:8:"22691145";s:11:"login_email";s:21:"wida.skydev@gmail.com";s:5:"token";s:40:"f9b29ac359ca5d77755e7588751c089bf96f0dc9";}
```
    
#### HTTP Request

   `GET http://api-sandbox.tiket.com/checkout/checkout_payment?token=87da88eaaa429d5513a3a3658b01701e`

#### Parameters
 
Name | Description | Format | Default | Mandatory  
---- | ----------  | -----  | ------- | ---------
token | for saving transaction that done by user | CHAR(128) |  | TRUE  



    
## Checkout Payment

Please see [Checkout Payment](http://docs.tiket.com/#checkout-payment-309) in General API