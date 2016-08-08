# Train API

NOTE :  
*Data that is provided for testing is different from the actual  
*UPDATE for INFANT passenger, LIVE. Please all developers to update the application

These are the API command for Train.

Diagram flow for Train API:  

![Train API](https://raw.githubusercontent.com/tiket-dev/slate/master/source/images/Flow-Train.png)

WARNING:  
Khusus untuk penggunaan API kereta api, berikut syarat yang harus dipenuhi:  
1. Membuat surat permohonan kerjasama ke Tiket.com  
2. Membuat surat pernyataan untuk PT KAI bahwa Anda adalah partner Tiket.com  
3. Membuat proposal untuk Tiket.com yang berisi:  
- Introduction mengenai perusahaan beserta portofolio  
- Rencana pengembangan (timeline dari planning, analysis, design, dan implemetation)  
- Mockup user interfaces  
- Strategi pemasaran yang akan dilakukan ketika launching

***Note* : Hanya proposal yang lolos dari pihak manajemen yang akan kami kirimkan proposalnya ke PT KAI. Dan untuk proses live module Train juga membutuhkan UAT (testing) dan persetujuan dari pihak KAI yang bisa memakan waktu 3-24 bulan.**

Download surat pemberitahuan  

[Permohonan Kerjasama ke Tiket.com](http://docs.tiket.com/wp-content/uploads/2012/07/Permohonan-Kerjasama-ke-Tiket.com-1.docx)  

[Surat_UAT_Kereta Api](http://docs.tiket.com/wp-content/uploads/2012/07/Surat_UAT_Kereta-Api.docx)


## Search Train

```xml
<?xml version="1.0" encoding="utf-8"?>
<tiket>
    <diagnostic>
        <status>200</status>
        <elapsetime>0.1478</elapsetime>
        <memoryusage>7.01MB</memoryusage>
        <unix_timestamp>1470629053</unix_timestamp>
        <confirm>success</confirm>
        <lang>id</lang>
        <currency>IDR</currency>
    </diagnostic>
    <output_type>xml</output_type>
    <search_queries>
        <dep_station>GMR</dep_station>
        <arr_station>BD</arr_station>
        <date>2016-09-03</date>
        <train_class>all</train_class>
        <count_adult>1</count_adult>
        <count_child>0</count_child>
        <count_infant>0</count_infant>
        <dep_city>Gambir, Jakarta Pusat</dep_city>
        <arr_city>Bandung, Bandung</arr_city>
    </search_queries>
    <departures>
        <result>
            <id>8314369</id>
            <detail_availability>10</detail_availability>
            <train_id>A32</train_id>
            <train_name>Tiket.com Kuda Kencana</train_name>
            <departure_station>GMR</departure_station>
            <departure_time>05:30</departure_time>
            <departure_timestamp>1472855400</departure_timestamp>
            <arrival_station>BD</arrival_station>
            <arrival_time>11:34</arrival_time>
            <arrival_timestamp>1472877240</arrival_timestamp>
            <class_name>eko</class_name>
            <class_name_lang>Ekonomi</class_name_lang>
            <detail_class_name>ekonomi</detail_class_name>
            <subclass_name>P</subclass_name>
            <is_promo>0</is_promo>
            <timestamp>2016-08-08 10:52:40</timestamp>
            <time_diff>
                <is_next_day></is_next_day>
                <diff_hour>6</diff_hour>
                <diff_minute>4</diff_minute>
            </time_diff>
            <can_be_shown>1</can_be_shown>
            <is_closing></is_closing>
            <formatted_schedule_date>Sab, 03 Sep 2016</formatted_schedule_date>
            <price_adult_clean>150000</price_adult_clean>
            <price_adult>150000.00</price_adult>
            <price_child_clean>150000</price_child_clean>
            <price_child>150000.00</price_child>
            <price_infant_clean>0</price_infant_clean>
            <price_infant>0.00</price_infant>
            <price_total_clean>150000</price_total_clean>
            <price_total>IDR 150.000</price_total>
            <selected_schedule>1</selected_schedule>
            <duration>6 j 4 m</duration>
        </result>
    </departures>
</tiket>
```

```json
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.1770",
    "memoryusage": "7MB",
    "unix_timestamp": 1470628869,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "search_queries": {
    "dep_station": "GMR",
    "arr_station": "BD",
    "date": "2016-09-03",
    "train_class": "all",
    "count_adult": 1,
    "count_child": 0,
    "count_infant": 0,
    "dep_city": "Gambir, Jakarta Pusat",
    "arr_city": "Bandung, Bandung",
    "return_date": "2016-09-09"
  },
  "departures": {
    "result": [
      {
        "id": "8314369",
        "detail_availability": "10",
        "train_id": "A32",
        "train_name": "Tiket.com Kuda Kencana",
        "departure_station": "GMR",
        "departure_time": "05:30",
        "departure_timestamp": 1472855400,
        "arrival_station": "BD",
        "arrival_time": "11:34",
        "arrival_timestamp": 1472877240,
        "class_name": "eko",
        "class_name_lang": "Ekonomi",
        "detail_class_name": "ekonomi",
        "subclass_name": "P",
        "is_promo": "0",
        "timestamp": "2016-08-08 10:52:40",
        "time_diff": {
          "is_next_day": false,
          "diff_hour": 6,
          "diff_minute": 4
        }
      }
    ]
  }
  "login_status": "true",
  "guest_id": "22691145",
  "login_email": "wida.skydev@gmail.com",
  "token": "f9b29ac359ca5d77755e7588751c089bf96f0dc9"
}
```

```matlab
a:8:{s:10:"diagnostic";a:7:{s:6:"status";i:200;s:10:"elapsetime";s:14:"0.1567";s:11:"memoryusage";s:14:"7MB";s:14:"unix_timestamp";i:1470629121;s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:11:"output_type";s:9:"serialize";s:14:"search_queries";a:9:{s:11:"dep_station";s:3:"GMR";s:11:"arr_station";s:2:"BD";s:4:"date";s:10:"2016-09-03";s:11:"train_class";s:3:"all";s:11:"count_adult";i:1;s:11:"count_child";i:0;s:12:"count_infant";i:0;s:8:"dep_city";s:21:"Gambir, Jakarta Pusat";s:8:"arr_city";s:16:"Bandung, Bandung";}s:10:"departures";a:1:{s:6:"result";a:18:{i:0;a:30:{s:2:"id";s:7:"8314369";s:19:"detail_availability";s:2:"10";s:8:"train_id";s:3:"A32";s:10:"train_name";s:22:"Tiket.com Kuda Kencana";s:17:"departure_station";s:3:"GMR";s:14:"departure_time";s:5:"05:30";s:19:"departure_timestamp";i:1472855400;s:15:"arrival_station";s:2:"BD";s:12:"arrival_time";s:5:"11:34";s:17:"arrival_timestamp";i:1472877240;s:10:"class_name";s:3:"eko";s:15:"class_name_lang";s:15:"Ekonomi";s:17:"detail_class_name";s:7:"ekonomi";s:13:"subclass_name";s:1:"P";s:8:"is_promo";s:1:"0";s:9:"timestamp";s:19:"2016-08-08 10:52:40";s:9:"time_diff";a:3:{s:11:"is_next_day";b:0;s:9:"diff_hour";i:6;s:11:"diff_minute";i:4;}s:12:"can_be_shown";b:1;s:10:"is_closing";b:0;s:23:"formatted_schedule_date";s:16:"Sab, 03 Sep 2016";s:17:"price_adult_clean";i:150000;s:11:"price_adult";s:9:"150000.00";s:17:"price_child_clean";i:150000;s:11:"price_child";s:9:"150000.00";s:18:"price_infant_clean";i:0;s:12:"price_infant";s:4:"0.00";s:17:"price_total_clean";i:150000;s:11:"price_total";s:11:"IDR 150.000";s:17:"selected_schedule";b:1;s:8:"duration";s:23:"6 j 4 m";}i:1;a:30:{s:2:"id";s:7:"8314363";s:19:"detail_availability";s:2:"77";s:8:"train_id";s:3:"A32";s:10:"train_name";s:22:"Tiket.com Kuda Kencana";s:17:"departure_station";s:3:"GMR";s:14:"departure_time";s:5:"05:30";s:19:"departure_timestamp";i:1472855400;s:15:"arrival_station";s:2:"BD";s:12:"arrival_time";s:5:"11:34";s:17:"arrival_timestamp";i:1472877240;s:10:"class_name";s:3:"eks";s:15:"class_name_lang";s:17:"Eksekutif";s:17:"detail_class_name";s:9:"eksekutif";s:13:"subclass_name";s:1:"A";s:8:"is_promo";s:1:"0";s:9:"timestamp";s:19:"2016-08-08 10:52:40";s:9:"time_diff";a:3:{s:11:"is_next_day";b:0;s:9:"diff_hour";i:6;s:11:"diff_minute";i:4;}s:12:"can_be_shown";b:1;s:10:"is_closing";b:0;s:23:"formatted_schedule_date";s:16:"Sab, 03 Sep 2016";s:17:"price_adult_clean";i:275000;s:11:"price_adult";s:9:"275000.00";s:17:"price_child_clean";i:275000;s:11:"price_child";s:9:"275000.00";s:18:"price_infant_clean";i:0;s:12:"price_infant";s:4:"0.00";s:17:"price_total_clean";i:275000;s:11:"price_total";s:11:"IDR 275.000";s:17:"selected_schedule";b:0;s:8:"duration";s:23:"6 j 4 m";}i:2;a:30:{s:2:"id";s:7:"8314367";s:19:"detail_availability";s:2:"20";s:8:"train_id";s:3:"A32";s:10:"train_name";s:22:"Tiket.com Kuda Kencana";s:17:"departure_station";s:3:"GMR";s:14:"departure_time";s:5:"05:30";s:19:"departure_timestamp";i:1472855400;s:15:"arrival_station";s:2:"BD";s:12:"arrival_time";s:5:"11:34";s:17:"arrival_timestamp";i:1472877240;s:10:"class_name";s:3:"bis";s:15:"class_name_lang";s:16:"Bisnis";s:17:"detail_class_name";s:6:"bisnis";s:13:"subclass_name";s:1:"M";s:8:"is_promo";s:1:"0";s:9:"timestamp";s:19:"2016-08-08 10:52:40";s:9:"time_diff";a:3:{s:11:"is_next_day";b:0;s:9:"diff_hour";i:6;s:11:"diff_minute";i:4;}s:12:"can_be_shown";b:1;s:10:"is_closing";b:0;s:23:"formatted_schedule_date";s:16:"Sab, 03 Sep 2016";s:17:"price_adult_clean";i:200000;s:11:"price_adult";s:9:"200000.00";s:17:"price_child_clean";i:200000;s:11:"price_child";s:9:"200000.00";s:18:"price_infant_clean";i:0;s:12:"price_infant";s:4:"0.00";s:17:"price_total_clean";i:200000;s:11:"price_total";s:11:"IDR 200.000";s:17:"selected_schedule";b:0;s:8:"duration";s:23:"6 j 4 m";}i:3;a:30:{s:2:"id";s:7:"8314371";s:19:"detail_availability";s:2:"77";s:8:"train_id";s:1:"8";s:10:"train_name";s:24:"Tiket.com Selancar Angin";s:17:"departure_station";s:3:"GMR";s:14:"departure_time";s:5:"11:58";s:19:"departure_timestamp";i:1472878680;s:15:"arrival_station";s:2:"BD";s:12:"arrival_time";s:5:"17:58";s:17:"arrival_timestamp";i:1472900280;s:10:"class_name";s:3:"eks";s:15:"class_name_lang";s:17:"Eksekutif";s:17:"detail_class_name";s:9:"eksekutif";s:13:"subclass_name";s:1:"A";s:8:"is_promo";s:1:"0";s:9:"timestamp";s:19:"2016-08-08 10:52:40";s:9:"time_diff";a:3:{s:11:"is_next_day";b:0;s:9:"diff_hour";i:6;s:11:"diff_minute";i:0;}s:12:"can_be_shown";b:1;s:10:"is_closing";b:0;s:23:"formatted_schedule_date";s:16:"Sab, 03 Sep 2016";s:17:"price_adult_clean";i:275000;s:11:"price_adult";s:9:"275000.00";s:17:"price_child_clean";i:275000;s:11:"price_child";s:9:"275000.00";s:18:"price_infant_clean";i:0;s:12:"price_infant";s:4:"0.00";s:17:"price_total_clean";i:275000;s:11:"price_total";s:11:"IDR 275.000";s:17:"selected_schedule";b:0;s:8:"duration";s:23:"6 j 0 m";}i:4;a:30:{s:2:"id";s:7:"8314375";s:19:"detail_availability";s:2:"20";s:8:"train_id";s:1:"8";s:10:"train_name";s:24:"Tiket.com Selancar Angin";s:17:"departure_station";s:3:"GMR";s:14:"departure_time";s:5:"11:58";s:19:"departure_timestamp";i:1472878680;s:15:"arrival_station";s:2:"BD";s:12:"arrival_time";s:5:"17:58";s:17:"arrival_timestamp";i:1472900280;s:10:"class_name";s:3:"bis";s:15:"class_name_lang";s:16:"Bisnis";s:17:"detail_class_name";s:6:"bisnis";s:13:"subclass_name";s:1:"M";s:8:"is_promo";s:1:"0";s:9:"timestamp";s:19:"2016-08-08 10:52:40";s:9:"time_diff";a:3:{s:11:"is_next_day";b:0;s:9:"diff_hour";i:6;s:11:"diff_minute";i:0;}s:12:"can_be_shown";b:1;s:10:"is_closing";b:0;s:23:"formatted_schedule_date";s:16:"Sab, 03 Sep 2016";s:17:"price_adult_clean";i:200000;s:11:"price_adult";s:9:"200000.00";s:17:"price_child_clean";i:200000;s:11:"price_child";s:9:"200000.00";s:18:"price_infant_clean";i:0;s:12:"price_infant";s:4:"0.00";s:17:"price_total_clean";i:200000;s:11:"price_total";s:11:"IDR 200.000";s:17:"selected_schedule";b:0;s:8:"duration";s:23:"6 j 0 m";}i:5;a:30:{s:2:"id";s:7:"8314377";s:19:"detail_availability";s:2:"10";s:8:"train_id";s:1:"8";s:10:"train_name";s:24:"Tiket.com Selancar Angin";s:17:"departure_station";s:3:"GMR";s:14:"departure_time";s:5:"11:58";s:19:"departure_timestamp";i:1472878680;s:15:"arrival_station";s:2:"BD";s:12:"arrival_time";s:5:"17:58";s:17:"arrival_timestamp";i:1472900280;s:10:"class_name";s:3:"eko";s:15:"class_name_lang";s:15:"Ekonomi";s:17:"detail_class_name";s:7:"ekonomi";s:13:"subclass_name";s:1:"P";s:8:"is_promo";s:1:"0";s:9:"timestamp";s:19:"2016-08-08 10:52:40";s:9:"time_diff";a:3:{s:11:"is_next_day";b:0;s:9:"diff_hour";i:6;s:11:"diff_minute";i:0;}s:12:"can_be_shown";b:1;s:10:"is_closing";b:0;s:23:"formatted_schedule_date";s:16:"Sab, 03 Sep 2016";s:17:"price_adult_clean";i:150000;s:11:"price_adult";s:9:"150000.00";s:17:"price_child_clean";i:150000;s:11:"price_child";s:9:"150000.00";s:18:"price_infant_clean";i:0;s:12:"price_infant";s:4:"0.00";s:17:"price_total_clean";i:150000;s:11:"price_total";s:11:"IDR 150.000";s:17:"selected_schedule";b:0;s:8:"duration";s:23:"6 j 0 m";}i:6;a:30:{s:2:"id";s:7:"8314379";s:19:"detail_availability";s:2:"77";s:8:"train_id";s:4:"8890";s:10:"train_name";s:20:"Tiket.com Bima Sakti";s:17:"departure_station";s:3:"GMR";s:14:"departure_time";s:5:"16:00";s:19:"departure_timestamp";i:1472893200;s:15:"arrival_station";s:2:"BD";s:12:"arrival_time";s:5:"22:04";s:17:"arrival_timestamp";i:1472915040;s:10:"class_name";s:3:"eks";s:15:"class_name_lang";s:17:"Eksekutif";s:17:"detail_class_name";s:9:"eksekutif";s:13:"subclass_name";s:1:"A";s:8:"is_promo";s:1:"0";s:9:"timestamp";s:19:"2016-08-08 10:52:40";s:9:"time_diff";a:3:{s:11:"is_next_day";b:0;s:9:"diff_hour";i:6;s:11:"diff_minute";i:4;}s:12:"can_be_shown";b:1;s:10:"is_closing";b:0;s:23:"formatted_schedule_date";s:16:"Sab, 03 Sep 2016";s:17:"price_adult_clean";i:275000;s:11:"price_adult";s:9:"275000.00";s:17:"price_child_clean";i:275000;s:11:"price_child";s:9:"275000.00";s:18:"price_infant_clean";i:0;s:12:"price_infant";s:4:"0.00";s:17:"price_total_clean";i:275000;s:11:"price_total";s:11:"IDR 275.000";s:17:"selected_schedule";b:0;s:8:"duration";s:23:"6 j 4 m";}i:7;a:30:{s:2:"id";s:7:"8314383";s:19:"detail_availability";s:2:"20";s:8:"train_id";s:4:"8890";s:10:"train_name";s:20:"Tiket.com Bima Sakti";s:17:"departure_station";s:3:"GMR";s:14:"departure_time";s:5:"16:00";s:19:"departure_timestamp";i:1472893200;s:15:"arrival_station";s:2:"BD";s:12:"arrival_time";s:5:"22:04";s:17:"arrival_timestamp";i:1472915040;s:10:"class_name";s:3:"bis";s:15:"class_name_lang";s:16:"Bisnis";s:17:"detail_class_name";s:6:"bisnis";s:13:"subclass_name";s:1:"M";s:8:"is_promo";s:1:"0";s:9:"timestamp";s:19:"2016-08-08 10:52:40";s:9:"time_diff";a:3:{s:11:"is_next_day";b:0;s:9:"diff_hour";i:6;s:11:"diff_minute";i:4;}s:12:"can_be_shown";b:1;s:10:"is_closing";b:0;s:23:"formatted_schedule_date";s:16:"Sab, 03 Sep 2016";s:17:"price_adult_clean";i:200000;s:11:"price_adult";s:9:"200000.00";s:17:"price_child_clean";i:200000;s:11:"price_child";s:9:"200000.00";s:18:"price_infant_clean";i:0;s:12:"price_infant";s:4:"0.00";s:17:"price_total_clean";i:200000;s:11:"price_total";s:11:"IDR 200.000";s:17:"selected_schedule";b:0;s:8:"duration";s:23:"6 j 4 m";}i:8;a:30:{s:2:"id";s:7:"8314385";s:19:"detail_availability";s:2:"10";s:8:"train_id";s:4:"8890";s:10:"train_name";s:20:"Tiket.com Bima Sakti";s:17:"departure_station";s:3:"GMR";s:14:"departure_time";s:5:"16:00";s:19:"departure_timestamp";i:1472893200;s:15:"arrival_station";s:2:"BD";s:12:"arrival_time";s:5:"22:04";s:17:"arrival_timestamp";i:1472915040;s:10:"class_name";s:3:"eko";s:15:"class_name_lang";s:15:"Ekonomi";s:17:"detail_class_name";s:7:"ekonomi";s:13:"subclass_name";s:1:"P";s:8:"is_promo";s:1:"0";s:9:"timestamp";s:19:"2016-08-08 10:52:40";s:9:"time_diff";a:3:{s:11:"is_next_day";b:0;s:9:"diff_hour";i:6;s:11:"diff_minute";i:4;}s:12:"can_be_shown";b:1;s:10:"is_closing";b:0;s:23:"formatted_schedule_date";s:16:"Sab, 03 Sep 2016";s:17:"price_adult_clean";i:150000;s:11:"price_adult";s:9:"150000.00";s:17:"price_child_clean";i:150000;s:11:"price_child";s:9:"150000.00";s:18:"price_infant_clean";i:0;s:12:"price_infant";s:4:"0.00";s:17:"price_total_clean";i:150000;s:11:"price_total";s:11:"IDR 150.000";s:17:"selected_schedule";b:0;s:8:"duration";s:23:"6 j 4 m";}i:9;a:30:{s:2:"id";s:7:"8314387";s:19:"detail_availability";s:2:"77";s:8:"train_id";s:3:"A76";s:10:"train_name";s:10:"Kereta Yes";s:17:"departure_station";s:3:"GMR";s:14:"departure_time";s:5:"21:03";s:19:"departure_timestamp";i:1472911380;s:15:"arrival_station";s:2:"BD";s:12:"arrival_time";s:5:"04:43";s:17:"arrival_timestamp";i:1472938980;s:10:"class_name";s:3:"eks";s:15:"class_name_lang";s:17:"Eksekutif";s:17:"detail_class_name";s:9:"eksekutif";s:13:"subclass_name";s:1:"A";s:8:"is_promo";s:1:"0";s:9:"timestamp";s:19:"2016-08-08 10:52:40";s:9:"time_diff";a:3:{s:11:"is_next_day";b:1;s:9:"diff_hour";i:7;s:11:"diff_minute";i:40;}s:12:"can_be_shown";b:1;s:10:"is_closing";b:0;s:23:"formatted_schedule_date";s:16:"Sab, 03 Sep 2016";s:17:"price_adult_clean";i:275000;s:11:"price_adult";s:9:"275000.00";s:17:"price_child_clean";i:275000;s:11:"price_child";s:9:"275000.00";s:18:"price_infant_clean";i:0;s:12:"price_infant";s:4:"0.00";s:17:"price_total_clean";i:275000;s:11:"price_total";s:11:"IDR 275.000";s:17:"selected_schedule";b:0;s:8:"duration";s:24:"7 j 40 m";}i:10;a:30:{s:2:"id";s:7:"8314391";s:19:"detail_availability";s:2:"20";s:8:"train_id";s:3:"A76";s:10:"train_name";s:10:"Kereta Yes";s:17:"departure_station";s:3:"GMR";s:14:"departure_time";s:5:"21:03";s:19:"departure_timestamp";i:1472911380;s:15:"arrival_station";s:2:"BD";s:12:"arrival_time";s:5:"04:43";s:17:"arrival_timestamp";i:1472938980;s:10:"class_name";s:3:"bis";s:15:"class_name_lang";s:16:"Bisnis";s:17:"detail_class_name";s:6:"bisnis";s:13:"subclass_name";s:1:"M";s:8:"is_promo";s:1:"0";s:9:"timestamp";s:19:"2016-08-08 10:52:40";s:9:"time_diff";a:3:{s:11:"is_next_day";b:1;s:9:"diff_hour";i:7;s:11:"diff_minute";i:40;}s:12:"can_be_shown";b:1;s:10:"is_closing";b:0;s:23:"formatted_schedule_date";s:16:"Sab, 03 Sep 2016";s:17:"price_adult_clean";i:200000;s:11:"price_adult";s:9:"200000.00";s:17:"price_child_clean";i:200000;s:11:"price_child";s:9:"200000.00";s:18:"price_infant_clean";i:0;s:12:"price_infant";s:4:"0.00";s:17:"price_total_clean";i:200000;s:11:"price_total";s:11:"IDR 200.000";s:17:"selected_schedule";b:0;s:8:"duration";s:24:"7 j 40 m";}i:11;a:30:{s:2:"id";s:7:"8314393";s:19:"detail_availability";s:2:"10";s:8:"train_id";s:3:"A76";s:10:"train_name";s:10:"Kereta Yes";s:17:"departure_station";s:3:"GMR";s:14:"departure_time";s:5:"21:03";s:19:"departure_timestamp";i:1472911380;s:15:"arrival_station";s:2:"BD";s:12:"arrival_time";s:5:"04:43";s:17:"arrival_timestamp";i:1472938980;s:10:"class_name";s:3:"eko";s:15:"class_name_lang";s:15:"Ekonomi";s:17:"detail_class_name";s:7:"ekonomi";s:13:"subclass_name";s:1:"P";s:8:"is_promo";s:1:"0";s:9:"timestamp";s:19:"2016-08-08 10:52:40";s:9:"time_diff";a:3:{s:11:"is_next_day";b:1;s:9:"diff_hour";i:7;s:11:"diff_minute";i:40;}s:12:"can_be_shown";b:1;s:10:"is_closing";b:0;s:23:"formatted_schedule_date";s:16:"Sab, 03 Sep 2016";s:17:"price_adult_clean";i:150000;s:11:"price_adult";s:9:"150000.00";s:17:"price_child_clean";i:150000;s:11:"price_child";s:9:"150000.00";s:18:"price_infant_clean";i:0;s:12:"price_infant";s:4:"0.00";s:17:"price_total_clean";i:150000;s:11:"price_total";s:11:"IDR 150.000";s:17:"selected_schedule";b:0;s:8:"duration";s:24:"7 j 40 m";}i:12;a:30:{s:2:"id";s:7:"8314395";s:19:"detail_availability";s:2:"77";s:8:"train_id";s:2:"35";s:10:"train_name";s:13:"Kuda Jingkrak";s:17:"departure_station";s:3:"GMR";s:14:"departure_time";s:5:"23:02";s:19:"departure_timestamp";i:1472918520;s:15:"arrival_station";s:2:"BD";s:12:"arrival_time";s:5:"05:38";s:17:"arrival_timestamp";i:1472942280;s:10:"class_name";s:3:"eks";s:15:"class_name_lang";s:17:"Eksekutif";s:17:"detail_class_name";s:9:"eksekutif";s:13:"subclass_name";s:1:"A";s:8:"is_promo";s:1:"0";s:9:"timestamp";s:19:"2016-08-08 10:52:40";s:9:"time_diff";a:3:{s:11:"is_next_day";b:1;s:9:"diff_hour";i:6;s:11:"diff_minute";i:36;}s:12:"can_be_shown";b:1;s:10:"is_closing";b:0;s:23:"formatted_schedule_date";s:16:"Sab, 03 Sep 2016";s:17:"price_adult_clean";i:275000;s:11:"price_adult";s:9:"275000.00";s:17:"price_child_clean";i:275000;s:11:"price_child";s:9:"275000.00";s:18:"price_infant_clean";i:0;s:12:"price_infant";s:4:"0.00";s:17:"price_total_clean";i:275000;s:11:"price_total";s:11:"IDR 275.000";s:17:"selected_schedule";b:0;s:8:"duration";s:24:"6 j 36 m";}i:13;a:30:{s:2:"id";s:7:"8314399";s:19:"detail_availability";s:2:"20";s:8:"train_id";s:2:"35";s:10:"train_name";s:13:"Kuda Jingkrak";s:17:"departure_station";s:3:"GMR";s:14:"departure_time";s:5:"23:02";s:19:"departure_timestamp";i:1472918520;s:15:"arrival_station";s:2:"BD";s:12:"arrival_time";s:5:"05:38";s:17:"arrival_timestamp";i:1472942280;s:10:"class_name";s:3:"bis";s:15:"class_name_lang";s:16:"Bisnis";s:17:"detail_class_name";s:6:"bisnis";s:13:"subclass_name";s:1:"M";s:8:"is_promo";s:1:"0";s:9:"timestamp";s:19:"2016-08-08 10:52:40";s:9:"time_diff";a:3:{s:11:"is_next_day";b:1;s:9:"diff_hour";i:6;s:11:"diff_minute";i:36;}s:12:"can_be_shown";b:1;s:10:"is_closing";b:0;s:23:"formatted_schedule_date";s:16:"Sab, 03 Sep 2016";s:17:"price_adult_clean";i:200000;s:11:"price_adult";s:9:"200000.00";s:17:"price_child_clean";i:200000;s:11:"price_child";s:9:"200000.00";s:18:"price_infant_clean";i:0;s:12:"price_infant";s:4:"0.00";s:17:"price_total_clean";i:200000;s:11:"price_total";s:11:"IDR 200.000";s:17:"selected_schedule";b:0;s:8:"duration";s:24:"6 j 36 m";}i:14;a:30:{s:2:"id";s:7:"8314401";s:19:"detail_availability";s:2:"10";s:8:"train_id";s:2:"35";s:10:"train_name";s:13:"Kuda Jingkrak";s:17:"departure_station";s:3:"GMR";s:14:"departure_time";s:5:"23:02";s:19:"departure_timestamp";i:1472918520;s:15:"arrival_station";s:2:"BD";s:12:"arrival_time";s:5:"05:38";s:17:"arrival_timestamp";i:1472942280;s:10:"class_name";s:3:"eko";s:15:"class_name_lang";s:15:"Ekonomi";s:17:"detail_class_name";s:7:"ekonomi";s:13:"subclass_name";s:1:"P";s:8:"is_promo";s:1:"0";s:9:"timestamp";s:19:"2016-08-08 10:52:40";s:9:"time_diff";a:3:{s:11:"is_next_day";b:1;s:9:"diff_hour";i:6;s:11:"diff_minute";i:36;}s:12:"can_be_shown";b:1;s:10:"is_closing";b:0;s:23:"formatted_schedule_date";s:16:"Sab, 03 Sep 2016";s:17:"price_adult_clean";i:150000;s:11:"price_adult";s:9:"150000.00";s:17:"price_child_clean";i:150000;s:11:"price_child";s:9:"150000.00";s:18:"price_infant_clean";i:0;s:12:"price_infant";s:4:"0.00";s:17:"price_total_clean";i:150000;s:11:"price_total";s:11:"IDR 150.000";s:17:"selected_schedule";b:0;s:8:"duration";s:24:"6 j 36 m";}i:15;a:30:{s:2:"id";s:7:"8314403";s:19:"detail_availability";s:2:"77";s:8:"train_id";s:1:"3";s:10:"train_name";s:14:"Polar Ekspress";s:17:"departure_station";s:3:"GMR";s:14:"departure_time";s:5:"23:58";s:19:"departure_timestamp";i:1472921880;s:15:"arrival_station";s:2:"BD";s:12:"arrival_time";s:5:"05:57";s:17:"arrival_timestamp";i:1472943420;s:10:"class_name";s:3:"eks";s:15:"class_name_lang";s:17:"Eksekutif";s:17:"detail_class_name";s:9:"eksekutif";s:13:"subclass_name";s:1:"A";s:8:"is_promo";s:1:"0";s:9:"timestamp";s:19:"2016-08-08 10:52:40";s:9:"time_diff";a:3:{s:11:"is_next_day";b:1;s:9:"diff_hour";i:5;s:11:"diff_minute";i:59;}s:12:"can_be_shown";b:1;s:10:"is_closing";b:0;s:23:"formatted_schedule_date";s:16:"Sab, 03 Sep 2016";s:17:"price_adult_clean";i:275000;s:11:"price_adult";s:9:"275000.00";s:17:"price_child_clean";i:275000;s:11:"price_child";s:9:"275000.00";s:18:"price_infant_clean";i:0;s:12:"price_infant";s:4:"0.00";s:17:"price_total_clean";i:275000;s:11:"price_total";s:11:"IDR 275.000";s:17:"selected_schedule";b:0;s:8:"duration";s:24:"5 j 59 m";}i:16;a:30:{s:2:"id";s:7:"8314407";s:19:"detail_availability";s:2:"20";s:8:"train_id";s:1:"3";s:10:"train_name";s:14:"Polar Ekspress";s:17:"departure_station";s:3:"GMR";s:14:"departure_time";s:5:"23:58";s:19:"departure_timestamp";i:1472921880;s:15:"arrival_station";s:2:"BD";s:12:"arrival_time";s:5:"05:57";s:17:"arrival_timestamp";i:1472943420;s:10:"class_name";s:3:"bis";s:15:"class_name_lang";s:16:"Bisnis";s:17:"detail_class_name";s:6:"bisnis";s:13:"subclass_name";s:1:"M";s:8:"is_promo";s:1:"0";s:9:"timestamp";s:19:"2016-08-08 10:52:40";s:9:"time_diff";a:3:{s:11:"is_next_day";b:1;s:9:"diff_hour";i:5;s:11:"diff_minute";i:59;}s:12:"can_be_shown";b:1;s:10:"is_closing";b:0;s:23:"formatted_schedule_date";s:16:"Sab, 03 Sep 2016";s:17:"price_adult_clean";i:200000;s:11:"price_adult";s:9:"200000.00";s:17:"price_child_clean";i:200000;s:11:"price_child";s:9:"200000.00";s:18:"price_infant_clean";i:0;s:12:"price_infant";s:4:"0.00";s:17:"price_total_clean";i:200000;s:11:"price_total";s:11:"IDR 200.000";s:17:"selected_schedule";b:0;s:8:"duration";s:24:"5 j 59 m";}i:17;a:30:{s:2:"id";s:7:"8314409";s:19:"detail_availability";s:2:"10";s:8:"train_id";s:1:"3";s:10:"train_name";s:14:"Polar Ekspress";s:17:"departure_station";s:3:"GMR";s:14:"departure_time";s:5:"23:58";s:19:"departure_timestamp";i:1472921880;s:15:"arrival_station";s:2:"BD";s:12:"arrival_time";s:5:"05:57";s:17:"arrival_timestamp";i:1472943420;s:10:"class_name";s:3:"eko";s:15:"class_name_lang";s:15:"Ekonomi";s:17:"detail_class_name";s:7:"ekonomi";s:13:"subclass_name";s:1:"P";s:8:"is_promo";s:1:"0";s:9:"timestamp";s:19:"2016-08-08 10:52:40";s:9:"time_diff";a:3:{s:11:"is_next_day";b:1;s:9:"diff_hour";i:5;s:11:"diff_minute";i:59;}s:12:"can_be_shown";b:1;s:10:"is_closing";b:0;s:23:"formatted_schedule_date";s:16:"Sab, 03 Sep 2016";s:17:"price_adult_clean";i:150000;s:11:"price_adult";s:9:"150000.00";s:17:"price_child_clean";i:150000;s:11:"price_child";s:9:"150000.00";s:18:"price_infant_clean";i:0;s:12:"price_infant";s:4:"0.00";s:17:"price_total_clean";i:150000;s:11:"price_total";s:11:"IDR 150.000";s:17:"selected_schedule";b:0;s:8:"duration";s:24:"5 j 59 m";}}}s:12:"login_status";s:4:"true";s:8:"guest_id";s:8:"22691145";s:11:"login_email";s:21:"wida.skydev@gmail.com";s:5:"token";s:40:"f9b29ac359ca5d77755e7588751c089bf96f0dc9";}
```

* NOTE : UPDATE for INFANT passenger,just now is for development server (api-sandbox.tiket.com)  
We will inform you if its already provided in production server (api.tiket.com)

#### HTTP Request
    `https://api-sandbox.tiket.com/search/train?d=GMR&a=BD&date=2016-09-03&ret_date=&adult=1&child=0&class=all&token=f9b29ac359ca5d77755e7588751c089bf96f0dc9&output=json`

#### Parameters
  
Name | Description | Format | Default | Mandatory
---- | ----------- | ------ | ------- | ---------
d | Depart train station code | CHAR(3) |  | TRUE  
a | Arrival train station code | CHAR(3) |  | TRUE  
date | depart date. Result will be in | YYYY-MM-DD |  | TRUE  
ret_date | return date. If provided, then system will return | YYYY-MM-DD |  | FALSE  
adult | number of adult passenger (max adult+child+infant 4 persons) | INT | 1 | FALSE  
child | number of child passenger (max adult+child+infant 4 persons) | INT | 0 | FALSE  
infant | number of infant passenger (max adult+child+infant 4 persons) | INT | 0 |FALSE  
class | train class (ALL) | all,bis,eks,eco | all | FALSE  
token | for saving transaction that done by user | CHAR(128) |  | TRUE  

         
## Search Station

```xml
<?xml version="1.0" encoding="utf-8"?>
<tiket>
    <diagnostic>
        <status>200</status>
        <elapsetime>0.1420</elapsetime>
        <memoryusage>6.23MB</memoryusage>
        <unix_timestamp>1470629338</unix_timestamp>
        <confirm>success</confirm>
        <lang>id</lang>
        <currency>IDR</currency>
    </diagnostic>
    <output_type>xml</output_type>
    <stations>
        <station>
            <station_name>aekloba</station_name>
            <city_name>Labuhan Batu</city_name>
            <station_code>AKB</station_code>
            <latitude>2.26705500000000000000</latitude>
            <longitude>100.08064300000000000000</longitude>
        </station>
        <station>
            <station_name>alastuwa</station_name>
            <city_name>Semarang</city_name>
            <station_code>ATA</station_code>
            <latitude>-6.98444700000000000000</latitude>
            <longitude>110.47637000000000000000</longitude>
        </station>
        <station>
            <station_name>ambarawa</station_name>
            <city_name>Lampung Tengah</city_name>
            <station_code>ABR</station_code>
            <latitude>-7.26472200000000000000</latitude>
            <longitude>110.40222200000000000000</longitude>
        </station>
    </stations>
</tiket>
``` 


```json 
{
  "diagnostic": {
    "status": 200,
    "elapsetime": "0.1347",
    "memoryusage": "6.17MB",
    "unix_timestamp": 1470629275,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "stations": {
    "station": [
      {
        "station_name": "aekloba",
        "city_name": "Labuhan Batu",
        "station_code": "AKB",
        "latitude": "2.26705500000000000000",
        "longitude": "100.08064300000000000000"
      },
      {
        "station_name": "alastuwa",
        "city_name": "Semarang",
        "station_code": "ATA",
        "latitude": "-6.98444700000000000000",
        "longitude": "110.47637000000000000000"
      },
      {
        "station_name": "ambarawa",
        "city_name": "Lampung Tengah",
        "station_code": "ABR",
        "latitude": "-7.26472200000000000000",
        "longitude": "110.40222200000000000000"
      }
    ]
  }
}
```


```matlab
a:7:{s:10:"diagnostic";a:7:{s:6:"status";i:200;s:10:"elapsetime";s:14:"0.1216";s:11:"memoryusage";s:14:"6.22MB";s:14:"unix_timestamp";i:1470629542;s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:11:"output_type";s:9:"serialize";s:8:"stations";a:1:{s:7:"station";a:411:{i:0;a:5:{s:12:"station_name";s:7:"aekloba";s:9:"city_name";s:12:"Labuhan Batu";s:12:"station_code";s:3:"AKB";s:8:"latitude";s:22:"2.26705500000000000000";s:9:"longitude";s:24:"100.08064300000000000000";}i:1;a:5:{s:12:"station_name";s:8:"alastuwa";s:9:"city_name";s:8:"Semarang";s:12:"station_code";s:3:"ATA";s:8:"latitude";s:23:"-6.98444700000000000000";s:9:"longitude";s:24:"110.47637000000000000000";}i:2;a:5:{s:12:"station_name";s:8:"ambarawa";s:9:"city_name";s:14:"Lampung Tengah";s:12:"station_code";s:3:"ABR";s:8:"latitude";s:23:"-7.26472200000000000000";s:9:"longitude";s:24:"110.40222200000000000000";}i:3;a:5:{s:12:"station_name";s:5:"angke";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"AK";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:4;a:5:{s:12:"station_name";s:8:"argopuro";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"AGO";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:5;a:5:{s:12:"station_name";s:6:"arjasa";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"AJ";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:6;a:5:{s:12:"station_name";s:12:"arjawinangun";s:9:"city_name";s:7:"Cirebon";s:12:"station_code";s:3:"AWN";s:8:"latitude";s:23:"-6.64971000000000000000";s:9:"longitude";s:24:"108.42422200000000000000";}i:7;a:5:{s:12:"station_name";s:8:"awipari ";s:9:"city_name";s:11:"Tasikmalaya";s:12:"station_code";s:2:"AW";s:8:"latitude";s:23:"-7.35318800000000000000";s:9:"longitude";s:24:"108.27103600000000000000";}i:8;a:5:{s:12:"station_name";s:8:"babadan ";s:9:"city_name";s:6:"Madiun";s:12:"station_code";s:3:"BBD";s:8:"latitude";s:23:"-7.50564200000000000000";s:9:"longitude";s:24:"111.55386700000000000000";}i:9;a:5:{s:12:"station_name";s:8:"babakan ";s:9:"city_name";s:7:"Cirebon";s:12:"station_code";s:3:"BBK";s:8:"latitude";s:23:"-6.86133700000000000000";s:9:"longitude";s:24:"108.72131500000000000000";}i:10;a:5:{s:12:"station_name";s:6:"babat ";s:9:"city_name";s:8:"Lamongan";s:12:"station_code";s:3:"BBT";s:8:"latitude";s:23:"-7.10332000000000000000";s:9:"longitude";s:24:"112.17684700000000000000";}i:11;a:5:{s:12:"station_name";s:6:"bagor ";s:9:"city_name";s:7:"Nganjuk";s:12:"station_code";s:3:"BGR";s:8:"latitude";s:23:"-7.57325500000000000000";s:9:"longitude";s:24:"111.86094800000000000000";}i:12;a:5:{s:12:"station_name";s:11:"bajalinggei";s:9:"city_name";s:15:"Serdang Bedagai";s:12:"station_code";s:3:"BJL";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:13;a:5:{s:12:"station_name";s:6:"bamban";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"BMB";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:14;a:5:{s:12:"station_name";s:14:"bandar kalipah";s:9:"city_name";s:12:"Deli Serdang";s:12:"station_code";s:3:"BAP";s:8:"latitude";s:22:"3.55323500000000000000";s:9:"longitude";s:23:"98.69617200000000000000";}i:15;a:5:{s:12:"station_name";s:13:"bandar tinggi";s:9:"city_name";s:16:"Pematang Siantar";s:12:"station_code";s:3:"BDT";s:8:"latitude";s:22:"3.17000000000000000000";s:9:"longitude";s:23:"99.38000000000000000000";}i:16;a:5:{s:12:"station_name";s:7:"bandung";s:9:"city_name";s:7:"Bandung";s:12:"station_code";s:2:"BD";s:8:"latitude";s:23:"-6.91278600000000000000";s:9:"longitude";s:24:"107.60288200000000000000";}i:17;a:5:{s:12:"station_name";s:6:"bangil";s:9:"city_name";s:8:"Pasuruan";s:12:"station_code";s:2:"BG";s:8:"latitude";s:23:"-7.60008700000000000000";s:9:"longitude";s:24:"112.78000100000000000000";}i:18;a:5:{s:12:"station_name";s:9:"bangoduwa";s:9:"city_name";s:7:"Cirebon";s:12:"station_code";s:3:"BDW";s:8:"latitude";s:23:"-6.66288700000000000000";s:9:"longitude";s:24:"108.45977200000000000000";}i:19;a:5:{s:12:"station_name";s:11:"bangsalsari";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"BSS";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:20;a:5:{s:12:"station_name";s:6:"banjar";s:9:"city_name";s:6:"Banjar";s:12:"station_code";s:3:"BJR";s:8:"latitude";s:23:"-7.36676600000000000000";s:9:"longitude";s:24:"108.54492200000000000000";}i:21;a:5:{s:12:"station_name";s:10:"banjarsari";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"BJI";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:22;a:5:{s:12:"station_name";s:15:"banyuwangi baru";s:9:"city_name";s:10:"Banyuwangi";s:12:"station_code";s:2:"BW";s:8:"latitude";s:23:"-8.13347700000000000000";s:9:"longitude";s:24:"114.39895000000000000000";}i:23;a:5:{s:12:"station_name";s:5:"barat";s:9:"city_name";s:7:"Magetan";s:12:"station_code";s:3:"BAT";s:8:"latitude";s:23:"-7.56221100000000000000";s:9:"longitude";s:24:"111.45122400000000000000";}i:24;a:5:{s:12:"station_name";s:5:"baron";s:9:"city_name";s:7:"Nganjuk";s:12:"station_code";s:3:"BRN";s:8:"latitude";s:23:"-7.60272500000000000000";s:9:"longitude";s:24:"112.03917100000000000000";}i:25;a:5:{s:12:"station_name";s:6:"batang";s:9:"city_name";s:6:"Batang";s:12:"station_code";s:3:"BTG";s:8:"latitude";s:23:"-6.90746900000000000000";s:9:"longitude";s:24:"109.73021100000000000000";}i:26;a:5:{s:12:"station_name";s:11:"batang kuis";s:9:"city_name";s:12:"Deli Serdang";s:12:"station_code";s:3:"BTK";s:8:"latitude";s:22:"3.63399300000000000000";s:9:"longitude";s:23:"98.80266700000000000000";}i:27;a:5:{s:12:"station_name";s:10:"batu tulis";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"BTT";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:28;a:5:{s:12:"station_name";s:8:"baturaja";s:9:"city_name";s:17:"Ogan Komering Ulu";s:12:"station_code";s:3:"BTA";s:8:"latitude";s:23:"-2.92624000000000000000";s:9:"longitude";s:24:"104.69730400000000000000";}i:29;a:5:{s:12:"station_name";s:6:"bekasi";s:9:"city_name";s:6:"Bekasi";s:12:"station_code";s:3:"BKS";s:8:"latitude";s:23:"-6.23495200000000000000";s:9:"longitude";s:24:"106.99715900000000000000";}i:30;a:5:{s:12:"station_name";s:5:"bekri";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"BKI";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:31;a:5:{s:12:"station_name";s:6:"benowo";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"BNW";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:32;a:5:{s:12:"station_name";s:6:"binjai";s:9:"city_name";s:6:"Binjai";s:12:"station_code";s:3:"BIJ";s:8:"latitude";s:22:"3.62703300000000000000";s:9:"longitude";s:23:"98.49444900000000000000";}i:33;a:5:{s:12:"station_name";s:15:"blambanganpagar";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"BBA";s:8:"latitude";s:23:"-4.89389000000000000000";s:9:"longitude";s:24:"105.07214500000000000000";}i:34;a:5:{s:12:"station_name";s:14:"blambanganumpu";s:9:"city_name";s:9:"Way Kanan";s:12:"station_code";s:3:"BBU";s:8:"latitude";s:23:"-4.49815700000000000000";s:9:"longitude";s:24:"104.52017600000000000000";}i:35;a:5:{s:12:"station_name";s:9:"blimbing ";s:9:"city_name";s:6:"Malang";s:12:"station_code";s:3:"BMG";s:8:"latitude";s:23:"-7.93989600000000000000";s:9:"longitude";s:24:"112.64447500000000000000";}i:36;a:5:{s:12:"station_name";s:16:"blimbing pendopo";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"BIB";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:37;a:5:{s:12:"station_name";s:6:"blitar";s:9:"city_name";s:6:"Blitar";s:12:"station_code";s:2:"BL";s:8:"latitude";s:23:"-8.10126800000000000000";s:9:"longitude";s:24:"112.16276600000000000000";}i:38;a:5:{s:12:"station_name";s:5:"bogor";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"BOO";s:8:"latitude";s:23:"-6.59459800000000000000";s:9:"longitude";s:24:"106.79058000000000000000";}i:39;a:5:{s:12:"station_name";s:8:"boharan ";s:9:"city_name";s:8:"Sidoarjo";s:12:"station_code";s:2:"BH";s:8:"latitude";s:23:"-7.39402500000000000000";s:9:"longitude";s:24:"112.60791100000000000000";}i:40;a:5:{s:12:"station_name";s:10:"bojonegoro";s:9:"city_name";s:10:"Bojonegoro";s:12:"station_code";s:2:"BJ";s:8:"latitude";s:23:"-7.16684300000000000000";s:9:"longitude";s:24:"111.89027000000000000000";}i:41;a:5:{s:12:"station_name";s:6:"bojong";s:9:"city_name";s:6:"Ciamis";s:12:"station_code";s:3:"BJG";s:8:"latitude";s:23:"-7.35140100000000000000";s:9:"longitude";s:24:"108.44804000000000000000";}i:42;a:5:{s:12:"station_name";s:7:"bowerno";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"BWO";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:43;a:5:{s:12:"station_name";s:9:"brambanan";s:9:"city_name";s:6:"Klaten";s:12:"station_code";s:3:"BBN";s:8:"latitude";s:23:"-7.75604700000000000000";s:9:"longitude";s:24:"110.49711900000000000000";}i:44;a:5:{s:12:"station_name";s:6:"brebes";s:9:"city_name";s:6:"Brebes";s:12:"station_code";s:2:"BB";s:8:"latitude";s:23:"-6.87425200000000000000";s:9:"longitude";s:24:"109.04235400000000000000";}i:45;a:5:{s:12:"station_name";s:8:"brumbung";s:9:"city_name";s:5:"Demak";s:12:"station_code";s:3:"BBG";s:8:"latitude";s:23:"-7.04303600000000000000";s:9:"longitude";s:24:"110.54660100000000000000";}i:46;a:5:{s:12:"station_name";s:9:"bulakamba";s:9:"city_name";s:6:"Brebes";s:12:"station_code";s:3:"BKA";s:8:"latitude";s:23:"-6.87122200000000000000";s:9:"longitude";s:24:"108.89647400000000000000";}i:47;a:5:{s:12:"station_name";s:7:"bumiayu";s:9:"city_name";s:6:"Brebes";s:12:"station_code";s:3:"BMA";s:8:"latitude";s:23:"-7.23537100000000000000";s:9:"longitude";s:24:"109.01007100000000000000";}i:48;a:5:{s:12:"station_name";s:8:"bungamas";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"BGM";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:49;a:5:{s:12:"station_name";s:8:"candimas";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CMS";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:50;a:5:{s:12:"station_name";s:7:"caruban";s:9:"city_name";s:6:"Madiun";s:12:"station_code";s:3:"CRB";s:8:"latitude";s:23:"-7.54867700000000000000";s:9:"longitude";s:24:"111.67619700000000000000";}i:51;a:5:{s:12:"station_name";s:6:"catang";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"CT";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:52;a:5:{s:12:"station_name";s:4:"cepu";s:9:"city_name";s:5:"Blora";s:12:"station_code";s:2:"CU";s:8:"latitude";s:23:"-7.59217500000000000000";s:9:"longitude";s:24:"112.10053900000000000000";}i:53;a:5:{s:12:"station_name";s:5:"cerme";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CME";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:54;a:5:{s:12:"station_name";s:6:"ciamis";s:9:"city_name";s:6:"Ciamis";s:12:"station_code";s:2:"CI";s:8:"latitude";s:23:"-7.00000000000000000000";s:9:"longitude";s:24:"108.00000000000000000000";}i:55;a:5:{s:12:"station_name";s:7:"cianjur";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"CJ";s:8:"latitude";s:23:"-6.82457900000000000000";s:9:"longitude";s:24:"107.14282800000000000000";}i:56;a:5:{s:12:"station_name";s:5:"ciawi";s:9:"city_name";s:11:"Tasikmalaya";s:12:"station_code";s:3:"CAW";s:8:"latitude";s:23:"-7.16510800000000000000";s:9:"longitude";s:24:"108.15417800000000000000";}i:57;a:5:{s:12:"station_name";s:7:"cibadak";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CBD";s:8:"latitude";s:23:"-6.88822800000000000000";s:9:"longitude";s:24:"106.78035300000000000000";}i:58;a:5:{s:12:"station_name";s:6:"cibatu";s:9:"city_name";s:5:"Garut";s:12:"station_code";s:2:"CB";s:8:"latitude";s:23:"-7.10872800000000000000";s:9:"longitude";s:24:"107.96964200000000000000";}i:59;a:5:{s:12:"station_name";s:7:"cibeber";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CBB";s:8:"latitude";s:23:"-6.93759900000000000000";s:9:"longitude";s:24:"107.12128900000000000000";}i:60;a:5:{s:12:"station_name";s:8:"cibungur";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CBR";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:61;a:5:{s:12:"station_name";s:10:"cicalengka";s:9:"city_name";s:7:"Bandung";s:12:"station_code";s:3:"CCL";s:8:"latitude";s:23:"-6.99588500000000000000";s:9:"longitude";s:24:"107.84272000000000000000";}i:62;a:5:{s:12:"station_name";s:7:"cicayur";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CCY";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:63;a:5:{s:12:"station_name";s:7:"cicurug";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CCR";s:8:"latitude";s:23:"-6.79027500000000000000";s:9:"longitude";s:24:"106.77941900000000000000";}i:64;a:5:{s:12:"station_name";s:7:"ciganea";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"CA";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:65;a:5:{s:12:"station_name";s:9:"cigombong";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CGB";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:66;a:5:{s:12:"station_name";s:13:"cikadongdong ";s:9:"city_name";s:13:"Bandung Barat";s:12:"station_code";s:2:"CD";s:8:"latitude";s:23:"-6.71588300000000000000";s:9:"longitude";s:24:"107.39082100000000000000";}i:67;a:5:{s:12:"station_name";s:8:"cikampek";s:9:"city_name";s:8:"Karawang";s:12:"station_code";s:3:"CKP";s:8:"latitude";s:23:"-6.40706800000000000000";s:9:"longitude";s:24:"107.45649800000000000000";}i:68;a:5:{s:12:"station_name";s:8:"cikarang";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CKR";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:69;a:5:{s:12:"station_name";s:8:"cikeusal";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CKL";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:70;a:5:{s:12:"station_name";s:12:"cikudapateuh";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CTH";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:71;a:5:{s:12:"station_name";s:7:"cilacap";s:9:"city_name";s:7:"Cilacap";s:12:"station_code";s:2:"CP";s:8:"latitude";s:23:"-7.71647800000000000000";s:9:"longitude";s:24:"109.01197000000000000000";}i:72;a:5:{s:12:"station_name";s:6:"cilaku";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CLK";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:73;a:5:{s:12:"station_name";s:6:"cilame";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CLE";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:74;a:5:{s:12:"station_name";s:7:"ciledug";s:9:"city_name";s:7:"Cirebon";s:12:"station_code";s:3:"CLD";s:8:"latitude";s:23:"-6.89617800000000000000";s:9:"longitude";s:24:"108.75697700000000000000";}i:75;a:5:{s:12:"station_name";s:8:"cilegeh ";s:9:"city_name";s:9:"Indramayu";s:12:"station_code";s:3:"CLH";s:8:"latitude";s:23:"-6.48951400000000000000";s:9:"longitude";s:24:"108.03723300000000000000";}i:76;a:5:{s:12:"station_name";s:7:"cilegon";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CLG";s:8:"latitude";s:23:"-6.01963500000000000000";s:9:"longitude";s:24:"106.05311300000000000000";}i:77;a:5:{s:12:"station_name";s:7:"cilejit";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CJT";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:78;a:5:{s:12:"station_name";s:6:"cimahi";s:9:"city_name";s:6:"Cimahi";s:12:"station_code";s:3:"CMI";s:8:"latitude";s:23:"-6.87140300000000000000";s:9:"longitude";s:24:"107.55538000000000000000";}i:79;a:5:{s:12:"station_name";s:7:"cimekar";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CMK";s:8:"latitude";s:23:"-6.94964300000000000000";s:9:"longitude";s:24:"107.71445500000000000000";}i:80;a:5:{s:12:"station_name";s:7:"cimindi";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CMD";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:81;a:5:{s:12:"station_name";s:6:"cipari";s:9:"city_name";s:7:"Cilacap";s:12:"station_code";s:3:"CPI";s:8:"latitude";s:23:"-7.43910300000000000000";s:9:"longitude";s:24:"108.76307100000000000000";}i:82;a:5:{s:12:"station_name";s:10:"cipeundeuy";s:9:"city_name";s:5:"Garut";s:12:"station_code";s:3:"CPD";s:8:"latitude";s:23:"-7.10432100000000000000";s:9:"longitude";s:24:"108.08153300000000000000";}i:83;a:5:{s:12:"station_name";s:10:"cipunegara";s:9:"city_name";s:6:"Subang";s:12:"station_code";s:3:"CRA";s:8:"latitude";s:23:"-6.45493200000000000000";s:9:"longitude";s:24:"107.85608800000000000000";}i:84;a:5:{s:12:"station_name";s:7:"cirebon";s:9:"city_name";s:7:"Cirebon";s:12:"station_code";s:2:"CN";s:8:"latitude";s:23:"-6.70478600000000000000";s:9:"longitude";s:24:"108.55672400000000000000";}i:85;a:5:{s:12:"station_name";s:16:"cirebon prujakan";s:9:"city_name";s:7:"Cirebon";s:12:"station_code";s:3:"CNP";s:8:"latitude";s:23:"-6.72985700000000000000";s:9:"longitude";s:24:"108.56728100000000000000";}i:86;a:5:{s:12:"station_name";s:9:"cireungas";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CRG";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:87;a:5:{s:12:"station_name";s:7:"ciroyom";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CIR";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:88;a:5:{s:12:"station_name";s:6:"cisaat";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CSA";s:8:"latitude";s:23:"-6.91396300000000000000";s:9:"longitude";s:24:"106.88749400000000000000";}i:89;a:5:{s:12:"station_name";s:6:"cisauk";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CSK";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:90;a:5:{s:12:"station_name";s:8:"cisomang";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"CG";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:91;a:5:{s:12:"station_name";s:7:"citeras";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CTR";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:92;a:5:{s:12:"station_name";s:5:"comal";s:9:"city_name";s:8:"Pemalang";s:12:"station_code";s:2:"CO";s:8:"latitude";s:23:"-6.90959900000000000000";s:9:"longitude";s:24:"109.53862700000000000000";}i:93;a:5:{s:12:"station_name";s:11:"curahmalang";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"CRM";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:94;a:5:{s:12:"station_name";s:4:"daru";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"DAR";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:95;a:5:{s:12:"station_name";s:6:"dawuan";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"DWN";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:96;a:5:{s:12:"station_name";s:8:"denpasar";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"DEN";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:97;a:5:{s:12:"station_name";s:13:"dolokmerangir";s:9:"city_name";s:10:"Simalungun";s:12:"station_code";s:3:"DMR";s:8:"latitude";s:22:"3.12048300000000000000";s:9:"longitude";s:23:"99.15882100000000000000";}i:98;a:5:{s:12:"station_name";s:7:"doplang";s:9:"city_name";s:5:"Blora";s:12:"station_code";s:3:"DPL";s:8:"latitude";s:23:"-7.16682200000000000000";s:9:"longitude";s:24:"111.29584900000000000000";}i:99;a:5:{s:12:"station_name";s:5:"duduk";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"DD";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:100;a:5:{s:12:"station_name";s:4:"duku";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"DUK";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:101;a:5:{s:12:"station_name";s:4:"duri";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"DU";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:102;a:5:{s:12:"station_name";s:12:"gadobangkong";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"GK";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:103;a:5:{s:12:"station_name";s:6:"gambir";s:9:"city_name";s:13:"Jakarta Pusat";s:12:"station_code";s:3:"GMR";s:8:"latitude";s:23:"-6.17664400000000000000";s:9:"longitude";s:24:"106.83057500000000000000";}i:104;a:5:{s:12:"station_name";s:10:"gandasolih";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"GDS";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:105;a:5:{s:12:"station_name";s:14:"gandrungmangun";s:9:"city_name";s:7:"Cilacap";s:12:"station_code";s:3:"GDM";s:8:"latitude";s:23:"-7.50976900000000000000";s:9:"longitude";s:24:"108.83902100000000000000";}i:106;a:5:{s:12:"station_name";s:7:"garahan";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"GRN";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:107;a:5:{s:12:"station_name";s:5:"garum";s:9:"city_name";s:6:"Blitar";s:12:"station_code";s:3:"GRM";s:8:"latitude";s:23:"-8.07360200000000000000";s:9:"longitude";s:24:"112.21683300000000000000";}i:108;a:5:{s:12:"station_name";s:8:"gedangan";s:9:"city_name";s:8:"Sidoarjo";s:12:"station_code";s:3:"GDG";s:8:"latitude";s:23:"-7.38913100000000000000";s:9:"longitude";s:24:"112.72824500000000000000";}i:109;a:5:{s:12:"station_name";s:8:"gedebage";s:9:"city_name";s:7:"Bandung";s:12:"station_code";s:3:"GDB";s:8:"latitude";s:23:"-6.94193400000000000000";s:9:"longitude";s:24:"107.69197900000000000000";}i:110;a:5:{s:12:"station_name";s:7:"gembong";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"GEB";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:111;a:5:{s:12:"station_name";s:6:"geneng";s:9:"city_name";s:5:"Ngawi";s:12:"station_code";s:2:"GG";s:8:"latitude";s:23:"-7.49797300000000000000";s:9:"longitude";s:24:"111.41905900000000000000";}i:112;a:5:{s:12:"station_name";s:5:"giham";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"GHM";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:113;a:5:{s:12:"station_name";s:8:"glenmore";s:9:"city_name";s:10:"Banyuwangi";s:12:"station_code";s:3:"GLM";s:8:"latitude";s:23:"-8.30526500000000000000";s:9:"longitude";s:24:"114.09173000000000000000";}i:114;a:5:{s:12:"station_name";s:7:"gombong";s:9:"city_name";s:7:"Kebumen";s:12:"station_code";s:2:"GB";s:8:"latitude";s:23:"-7.61040300000000000000";s:9:"longitude";s:24:"109.50953000000000000000";}i:115;a:5:{s:12:"station_name";s:5:"grati";s:9:"city_name";s:8:"Pasuruan";s:12:"station_code";s:2:"GI";s:8:"latitude";s:23:"-7.73767700000000000000";s:9:"longitude";s:24:"112.98455700000000000000";}i:116;a:5:{s:12:"station_name";s:5:"gubug";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"GUB";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:117;a:5:{s:12:"station_name";s:7:"gumilir";s:9:"city_name";s:7:"Cilacap";s:12:"station_code";s:2:"GM";s:8:"latitude";s:23:"-7.68498500000000000000";s:9:"longitude";s:24:"109.04280400000000000000";}i:118;a:5:{s:12:"station_name";s:6:"gundih";s:9:"city_name";s:8:"Grobogan";s:12:"station_code";s:2:"GD";s:8:"latitude";s:23:"-7.20587700000000000000";s:9:"longitude";s:24:"110.85851000000000000000";}i:119;a:5:{s:12:"station_name";s:13:"gunungmegang ";s:9:"city_name";s:10:"Muara Enim";s:12:"station_code";s:3:"GNM";s:8:"latitude";s:23:"-3.45525000000000000000";s:9:"longitude";s:24:"103.85350200000000000000";}i:120;a:5:{s:12:"station_name";s:15:"hajipemanggilan";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"HJP";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:121;a:5:{s:12:"station_name";s:10:"haurgeulis";s:9:"city_name";s:9:"Indramayu";s:12:"station_code";s:3:"HGL";s:8:"latitude";s:23:"-6.47108300000000000000";s:9:"longitude";s:24:"107.95092000000000000000";}i:122;a:5:{s:12:"station_name";s:9:"haurpugur";s:9:"city_name";s:7:"Bandung";s:12:"station_code";s:3:"HRP";s:8:"latitude";s:23:"-6.98023000000000000000";s:9:"longitude";s:24:"107.79750800000000000000";}i:123;a:5:{s:12:"station_name";s:7:"hengelo";s:9:"city_name";s:4:"Karo";s:12:"station_code";s:2:"HL";s:8:"latitude";s:22:"2.92246900000000000000";s:9:"longitude";s:23:"99.72908000000000000000";}i:124;a:5:{s:12:"station_name";s:3:"ijo";s:9:"city_name";s:7:"Kebumen";s:12:"station_code";s:2:"IJ";s:8:"latitude";s:23:"-7.61531600000000000000";s:9:"longitude";s:24:"109.44635900000000000000";}i:125;a:5:{s:12:"station_name";s:9:"indralaya";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"IDR";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:126;a:5:{s:12:"station_name";s:9:"indralaya";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"IDY";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:127;a:5:{s:12:"station_name";s:12:"jakarta kota";s:9:"city_name";s:13:"Jakarta Barat";s:12:"station_code";s:4:"JAKK";s:8:"latitude";s:23:"-6.13758900000000000000";s:9:"longitude";s:24:"106.81467200000000000000";}i:128;a:5:{s:12:"station_name";s:6:"jambon";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"JBN";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:129;a:5:{s:12:"station_name";s:10:"jambu baru";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"JBU";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:130;a:5:{s:12:"station_name";s:10:"jatibarang";s:9:"city_name";s:9:"Indramayu";s:12:"station_code";s:3:"JTB";s:8:"latitude";s:23:"-6.47284200000000000000";s:9:"longitude";s:24:"108.30580800000000000000";}i:131;a:5:{s:12:"station_name";s:10:"jatinegara";s:9:"city_name";s:13:"Jakarta Timur";s:12:"station_code";s:3:"JNG";s:8:"latitude";s:23:"-6.21495400000000000000";s:9:"longitude";s:24:"106.87040300000000000000";}i:132;a:5:{s:12:"station_name";s:8:"jatiroto";s:9:"city_name";s:6:"Jember";s:12:"station_code";s:3:"JTR";s:8:"latitude";s:23:"-8.12339200000000000000";s:9:"longitude";s:24:"113.36469600000000000000";}i:133;a:5:{s:12:"station_name";s:6:"jember";s:9:"city_name";s:6:"Jember";s:12:"station_code";s:2:"JR";s:8:"latitude";s:23:"-8.16465800000000000000";s:9:"longitude";s:24:"113.70388300000000000000";}i:134;a:5:{s:12:"station_name";s:5:"jenar";s:9:"city_name";s:9:"Purworejo";s:12:"station_code";s:2:"JN";s:8:"latitude";s:23:"-7.79091400000000000000";s:9:"longitude";s:24:"110.00299200000000000000";}i:135;a:5:{s:12:"station_name";s:9:"jeruklegi";s:9:"city_name";s:7:"Cilacap";s:12:"station_code";s:3:"JRL";s:8:"latitude";s:23:"-7.58745300000000000000";s:9:"longitude";s:24:"109.01493100000000000000";}i:136;a:5:{s:12:"station_name";s:7:"jombang";s:9:"city_name";s:7:"Jombang";s:12:"station_code";s:2:"JG";s:8:"latitude";s:23:"-7.55869600000000000000";s:9:"longitude";s:24:"112.23153800000000000000";}i:137;a:5:{s:12:"station_name";s:12:"kalibalangan";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"KAG";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:138;a:5:{s:12:"station_name";s:8:"kalibaru";s:9:"city_name";s:10:"Banyuwangi";s:12:"station_code";s:3:"KBR";s:8:"latitude";s:23:"-8.28849100000000000000";s:9:"longitude";s:24:"113.98038600000000000000";}i:139;a:5:{s:12:"station_name";s:9:"kalibodri";s:9:"city_name";s:6:"Kendal";s:12:"station_code";s:3:"KBD";s:8:"latitude";s:23:"-6.97394700000000000000";s:9:"longitude";s:24:"110.14787400000000000000";}i:140;a:5:{s:12:"station_name";s:7:"kalisat";s:9:"city_name";s:6:"Jember";s:12:"station_code";s:3:"KLT";s:8:"latitude";s:23:"-8.12100800000000000000";s:9:"longitude";s:24:"113.85037400000000000000";}i:141;a:5:{s:12:"station_name";s:10:"kalisetail";s:9:"city_name";s:10:"Banyuwangi";s:12:"station_code";s:3:"KSL";s:8:"latitude";s:23:"-8.33732500000000000000";s:9:"longitude";s:24:"114.15198300000000000000";}i:142;a:5:{s:12:"station_name";s:8:"kalitidu";s:9:"city_name";s:10:"Bojonegoro";s:12:"station_code";s:3:"KIT";s:8:"latitude";s:23:"-7.13091500000000000000";s:9:"longitude";s:24:"111.78056700000000000000";}i:143;a:5:{s:12:"station_name";s:9:"kaliwungu";s:9:"city_name";s:6:"Kendal";s:12:"station_code";s:3:"KLN";s:8:"latitude";s:23:"-6.95888900000000000000";s:9:"longitude";s:24:"110.25417600000000000000";}i:144;a:5:{s:12:"station_name";s:14:"kampung bandan";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"KPB";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:145;a:5:{s:12:"station_name";s:9:"kandangan";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"KDA";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:146;a:5:{s:12:"station_name";s:5:"kapas";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"KPS";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:147;a:5:{s:12:"station_name";s:11:"karang sari";s:9:"city_name";s:1:" ";s:12:"station_code";s:4:"KRAI";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:148;a:5:{s:12:"station_name";s:13:"karang tengah";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"KE";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:149;a:5:{s:12:"station_name";s:10:"karangantu";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"KRA";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:150;a:5:{s:12:"station_name";s:11:"karanganyar";s:9:"city_name";s:7:"Kebumen";s:12:"station_code";s:2:"KA";s:8:"latitude";s:23:"-7.63511600000000000000";s:9:"longitude";s:24:"109.57830200000000000000";}i:151;a:5:{s:12:"station_name";s:10:"karangasem";s:9:"city_name";s:10:"Banyuwangi";s:12:"station_code";s:3:"KNE";s:8:"latitude";s:23:"-8.22162100000000000000";s:9:"longitude";s:24:"114.34094000000000000000";}i:152;a:5:{s:12:"station_name";s:10:"karangjati";s:9:"city_name";s:8:"Grobogan";s:12:"station_code";s:3:"KGT";s:8:"latitude";s:23:"-7.09505800000000000000";s:9:"longitude";s:24:"110.76630600000000000000";}i:153;a:5:{s:12:"station_name";s:10:"karangsari";s:9:"city_name";s:8:"Banyumas";s:12:"station_code";s:3:"KRR";s:8:"latitude";s:23:"-7.38598100000000000000";s:9:"longitude";s:24:"109.11651100000000000000";}i:154;a:5:{s:12:"station_name";s:12:"karangsuwung";s:9:"city_name";s:7:"Cirebon";s:12:"station_code";s:3:"KRW";s:8:"latitude";s:23:"-6.84464500000000000000";s:9:"longitude";s:24:"108.63940000000000000000";}i:155;a:5:{s:12:"station_name";s:8:"karawang";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"KW";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:156;a:5:{s:12:"station_name";s:11:"kawunganten";s:9:"city_name";s:7:"Cilacap";s:12:"station_code";s:3:"KWG";s:8:"latitude";s:23:"-7.59316400000000000000";s:9:"longitude";s:24:"108.91962600000000000000";}i:157;a:5:{s:12:"station_name";s:7:"kebasen";s:9:"city_name";s:8:"Banyumas";s:12:"station_code";s:3:"KBS";s:8:"latitude";s:23:"-7.53272300000000000000";s:9:"longitude";s:24:"109.21272800000000000000";}i:158;a:5:{s:12:"station_name";s:9:"kebayoran";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"KBY";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:159;a:5:{s:12:"station_name";s:9:"kebonromo";s:9:"city_name";s:6:"Sragen";s:12:"station_code";s:3:"KRO";s:8:"latitude";s:23:"-7.39264200000000000000";s:9:"longitude";s:24:"111.06907400000000000000";}i:160;a:5:{s:12:"station_name";s:7:"kebumen";s:9:"city_name";s:7:"Kebumen";s:12:"station_code";s:2:"KM";s:8:"latitude";s:23:"-7.66922800000000000000";s:9:"longitude";s:24:"109.65106500000000000000";}i:161;a:5:{s:12:"station_name";s:9:"kedinding";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"KDN";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:162;a:5:{s:12:"station_name";s:6:"kediri";s:9:"city_name";s:6:"Kediri";s:12:"station_code";s:2:"KD";s:8:"latitude";s:23:"-7.81703600000000000000";s:9:"longitude";s:24:"112.01465400000000000000";}i:163;a:5:{s:12:"station_name";s:12:"kedokangabus";s:9:"city_name";s:9:"Indramayu";s:12:"station_code";s:3:"KAB";s:8:"latitude";s:23:"-6.46403600000000000000";s:9:"longitude";s:24:"108.09594200000000000000";}i:164;a:5:{s:12:"station_name";s:13:"kedungbanteng";s:9:"city_name";s:6:"Sragen";s:12:"station_code";s:3:"KDB";s:8:"latitude";s:24:"111.11374900000000000000";s:9:"longitude";s:23:"-7.40609000000000000000";}i:165;a:5:{s:12:"station_name";s:11:"kedunggalar";s:9:"city_name";s:5:"Ngawi";s:12:"station_code";s:2:"KG";s:8:"latitude";s:23:"-7.42673000000000000000";s:9:"longitude";s:24:"111.30815500000000000000";}i:166;a:5:{s:12:"station_name";s:11:"kedunggedeh";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"KDH";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:167;a:5:{s:12:"station_name";s:11:"kedungjati ";s:9:"city_name";s:8:"Grobogan";s:12:"station_code";s:3:"KEJ";s:8:"latitude";s:23:"-7.16342600000000000000";s:9:"longitude";s:24:"110.63500600000000000000";}i:168;a:5:{s:12:"station_name";s:9:"kemayoran";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"KMO";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:169;a:5:{s:12:"station_name";s:6:"kemiri";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"KMR";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:170;a:5:{s:12:"station_name";s:9:"kemranjen";s:9:"city_name";s:8:"Banyumas";s:12:"station_code";s:2:"KJ";s:8:"latitude";s:23:"-7.62279700000000000000";s:9:"longitude";s:24:"109.31117500000000000000";}i:171;a:5:{s:12:"station_name";s:8:"kepanjen";s:9:"city_name";s:6:"Malang";s:12:"station_code";s:3:"KPN";s:8:"latitude";s:23:"-8.13296700000000000000";s:9:"longitude";s:24:"112.57289200000000000000";}i:172;a:5:{s:12:"station_name";s:9:"kertapati";s:9:"city_name";s:9:"Palembang";s:12:"station_code";s:3:"KPT";s:8:"latitude";s:23:"-3.04444000000000000000";s:9:"longitude";s:24:"104.72959800000000000000";}i:173;a:5:{s:12:"station_name";s:12:"kertasemaya ";s:9:"city_name";s:9:"Indramayu";s:12:"station_code";s:3:"KTM";s:8:"latitude";s:23:"-6.51668600000000000000";s:9:"longitude";s:24:"108.34896000000000000000";}i:174;a:5:{s:12:"station_name";s:9:"kertosono";s:9:"city_name";s:7:"Nganjuk";s:12:"station_code";s:3:"KTS";s:8:"latitude";s:23:"-7.59244100000000000000";s:9:"longitude";s:24:"112.10324200000000000000";}i:175;a:5:{s:12:"station_name";s:8:"kesamben";s:9:"city_name";s:6:"Blitar";s:12:"station_code";s:3:"KSB";s:8:"latitude";s:23:"-8.14607300000000000000";s:9:"longitude";s:24:"112.35406600000000000000";}i:176;a:5:{s:12:"station_name";s:12:"ketanggungan";s:9:"city_name";s:6:"Brebes";s:12:"station_code";s:3:"KGG";s:8:"latitude";s:23:"-6.94034700000000000000";s:9:"longitude";s:24:"108.89310500000000000000";}i:177;a:5:{s:12:"station_name";s:18:"ketanggungan barat";s:9:"city_name";s:6:"Brebes";s:12:"station_code";s:3:"KGB";s:8:"latitude";s:23:"-6.92919600000000000000";s:9:"longitude";s:24:"108.85627300000000000000";}i:178;a:5:{s:12:"station_name";s:8:"ketapang";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"KTP";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:179;a:5:{s:12:"station_name";s:12:"kiaracondong";s:9:"city_name";s:7:"Bandung";s:12:"station_code";s:3:"KAC";s:8:"latitude";s:23:"-6.92530300000000000000";s:9:"longitude";s:24:"107.64650500000000000000";}i:180;a:5:{s:12:"station_name";s:7:"kisaran";s:9:"city_name";s:6:"Asahan";s:12:"station_code";s:3:"KIS";s:8:"latitude";s:22:"2.98617700000000000000";s:9:"longitude";s:23:"99.61968400000000000000";}i:181;a:5:{s:12:"station_name";s:6:"klakah";s:9:"city_name";s:8:"Lumajang";s:12:"station_code";s:2:"KK";s:8:"latitude";s:23:"-7.99319200000000000000";s:9:"longitude";s:24:"113.25487400000000000000";}i:182;a:5:{s:12:"station_name";s:5:"klari";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"KLI";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:183;a:5:{s:12:"station_name";s:6:"klaten";s:9:"city_name";s:6:"Klaten";s:12:"station_code";s:2:"KT";s:8:"latitude";s:23:"-7.70440000000000000000";s:9:"longitude";s:24:"110.59859300000000000000";}i:184;a:5:{s:12:"station_name";s:7:"kosambi";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"KOS";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:185;a:5:{s:12:"station_name";s:8:"kotabumi";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"KB";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:186;a:5:{s:12:"station_name";s:10:"kotapadang";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"KOP";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:187;a:5:{s:12:"station_name";s:5:"kotok";s:9:"city_name";s:6:"Jember";s:12:"station_code";s:3:"KTK";s:8:"latitude";s:23:"-8.12023200000000000000";s:9:"longitude";s:24:"113.77569100000000000000";}i:188;a:5:{s:12:"station_name";s:8:"kradenan";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"KNN";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:189;a:5:{s:12:"station_name";s:4:"kras";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"KRS";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:190;a:5:{s:12:"station_name";s:8:"krenceng";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"KEN";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:191;a:5:{s:12:"station_name";s:9:"krengseng";s:9:"city_name";s:6:"Batang";s:12:"station_code";s:3:"KNS";s:8:"latitude";s:23:"-6.94690700000000000000";s:9:"longitude";s:24:"110.02354900000000000000";}i:192;a:5:{s:12:"station_name";s:6:"kretek";s:9:"city_name";s:6:"Brebes";s:12:"station_code";s:3:"KRT";s:8:"latitude";s:23:"-7.30606900000000000000";s:9:"longitude";s:24:"109.04303300000000000000";}i:193;a:5:{s:12:"station_name";s:5:"krian";s:9:"city_name";s:8:"Sidoarjo";s:12:"station_code";s:3:"KRN";s:8:"latitude";s:23:"-7.41045200000000000000";s:9:"longitude";s:24:"112.58615100000000000000";}i:194;a:5:{s:12:"station_name";s:5:"kroya";s:9:"city_name";s:7:"Cilacap";s:12:"station_code";s:3:"KYA";s:8:"latitude";s:23:"-7.63298400000000000000";s:9:"longitude";s:24:"109.24522500000000000000";}i:195;a:5:{s:12:"station_name";s:9:"kuraitaji";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"KI";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:196;a:5:{s:12:"station_name";s:8:"kutoarjo";s:9:"city_name";s:9:"Purworejo";s:12:"station_code";s:3:"KTA";s:8:"latitude";s:23:"-7.72260100000000000000";s:9:"longitude";s:24:"109.90812800000000000000";}i:197;a:5:{s:12:"station_name";s:12:"kutowinangun";s:9:"city_name";s:7:"Kebumen";s:12:"station_code";s:3:"KWN";s:8:"latitude";s:23:"-7.72094300000000000000";s:9:"longitude";s:24:"109.73837600000000000000";}i:198;a:5:{s:12:"station_name";s:10:"labuanratu";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"LAR";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:199;a:5:{s:12:"station_name";s:5:"lahat";s:9:"city_name";s:5:"Lahat";s:12:"station_code";s:2:"LT";s:8:"latitude";s:23:"-3.78353900000000000000";s:9:"longitude";s:24:"103.54986500000000000000";}i:200;a:5:{s:12:"station_name";s:8:"lamongan";s:9:"city_name";s:8:"Lamongan";s:12:"station_code";s:3:"LMG";s:8:"latitude";s:23:"-7.11395600000000000000";s:9:"longitude";s:24:"112.41573800000000000000";}i:201;a:5:{s:12:"station_name";s:8:"lampegan";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"LP";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:202;a:5:{s:12:"station_name";s:7:"langen ";s:9:"city_name";s:6:"Banjar";s:12:"station_code";s:2:"LN";s:8:"latitude";s:23:"-7.36425400000000000000";s:9:"longitude";s:24:"108.62148300000000000000";}i:203;a:5:{s:12:"station_name";s:9:"larangan ";s:9:"city_name";s:6:"Brebes";s:12:"station_code";s:2:"LR";s:8:"latitude";s:23:"-6.98981500000000000000";s:9:"longitude";s:24:"108.94798300000000000000";}i:204;a:5:{s:12:"station_name";s:8:"larangan";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"LRA";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:205;a:5:{s:12:"station_name";s:7:"lawang ";s:9:"city_name";s:6:"Malang";s:12:"station_code";s:2:"LW";s:8:"latitude";s:23:"-7.83611000000000000000";s:9:"longitude";s:24:"112.69781800000000000000";}i:206;a:5:{s:12:"station_name";s:10:"lebakjero ";s:9:"city_name";s:7:"Bandung";s:12:"station_code";s:3:"LBJ";s:8:"latitude";s:23:"-7.02930000000000000000";s:9:"longitude";s:24:"107.89715800000000000000";}i:207;a:5:{s:12:"station_name";s:6:"lebeng";s:9:"city_name";s:7:"Cilacap";s:12:"station_code";s:3:"LBG";s:8:"latitude";s:23:"-7.62039900000000000000";s:9:"longitude";s:24:"109.07698600000000000000";}i:208;a:5:{s:12:"station_name";s:5:"leces";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"LEC";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:209;a:5:{s:12:"station_name";s:9:"ledokombo";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"LDO";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:210;a:5:{s:12:"station_name";s:5:"leles";s:9:"city_name";s:5:"Garut";s:12:"station_code";s:2:"LL";s:8:"latitude";s:23:"-7.11209300000000000000";s:9:"longitude";s:24:"107.88385400000000000000";}i:211;a:5:{s:12:"station_name";s:10:"lemahabang";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"LMB";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:212;a:5:{s:12:"station_name";s:11:"lempuyangan";s:9:"city_name";s:10:"Yogyakarta";s:12:"station_code";s:3:"LPN";s:8:"latitude";s:23:"-7.79019100000000000000";s:9:"longitude";s:24:"110.37496400000000000000";}i:213;a:5:{s:12:"station_name";s:11:"leuwi goong";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"LO";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:214;a:5:{s:12:"station_name";s:11:"lidah tanah";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"LDT";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:215;a:5:{s:12:"station_name";s:9:"limapuluh";s:9:"city_name";s:9:"Batu Bara";s:12:"station_code";s:3:"LMP";s:8:"latitude";s:22:"3.22278700000000000000";s:9:"longitude";s:23:"99.42249300000000000000";}i:216;a:5:{s:12:"station_name";s:10:"linggapura";s:9:"city_name";s:6:"Brebes";s:12:"station_code";s:2:"LG";s:8:"latitude";s:23:"-7.19804300000000000000";s:9:"longitude";s:24:"109.02341700000000000000";}i:217;a:5:{s:12:"station_name";s:6:"losari";s:9:"city_name";s:7:"Cirebon";s:12:"station_code";s:3:"LOS";s:8:"latitude";s:23:"-6.81676700000000000000";s:9:"longitude";s:24:"108.80272500000000000000";}i:218;a:5:{s:12:"station_name";s:11:"lubuk alung";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"LA";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:219;a:5:{s:12:"station_name";s:13:"lubuk linggau";s:9:"city_name";s:13:"Lubuk Linggau";s:12:"station_code";s:3:"LLG";s:8:"latitude";s:23:"-3.25496400000000000000";s:9:"longitude";s:24:"102.85448700000000000000";}i:220;a:5:{s:12:"station_name";s:10:"lubukpakam";s:9:"city_name";s:12:"Deli Serdang";s:12:"station_code";s:3:"LBP";s:8:"latitude";s:22:"3.55248500000000000000";s:9:"longitude";s:23:"98.85592500000000000000";}i:221;a:5:{s:12:"station_name";s:10:"lubukrukam";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"LRM";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:222;a:5:{s:12:"station_name";s:6:"luwung";s:9:"city_name";s:7:"Cirebon";s:12:"station_code";s:3:"LWG";s:8:"latitude";s:23:"-6.77160700000000000000";s:9:"longitude";s:24:"108.59423200000000000000";}i:223;a:5:{s:12:"station_name";s:6:"madiun";s:9:"city_name";s:6:"Madiun";s:12:"station_code";s:2:"MN";s:8:"latitude";s:23:"-7.61896600000000000000";s:9:"longitude";s:24:"111.52564500000000000000";}i:224;a:5:{s:12:"station_name";s:6:"maguwo";s:9:"city_name";s:6:"Sleman";s:12:"station_code";s:3:"MGW";s:8:"latitude";s:23:"-7.77690400000000000000";s:9:"longitude";s:24:"110.43030000000000000000";}i:225;a:5:{s:12:"station_name";s:4:"maja";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"MJ";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:226;a:5:{s:12:"station_name";s:6:"malang";s:9:"city_name";s:6:"Malang";s:12:"station_code";s:2:"ML";s:8:"latitude";s:23:"-7.97772000000000000000";s:9:"longitude";s:24:"112.63705600000000000000";}i:227;a:5:{s:12:"station_name";s:17:"malang kota lama ";s:9:"city_name";s:6:"Malang";s:12:"station_code";s:3:"MLK";s:8:"latitude";s:23:"-7.99518500000000000000";s:9:"longitude";s:24:"112.63162700000000000000";}i:228;a:5:{s:12:"station_name";s:7:"malasan";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"MLS";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:229;a:5:{s:12:"station_name";s:10:"manggarai ";s:9:"city_name";s:15:"Jakarta Selatan";s:12:"station_code";s:3:"MRI";s:8:"latitude";s:23:"-6.21042100000000000000";s:9:"longitude";s:24:"106.84994300000000000000";}i:230;a:5:{s:12:"station_name";s:8:"mangkang";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"MKG";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:231;a:5:{s:12:"station_name";s:9:"manonjaya";s:9:"city_name";s:11:"Tasikmalaya";s:12:"station_code";s:3:"MNJ";s:8:"latitude";s:23:"-7.35314600000000000000";s:9:"longitude";s:24:"108.30269700000000000000";}i:232;a:5:{s:12:"station_name";s:4:"maos";s:9:"city_name";s:7:"Cilacap";s:12:"station_code";s:2:"MA";s:8:"latitude";s:23:"-7.61906400000000000000";s:9:"longitude";s:24:"109.13939600000000000000";}i:233;a:5:{s:12:"station_name";s:6:"marbau";s:9:"city_name";s:12:"Labuhan Batu";s:12:"station_code";s:3:"MBU";s:8:"latitude";s:22:"2.23858100000000000000";s:9:"longitude";s:23:"99.77639400000000000000";}i:234;a:5:{s:12:"station_name";s:9:"martapura";s:9:"city_name";s:23:"Ogan Komering Ulu Timur";s:12:"station_code";s:2:"MP";s:8:"latitude";s:23:"-4.35565400000000000000";s:9:"longitude";s:24:"104.30179600000000000000";}i:235;a:5:{s:12:"station_name";s:7:"masaran";s:9:"city_name";s:6:"Sragen";s:12:"station_code";s:3:"MSR";s:8:"latitude";s:23:"-7.47063400000000000000";s:9:"longitude";s:24:"110.92974900000000000000";}i:236;a:5:{s:12:"station_name";s:6:"maseng";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"MSG";s:8:"latitude";s:23:"-6.70254000000000000000";s:9:"longitude";s:24:"106.81458600000000000000";}i:237;a:5:{s:12:"station_name";s:7:"maswati";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"MSI";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:238;a:5:{s:12:"station_name";s:5:"medan";s:9:"city_name";s:5:"Medan";s:12:"station_code";s:3:"MDN";s:8:"latitude";s:22:"3.59209400000000000000";s:9:"longitude";s:23:"98.67969300000000000000";}i:239;a:5:{s:12:"station_name";s:8:"meluwung";s:9:"city_name";s:7:"Cilacap";s:12:"station_code";s:3:"MLW";s:8:"latitude";s:23:"-7.65193800000000000000";s:9:"longitude";s:24:"109.17350300000000000000";}i:240;a:5:{s:12:"station_name";s:12:"membang muda";s:9:"city_name";s:12:"Labuhan Batu";s:12:"station_code";s:3:"MBM";s:8:"latitude";s:23:"99.66075900000000000000";s:9:"longitude";s:22:"2.54265000000000000000";}i:241;a:5:{s:12:"station_name";s:5:"merak";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"MER";s:8:"latitude";s:23:"-5.93012800000000000000";s:9:"longitude";s:24:"105.99684100000000000000";}i:242;a:5:{s:12:"station_name";s:9:"minggiran";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"MGN";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:243;a:5:{s:12:"station_name";s:9:"mojokerto";s:9:"city_name";s:9:"Mojokerto";s:12:"station_code";s:2:"MR";s:8:"latitude";s:23:"-7.47238400000000000000";s:9:"longitude";s:24:"112.43379800000000000000";}i:244;a:5:{s:12:"station_name";s:6:"mrawan";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"MRW";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:245;a:5:{s:12:"station_name";s:10:"muara enim";s:9:"city_name";s:10:"Muara Enim";s:12:"station_code";s:2:"ME";s:8:"latitude";s:23:"-3.66812700000000000000";s:9:"longitude";s:24:"103.75793000000000000000";}i:246;a:5:{s:12:"station_name";s:11:"muarasaling";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"MSL";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:247;a:5:{s:12:"station_name";s:6:"nagreg";s:9:"city_name";s:7:"Bandung";s:12:"station_code";s:2:"NG";s:8:"latitude";s:23:"-7.01905600000000000000";s:9:"longitude";s:24:"107.88587100000000000000";}i:248;a:5:{s:12:"station_name";s:10:"negararatu";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"NRR";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:249;a:5:{s:12:"station_name";s:11:"negeriagung";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"NGN";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:250;a:5:{s:12:"station_name";s:10:"ngadiluwih";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"NDL";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:251;a:5:{s:12:"station_name";s:7:"nganjuk";s:9:"city_name";s:7:"Nganjuk";s:12:"station_code";s:2:"NJ";s:8:"latitude";s:23:"-7.59941700000000000000";s:9:"longitude";s:24:"111.91135200000000000000";}i:252;a:5:{s:12:"station_name";s:7:"ngebruk";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"NB";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:253;a:5:{s:12:"station_name";s:8:"ngrombro";s:9:"city_name";s:8:"Grobogan";s:12:"station_code";s:3:"NBO";s:8:"latitude";s:23:"-7.13276700000000000000";s:9:"longitude";s:24:"110.88433900000000000000";}i:254;a:5:{s:12:"station_name";s:6:"ngunut";s:9:"city_name";s:11:"Tulungagung";s:12:"station_code";s:2:"NT";s:8:"latitude";s:23:"-8.10327000000000000000";s:9:"longitude";s:24:"112.00852300000000000000";}i:255;a:5:{s:12:"station_name";s:5:"notog";s:9:"city_name";s:8:"Banyumas";s:12:"station_code";s:3:"NTG";s:8:"latitude";s:23:"-7.49103700000000000000";s:9:"longitude";s:24:"109.21397200000000000000";}i:256;a:5:{s:12:"station_name";s:10:"padalarang";s:9:"city_name";s:13:"Bandung Barat";s:12:"station_code";s:3:"PDL";s:8:"latitude";s:23:"-6.84292500000000000000";s:9:"longitude";s:24:"107.49731500000000000000";}i:257;a:5:{s:12:"station_name";s:6:"padang";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"PD";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:258;a:5:{s:12:"station_name";s:13:"padanghalaban";s:9:"city_name";s:12:"Labuhan Batu";s:12:"station_code";s:3:"PHA";s:8:"latitude";s:22:"2.26739800000000000000";s:9:"longitude";s:24:"100.07926900000000000000";}i:259;a:5:{s:12:"station_name";s:11:"pagergunung";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"PGG";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:260;a:5:{s:12:"station_name";s:9:"pakishaji";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"PSI";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:261;a:5:{s:12:"station_name";s:8:"paledang";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"PLG";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:262;a:5:{s:12:"station_name";s:8:"palmerah";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"PLM";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:263;a:5:{s:12:"station_name";s:8:"pamingke";s:9:"city_name";s:12:"Labuhan Batu";s:12:"station_code";s:3:"PME";s:8:"latitude";s:22:"2.23995300000000000000";s:9:"longitude";s:23:"99.77989200000000000000";}i:264;a:5:{s:12:"station_name";s:10:"paninjawan";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"PNW";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:265;a:5:{s:12:"station_name";s:11:"panunggalan";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"PNL";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:266;a:5:{s:12:"station_name";s:5:"papar";s:9:"city_name";s:6:"Kediri";s:12:"station_code";s:3:"PPR";s:8:"latitude";s:23:"-7.70291100000000000000";s:9:"longitude";s:24:"112.10379500000000000000";}i:267;a:5:{s:12:"station_name";s:8:"pariaman";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"PMN";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:268;a:5:{s:12:"station_name";s:5:"paron";s:9:"city_name";s:5:"Ngawi";s:12:"station_code";s:2:"PA";s:8:"latitude";s:23:"-7.43656000000000000000";s:9:"longitude";s:24:"111.39136800000000000000";}i:269;a:5:{s:12:"station_name";s:11:"parung kuda";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"PRK";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:270;a:5:{s:12:"station_name";s:14:"parung panjang";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"PRP";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:271;a:5:{s:12:"station_name";s:11:"pasar senen";s:9:"city_name";s:13:"Jakarta Pusat";s:12:"station_code";s:3:"PSE";s:8:"latitude";s:23:"-6.17447600000000000000";s:9:"longitude";s:24:"106.84446600000000000000";}i:272;a:5:{s:12:"station_name";s:8:"pasuruan";s:9:"city_name";s:8:"Pasuruan";s:12:"station_code";s:2:"PS";s:8:"latitude";s:23:"-7.63839100000000000000";s:9:"longitude";s:24:"112.90726700000000000000";}i:273;a:5:{s:12:"station_name";s:9:"patuguran";s:9:"city_name";s:6:"Brebes";s:12:"station_code";s:3:"PAT";s:8:"latitude";s:23:"-7.30642000000000000000";s:9:"longitude";s:24:"109.04345900000000000000";}i:274;a:5:{s:12:"station_name";s:10:"pauhkambar";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"PAK";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:275;a:5:{s:12:"station_name";s:11:"pegadenbaru";s:9:"city_name";s:6:"Subang";s:12:"station_code";s:3:"PGB";s:8:"latitude";s:23:"-6.45394600000000000000";s:9:"longitude";s:24:"107.81567800000000000000";}i:276;a:5:{s:12:"station_name";s:10:"pekalongan";s:9:"city_name";s:10:"Pekalongan";s:12:"station_code";s:2:"PK";s:8:"latitude";s:23:"-6.89002500000000000000";s:9:"longitude";s:24:"109.64916300000000000000";}i:277;a:5:{s:12:"station_name";s:8:"pemalang";s:9:"city_name";s:8:"Pemalang";s:12:"station_code";s:3:"PML";s:8:"latitude";s:23:"-6.89070400000000000000";s:9:"longitude";s:24:"109.39060600000000000000";}i:278;a:5:{s:12:"station_name";s:10:"perbaungan";s:9:"city_name";s:15:"Serdang Bedagai";s:12:"station_code";s:3:"PBA";s:8:"latitude";s:22:"3.35200600000000000000";s:9:"longitude";s:23:"99.02389500000000000000";}i:279;a:5:{s:12:"station_name";s:9:"perlanaan";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"PRA";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:280;a:5:{s:12:"station_name";s:9:"petarukan";s:9:"city_name";s:8:"Pemalang";s:12:"station_code";s:3:"PTA";s:8:"latitude";s:23:"-6.89703000000000000000";s:9:"longitude";s:24:"109.44620800000000000000";}i:281;a:5:{s:12:"station_name";s:10:"peterongan";s:9:"city_name";s:7:"Jombang";s:12:"station_code";s:3:"PTR";s:8:"latitude";s:23:"-7.53914700000000000000";s:9:"longitude";s:24:"112.27842800000000000000";}i:282;a:5:{s:12:"station_name";s:7:"plabuan";s:9:"city_name";s:6:"Batang";s:12:"station_code";s:3:"PLB";s:8:"latitude";s:23:"-6.93758800000000000000";s:9:"longitude";s:24:"109.96391800000000000000";}i:283;a:5:{s:12:"station_name";s:6:"plered";s:9:"city_name";s:7:"Cirebon";s:12:"station_code";s:3:"PLD";s:8:"latitude";s:23:"-6.70618700000000000000";s:9:"longitude";s:24:"108.51096500000000000000";}i:284;a:5:{s:12:"station_name";s:8:"pohgajih";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"PGJ";s:8:"latitude";s:23:"-8.15702300000000000000";s:9:"longitude";s:24:"112.42014500000000000000";}i:285;a:5:{s:12:"station_name";s:12:"pondok ranji";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"PDJ";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:286;a:5:{s:12:"station_name";s:6:"porong";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"PR";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:287;a:5:{s:12:"station_name";s:10:"prabumulih";s:9:"city_name";s:10:"Prabumulih";s:12:"station_code";s:3:"PBM";s:8:"latitude";s:23:"-3.44085600000000000000";s:9:"longitude";s:24:"104.23553500000000000000";}i:288;a:5:{s:12:"station_name";s:7:"prembun";s:9:"city_name";s:7:"Kebumen";s:12:"station_code";s:3:"PRB";s:8:"latitude";s:23:"-7.72329200000000000000";s:9:"longitude";s:24:"109.79652600000000000000";}i:289;a:5:{s:12:"station_name";s:11:"probolinggo";s:9:"city_name";s:11:"Probolinggo";s:12:"station_code";s:2:"PB";s:8:"latitude";s:23:"-7.74319400000000000000";s:9:"longitude";s:24:"113.21538300000000000000";}i:290;a:5:{s:12:"station_name";s:6:"prupuk";s:9:"city_name";s:5:"Tegal";s:12:"station_code";s:3:"PPK";s:8:"latitude";s:23:"-7.13519500000000000000";s:9:"longitude";s:24:"108.96698400000000000000";}i:291;a:5:{s:12:"station_name";s:5:"pucuk";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"PC";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:292;a:5:{s:12:"station_name";s:8:"puluraja";s:9:"city_name";s:10:"Simalungun";s:12:"station_code";s:3:"PUR";s:8:"latitude";s:22:"2.97449900000000000000";s:9:"longitude";s:23:"99.08277500000000000000";}i:293;a:5:{s:12:"station_name";s:10:"purwakarta";s:9:"city_name";s:10:"Purwakarta";s:12:"station_code";s:3:"PWK";s:8:"latitude";s:23:"-6.55858200000000000000";s:9:"longitude";s:24:"107.45056500000000000000";}i:294;a:5:{s:12:"station_name";s:9:"purwoasri";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"PWA";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:295;a:5:{s:12:"station_name";s:10:"purwokerto";s:9:"city_name";s:8:"Banyumas";s:12:"station_code";s:3:"PWT";s:8:"latitude";s:23:"-7.43145400000000000000";s:9:"longitude";s:24:"109.24753200000000000000";}i:296;a:5:{s:12:"station_name";s:9:"purwosari";s:9:"city_name";s:16:"Surakarta (Solo)";s:12:"station_code";s:3:"PWS";s:8:"latitude";s:23:"-7.56402400000000000000";s:9:"longitude";s:24:"110.80092800000000000000";}i:297;a:5:{s:12:"station_name";s:9:"rajapolah";s:9:"city_name";s:11:"Tasikmalaya";s:12:"station_code";s:3:"RJP";s:8:"latitude";s:23:"-7.21950600000000000000";s:9:"longitude";s:24:"108.19095000000000000000";}i:298;a:5:{s:12:"station_name";s:9:"rambipuji";s:9:"city_name";s:6:"Jember";s:12:"station_code";s:3:"RBP";s:8:"latitude";s:23:"-8.20268700000000000000";s:9:"longitude";s:24:"113.61602400000000000000";}i:299;a:5:{s:12:"station_name";s:6:"rampah";s:9:"city_name";s:15:"Serdang Bedagai";s:12:"station_code";s:3:"RPH";s:8:"latitude";s:22:"3.48934800000000000000";s:9:"longitude";s:23:"99.12783600000000000000";}i:300;a:5:{s:12:"station_name";s:9:"rancaekek";s:9:"city_name";s:7:"Bandung";s:12:"station_code";s:3:"RCK";s:8:"latitude";s:23:"-6.96531600000000000000";s:9:"longitude";s:24:"107.75723200000000000000";}i:301;a:5:{s:12:"station_name";s:8:"randegan";s:9:"city_name";s:8:"Banyumas";s:12:"station_code";s:3:"RDG";s:8:"latitude";s:24:"109.04874800000000000000";s:9:"longitude";s:23:"-7.53510500000000000000";}i:302;a:5:{s:12:"station_name";s:8:"randegan";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"RDN";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:303;a:5:{s:12:"station_name";s:10:"randuagung";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"RDA";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:304;a:5:{s:12:"station_name";s:12:"randublatung";s:9:"city_name";s:5:"Blora";s:12:"station_code";s:3:"RBG";s:8:"latitude";s:23:"-7.21224200000000000000";s:9:"longitude";s:24:"111.38484500000000000000";}i:305;a:5:{s:12:"station_name";s:13:"rangkasbitung";s:9:"city_name";s:5:"Lebak";s:12:"station_code";s:2:"RK";s:8:"latitude";s:23:"-6.35272200000000000000";s:9:"longitude";s:24:"106.25148800000000000000";}i:306;a:5:{s:12:"station_name";s:13:"rantau prapat";s:9:"city_name";s:12:"Labuhan Batu";s:12:"station_code";s:3:"RAP";s:8:"latitude";s:22:"2.09931400000000000000";s:9:"longitude";s:23:"99.83104700000000000000";}i:307;a:5:{s:12:"station_name";s:8:"rejosari";s:9:"city_name";s:15:"Lampung Selatan";s:12:"station_code";s:3:"RJS";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:308;a:5:{s:12:"station_name";s:10:"rejotangan";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"RJ";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:309;a:5:{s:12:"station_name";s:6:"rendeh";s:9:"city_name";s:13:"Bandung Barat";s:12:"station_code";s:2:"RH";s:8:"latitude";s:23:"-6.73670300000000000000";s:9:"longitude";s:24:"107.39867400000000000000";}i:310;a:5:{s:12:"station_name";s:6:"rengas";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"RGS";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:311;a:5:{s:12:"station_name";s:9:"rogojampi";s:9:"city_name";s:10:"Banyuwangi";s:12:"station_code";s:3:"RGP";s:8:"latitude";s:23:"-8.33144400000000000000";s:9:"longitude";s:24:"114.30483700000000000000";}i:312;a:5:{s:12:"station_name";s:6:"sadang";s:9:"city_name";s:10:"Purwakarta";s:12:"station_code";s:3:"SAD";s:8:"latitude";s:23:"-7.53114800000000000000";s:9:"longitude";s:24:"109.71352800000000000000";}i:313;a:5:{s:12:"station_name";s:5:"salem";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"SLM";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:314;a:5:{s:12:"station_name";s:7:"saradan";s:9:"city_name";s:6:"Madiun";s:12:"station_code";s:3:"SRD";s:8:"latitude";s:23:"-7.54803800000000000000";s:9:"longitude";s:24:"111.73207300000000000000";}i:315;a:5:{s:12:"station_name";s:9:"sasaksaat";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"SKT";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:316;a:5:{s:12:"station_name";s:9:"saungnaga";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"SNA";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:317;a:5:{s:12:"station_name";s:6:"sedadi";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"SDI";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:318;a:5:{s:12:"station_name";s:12:"seibejangkar";s:9:"city_name";s:9:"Batu Bara";s:12:"station_code";s:3:"SBJ";s:8:"latitude";s:22:"2.97389900000000000000";s:9:"longitude";s:23:"99.61200700000000000000";}i:319;a:5:{s:12:"station_name";s:15:"semarang poncol";s:9:"city_name";s:8:"Semarang";s:12:"station_code";s:3:"SMC";s:8:"latitude";s:23:"-6.97200400000000000000";s:9:"longitude";s:24:"110.41518300000000000000";}i:320;a:5:{s:12:"station_name";s:15:"semarang tawang";s:9:"city_name";s:8:"Semarang";s:12:"station_code";s:3:"SMT";s:8:"latitude";s:23:"-6.96525700000000000000";s:9:"longitude";s:24:"110.42729600000000000000";}i:321;a:5:{s:12:"station_name";s:7:"sembung";s:9:"city_name";s:7:"Jombang";s:12:"station_code";s:3:"SMB";s:8:"latitude";s:23:"-7.57737100000000000000";s:9:"longitude";s:24:"112.17811300000000000000";}i:322;a:5:{s:12:"station_name";s:8:"sempolan";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"SPL";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:323;a:5:{s:12:"station_name";s:7:"sentolo";s:9:"city_name";s:11:"Kulon Progo";s:12:"station_code";s:3:"STL";s:8:"latitude";s:23:"-7.82699000000000000000";s:9:"longitude";s:24:"110.22445700000000000000";}i:324;a:5:{s:12:"station_name";s:9:"sepanjang";s:9:"city_name";s:8:"Sidoarjo";s:12:"station_code";s:3:"SPJ";s:8:"latitude";s:23:"-7.34714400000000000000";s:9:"longitude";s:24:"112.69779500000000000000";}i:325;a:5:{s:12:"station_name";s:6:"serang";s:9:"city_name";s:6:"Serang";s:12:"station_code";s:2:"SG";s:8:"latitude";s:23:"-6.11234400000000000000";s:9:"longitude";s:24:"106.15863800000000000000";}i:326;a:5:{s:12:"station_name";s:7:"serpong";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"SRP";s:8:"latitude";s:23:"-6.32009900000000000000";s:9:"longitude";s:24:"106.66558800000000000000";}i:327;a:5:{s:12:"station_name";s:7:"siantar";s:9:"city_name";s:16:"Pematang Siantar";s:12:"station_code";s:3:"SIR";s:8:"latitude";s:22:"2.95932700000000000000";s:9:"longitude";s:23:"99.06307300000000000000";}i:328;a:5:{s:12:"station_name";s:8:"sidareja";s:9:"city_name";s:7:"Cilacap";s:12:"station_code";s:3:"SDR";s:8:"latitude";s:23:"-7.47847200000000000000";s:9:"longitude";s:24:"108.79352000000000000000";}i:329;a:5:{s:12:"station_name";s:8:"sidoarjo";s:9:"city_name";s:8:"Sidoarjo";s:12:"station_code";s:3:"SDA";s:8:"latitude";s:23:"-7.45652000000000000000";s:9:"longitude";s:24:"112.71295700000000000000";}i:330;a:5:{s:12:"station_name";s:8:"sikampuh";s:9:"city_name";s:7:"Cilacap";s:12:"station_code";s:3:"SKP";s:8:"latitude";s:23:"-7.63199000000000000000";s:9:"longitude";s:24:"109.20133000000000000000";}i:331;a:5:{s:12:"station_name";s:11:"sindanglaut";s:9:"city_name";s:7:"Cirebon";s:12:"station_code";s:3:"SDU";s:8:"latitude";s:23:"-6.83793400000000000000";s:9:"longitude";s:24:"108.61217000000000000000";}i:332;a:5:{s:12:"station_name";s:10:"singojuruh";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"SGJ";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:333;a:5:{s:12:"station_name";s:9:"singosari";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"SGS";s:8:"latitude";s:23:"-7.89683900000000000000";s:9:"longitude";s:24:"112.66473300000000000000";}i:334;a:5:{s:12:"station_name";s:5:"slawi";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"SLW";s:8:"latitude";s:23:"-6.98192200000000000000";s:9:"longitude";s:24:"109.13714500000000000000";}i:335;a:5:{s:12:"station_name";s:11:"solobalapan";s:9:"city_name";s:16:"Surakarta (Solo)";s:12:"station_code";s:3:"SLO";s:8:"latitude";s:23:"-7.55675500000000000000";s:9:"longitude";s:24:"110.82139900000000000000";}i:336;a:5:{s:12:"station_name";s:10:"solojebres";s:9:"city_name";s:16:"Surakarta (Solo)";s:12:"station_code";s:2:"SK";s:8:"latitude";s:23:"-7.56461700000000000000";s:9:"longitude";s:24:"110.85717100000000000000";}i:337;a:5:{s:12:"station_name";s:7:"songgom";s:9:"city_name";s:6:"Brebes";s:12:"station_code";s:3:"SGG";s:8:"latitude";s:23:"-7.02514700000000000000";s:9:"longitude";s:24:"108.98834500000000000000";}i:338;a:5:{s:12:"station_name";s:6:"sragen";s:9:"city_name";s:6:"Sragen";s:12:"station_code";s:2:"SR";s:8:"latitude";s:23:"-7.42910300000000000000";s:9:"longitude";s:24:"111.01709200000000000000";}i:339;a:5:{s:12:"station_name";s:5:"sragi";s:9:"city_name";s:10:"Pekalongan";s:12:"station_code";s:3:"SRI";s:8:"latitude";s:23:"-6.92451000000000000000";s:9:"longitude";s:24:"109.56547000000000000000";}i:340;a:5:{s:12:"station_name";s:6:"srowot";s:9:"city_name";s:6:"Klaten";s:12:"station_code";s:3:"SWT";s:8:"latitude";s:23:"-7.74165300000000000000";s:9:"longitude";s:24:"110.56765100000000000000";}i:341;a:5:{s:12:"station_name";s:7:"sruweng";s:9:"city_name";s:7:"Kebumen";s:12:"station_code";s:3:"SRW";s:8:"latitude";s:23:"-7.65693600000000000000";s:9:"longitude";s:24:"109.60168500000000000000";}i:342;a:5:{s:12:"station_name";s:8:"sudimara";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"SDM";s:8:"latitude";s:23:"-6.29686800000000000000";s:9:"longitude";s:24:"106.71266700000000000000";}i:343;a:5:{s:12:"station_name";s:8:"sukabumi";s:9:"city_name";s:8:"Sukabumi";s:12:"station_code";s:2:"SI";s:8:"latitude";s:23:"-6.92714000000000000000";s:9:"longitude";s:24:"106.92279200000000000000";}i:344;a:5:{s:12:"station_name";s:8:"sukatani";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"SUT";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:345;a:5:{s:12:"station_name";s:8:"sukomoro";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"SKM";s:8:"latitude";s:23:"-7.60254200000000000000";s:9:"longitude";s:24:"111.94258000000000000000";}i:346;a:5:{s:12:"station_name";s:8:"sukorejo";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"SKJ";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:347;a:5:{s:12:"station_name";s:9:"sulusuban";s:9:"city_name";s:15:"Lampung Selatan";s:12:"station_code";s:3:"SLS";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:348;a:5:{s:12:"station_name";s:12:"sumbergempol";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"SBL";s:8:"latitude";s:23:"-8.08193800000000000000";s:9:"longitude";s:24:"111.94481300000000000000";}i:349;a:5:{s:12:"station_name";s:12:"sumberlawang";s:9:"city_name";s:6:"Sragen";s:12:"station_code";s:3:"SUM";s:8:"latitude";s:23:"-7.43592200000000000000";s:9:"longitude";s:24:"110.99410100000000000000";}i:350;a:5:{s:12:"station_name";s:12:"sumberpucung";s:9:"city_name";s:6:"Malang";s:12:"station_code";s:3:"SBP";s:8:"latitude";s:23:"-8.15838200000000000000";s:9:"longitude";s:24:"112.46356500000000000000";}i:351;a:5:{s:12:"station_name";s:10:"sumberrejo";s:9:"city_name";s:10:"Bojonegoro";s:12:"station_code";s:3:"SRJ";s:8:"latitude";s:23:"-7.17671100000000000000";s:9:"longitude";s:24:"112.00231100000000000000";}i:352;a:5:{s:12:"station_name";s:12:"sumberwadung";s:9:"city_name";s:10:"Banyuwangi";s:12:"station_code";s:3:"SWD";s:8:"latitude";s:23:"-8.30203700000000000000";s:9:"longitude";s:24:"114.10606400000000000000";}i:353;a:5:{s:12:"station_name";s:8:"sumlaran";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"SLR";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:354;a:5:{s:12:"station_name";s:8:"sumobito";s:9:"city_name";s:7:"Jombang";s:12:"station_code";s:3:"SBO";s:8:"latitude";s:23:"-7.52040600000000000000";s:9:"longitude";s:24:"112.34389200000000000000";}i:355;a:5:{s:12:"station_name";s:7:"sumpiuh";s:9:"city_name";s:8:"Banyumas";s:12:"station_code";s:3:"SPH";s:8:"latitude";s:23:"-7.61342300000000000000";s:9:"longitude";s:24:"109.35961200000000000000";}i:356;a:5:{s:12:"station_name";s:15:"surabaya gubeng";s:9:"city_name";s:8:"Surabaya";s:12:"station_code";s:3:"SGU";s:8:"latitude";s:23:"-7.26541100000000000000";s:9:"longitude";s:24:"112.75188900000000000000";}i:357;a:5:{s:12:"station_name";s:15:"surabaya gubeng";s:9:"city_name";s:1:" ";s:12:"station_code";s:4:"SGUX";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:358;a:5:{s:12:"station_name";s:13:"surabaya kota";s:9:"city_name";s:8:"Surabaya";s:12:"station_code";s:2:"SB";s:8:"latitude";s:23:"-7.24251200000000000000";s:9:"longitude";s:24:"112.74250700000000000000";}i:359;a:5:{s:12:"station_name";s:19:"surabaya pasar turi";s:9:"city_name";s:8:"Surabaya";s:12:"station_code";s:3:"SBI";s:8:"latitude";s:23:"-7.24883200000000000000";s:9:"longitude";s:24:"112.73138100000000000000";}i:360;a:5:{s:12:"station_name";s:8:"surodadi";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"SD";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:361;a:5:{s:12:"station_name";s:7:"susuhan";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"SS";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:362;a:5:{s:12:"station_name";s:6:"tabing";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"TAB";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:363;a:5:{s:12:"station_name";s:5:"talun";s:9:"city_name";s:6:"Blitar";s:12:"station_code";s:3:"TAL";s:8:"latitude";s:23:"-8.09012000000000000000";s:9:"longitude";s:24:"112.27230900000000000000";}i:364;a:5:{s:12:"station_name";s:6:"tambak";s:9:"city_name";s:8:"Banyumas";s:12:"station_code";s:3:"TBK";s:8:"latitude";s:23:"-7.62063300000000000000";s:9:"longitude";s:24:"109.40983600000000000000";}i:365;a:5:{s:12:"station_name";s:6:"tambun";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"TB";s:8:"latitude";s:23:"-6.23563500000000000000";s:9:"longitude";s:24:"106.99893700000000000000";}i:366;a:5:{s:12:"station_name";s:11:"tanah abang";s:9:"city_name";s:13:"Jakarta Pusat";s:12:"station_code";s:3:"THB";s:8:"latitude";s:23:"-6.18571800000000000000";s:9:"longitude";s:24:"106.81079900000000000000";}i:367;a:5:{s:12:"station_name";s:6:"tandes";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"TES";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:368;a:5:{s:12:"station_name";s:9:"tangerang";s:9:"city_name";s:9:"Tangerang";s:12:"station_code";s:3:"TNG";s:8:"latitude";s:23:"-6.17700400000000000000";s:9:"longitude";s:24:"106.63282900000000000000";}i:369;a:5:{s:12:"station_name";s:7:"tanggul";s:9:"city_name";s:6:"Jember";s:12:"station_code";s:3:"TGL";s:8:"latitude";s:23:"-8.18572800000000000000";s:9:"longitude";s:24:"113.45062300000000000000";}i:370;a:5:{s:12:"station_name";s:12:"tanggulangin";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"TGA";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:371;a:5:{s:12:"station_name";s:7:"tanjung";s:9:"city_name";s:6:"Brebes";s:12:"station_code";s:3:"TGN";s:8:"latitude";s:23:"-6.87491800000000000000";s:9:"longitude";s:24:"108.85537100000000000000";}i:372;a:5:{s:12:"station_name";s:13:"tanjung priuk";s:9:"city_name";s:13:"Jakarta Utara";s:12:"station_code";s:3:"TPK";s:8:"latitude";s:23:"-6.11086700000000000000";s:9:"longitude";s:24:"106.88115800000000000000";}i:373;a:5:{s:12:"station_name";s:12:"tanjungbalai";s:9:"city_name";s:13:"Tanjung Balai";s:12:"station_code";s:3:"TNB";s:8:"latitude";s:22:"2.96488800000000000000";s:9:"longitude";s:23:"99.80898900000000000000";}i:374;a:5:{s:12:"station_name";s:13:"tanjungkarang";s:9:"city_name";s:14:"Bandar Lampung";s:12:"station_code";s:3:"TNK";s:8:"latitude";s:23:"-5.41299600000000000000";s:9:"longitude";s:24:"105.23865900000000000000";}i:375;a:5:{s:12:"station_name";s:11:"tanjungrasa";s:9:"city_name";s:6:"Subang";s:12:"station_code";s:3:"TJS";s:8:"latitude";s:23:"-6.40064400000000000000";s:9:"longitude";s:24:"107.55988600000000000000";}i:376;a:5:{s:12:"station_name";s:5:"tarik";s:9:"city_name";s:8:"Sidoarjo";s:12:"station_code";s:3:"TRK";s:8:"latitude";s:23:"-7.45949600000000000000";s:9:"longitude";s:24:"112.51802400000000000000";}i:377;a:5:{s:12:"station_name";s:11:"tasikmalaya";s:9:"city_name";s:11:"Tasikmalaya";s:12:"station_code";s:3:"TSM";s:8:"latitude";s:23:"-7.32270700000000000000";s:9:"longitude";s:24:"108.22386100000000000000";}i:378;a:5:{s:12:"station_name";s:13:"tebing tinggi";s:9:"city_name";s:13:"Tebing Tinggi";s:12:"station_code";s:3:"TBI";s:8:"latitude";s:22:"3.31953100000000000000";s:9:"longitude";s:23:"99.15221200000000000000";}i:379;a:5:{s:12:"station_name";s:13:"tebing tinggi";s:9:"city_name";s:13:"Tebing Tinggi";s:12:"station_code";s:2:"TI";s:8:"latitude";s:22:"3.32109500000000000000";s:9:"longitude";s:23:"99.16478600000000000000";}i:380;a:5:{s:12:"station_name";s:5:"tegal";s:9:"city_name";s:5:"Tegal";s:12:"station_code";s:2:"TG";s:8:"latitude";s:23:"-6.87223400000000000000";s:9:"longitude";s:24:"109.13642400000000000000";}i:381;a:5:{s:12:"station_name";s:10:"tegineneng";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"TGI";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:382;a:5:{s:12:"station_name";s:6:"telawa";s:9:"city_name";s:8:"Boyolali";s:12:"station_code";s:2:"TW";s:8:"latitude";s:23:"-7.19521100000000000000";s:9:"longitude";s:24:"110.74600000000000000000";}i:383;a:5:{s:12:"station_name";s:9:"temuguruh";s:9:"city_name";s:10:"Banyuwangi";s:12:"station_code";s:3:"TGR";s:8:"latitude";s:23:"-8.33734600000000000000";s:9:"longitude";s:24:"114.15195100000000000000";}i:384;a:5:{s:12:"station_name";s:5:"tenjo";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"TEJ";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:385;a:5:{s:12:"station_name";s:6:"terisi";s:9:"city_name";s:9:"Indramayu";s:12:"station_code";s:3:"TIS";s:8:"latitude";s:23:"-6.47960000000000000000";s:9:"longitude";s:24:"108.16067900000000000000";}i:386;a:5:{s:12:"station_name";s:6:"testes";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"124";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:387;a:5:{s:12:"station_name";s:9:"tigaraksa";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"TGS";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:388;a:5:{s:12:"station_name";s:9:"tigaraksa";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"TIG";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:389;a:5:{s:12:"station_name";s:12:"tonjong baru";s:9:"city_name";s:1:" ";s:12:"station_code";s:4:"TOJB";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:390;a:5:{s:12:"station_name";s:15:"tugu yogyakarta";s:9:"city_name";s:10:"Yogyakarta";s:12:"station_code";s:2:"YK";s:8:"latitude";s:23:"-7.78910700000000000000";s:9:"longitude";s:24:"110.36408200000000000000";}i:391;a:5:{s:12:"station_name";s:8:"tulangan";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"TLN";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:392;a:5:{s:12:"station_name";s:11:"tulungagung";s:9:"city_name";s:11:"Tulungagung";s:12:"station_code";s:2:"TA";s:8:"latitude";s:23:"-8.06437100000000000000";s:9:"longitude";s:24:"111.90457100000000000000";}i:393;a:5:{s:12:"station_name";s:11:"tulungbuyut";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"TLY";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:394;a:5:{s:12:"station_name";s:7:"ujanmas";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"UJM";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:395;a:5:{s:12:"station_name";s:11:"ujungnegoro";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"UJN";s:8:"latitude";s:23:"-6.90896000000000000000";s:9:"longitude";s:24:"109.79214900000000000000";}i:396;a:5:{s:12:"station_name";s:4:"wadu";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"WDU";s:8:"latitude";s:22:"0.00000000000000000000";s:9:"longitude";s:22:"0.00000000000000000000";}i:397;a:5:{s:12:"station_name";s:9:"walantaka";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"WLT";s:8:"latitude";s:23:"-6.11192400000000000000";s:9:"longitude";s:24:"106.15831900000000000000";}i:398;a:5:{s:12:"station_name";s:9:"walikukun";s:9:"city_name";s:5:"Ngawi";s:12:"station_code";s:2:"WK";s:8:"latitude";s:23:"-7.37802800000000000000";s:9:"longitude";s:24:"111.24382500000000000000";}i:399;a:5:{s:12:"station_name";s:4:"waru";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"WR";s:8:"latitude";s:23:"-7.35260700000000000000";s:9:"longitude";s:24:"112.72926800000000000000";}i:400;a:5:{s:12:"station_name";s:9:"waruduwur";s:9:"city_name";s:7:"Cirebon";s:12:"station_code";s:3:"WDW";s:8:"latitude";s:23:"-6.78196200000000000000";s:9:"longitude";s:24:"108.60253600000000000000";}i:401;a:5:{s:12:"station_name";s:14:"warung bandrek";s:9:"city_name";s:5:"Garut";s:12:"station_code";s:2:"WB";s:8:"latitude";s:23:"-7.06765300000000000000";s:9:"longitude";s:24:"107.99609900000000000000";}i:402;a:5:{s:12:"station_name";s:5:"wates";s:9:"city_name";s:11:"Kulon Progo";s:12:"station_code";s:2:"WT";s:8:"latitude";s:23:"-7.86018300000000000000";s:9:"longitude";s:24:"110.15798100000000000000";}i:403;a:5:{s:12:"station_name";s:7:"waytuba";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"WAY";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:404;a:5:{s:12:"station_name";s:6:"weleri";s:9:"city_name";s:6:"Kendal";s:12:"station_code";s:3:"WLR";s:8:"latitude";s:23:"-6.96674800000000000000";s:9:"longitude";s:24:"110.06900100000000000000";}i:405;a:5:{s:12:"station_name";s:8:"wilangan";s:9:"city_name";s:7:"Nganjuk";s:12:"station_code";s:3:"WIL";s:8:"latitude";s:23:"-7.56254600000000000000";s:9:"longitude";s:24:"111.82913300000000000000";}i:406;a:5:{s:12:"station_name";s:6:"wlingi";s:9:"city_name";s:6:"Blitar";s:12:"station_code";s:2:"WG";s:8:"latitude";s:23:"-8.08117600000000000000";s:9:"longitude";s:24:"112.32428300000000000000";}i:407;a:5:{s:12:"station_name";s:9:"wonokerto";s:9:"city_name";s:1:" ";s:12:"station_code";s:2:"WN";s:8:"latitude";N;s:9:"longitude";s:22:"0.00000000000000000000";}i:408;a:5:{s:12:"station_name";s:9:"wonokromo";s:9:"city_name";s:8:"Surabaya";s:12:"station_code";s:2:"WO";s:8:"latitude";s:23:"-7.30197800000000000000";s:9:"longitude";s:24:"112.73917000000000000000";}i:409;a:5:{s:12:"station_name";s:10:"wonokromox";s:9:"city_name";s:1:" ";s:12:"station_code";s:3:"WOX";s:8:"latitude";s:22:"7.30199200000000000000";s:9:"longitude";s:24:"112.73918500000000000000";}i:410;a:5:{s:12:"station_name";s:8:"wonosari";s:9:"city_name";s:7:"Kebumen";s:12:"station_code";s:3:"WNS";s:8:"latitude";s:23:"-7.69445900000000000000";s:9:"longitude";s:24:"109.69679100000000000000";}}}s:12:"login_status";s:4:"true";s:8:"guest_id";s:8:"22691145";s:11:"login_email";s:21:"wida.skydev@gmail.com";s:5:"token";s:40:"f9b29ac359ca5d77755e7588751c089bf96f0dc9";}
``` 

Display all train station and their codes for use in search train API (variable d and a).

#### HTTP Request

    `GET https://api-sandbox.tiket.com/train_api/train_station?token=11b534a0394d9bb140f18bc1a87adf1a&output=json`

#### Parameters
  
Name | Description | Format | Default | Mandatory  
---- | ----------- | ------ | ------- | ---------
token | for saving transaction that done by user | CHAR(128) |  | TRUE  


## Get Train Seat Map

```xml
 <tiket>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.1222</elapsetime>
    <memoryusage>4.66MB</memoryusage>
    <unix_timestamp>1435115652</unix_timestamp>
    <confirm>success</confirm>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <output_type>xml</output_type>
  <result>
    <train_schedule_id>34049</train_schedule_id>
    <departure_station>GMR</departure_station>
    <departure_station_name>Gambir</departure_station_name>
    <arrival_station>BD</arrival_station>
    <arrival_station_name>Bandung</arrival_station_name>
    <train_no>A32</train_no>
    <train_name>Tiket.com Kuda Kencana</train_name>
    <departure_date>2015-06-30</departure_date>
    <departure_time>05:30:00</departure_time>
    <arrival_date>2015-06-30</arrival_date>
    <arrival_time>11:34:00</arrival_time>
    <class_code>E</class_code>
    <class_id>eks</class_id>
    <class_detail>eksekutif</class_detail>
    <subclass>A</subclass>
    <price_adult>275000.00</price_adult>
    <price_child>275000.00</price_child>
    <price_infant>0.00</price_infant>
    <availability>77</availability>
    <is_promo>0</is_promo>
    <is_active>1</is_active>
    <seat_map_subclass>[["K3AC",1,[[1,1,1,"A","J",1],[1,2,1,"B","J",1],[1,4,1,"C","J",1],[2,1,2,"A","J",1]]],["K3AC",2,[[1,1,1,"A","J",1],[1,2,1,"B","J",1],[1,4,1,"C","J",1],[2,1,2,"A","J",1],[2,2,2,"B","J",1],[2,4,2,"C","J",1],[2,5,2,"D","J",1],[3,1,3,"A","J",1],[3,2,3,"B","J",1],[3,4,3,"C","J",1],[3,5,3,"D","J",1],[4,1,4,"A","J",1],[4,2,4,"B","J",1],[4,4,4,"C","J",1],[4,5,4,"D","J",1],[10,1,10,"A","J",1],[10,2,10,"B","J",1],[10,4,10,"C","J",1],[10,5,10,"D","J",1],[11,1,11,"A","J",0],[11,2,11,"B","J",0],[11,4,11,"C","J",0],[11,5,11,"D","J",1],[12,1,12,"A","J",0],[12,2,12,"B","J",0],[12,4,12,"C","J",0],[12,5,12,"D","J",0],[13,2,13,"B","J",1],[13,4,13,"C","J",0],[13,5,13,"D","J",0]]],["K3AC",3,[[1,1,1,"A","J",1],[1,2,1,"B","J",1],[1,4,1,"C","J",1],[2,1,2,"A","J",0]]],["K3AC",4,[[1,1,1,"A","J",1],[1,2,1,"B","J",1],[1,4,1,"C","J",0],[2,1,2,"A","J",0]]],["K3AC",5,[[1,1,1,"A","J",1],[1,2,1,"B","J",1],[1,4,1,"C","J",1],[2,1,2,"A","J",0]]]]</seat_map_subclass>
    <timestamp>2015-06-24 09:11:09</timestamp>
  </result>
  <login_status>false</login_status>
  <token>a86d0826af2e445be7c8ad36a5ab2b601358c040</token>
</tiket>
```

```json
{
"diagnostic": {
  "status": 200,
  "elapsetime": "0.1097",
  "memoryusage": "4.62MB",
  "unix_timestamp": 1435115518,
  "confirm": "success",
  "lang": "id",
  "currency": "IDR"
},
"output_type": "json",
"result": {
  "train_schedule_id": "34049",
  "departure_station": "GMR",
  "departure_station_name": "Gambir",
  "arrival_station": "BD",
  "arrival_station_name": "Bandung",
  "train_no": "A32",
  "train_name": "Tiket.com Kuda Kencana",
  "departure_date": "2015-06-30",
  "departure_time": "05:30:00",
  "arrival_date": "2015-06-30",
  "arrival_time": "11:34:00",
  "class_code": "E",
  "class_id": "eks",
  "class_detail": "eksekutif",
  "subclass": "A",
  "price_adult": "275000.00",
  "price_child": "275000.00",
  "price_infant": "0.00",
  "availability": "77",
  "is_promo": "0",
  "is_active": "1",
  "seat_map_subclass": "[[\"K3AC\",1,[[1,1,1,\"A\",\"J\",1],[1,2,1,\"B\",\"J\",1],[1,4,1,\"C\",\"J\",1],[2,1,2,\"A\",\"J\",1]]],[\"K3AC\",2,[[1,1,1,\"A\",\"J\",1],[1,2,1,\"B\",\"J\",1],[1,4,1,\"C\",\"J\",1],[2,1,2,\"A\",\"J\",1],[2,2,2,\"B\",\"J\",1],[2,4,2,\"C\",\"J\",1],[2,5,2,\"D\",\"J\",1],[3,1,3,\"A\",\"J\",1],[3,2,3,\"B\",\"J\",1],[3,4,3,\"C\",\"J\",1],[3,5,3,\"D\",\"J\",1],[4,1,4,\"A\",\"J\",1],[4,2,4,\"B\",\"J\",1],[4,4,4,\"C\",\"J\",1],[4,5,4,\"D\",\"J\",1],[10,1,10,\"A\",\"J\",1],[10,2,10,\"B\",\"J\",1],[10,4,10,\"C\",\"J\",1],[10,5,10,\"D\",\"J\",1],[11,1,11,\"A\",\"J\",0],[11,2,11,\"B\",\"J\",0],[11,4,11,\"C\",\"J\",0],[11,5,11,\"D\",\"J\",1],[12,1,12,\"A\",\"J\",0],[12,2,12,\"B\",\"J\",0],[12,4,12,\"C\",\"J\",0],[12,5,12,\"D\",\"J\",0],[13,2,13,\"B\",\"J\",1],[13,4,13,\"C\",\"J\",0],[13,5,13,\"D\",\"J\",0]]],[\"K3AC\",3,[[1,1,1,\"A\",\"J\",1],[1,2,1,\"B\",\"J\",1],[1,4,1,\"C\",\"J\",1],[2,1,2,\"A\",\"J\",0]]],[\"K3AC\",4,[[1,1,1,\"A\",\"J\",1],[1,2,1,\"B\",\"J\",1],[1,4,1,\"C\",\"J\",0],[2,1,2,\"A\",\"J\",0]]],[\"K3AC\",5,[[1,1,1,\"A\",\"J\",1],[1,2,1,\"B\",\"J\",1],[1,4,1,\"C\",\"J\",1],[2,1,2,\"A\",\"J\",0]]]]",
  "timestamp": "2015-06-24 09:11:09"
},
"login_status": "false",
"token": "a86d0826af2e445be7c8ad36a5ab2b601358c040"
}
```

```matlab
a: 5: {
s: 10: "diagnostic";a: 7: {
  s: 6: "status";i: 200;s: 10: "elapsetime";s: 14: "0.1015";s: 11: "memoryusage";s: 14: "4.62MB";s: 14: "unix_timestamp";i: 1435115714;s: 7: "confirm";s: 7: "success";s: 4: "lang";s: 2: "id";s: 8: "currency";s: 3: "IDR";
}
s: 11: "output_type";s: 9: "serialize";s: 6: "result";a: 23: {
  s: 17: "train_schedule_id";s: 5: "34049";s: 17: "departure_station";s: 3: "GMR";s: 22: "departure_station_name";s: 6: "Gambir";s: 15: "arrival_station";s: 2: "BD";s: 20: "arrival_station_name";s: 7: "Bandung";s: 8: "train_no";s: 3: "A32";s: 10: "train_name";s: 22: "Tiket.com Kuda Kencana";s: 14: "departure_date";s: 10: "2015-06-30";s: 14: "departure_time";s: 8: "05:30:00";s: 12: "arrival_date";s: 10: "2015-06-30";s: 12: "arrival_time";s: 8: "11:34:00";s: 10: "class_code";s: 1: "E";s: 8: "class_id";s: 3: "eks";s: 12: "class_detail";s: 9: "eksekutif";s: 8: "subclass";s: 1: "A";s: 11: "price_adult";s: 9: "275000.00";s: 11: "price_child";s: 9: "275000.00";s: 12: "price_infant";s: 4: "0.00";s: 12: "availability";s: 2: "77";s: 8: "is_promo";s: 1: "0";s: 9: "is_active";s: 1: "1";s: 17: "seat_map_subclass";s: 924: "[["
  K3AC ",1,[[1,1,1,"
  A ","
  J ",1],[1,2,1,"
  B ","
  J ",1],[1,4,1,"
  C ","
  J ",1],[2,1,2,"
  A ","
  J ",1]]],["
  K3AC ",2,[[1,1,1,"
  A ","
  J ",1],[1,2,1,"
  B ","
  J ",1],[1,4,1,"
  C ","
  J ",1],[2,1,2,"
  A ","
  J ",1],[2,2,2,"
  B ","
  J ",1],[2,4,2,"
  C ","
  J ",1],[2,5,2,"
  D ","
  J ",1],[3,1,3,"
  A ","
  J ",1],[3,2,3,"
  B ","
  J ",1],[3,4,3,"
  C ","
  J ",1],[3,5,3,"
  D ","
  J ",1],[4,1,4,"
  A ","
  J ",1],[4,2,4,"
  B ","
  J ",1],[4,4,4,"
  C ","
  J ",1],[4,5,4,"
  D ","
  J ",1],[10,1,10,"
  A ","
  J ",1],[10,2,10,"
  B ","
  J ",1],[10,4,10,"
  C ","
  J ",1],[10,5,10,"
  D ","
  J ",1],[11,1,11,"
  A ","
  J ",0],[11,2,11,"
  B ","
  J ",0],[11,4,11,"
  C ","
  J ",0],[11,5,11,"
  D ","
  J ",1],[12,1,12,"
  A ","
  J ",0],[12,2,12,"
  B ","
  J ",0],[12,4,12,"
  C ","
  J ",0],[12,5,12,"
  D ","
  J ",0],[13,2,13,"
  B ","
  J ",1],[13,4,13,"
  C ","
  J ",0],[13,5,13,"
  D ","
  J ",0]]],["
  K3AC ",3,[[1,1,1,"
  A ","
  J ",1],[1,2,1,"
  B ","
  J ",1],[1,4,1,"
  C ","
  J ",1],[2,1,2,"
  A ","
  J ",0]]],["
  K3AC ",4,[[1,1,1,"
  A ","
  J ",1],[1,2,1,"
  B ","
  J ",1],[1,4,1,"
  C ","
  J ",0],[2,1,2,"
  A ","
  J ",0]]],["
  K3AC ",5,[[1,1,1,"
  A ","
  J ",1],[1,2,1,"
  B ","
  J ",1],[1,4,1,"
  C ","
  J ",1],[2,1,2,"
  A ","
  J ",0]]]]";s: 9: "timestamp";s: 19: "2015-06-24 09:11:09";
}
s: 12: "login_status";s: 5: "false";s: 5: "token";s: 40: "a86d0826af2e445be7c8ad36a5ab2b601358c040";
}
```

Get train seat map.

#### HTTP Request

   `GET https://api-sandbox.tiket.com/general_api/get_train_seat_map?date=2015-06-30&train_id=A32&subclass=A&org=GMR&dest=BD&token=a86d0826af2e445be7c8ad36a5ab2b601358c040`

#### Parameters

Name | Description | Format | Default | Mandatory  
---- | ----------- | ------ | ------- | --------- 
date | Departure date | yyyy-mm-dd |  | TRUE  
train_id | Train ID that choosen by user | CHAR(~) |  | TRUE  
subclass | Subclass from train that choosen by user | CHAR(~) |  | FALSE  
token | for saving transaction that done by user | CHAR(128) |  | TRUE  
org | Depart train station code | CHAR(3) |  | TRUE  
dest | Arrival train station code | CHAR(3) |  | TRUE  

#### Output

NOTE for seat_map_subclass :  
[["EKSASL",1,[[1,1,1,"A","A",1],[2,1,2,"A","A",0]]]  
structure : [ baris, kolom, seat row, seat column, subclass, status(0 : kursi kosong, 1 : kursi sudah ditempati) ]

[["EKSASL",1  
Wagon name : EKSASL  
Wagon number : 1

[1,1,1,"A","A",1]  
Row : 1  
Coloumn : 1  
Seat number : 1, "A" (usually written 1A)  
Subclass : A  
Flag : 1 (1 = Filled, 0 = Empty)

[2,1,2,"A","A",0]  
Row : 2  
Coloumn : 1  
Seat number : 2, "A" (usually written 2A)  
Subclass : A  
Flag : 0 (1 = Filled, 0 = Empty)

Note for seat_map_all :  
Seat_map_all for all wagon layout (any subclass)  
structure : [ seat row, seat column, subclass, status(0 : kursi kosong, 1 : kursi sudah ditempati) ]  
[["EKSASL",1,[[1,"A","A",1],[1,"B","A",1],[1,"C","A",0],  
Wagon name : EKSASL  
Wagon number : 1

[1,"A","A",1]  
Row : 1  
Coloumn : A  
Subclass : A  
Status : Taken (availability = 1)
    

## Add Order

```xml
<?xml version="1.0" encoding="utf-8"?>
<tiket>
    <diagnostic>
        <error_msgs>Anda sudah pernah melakukan pemesanan yang sama sebelumnya, mohon tunggu 10 menit untuk melakukan pemesanan</error_msgs>
        <status>204</status>
        <elapsetime>0.1464</elapsetime>
        <memoryusage>5.94MB</memoryusage>
        <unix_timestamp>1470630702</unix_timestamp>
        <lang>id</lang>
        <currency>IDR</currency>
    </diagnostic>
    <output_type>xml</output_type>
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
    "elapsetime": "0.3511",
    "memoryusage": "6.07MB",
    "unix_timestamp": 1470630633,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "login_status": "true",
  "guest_id": "22691145",
  "login_email": "wida.skydev@gmail.com",
  "token": "f9b29ac359ca5d77755e7588751c089bf96f0dc9"
}
```


```matlab
a:6:{s:10:"diagnostic";a:7:{s:10:"error_msgs";s:48:"Anda sudah pernah melakukan pemesanan yang sama sebelumnya, mohon tunggu 10 menit untuk melakukan pemesanan";s:6:"status";i:204;s:10:"elapsetime";s:14:"0.1681";s:11:"memoryusage";s:14:"5.93MB";s:14:"unix_timestamp";i:1470630723;s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:11:"output_type";s:9:"serialize";s:12:"login_status";s:4:"true";s:8:"guest_id";s:8:"22691145";s:11:"login_email";s:21:"wida.skydev@gmail.com";s:5:"token";s:40:"f9b29ac359ca5d77755e7588751c089bf96f0dc9";}
```

* NOTE : UPDATE for INFANT passenger,just now is for development server (api-sandbox.tiket.com)  
We will inform you if its already provided in production server (api.tiket.com)

Add train order to shopping cart.

*Note : adult must more than or equal to infant

#### HTTP Request

    `GET https://api-sandbox.tiket.com/order/add/train?d=GMR&a=BD&date=2016-09-03&ret_date=&adult=1&child=0&token=f9b29ac359ca5d77755e7588751c089bf96f0dc9&train_id=A32&subclass=A&output=json&conSalutation=Mr&conFirstName=ronni&conLastName=wijaya&conEmailAddress=test@gmail.com&conPhone=085642020047&nameAdult1=ronni wijayanto&IdCardAdult1=111&noHpAdult1=%2B6285642020047&salutationAdult1=Mr&birthDateAdult1=1990-02-02`

#### Parameters
  
Name | Description | Format | Default | Mandatory  
---- | ----------- | ------ | ------- | ---------   
d | Depart | train station code | CHAR(3) |  | TRUE  
a | Arrival train station code | CHAR(3) |  | TRUE  
date | depart date | YYYY-MM-DD |  | TRUE  
ret_date | return date. If want to book return | YYYY-MM-DD |  | FALSE  
adult | number of adult passenger (max adult+child+infant 4 persons) | INT | 1 | FALSE  
child | number of child passenger (max adult+child+infant 4 persons) | INT | 0 | FALSE  
infant | number of infant passenger (max adult+child+infant 4 persons) | INT | 0 | FALSE  
token | for saving transaction that done by user | CHAR(128) |  | TRUE  
train_id | train id that choosen by user | CHAR(~) |  | TRUE  
subclass | subclass from train that choosen by user | CHAR(1) |  | TRUE  
train_id_ret | train id that choosen by user for return |  |  |   
subclass_ret | subclass from train that choosen by user for return |  |  |   
conSalutation | contact person title ( ex: Mr., Mrs., Ms.) | CHAR(5) |  | TRUE  
conFirstName | contact person first name | CHAR(50) |  | TRUE  
conLastName | contact person last name | CHAR(50) |  | TRUE  
conEmailAddress | contact person email address | CHAR(50) |  | TRUE  
conPhone | contact person phone | [must begin with 08 or +62] | CHAR(20) |  | TRUE  
nameAdult1 | as an array like nameAdult1 nameAdult2 if you have adult passager | CHAR(100) |  |   
IdCardAdult1 | as an array like IdCardAdult1 IdCardAdult2 if you have adult passager | [max 16 character] | CHAR(50) |  |   
noHpAdult1 | as an array like noHpAdult1 noHpAdult2 if you have adult passager |  [must begin with 08 or +62]. Don't forget to urlencode + into %2B in the GET parameter | CHAR(20) |  |   
salutationAdult1 | as an array like salutationAdult1 salutationAdult2 if you have adult passager : Mr., Ms., Mrs. | CHAR(4) |  |   
birthDateAdult1 | as an array like birthDateAdult1 birthDateAdult2 if you have adult passager : format YYYY-MM-DD | DATE |  |   
nameChild1 | as an array like nameChild1 nameChild2 if you have Child passager | CHAR(50) |  |   
salutationChild1 | as an array like salutationChild1 salutationChild2 if you have Child passager : Mr., Ms., Mrs. | CHAR(4) |  |   
birthDateChild1 | as an array like birthDateChild1 birthDateChild2 if you have Child passager : format YYYY-MM-DD | [child must below 10 years old] | DATE |  |   
salutationInfant1 | as an array like salutationInfant1 salutationInfant2 if you have infant passager : Mr., Ms., Mrs. | CHAR(4) |  |   
nameInfant1 | as an array like nameInfant1 nameInfant2 if you have infant passager | CHAR(50) |  |   
birthDateInfant1 | as an array like birthDateInfant1 birthDateInfant2 if you have infant passager : format YYYY-MM-DD [infant must below 2 years old] | DATE |  |   
 
   
       
## Order

```xml
<?xml version="1.0" encoding="utf-8"?>
<tiket>
    <diagnostic>
        <status>200</status>
        <elapsetime>15.1432</elapsetime>
        <memoryusage>6.54MB</memoryusage>
        <unix_timestamp>1470631727</unix_timestamp>
        <confirm>success</confirm>
        <lang>id</lang>
        <currency>IDR</currency>
    </diagnostic>
    <output_type>xml</output_type>
    <myorder>
        <order_id>22385759</order_id>
        <data>
            <expire>41</expire>
            <order_detail_id>12743753</order_detail_id>
            <order_expire_datetime>2016-08-08 12:15:33</order_expire_datetime>
            <order_type>train</order_type>
            <order_name_detail>Tiket.com Kuda Kencana (Eksekutif)</order_name_detail>
            <order_detail_status>active</order_detail_status>
            <detail>
                <arrival_datetime>2016-09-03 11:34:00</arrival_datetime>
                <departure_datetime>2016-09-03 05:30:00</departure_datetime>
                <count_adult>1</count_adult>
                <count_child>0</count_child>
                <count_infant>0</count_infant>
                <book_code>GMRBD1470630633</book_code>
                <train_subclass>A</train_subclass>
                <tiket_seating>K3AC-2-1-A</tiket_seating>
                <num_code>9992833283701</num_code>
                <train_from>GMR</train_from>
                <train_to>BD</train_to>
                <train_no>A32</train_no>
                <train_name>TIKET.COM KUDA KENCANA</train_name>
                <discount_price>7500.00</discount_price>
                <subclass_type>umum</subclass_type>
                <class_name>eksekutif</class_name>
                <passengers>
                    <adult>
                        <traveller_id>3206215</traveller_id>
                        <order_detail_id>12743753</order_detail_id>
                        <profile_id>5108531</profile_id>
                        <type>adult</type>
                        <gender>M</gender>
                        <full_name>Ronni Wijayanto</full_name>
                        <salutation>Mr</salutation>
                        <birthdate>0000-00-00</birthdate>
                        <phone>+6285642020047</phone>
                        <id_card>111</id_card>
                        <last_update>2016-08-08 11:30:33</last_update>
                    </adult>
                </passengers>
                <train_from_station>gambir</train_from_station>
                <train_to_station>bandung</train_to_station>
                <price>267500.00</price>
            </detail>
            <order_photo>https://api-sandbox.tiket.com/images/icon_kai.jpg</order_photo>
            <tax_and_charge>16060.00</tax_and_charge>
            <subtotal_and_charge>283560.00</subtotal_and_charge>
            <delete_uri>https://api-sandbox.tiket.com/order/delete_order?order_detail_id=12743753</delete_uri>
            <business_id>80572</business_id>
        </data>
        <total>283560</total>
        <total_tax>16060</total_tax>
        <total_without_tax>267500</total_without_tax>
        <count_installment>0</count_installment>
        <discount>Dapatkan potongan hingga IDR 8.560,00 saat anda checkout . Tidak berlaku untuk Kartu Kredit.</discount>
        <discount_amount>8560.00</discount_amount>
    </myorder>
    <checkout>https://api-sandbox.tiket.com/order/checkout/22385759/IDR</checkout>
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
    "elapsetime": "15.1846",
    "memoryusage": "6.54MB",
    "unix_timestamp": 1470631654,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "myorder": {
    "order_id": "22385759",
    "data": [
      {
        "expire": 42,
        "order_detail_id": "12743753",
        "order_expire_datetime": "2016-08-08 12:15:33",
        "order_type": "train",
        "order_name_detail": "Tiket.com Kuda Kencana (Eksekutif)",
        "order_detail_status": "active",
        "detail": {
          "arrival_datetime": "2016-09-03 11:34:00",
          "departure_datetime": "2016-09-03 05:30:00",
          "count_adult": "1",
          "count_child": "0",
          "count_infant": "0",
          "book_code": "GMRBD1470630633",
          "train_subclass": "A",
          "tiket_seating": "K3AC-2-1-A",
          "num_code": "9992833283701",
          "train_from": "GMR",
          "train_to": "BD",
          "train_no": "A32",
          "train_name": "TIKET.COM KUDA KENCANA",
          "discount_price": "7500.00",
          "subclass_type": "umum",
          "class_name": "eksekutif",
          "passengers": {
            "adult": [
              {
                "traveller_id": "3206215",
                "order_detail_id": "12743753",
                "profile_id": "5108531",
                "type": "adult",
                "gender": "M",
                "full_name": "Ronni Wijayanto",
                "salutation": "Mr",
                "birthdate": "0000-00-00",
                "phone": "+6285642020047",
                "id_card": "111",
                "last_update": "2016-08-08 11:30:33"
              }
            ]
          },
          "train_from_station": "gambir",
          "train_to_station": "bandung",
          "price": "267500.00"
        },
        "order_photo": "https://api-sandbox.tiket.com/images/icon_kai.jpg",
        "tax_and_charge": "16060.00",
        "subtotal_and_charge": "283560.00",
        "delete_uri": "https://api-sandbox.tiket.com/order/delete_order?order_detail_id=12743753",
        "business_id": "80572"
      }
    ],
    "total": 283560,
    "total_tax": 16060,
    "total_without_tax": 267500,
    "count_installment": 0,
    "promo": [],
    "discount": "Dapatkan potongan hingga IDR 8.560,00 saat anda checkout . Tidak berlaku untuk Kartu Kredit.",
    "discount_amount": "8560.00"
  },
  "checkout": "https://api-sandbox.tiket.com/order/checkout/22385759/IDR",
  "login_status": "true",
  "guest_id": "22691145",
  "login_email": "wida.skydev@gmail.com",
  "token": "f9b29ac359ca5d77755e7588751c089bf96f0dc9"
}
```
    
```matlab
a:8:{s:10:"diagnostic";a:7:{s:6:"status";i:200;s:10:"elapsetime";s:14:"15.1474";s:11:"memoryusage";s:14:"6.53MB";s:14:"unix_timestamp";i:1470631793;s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:11:"output_type";s:9:"serialize";s:7:"myorder";a:9:{s:8:"order_id";s:8:"22385759";s:4:"data";a:1:{i:0;a:12:{s:6:"expire";i:40;s:15:"order_detail_id";s:8:"12743753";s:21:"order_expire_datetime";s:19:"2016-08-08 12:15:33";s:10:"order_type";s:5:"train";s:17:"order_name_detail";s:34:"Tiket.com Kuda Kencana (Eksekutif)";s:19:"order_detail_status";s:6:"active";s:6:"detail";a:20:{s:16:"arrival_datetime";s:19:"2016-09-03 11:34:00";s:18:"departure_datetime";s:19:"2016-09-03 05:30:00";s:11:"count_adult";s:1:"1";s:11:"count_child";s:1:"0";s:12:"count_infant";s:1:"0";s:9:"book_code";s:15:"GMRBD1470630633";s:14:"train_subclass";s:1:"A";s:13:"tiket_seating";s:10:"K3AC-2-1-A";s:8:"num_code";s:13:"9992833283701";s:10:"train_from";s:3:"GMR";s:8:"train_to";s:2:"BD";s:8:"train_no";s:3:"A32";s:10:"train_name";s:22:"TIKET.COM KUDA KENCANA";s:14:"discount_price";s:7:"7500.00";s:13:"subclass_type";s:4:"umum";s:10:"class_name";s:9:"eksekutif";s:10:"passengers";a:1:{s:5:"adult";a:1:{i:0;a:11:{s:12:"traveller_id";s:7:"3206215";s:15:"order_detail_id";s:8:"12743753";s:10:"profile_id";s:7:"5108531";s:4:"type";s:5:"adult";s:6:"gender";s:1:"M";s:9:"full_name";s:15:"Ronni Wijayanto";s:10:"salutation";s:2:"Mr";s:9:"birthdate";s:10:"0000-00-00";s:5:"phone";s:14:"+6285642020047";s:7:"id_card";s:3:"111";s:11:"last_update";s:19:"2016-08-08 11:30:33";}}}s:18:"train_from_station";s:6:"gambir";s:16:"train_to_station";s:7:"bandung";s:5:"price";s:9:"267500.00";}s:11:"order_photo";s:49:"https://api-sandbox.tiket.com/images/icon_kai.jpg";s:14:"tax_and_charge";s:8:"16060.00";s:19:"subtotal_and_charge";s:9:"283560.00";s:10:"delete_uri";s:73:"https://api-sandbox.tiket.com/order/delete_order?order_detail_id=12743753";s:11:"business_id";s:5:"80572";}}s:5:"total";d:283560;s:9:"total_tax";d:16060;s:17:"total_without_tax";d:267500;s:17:"count_installment";i:0;s:5:"promo";a:0:{}s:8:"discount";s:109:"Dapatkan potongan hingga IDR 8.560,00 saat anda checkout . Tidak berlaku untuk Kartu Kredit.";s:15:"discount_amount";s:7:"8560.00";}s:8:"checkout";s:57:"https://api-sandbox.tiket.com/order/checkout/22385759/IDR";s:12:"login_status";s:4:"true";s:8:"guest_id";s:8:"22691145";s:11:"login_email";s:21:"wida.skydev@gmail.com";s:5:"token";s:40:"f9b29ac359ca5d77755e7588751c089bf96f0dc9";}
```

* Display user shopping cart detail

#### HTTP Request
    
        `GET https://api-sandbox.tiket.com/order?token=2279a50a996f5a54a15db6b10bfc5657&output=json`
    
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


* Early stage to access checkout.
    
    link url can be get from order, variable checkout .
    
#### HTTP Request
    
     `GET https://api-sandbox.tiket.com/order/checkout/119978/IDR?token=9991e3092aea96042964220181374b60&output=json`
    
(Get from order page in checkout variable.)
    
    
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
    <elapsetime>1.2545</elapsetime>
    <memoryusage>20.54MB</memoryusage>
    <confirm>success</confirm>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <login_status>true</login_status>
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
    
        `GET https://api-sandbox.tiket.com/checkout/checkout_customer?token=87da88eaaa429d5513a3a3658b01701e&salutation=Ms&firstName=ba&lastName=ca&emailAddress=test@yahoocom&phone=%2B62878434343&saveContinue=2`
    
Setelah merequest link tersebut maka user akan dibuatkan account di tiket.com user akan dikirimkan email untuk mengubah password loginnya.

#### Parameters
    
Name | Description | Format | Default | Mandatory  
---- | ----------- | ------ | ------- | ---------  
salutation | your title ( ex: Mr.,  Mrs., Ms.) | CHAR(5) |  | TRUE  
firstName | your first name | CHAR(50) |  | TRUE  
lastName | your last name | CHAR(50) |  | TRUE  
emailAddress | your email | CHAR(50) |  | TRUE  
phone | your phone |  ex: 081232323343 or +62324324234234. Don't forget to urlencode + into %2B in the GET parameter | CHAR(20) |  | TRUE  
saveContinue | Flag for login (value=2) |  |  | TRUE  

    
  
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
---- | ----------- | ------ | ------- | ---------  
token | for saving transaction that done by user | CHAR(128) |  | TRUE  
        


## Checkout Payment

Please see [Checkout Payment](http://docs.tiket.com/#checkout-payment-309) in General API


## Register

```xml
<?xml version="1.0" encoding="utf-8"?>
<tiket>
    <diagnostic>
        <status>200</status>
        <elapsetime>0.1214</elapsetime>
        <memoryusage>4.75MB</memoryusage>
        <unix_timestamp>1470636576</unix_timestamp>
        <confirm>success</confirm>
        <lang>id</lang>
        <currency>IDR</currency>
    </diagnostic>
    <output_type>xml</output_type>
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
    "elapsetime": "0.1030",
    "memoryusage": "4.74MB",
    "unix_timestamp": 1470636461,
    "confirm": "success",
    "lang": "id",
    "currency": "IDR"
  },
  "output_type": "json",
  "login_status": "true",
  "guest_id": "22691145",
  "login_email": "wida.skydev@gmail.com",
  "token": "f9b29ac359ca5d77755e7588751c089bf96f0dc9"
}
```
    
```matlab
a:6:{s:10:"diagnostic";a:7:{s:6:"status";i:200;s:10:"elapsetime";s:14:"0.3031";s:11:"memoryusage";s:14:"4.74MB";s:14:"unix_timestamp";i:1470636611;s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:11:"output_type";s:9:"serialize";s:12:"login_status";s:4:"true";s:8:"guest_id";s:8:"22691145";s:11:"login_email";s:21:"wida.skydev@gmail.com";s:5:"token";s:40:"f9b29ac359ca5d77755e7588751c089bf96f0dc9";}
```

* For user registration.

#### HTTP Request
    
        `GET https://api-sandbox.tiket.com/auth/register?token=f9b29ac359ca5d77755e7588751c089bf96f0dc9&firstName=roni&lastName=wijayanto&email=wida.skydev@gmail.com&password=hahaha&conPassword=hahaha&country=id&output=json`
    
#### Parameters
    
Name | Description | Format | Default | Mandatory  
---- | ----------- | ------ | ------- | ---------   
firstName | your firstname | CHAR |  | TRUE  
lastName | your lastname | CHAR |  | TRUE  
email | your email [must email format] | CHAR |  | TRUE  
password | your password min 6 char | CHAR |  | TRUE  
conPassword | confirm password | CHAR |  | TRUE  
country | your country [must in country list] | CHAR(50) |  | TRUE     
    

## Change Train Seat

```xml
<tiket>
  <status>xml</status>
  <elapsetime>2.991</elapsetime>
  <memoryusage>3.31MB</memoryusage>
  <confirm>success</confirm>
  <lang>id</lang>
  <currency>IDR</currency>

  <output_type>JSON</output_type>
  <result>
    <err_code>0</err_code>
    <book_code>KIQWWR</book_code>
    <wagon_code>EKS</wagon_code>
    <wagon_no>2</wagon_no>
    <seat>3A</seat>
    <seat>3B</seat>
  </result>
  <token>2ee91e32f9113e863da4c57e235098d1</token>
</tiket>
```
    
```json
{
"diagnostic": {
  "status": 200,
  "elapsetime": "2.9133",
  "memoryusage": "3.31MB",
  "confirm": "success",
  "lang": "id",
  "currency": "IDR"
},
"output_type": "json",
"result": {
  "err_code": 0,
  "book_code": "KIQWWR",
  "wagon_code": "EKS",
  "wagon_no": 2,
  "seat": ["3A", "3B"]
},
"login_status": "false",
"token": "6d360dfd1dab82b3fa42e453abafff91"
}
```

* Change Train Seat

#### HTTP Request
    
        `GET https://api.tiket.com/general_api/train_change_seat?output=json&booking_code=5WWAS1&kode_wagon=EKS&nomor_wagon=2&nomor_kursi=4D&order_detail_id=327247&token=6d360dfd1dab82b3fa42e453abafff91`
    
#### Parameters
    
Name | Description | Format | Default | Mandatory  
---- | ----------- | ------ | ------- | ---------    
booking_code | Booking Code | CHAR(6) |  | TRUE  
kode_wagon | Wagon Code | VARCHAR(5) |  | TRUE  
nomor_wagon | Wagon number | VARCHAR(2) |  | TRUE  
nomor_kursi | Seating Number | VARCHAR(3) |  | TRUE  
order_detail_id | Order Detail ID | NUMERIC |  | TRUE  
token | for saving transaction that done by user | CHAR(128) |  | TRUE  
        
    
