# Train API

NOTE :  
*Data that is provided for testing is different from the actual  
*UPDATE for INFANT passenger, LIVE. Please all developers to update the application

These are the API command for Train.

Diagram flow for Train API:  

[![](http://docs.tiket.com/wp-content/uploads/2012/07/API-train-164x300.jpg "API train")](http://docs.tiket.com/wp-content/uploads/2012/07/API-train.jpg)

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
    <tiket>
    	<output_type>xml</output_type>
    	<diagnostic>
    		<elapsetime>2.4569</elapstime>
    		<memoryusage>5.19MB</memoryusage>
    		<status>200</status>
    		<lang>en</lang>
    		<currency>IDR</currency>
    	</diagnostic>
    	<search_queries>
    		<dep_station>GMR</dep_station>
    		<arr_station>BD</arr_station>
    		<date>2012-06-03</date>
    		<formatted_date>03 June 2012</formatted_date>
    		<train_class>all</train_class>
    		<count_adult>1</count_adult>
    		<count_child>0</count_child>
    		<count_infant>0</count_infant>
    	</search_queries>
    	<departures>
    		<result>
    			<detail_availability>90</detail_availability>
    			<schedule_id>3</schedule_id>
    			<train_id>IVHAN3</train_id>
    			<train_name>Argo Cantik</train_name>
    			<departure_time>17:00</departure_time>
    			<arrival_time>19:30</arrival_time>
    			<class_name>bis</class_name>
    			<subclass_name>B</subclass_name>
    			<is_promo>0</is_promo>
    			<price_adult>56.000,00</price_adult>
    			<price_child>46.000,00</price_child>
    			<price_infant>3.000,00</price_infant>
    			<duration>2 h 30 m</duration>
    		</result>
    	</departures>
    	<token>ebaa92ff1a060a7a5610b7159bd68b28</token>
    </tiket>
```

```json
    {"output_type":"json","diagnostic":{"elapstime":"0.5343","memoryusage":"5.16MB","status":"200","lang":"en","currency":"IDR"},"search_queries":{"dep_station":"GMR","arr_station":"BD","date":"2012-06-03","formatted_date":"03 June 2012","train_class":"all","count_adult":"1","count_child":"0","count_infant":"0"},"departures":{"result":[{"detail_availability":"90","schedule_id":"3","train_id":"IVHAN3","train_name":"Argo Cantik","departure_time":"17:00","arrival_time":"19:30","class_name":"bis","subclass_name":"B","is_promo":0,"price_adult":"56.000,00","price_child":"46.000,00","duration":"2 h 30 m","price_infant":"3.000,00"}]},"token":"ebaa92ff1a060a7a5610b7159bd68b28"}
```

```matlab
    a:5:{s:11:"output_type";s:9:"serialize";s:10:"diagnostic";a:5:{s:9:"elapstime";s:14:"0.1472";s:11:"memoryusage";s:14:"5.13MB";s:6:"status";s:3:"200";s:4:"lang";s:2:"en";s:8:"currency";s:3:"IDR";}s:14:"search_queries";a:7:{s:11:"dep_station";s:3:"GMR";s:11:"arr_station";s:2:"BD";s:4:"date";s:10:"2012-06-03";s:14:"formatted_date";s:12:"03 June 2012";s:11:"train_class";s:3:"all";s:11:"count_adult";s:1:"1";s:11:"count_child";s:12:"count_infant";s:1:"0";s:1:"0";}s:10:"departures";a:1:{s:6:"result";a:6:{i:5;a:12:{s:19:"detail_availability";s:2:"90";s:11:"schedule_id";s:1:"3";s:8:"train_id";s:6:"IVHAN3";s:10:"train_name";s:11:"Argo Cantik";s:14:"departure_time";s:5:"17:00";s:12:"arrival_time";s:5:"19:30";s:10:"class_name";s:3:"bis";s:13:"subclass_name";s:1:"B";s:8:"is_promo";i:0;s:11:"price_adult";s:9:"56.000,00";s:11:"price_child";s:9:"46.000,00";s:11:"price_infant";s:8:"3.000,00";s:8:"duration";s:24:"2 h 30 m";}}}s:5:"token";s:32:"ebaa92ff1a060a7a5610b7159bd68b28";}
```

* NOTE : UPDATE for INFANT passenger,just now is for development server (api-sandbox.tiket.com)  
We will inform you if its already provided in production server (api.tiket.com)

#### HTTP Request

    `https://api-sandbox.tiket.com/search/train?d=GMR&a=BD&date=2012-06-03&ret_date=&adult=1&child=0&class=all&token=80bfe5297f7c4fbaa7a1e6c022585946&output=json`

#### Parameters
  
Name | Description | Format | Default | Mandatory
---- | ----------- | ------ | ------- | ---------
d | Depart train station code | CHAR(3) |  | TRUE  
a | Arrival train station code | CHAR(3) |  | TRUE  
date | depart date. Result will be in | YYYY-MM-DD |  | TRUE  
ret_date | return date. If provided, then system will return | YYYY-MM-DD |  | FALSE  
adult | number of adult passenger (max adult+child+infant 4 persons) | INT | 1 | FALSE  
child | number of child passenger (max adult+child+infant 4 persons) | INT | 0 | FALSE  
infant | number of infant passenger (max adult+child+infant 4 persons) | INT |0 |FALSE  
class | train class (ALL)" | all|bis|eks|eco | all | FALSE  
token | for saving transaction that done by user | CHAR(128) |  | TRUE  

         
## Search Station

```xml 
<tiket>  
<output_type>xml</output_type>  
<diagnostic>  
<elapstime>0.1031</elapstime>  
<memoryusage>3.82MB</memoryusage>  
<status>200</status>  
<lang>en</lang>  
<currency>IDR</currency>  
</diagnostic>  
<stations>  
<station>  
<station_name>alastuwa</station_name>  
<city_name>Pariaman</city_name>  
<station_code>ATA</station_code>  
</station>  
<station>  
<station_name>ambarawa</station_name>  
<city_name>Lampung Tengah</city_name>  
<station_code>ABR</station_code>  
</station>  
<station>  
<station_name>arjawinangun</station_name>  
<city_name>Cirebon</city_name>  
<station_code>AWN</station_code>  
</station>  
</stations>  
<token>ebaa92ff1a060a7a5610b7159bd68b28</token>  
</tiket>  
```

```json
{"output_type":"json","diagnostic":{"elapstime":"0.0901","memoryusage":"3.79MB","status":"200","lang":"en","currency":"IDR"},"stations":{"station":[{"station_name":"alastuwa","city_name":"Pariaman","station_code":"ATA"},{"station_name":"ambarawa","city_name":"Lampung Tengah","station_code":"ABR"},{"station_name":"arjawinangun","city_name":"Cirebon","station_code":"AWN"}]},"token":"ebaa92ff1a060a7a5610b7159bd68b28"}  
``` 

```matlab
a:4:{s:11:"output_type";s:9:"serialize";s:10:"diagnostic";a:5:{s:9:"elapstime";s:14:"0.0881";s:11:"memoryusage";s:14:"3.79MB";s:6:"status";s:3:"200";s:4:"lang";s:2:"en";s:8:"currency";s:3:"IDR";}s:8:"stations";a:1:{s:7:"station";a:107:{i:0;a:3:{s:12:"station_name";s:8:"alastuwa";s:9:"city_name";s:8:"Pariaman";s:12:"station_code";s:3:"ATA";}i:1;a:3:{s:12:"station_name";s:8:"ambarawa";s:9:"city_name";s:14:"Lampung Tengah";s:12:"station_code";s:3:"ABR";}i:2;a:3:{s:12:"station_name";s:12:"arjawinangun";s:9:"city_name";s:7:"Cirebon";s:12:"station_code";s:3:"AWN";}i:3;a:3:{s:12:"station_name";s:14:"bandar kalipah";s:9:"city_name";s:12:"Deli Serdang";s:12:"station_code";s:3:"BAP";}i:4;}}}s:5:"token";s:32:"ebaa92ff1a060a7a5610b7159bd68b28";}  
``` 

Display all train station and their codes for use in search train API (variable d and a).

#### HTTP Request

    `https://api-sandbox.tiket.com/train_api/train_station?token=11b534a0394d9bb140f18bc1a87adf1a&output=json`  

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
    {"diagnostic":{"status":200,"elapsetime":"0.1097","memoryusage":"4.62MB","unix_timestamp":1435115518,"confirm":"success","lang":"id","currency":"IDR"},"output_type":"json","result":{"train_schedule_id":"34049","departure_station":"GMR","departure_station_name":"Gambir","arrival_station":"BD","arrival_station_name":"Bandung","train_no":"A32","train_name":"Tiket.com Kuda Kencana","departure_date":"2015-06-30","departure_time":"05:30:00","arrival_date":"2015-06-30","arrival_time":"11:34:00","class_code":"E","class_id":"eks","class_detail":"eksekutif","subclass":"A","price_adult":"275000.00","price_child":"275000.00","price_infant":"0.00","availability":"77","is_promo":"0","is_active":"1","seat_map_subclass":"[[\"K3AC\",1,[[1,1,1,\"A\",\"J\",1],[1,2,1,\"B\",\"J\",1],[1,4,1,\"C\",\"J\",1],[2,1,2,\"A\",\"J\",1]]],[\"K3AC\",2,[[1,1,1,\"A\",\"J\",1],[1,2,1,\"B\",\"J\",1],[1,4,1,\"C\",\"J\",1],[2,1,2,\"A\",\"J\",1],[2,2,2,\"B\",\"J\",1],[2,4,2,\"C\",\"J\",1],[2,5,2,\"D\",\"J\",1],[3,1,3,\"A\",\"J\",1],[3,2,3,\"B\",\"J\",1],[3,4,3,\"C\",\"J\",1],[3,5,3,\"D\",\"J\",1],[4,1,4,\"A\",\"J\",1],[4,2,4,\"B\",\"J\",1],[4,4,4,\"C\",\"J\",1],[4,5,4,\"D\",\"J\",1],[10,1,10,\"A\",\"J\",1],[10,2,10,\"B\",\"J\",1],[10,4,10,\"C\",\"J\",1],[10,5,10,\"D\",\"J\",1],[11,1,11,\"A\",\"J\",0],[11,2,11,\"B\",\"J\",0],[11,4,11,\"C\",\"J\",0],[11,5,11,\"D\",\"J\",1],[12,1,12,\"A\",\"J\",0],[12,2,12,\"B\",\"J\",0],[12,4,12,\"C\",\"J\",0],[12,5,12,\"D\",\"J\",0],[13,2,13,\"B\",\"J\",1],[13,4,13,\"C\",\"J\",0],[13,5,13,\"D\",\"J\",0]]],[\"K3AC\",3,[[1,1,1,\"A\",\"J\",1],[1,2,1,\"B\",\"J\",1],[1,4,1,\"C\",\"J\",1],[2,1,2,\"A\",\"J\",0]]],[\"K3AC\",4,[[1,1,1,\"A\",\"J\",1],[1,2,1,\"B\",\"J\",1],[1,4,1,\"C\",\"J\",0],[2,1,2,\"A\",\"J\",0]]],[\"K3AC\",5,[[1,1,1,\"A\",\"J\",1],[1,2,1,\"B\",\"J\",1],[1,4,1,\"C\",\"J\",1],[2,1,2,\"A\",\"J\",0]]]]","timestamp":"2015-06-24 09:11:09"},"login_status":"false","token":"a86d0826af2e445be7c8ad36a5ab2b601358c040"}
```

```matlab
    a:5:{s:10:"diagnostic";a:7:{s:6:"status";i:200;s:10:"elapsetime";s:14:"0.1015";s:11:"memoryusage";s:14:"4.62MB";s:14:"unix_timestamp";i:1435115714;s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:11:"output_type";s:9:"serialize";s:6:"result";a:23:{s:17:"train_schedule_id";s:5:"34049";s:17:"departure_station";s:3:"GMR";s:22:"departure_station_name";s:6:"Gambir";s:15:"arrival_station";s:2:"BD";s:20:"arrival_station_name";s:7:"Bandung";s:8:"train_no";s:3:"A32";s:10:"train_name";s:22:"Tiket.com Kuda Kencana";s:14:"departure_date";s:10:"2015-06-30";s:14:"departure_time";s:8:"05:30:00";s:12:"arrival_date";s:10:"2015-06-30";s:12:"arrival_time";s:8:"11:34:00";s:10:"class_code";s:1:"E";s:8:"class_id";s:3:"eks";s:12:"class_detail";s:9:"eksekutif";s:8:"subclass";s:1:"A";s:11:"price_adult";s:9:"275000.00";s:11:"price_child";s:9:"275000.00";s:12:"price_infant";s:4:"0.00";s:12:"availability";s:2:"77";s:8:"is_promo";s:1:"0";s:9:"is_active";s:1:"1";s:17:"seat_map_subclass";s:924:"[["K3AC",1,[[1,1,1,"A","J",1],[1,2,1,"B","J",1],[1,4,1,"C","J",1],[2,1,2,"A","J",1]]],["K3AC",2,[[1,1,1,"A","J",1],[1,2,1,"B","J",1],[1,4,1,"C","J",1],[2,1,2,"A","J",1],[2,2,2,"B","J",1],[2,4,2,"C","J",1],[2,5,2,"D","J",1],[3,1,3,"A","J",1],[3,2,3,"B","J",1],[3,4,3,"C","J",1],[3,5,3,"D","J",1],[4,1,4,"A","J",1],[4,2,4,"B","J",1],[4,4,4,"C","J",1],[4,5,4,"D","J",1],[10,1,10,"A","J",1],[10,2,10,"B","J",1],[10,4,10,"C","J",1],[10,5,10,"D","J",1],[11,1,11,"A","J",0],[11,2,11,"B","J",0],[11,4,11,"C","J",0],[11,5,11,"D","J",1],[12,1,12,"A","J",0],[12,2,12,"B","J",0],[12,4,12,"C","J",0],[12,5,12,"D","J",0],[13,2,13,"B","J",1],[13,4,13,"C","J",0],[13,5,13,"D","J",0]]],["K3AC",3,[[1,1,1,"A","J",1],[1,2,1,"B","J",1],[1,4,1,"C","J",1],[2,1,2,"A","J",0]]],["K3AC",4,[[1,1,1,"A","J",1],[1,2,1,"B","J",1],[1,4,1,"C","J",0],[2,1,2,"A","J",0]]],["K3AC",5,[[1,1,1,"A","J",1],[1,2,1,"B","J",1],[1,4,1,"C","J",1],[2,1,2,"A","J",0]]]]";s:9:"timestamp";s:19:"2015-06-24 09:11:09";}s:12:"login_status";s:5:"false";s:5:"token";s:40:"a86d0826af2e445be7c8ad36a5ab2b601358c040";}
```

Get train seat map.

#### HTTP Request

    `http://api-sandbox.tiket.com/general_api/get_train_seat_map?date=2015-06-30&train_id=A32&subclass=A&org=GMR&dest=BD&token=a86d0826af2e445be7c8ad36a5ab2b601358c040`

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

---

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
    
    	xml
    	0
    
    		7.7606
    		12.17MB
    		200
    		en
    		IDR
    
    	success booking train
    	13fc239d306bf7085708566b3d085b29
    
```



```json
    {"output_type":"json","error":"0","diagnostic":{"elapstime":"9.5301","memoryusage":"12.15MB","status":"200","lang":"en","currency":"IDR"},"status":"success booking train","token":"13fc239d306bf7085708566b3d085b29"}
```



```matlab
    a:5:{s:11:"output_type";s:9:"serialize";s:5:"error";s:1:"0";s:10:"diagnostic";a:5:{s:9:"elapstime";s:14:"5.9200";s:11:"memoryusage";s:14:"12.15MB";s:6:"status";s:3:"200";s:4:"lang";s:2:"en";s:8:"currency";s:3:"IDR";}s:6:"status";s:21:"success booking train";s:5:"token";s:32:"13fc239d306bf7085708566b3d085b29";}
```

* NOTE : UPDATE for INFANT passenger,just now is for development server (api-sandbox.tiket.com)  
We will inform you if its already provided in production server (api.tiket.com)

Add train order to shopping cart.

*Note : adult must more than or equal to infant

#### HTTP Request

    `https://api-sandbox.tiket.com/order/add/train?d=GMR&a=BD&date=2012-06-03&ret_date=&adult=1&child=0&token=13fc239d306bf7085708566b3d085b29&train_id=IVHAN1&subclass=A&output=json&conSalutation=Mr&conFirstName=b&conLastName=bl&conEmailAddress=be@scom&conPhone=0878121&nameAdult1=a&IdCardAdult1=111&noHpAdult1=%2B62878222&salutationAdult1=Mr&birthDateAdult1=1990-02-02`

#### Parameters
  
Name,Description,Format,Default,Mandatory  
d,Depart,train station code,CHAR(3),,TRUE  
a,Arrival train station code,CHAR(3),,TRUE  
date,depart date,YYYY-MM-DD,,TRUE  
ret_date,"return date. If want to book return",YYYY-MM-DD,,FALSE  
adult,"number of adult passenger (max adult+child+infant 4 persons)",INT,1,FALSE  
child,"number of child passenger (max adult+child+infant 4 persons)",INT,0,FALSE  
infant,"number of infant passenger (max adult+child+infant 4 persons)",INT,0,FALSE  
token,for saving transaction that done by user,CHAR(128),,TRUE  
train_id,train id that choosen by user,CHAR(~),,TRUE  
subclass,subclass from train that choosen by user,CHAR(1),,TRUE  
train_id_ret,train id that choosen by user for return,,,  
subclass_ret,subclass from train that choosen by user for return,,,  
conSalutation,"contact person title ( ex: Mr.,Mrs.,Ms.)",CHAR(5),,TRUE  
conFirstName,contact person first name,CHAR(50),,TRUE  
conLastName,contact person last name,CHAR(50),,TRUE  
conEmailAddress,contact person email address,CHAR(50),,TRUE  
conPhone,"contact person phone,[must begin with 08 or +62]",CHAR(20),,TRUE  
nameAdult1,as an array like nameAdult1 nameAdult2 if you have adult passager,CHAR(100),,  
IdCardAdult1,"as an array like IdCardAdult1 IdCardAdult2 if you have adult passager,[max 16 character]",CHAR(50),,  
noHpAdult1,"as an array like noHpAdult1 noHpAdult2 if you have adult passager, [must begin with 08 or +62]. Don't forget to urlencode + into %2B in the GET parameter",CHAR(20),,  
salutationAdult1,"as an array like salutationAdult1 salutationAdult2 if you have adult passager : Mr.,Ms.,Mrs.",CHAR(4),,  
birthDateAdult1,"as an array like birthDateAdult1 birthDateAdult2 if you have adult passager : format YYYY-MM-DD",DATE,,  
nameChild1,as an array like nameChild1 nameChild2 if you have Child passager,CHAR(50),,  
salutationChild1,"as an array like salutationChild1 salutationChild2 if you have Child passager : Mr.,Ms.,Mrs.",CHAR(4),,  
birthDateChild1,"as an array like birthDateChild1 birthDateChild2 if you have Child passager : format YYYY-MM-DD,[child must below 10 years old]",DATE,,  
salutationInfant1,"as an array like salutationInfant1 salutationInfant2 if you have infant passager : Mr.,Ms.,Mrs.",CHAR(4),,  
nameInfant1,as an array like nameInfant1 nameInfant2 if you have infant passager,CHAR(50),,  
birthDateInfant1,as an array like birthDateInfant1 birthDateInfant2 if you have infant passager : format YYYY-MM-DD [infant must below 2 years old],DATE,,  

   
    
    
## Order

* Display user shopping cart detail
    
    #### Parameters
    
      
    Name,Description,Format,Default,Mandatory  
    token,for saving transaction that done by user,CHAR(128),,TRUE  
    
    
    #### HTTP Request
    
        `https://api-sandbox.tiket.com/order?token=2279a50a996f5a54a15db6b10bfc5657&output=json`
    
    #### Output
    
    ```xml
        <tiket>
        	<output_type>xml</output_type>
        	<myorder>
        		<order_id>120687</order_id>
        		<data>
        			<expire>9</expire>
        			<order_detail_id>32754</order_detail_id>
        			<order_type>train</order_type>
        			<order_detail_status>active</order_detail_status>
        			<detail>
        				<arrival_datetime>2012-06-03 20:30:00</arrival_datetime>
        				<departure_datetime>2012-06-03 18:00:00</departure_datetime>
        				<count_adult>2</count_adult>
        				<book_code>KYVCY4</book_code>
        				<train_subclass>A</train_subclass>
        				<tiket_seating>EK-2-5-A,EK-2-5-B,EK-2-5-C,EK-2-5-D</tiket_seating>
        				<num_code>9995670208507</num_code>
        				<train_from>GMR</train_from>
        				<train_to>BD</train_to>
        				<train_name>Argo Jati</train_name>
        				<subclass_type>umum</subclass_type>
        				<class_name>eksekutif</class_name>
        				<train_from_station>gambir</train_from_station>
        				<train_to_station>bandung</train_to_station>
        				<price>404000</price>
        			</detail>
        			<order_photo>httpss://www.tiket.com/images/icon_kai.jpg</order_photo>
        			<tax_and_charge>14120</tax_and_charge>
        			<subtotal_and_charge>418120</subtotal_and_charge>
        			<delete_uri>
        				https://api.tiket.com/order/delete_order?order_detail_id=32754
        			</delete_uri>
        
        		</data>
        		<total>418120</total>
        		<total_tax>14120</total_tax>
        		<total_without_tax>404000</total_without_tax>
        		<count_installment>0</count_installment>
        	</myorder>
        	<diagnostic>
        		<elapstime>3.3222</elapstime>
        		<memoryusage>12.3MB</memoryusage>
        		<status>200</status>
        		<lang>en</lang>
        		<currency>IDR</currency>
        	</diagnostic>
        	<checkout>httpsss://www.tiket.com/order/checkout/120687/IDR</checkout>
        	<login_status>false</login_status>
        	<token>2279a50a996f5a54a15db6b10bfc5657</token>
        </tiket>
    ```
    
    ```json
        {"output_type":"json","myorder":{"order_id":120687,"currency":"IDR","data":[{"expire":2,"order_detail_id":"32754","order_type":"train","customer_price":"404000.00","customer_currency":"IDR","order_detail_status":"active","detail":[{"arrival_datetime":"2012-06-03 20:30:00","departure_datetime":"2012-06-03 18:00:00","count_adult":"2","count_child":"2","book_code":"KYVCY4","train_subclass":"A","tiket_seating":"EK-2-5-A,EK-2-5-B,EK-2-5-C,EK-2-5-D","num_code":"9995670208507","train_from":"GMR","train_to":"BD","train_name":"Argo Jati","subclass_type":"umum","class_name":"eksekutif","train_from_station":"gambir","train_to_station":"bandung","price":404000}],"order_photo":"httpss:\/\/api.tiket.com\/images\/icon_kai.jpg","tax_and_charge":14120,"subtotal_and_charge":418120,”delete_uri”https://api.tiket.com/order/delete_order?order_detail_id=32754”}],"total":418120,"total_tax":14120,"total_without_tax":404000,"count_installment":0},"diagnostic":{"elapstime":"3.6239","memoryusage":"12.28MB","status":"200","lang":"en","currency":"IDR"},"checkout":"httpsss:\/\/www.tiket.com\/order\/checkout\/120687\/IDR",”login_status":"false",token":"2279a50a996f5a54a15db6b10bfc5657"}
    ```
    
    ```matlab
        a:7:{s:11:"output_type";s:9:"serialize";s:7:"myorder";a:7:{s:8:"order_id";i:120687;s:8:"currency";s:3:"IDR";s:4:"data";a:1:{i:0;a:12:{s:6:"expire";i:1;s:15:"order_detail_id";s:5:"32754";s:10:"order_type";s:5:"train";s:14:"customer_price";s:9:"404000.00";s:17:"customer_currency";s:3:"IDR";s:19:"order_detail_status";s:6:"active";s:6:"detail";a:1:{i:0;a:22:{s:16:"arrival_datetime";s:19:"2012-06-03 20:30:00";s:18:"departure_datetime";s:19:"2012-06-03 18:00:00";s:11:"count_adult";s:1:"2";s:11:"count_child";s:1:"2";s:19:"sell_adult_currency";s:3:"IDR";s:19:"sell_child_currency";s:3:"IDR";s:22:"total_sell_adult_price";s:9:"212000.00";s:22:"total_sell_child_price";s:9:"192000.00";s:18:"extra_fee_currency";s:3:"IDR";s:15:"extra_fee_price";s:4:"0.00";s:9:"book_code";s:6:"KYVCY4";s:14:"train_subclass";s:1:"A";s:13:"tiket_seating";s:35:"EK-2-5-A,EK-2-5-B,EK-2-5-C,EK-2-5-D";s:8:"num_code";s:13:"9995670208507";s:10:"train_from";s:3:"GMR";s:8:"train_to";s:2:"BD";s:10:"train_name";s:9:"Argo Jati";s:13:"subclass_type";s:4:"umum";s:10:"class_name";s:9:"eksekutif";s:18:"train_from_station";s:6:"gambir";s:16:"train_to_station";s:7:"bandung";s:5:"price";d:404000;}}s:11:"order_photo";s:40:"httpss://api.tiket.com/images/icon_kai.jpg";s:8:"subtotal";d:404000;s:11:"item_charge";d:14120;s:14:"tax_and_charge";d:14120;s:19:"subtotal_and_charge";d:418120;d:14120;s:10:"delete_uri";s:40:”https://api.tiket.com/order/delete_order?order_detail_id=32754”;}}s:5:"total";d:418120;s:9:"total_tax";d:14120;s:17:"total_without_tax";d:404000;s:17:"count_installment";i:0;}s:10:"diagnostic";a:5:{s:9:"elapstime";s:14:"3.2849";s:11:"memoryusage";s:14:"12.28MB";s:6:"status";s:3:"200";s:4:"lang";s:2:"en";s:8:"currency";s:3:"IDR";}s:8:"checkout";s:47:"httpsss://www.tiket.com/order/checkout/120687/IDR";s:8:"login_status";s:0:"false";s:5:"token";s:32:"2279a50a996f5a54a15db6b10bfc5657";}
    ```
        
        
        
## Checkout Page Request

* Early stage to access checkout.
    
    link url can be get from order, variable checkout .
    
    #### Parameters
    
      
    Name,Description,Format,Default,Mandatory  
    token,for saving transaction that done by user,CHAR(128),,TRUE  
    
    
    #### HTTP Request
    
        `https://api-sandbox.tiket.com/order/checkout/119978/IDR?token=9991e3092aea96042964220181374b60&output=json`
    
    (Get from order page in checkout variable.)
    
    #### Output
    
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
        {"output_type":"json","next_checkout_uri":"httpsss:\/\/api-sandbox.tiket.com\/checkout\/checkout_customer","diagnostic":{“status":200,"elapsetime":"0.1157","memoryusage":"6.43MB","confirm":"success","lang":"id","currency":"IDR"},"login_status":"false","token":"9991e3092aea96042964220181374b60"}
    ```
    
    ```matlab
        a:5:{s:11:"output_type";s:9:"serialize";s:17:"next_checkout_uri";s:57:"httpsss://api-sandbox.tiket.com/checkout/checkout_customer";s:10:"diagnostic";a:7:{s:6:"status";i:200;s:10:"elapsetime";s:14:"0.1132";s:11:"memoryusage";s:14:"6.43MB";s:7:"confirm";s:7:"success";s:4:"lang";s:2:"id";s:8:"currency";s:3:"IDR";}s:12:"login_status";s:5:"false";s:5:"token";s:32:"9991e3092aea96042964220181374b60";}
    ```


## Checkout Login

* #### Parameters
    
      
    Name,Description,Format,Default,Mandatory  
    salutation,"your title( ex: Mr.,Mrs.,Ms.)",CHAR(5),,TRUE  
    firstName,your first name,CHAR(50),,TRUE  
    lastName,your last name,CHAR(50),,TRUE  
    emailAddress,your email,CHAR(50),,TRUE  
    phone,"your phone, ex: 081232323343 or +62324324234234. Don't forget to urlencode + into %2B in the GET parameter",CHAR(20),,TRUE  
    saveContinue,Flag for login (value=2),,,TRUE  
    
    
    #### HTTP Request
    
        [code]https://api-sandbox.tiket.com/checkout/checkout_customer?token=87da88eaaa429d5513a3a3658b01701e&salutation=Ms&firstName=ba&lastName=ca&emailAddress=test@yahoocom&phone=%2B62878434343&saveContinue=2[/code]
    
    Setelah merequest link tersebut maka user akan dibuatkan account di tiket.com user akan dikirimkan email untuk mengubah password loginnya.
    
    #### Output
    
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
        {"output_type":"json","diagnostic":{"status":200,"elapsetime":"0.1443","memoryusage":"7.77MB","confirm":"success","error_msgs":"","lang":"en","currency":"IDR"},"login_status":"true","guest_id":"21688","token":"5a80dc2ccce351eeb412e835b651edb9"}
    ```
    
    ```matlab
        [a:5:{s:11:"output_type";s:9:"serialize";s:10:"diagnostic";a:7:{s:6:"status";i:200;s:10:"elapsetime";s:14:"0.1628";s:11:"memoryusage";s:14:"7.77MB";s:7:"confirm";s:7:"success";s:10:"error_msgs";s:0:"";s:4:"lang";s:2:"en";s:8:"currency";s:3:"IDR";}s:12:"login_status";s:4:"true";s:8:"guest_id";s:5:"21688";s:5:"token";s:32:"9d4ccf0c966e37a4c112c59ac2bc2e97";}
    ```


## Available Payment

* #### Parameters
    
      
    Name,Description,Format,Default,Mandatory  
    token,for saving transaction that done by user,CHAR(128),,TRUE  
    
    
    #### HTTP Request
    
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

* #### Please see [Checkout Payment](http://docs.tiket.com/#checkout-payment-309) in General API



## Register


* For user registration.
    
    #### Parameters
    
      
    Name,Description,Format,Default,Mandatory  
    firstName,your firstname,CHAR,,TRUE  
    lastName,your lastname,CHAR,,TRUE  
    email,"your email [must email format]",CHAR,,TRUE  
    password,your password min 6 char,CHAR,,TRUE  
    conPassword,confirm password,CHAR,,TRUE  
    country,"your country [must in country list]",CHAR(50),,TRUE  
    
    
    #### HTTP Request
    
        `https://api-sandbox.tiket.com/auth/register?token=9d941b962ff17f828046a1d45432c6d4&firstName=cob&lastName=kib&email=youjulin@gmailcom&password=hahaha&conPassword=hahaha&country=id&output=json`
    
    #### Output
    
    ```xml
        <tiket>
        	<output_type>xml</output_type>
        	<diagnostic>
        		<status>200</status>
        		<elapsetime>7.5683</elapsetime>
        		<memoryusage>17.47MB</memoryusage>
        		<confirm>success</confirm>
        		<lang>en</lang>
        		<currency>IDR</currency>
        	</diagnostic>
        	<token>9d941b962ff17f828046a1d45432c6d4</token>
        </tiket>
    ```
    
    ```json
        {"output_type":"json","diagnostic":{"status":200,"elapsetime":"6.3380","memoryusage":"17.45MB","confirm":"success","lang":"en","currency":"IDR"},"token":"9d941b962ff17f828046a1d45432c6d4"}
    ```
    
    ```matlab
        a:3:{s:11:"output_type";s:9:"serialize";s:10:"diagnostic";a:6:{s:6:"status";i:200;s:10:"elapsetime";s:14:"5.7164";s:11:"memoryusage";s:14:"17.45MB";s:7:"confirm";s:7:"success";s:4:"lang";s:2:"en";s:8:"currency";s:3:"IDR";}s:5:"token";s:32:"9d941b962ff17f828046a1d45432c6d4";}
    ```


## Search Promo


* #### Parameters
    
      
    Name,Description,Format,Default,Mandatory  
    d,Departure station,CHAR,,TRUE  
    date,Date to depart,DATE,,TRUE  
    
    
    #### HTTP Request
    
        `https://api-sandbox.tiket.com/train_api/train_promo?d=GMR&date=2012-06-28&token=4206f440696c91b855581fb2eafac225&output=json`
    
    #### Output
    
    ```xml
        <tiket>
        	<promo>
        		<list_promo>
        			<train_name>Argo Jati</train_name>
        			<train_id>IVHAN1</train_id>
        			<schedule_departure_time>18:00:00</schedule_departure_time>
        			<schedule_arrival_time>20:30:00</schedule_arrival_time>
        			<class_id>eks</class_id>
        			<detail_price_adult_formatted>IDR 106.000,00</detail_price_adult_formatted>
        			<detail_price_children_formatted>IDR 96.000,00</detail_price_children_formatted>
        			<detail_price_adult_ori>106000</detail_price_adult_ori>
        			<detail_price_children_ori>96000</detail_price_children_ori>
        			<detail_availability>100</detail_availability>
        		</list_promo>
        		<list_promo>
        			<train_name>Argo Anggrek Malam</train_name>
        			<train_id>IVHAN2</train_id>
        			<schedule_departure_time>19:00:00</schedule_departure_time>
        			<schedule_arrival_time>20:40:00</schedule_arrival_time>
        			<class_id>eks</class_id>
        			<detail_price_adult_formatted>IDR 106.000,00</detail_price_adult_formatted>
        			<detail_price_children_formatted>IDR 96.000,00</detail_price_children_formatted>
        			<detail_price_adult_ori>106000</detail_price_adult_ori>
        			<detail_price_children_ori>96000</detail_price_children_ori>
        			<detail_availability>80</detail_availability>
        		</list_promo>
        	<des>BD</des>
        	<des_name>Bandung, Bandung</des_name>
        	</promo>
        	<promo>
        		<list_promo>
        			<train_name>Argo Jati</train_name>
        			<train_id>IVHAN1</train_id>
        			<schedule_departure_time>18:00:00</schedule_departure_time>
        			<schedule_arrival_time>23:50:00</schedule_arrival_time>
        			<class_id>eks</class_id>
        			<detail_price_adult_formatted>IDR 96.000,00</detail_price_adult_formatted>
        			<detail_price_children_formatted>IDR 86.000,00</detail_price_children_formatted>
        			<detail_price_adult_ori>96000</detail_price_adult_ori>
        			<detail_price_children_ori>86000</detail_price_children_ori>
        			<detail_availability>100</detail_availability>
        		</list_promo>
        		<list_promo>
        			<train_name>Argo Anggrek Malam</train_name>
        			<train_id>IVHAN2</train_id>
        			<schedule_departure_time>19:00:00</schedule_departure_time>
        			<schedule_arrival_time>23:30:00</schedule_arrival_time>
        			<class_id>eks</class_id>
        			<detail_price_adult_formatted>IDR 96.000,00</detail_price_adult_formatted>
        			<detail_price_children_formatted>IDR 86.000,00</detail_price_children_formatted>
        			<detail_price_adult_ori>96000</detail_price_adult_ori>
        			<detail_price_children_ori>86000</detail_price_children_ori>
        			<detail_availability>80</detail_availability>
        		</list_promo>
        		<des>YK</des>
        		<des_name>Tugu Yogyakarta, Yogyakarta</des_name>
        	</promo>
        	<output_type>xml</output_type>
        	<diagnostic>
        		<status>200</status>
        		<elapsetime>5.7507</elapsetime>
        		<memoryusage>15.74MB</memoryusage>
        		<confirm>success</confirm>
        		<lang>en</lang>
        		<currency>IDR</currency>
        	</diagnostic>
        	<token>4206f440696c91b855581fb2eafac225</token>
        </tiket>
    ```
    
    ```json
        {"promo":[{"list_promo":[{"train_name":"Argo Jati","train_id":"IVHAN1","schedule_departure_time":"18:00:00","schedule_arrival_time":"20:30:00","class_id":"eks","detail_price_adult_formatted":"IDR 106.000,00","detail_price_children_formatted":"IDR 96.000,00","detail_price_adult_ori":106000,"detail_price_children_ori":96000,"detail_availability":"100"},{"train_name":"Argo Anggrek Malam","train_id":"IVHAN2","schedule_departure_time":"19:00:00","schedule_arrival_time":"20:40:00","class_id":"eks","detail_price_adult_formatted":"IDR 106.000,00","detail_price_children_formatted":"IDR 96.000,00","detail_price_adult_ori":106000,"detail_price_children_ori":96000,"detail_availability":"80"}],"des":"BD","des_name":"Bandung, Bandung"},{"list_promo":[{"train_name":"Argo Jati","train_id":"IVHAN1","schedule_departure_time":"18:00:00","schedule_arrival_time":"23:50:00","class_id":"eks","detail_price_adult_formatted":"IDR 96.000,00","detail_price_children_formatted":"IDR 86.000,00","detail_price_adult_ori":96000,"detail_price_children_ori":86000,"detail_availability":"100"},{"train_name":"Argo Anggrek Malam","train_id":"IVHAN2","schedule_departure_time":"19:00:00","schedule_arrival_time":"23:30:00","class_id":"eks","detail_price_adult_formatted":"IDR 96.000,00","detail_price_children_formatted":"IDR 86.000,00","detail_price_adult_ori":96000,"detail_price_children_ori":86000,"detail_availability":"80"}],"des":"YK","des_name":"Tugu Yogyakarta, Yogyakarta"}],"output_type":"json","diagnostic":{"status":200,"elapsetime":"3.5902","memoryusage":"15.71MB","confirm":"success","lang":"en","currency":"IDR"},"token":"4206f440696c91b855581fb2eafac225"}
    ```
    
    ```matlab
        a:4:{s:5:"promo";a:2:{i:0;a:3:{s:10:"list_promo";a:3:{i:0;a:10:{s:10:"train_name";s:9:"Argo Jati";s:8:"train_id";s:6:"IVHAN1";s:23:"schedule_departure_time";s:8:"18:00:00";s:21:"schedule_arrival_time";s:8:"20:30:00";s:8:"class_id";s:3:"eks";s:28:"detail_price_adult_formatted";s:14:"IDR 106.000,00";s:31:"detail_price_children_formatted";s:13:"IDR 96.000,00";s:22:"detail_price_adult_ori";d:106000;s:25:"detail_price_children_ori";d:96000;s:19:"detail_availability";s:3:"100";}i:1;a:10:{s:10:"train_name";s:18:"Argo Anggrek Malam";s:8:"train_id";s:6:"IVHAN2";s:23:"schedule_departure_time";s:8:"19:00:00";s:21:"schedule_arrival_time";s:8:"20:40:00";s:8:"class_id";s:3:"eks";s:28:"detail_price_adult_formatted";s:14:"IDR 106.000,00";s:31:"detail_price_children_formatted";s:13:"IDR 96.000,00";s:22:"detail_price_adult_ori";d:106000;s:25:"detail_price_children_ori";d:96000;s:19:"detail_availability";s:2:"80";}}s:3:"des";s:2:"BD";s:8:"des_name";s:16:"Bandung, Bandung";}i:1;a:3:{s:10:"list_promo";a:3:{i:0;a:10:{s:10:"train_name";s:9:"Argo Jati";s:8:"train_id";s:6:"IVHAN1";s:23:"schedule_departure_time";s:8:"18:00:00";s:21:"schedule_arrival_time";s:8:"23:50:00";s:8:"class_id";s:3:"eks";s:28:"detail_price_adult_formatted";s:13:"IDR 96.000,00";s:31:"detail_price_children_formatted";s:13:"IDR 86.000,00";s:22:"detail_price_adult_ori";d:96000;s:25:"detail_price_children_ori";d:86000;s:19:"detail_availability";s:3:"100";}i:1;a:10:{s:10:"train_name";s:18:"Argo Anggrek Malam";s:8:"train_id";s:6:"IVHAN2";s:23:"schedule_departure_time";s:8:"19:00:00";s:21:"schedule_arrival_time";s:8:"23:30:00";s:8:"class_id";s:3:"eks";s:28:"detail_price_adult_formatted";s:13:"IDR 96.000,00";s:31:"detail_price_children_formatted";s:13:"IDR 86.000,00";s:22:"detail_price_adult_ori";d:96000;s:25:"detail_price_children_ori";d:86000;s:19:"detail_availability";s:2:"80";}}s:3:"des";s:2:"YK";s:8:"des_name";s:27:"Tugu Yogyakarta, Yogyakarta";}}s:11:"output_type";s:9:"serialize";s:10:"diagnostic";a:6:{s:6:"status";i:200;s:10:"elapsetime";s:14:"2.7337";s:11:"memoryusage";s:14:"15.72MB";s:7:"confirm";s:7:"success";s:4:"lang";s:2:"en";s:8:"currency";s:3:"IDR";}s:5:"token";s:32:"4206f440696c91b855581fb2eafac225";}
    ```



## Change Train Seat

* Change Train Seat
    
    #### Parameters
    
      
    Name,Description,Format,Default,Mandatory  
    booking_code,"Booking Code",CHAR(6),,TRUE  
    kode_wagon,"Wagon Code",VARCHAR(5),,TRUE  
    nomor_wagon,"Wagon number",VARCHAR(2),,TRUE  
    nomor_kursi,"Seating Number",VARCHAR(3),,TRUE  
    order_detail_id,"Order Detail ID",NUMERIC,,TRUE  
    token,for saving transaction that done by user,CHAR(128),,TRUE  
    
    
    #### HTTP Request
    
        `http://api.tiket.com/general_api/train_change_seat?output=json&booking_code=5WWAS1&kode_wagon=EKS&nomor_wagon=2&nomor_kursi=4D&order_detail_id=327247&token=6d360dfd1dab82b3fa42e453abafff91`
    
    #### Output
    
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
        { diagnostic: { status: 200, elapsetime: "2.9133", memoryusage: "3.31MB", confirm: "success", lang: "id", currency: "IDR" }, output_type: "json", result: { err_code: 0, book_code: "KIQWWR", wagon_code: "EKS", wagon_no: 2, seat: [ "3A","3B" ] }, login_status: "false", token: "6d360dfd1dab82b3fa42e453abafff91" }
    ```
    
    ```matlab
        { diagnostic: { status: 200, elapsetime: "2.9133", memoryusage: "3.31MB", confirm: "success", lang: "id", currency: "IDR" }, output_type: "json", result: { err_code: 0, book_code: "KIQWWR", wagon_code: "EKS", wagon_no: 2, seat: [ "3A","3B" ] }, login_status: "false", token: "6d360dfd1dab82b3fa42e453abafff91" }
    ```















