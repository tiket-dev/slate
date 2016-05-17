# Order History

## Check Order

```xml
    <tiket>
    	<diagnostic>
    		<status>200</status>
    		<elapsetime>0.1648</elapsetime>
    		<memoryusage>4.36MB</memoryusage>
    		<confirm>success</confirm>
    		<lang>en</lang>
    		<currency>IDR</currency>
    	</diagnostic>
    	<output_type>xml</output_type>
    	<result>
    		<order_id>783328</order_id>
    		<order_timestamp>2013-06-14 16:30:19</order_timestamp>
    		<payment_timestamp>2013-06-14 16:30:19</payment_timestamp>
    		<payment_status>paid</payment_status>
    		<total_customer_price>1454685.00</total_customer_price>
    		<customer_currency>IDR</customer_currency>
    		<mobile_phone>+628979331828</mobile_phone>
    		<all_order_type>flight</all_order_type>
    		<order__cart_detail>
    			<order_detail_id>46276</order_detail_id>
    			<order_type>flight</order_type>
    			<order_name>CGK (Jakarta) - DPS (Denpasar, Bali)</order_name>
    			<order_name_detail>Garuda (GA-724 - Depart)</order_name_detail>
    			<customer_currency>IDR</customer_currency>
    			<customer_price>1427700.00</customer_price>
    			<total_ticket>1</total_ticket>
    			<detail>
    				<order_timestamp>2013-06-14 16:30:19</order_timestamp>
    				<mobile_phone>+628979331828</mobile_phone>
    				<order_detail_status>active</order_detail_status>
    				<order_expire_datetime>2013-06-14 16:52:25</order_expire_datetime>
    				<flight_number>GA 724</flight_number>
    				<trip>trip</trip>
    				<airlines_name>GARUDA</airlines_name>
    				<departure_city>CGK</departure_city>
    				<departure_time>2013-06-18 06:15:00</departure_time>
    				<arrival_city>DPS</arrival_city>
    				<arrival_time>2013-06-18 09:20:00</arrival_time>
    				<ticket_class>Q</ticket_class>
    				<booking_code>JRA664</booking_code>
    				<count_adult>1</count_adult>
    				<count_child>0</count_child>
    				<count_infant>0</count_infant>
    				<contact_title>Ms</contact_title>
    				<contact_first_name>Dwi</contact_first_name>
    				<contact_phone>+628979331827</contact_phone>
    				<contact_other_phone/>
    				<ticket_status>issued</ticket_status>
    				<depart_airport>SOEKARNO-HATTA</depart_airport>
    				<arrival_airport>NGURAH RAI</arrival_airport>
    			</detail>
    			<send_uri>
    			http://api-sandbox.tiket.com/check_order/resendVoucher?												type=flight&order_id=783328&order_detail_id=46276&order_hash=f83621c837ace2da7f2decf9d6cd14e9&account_id=212868
    			</send_uri>
    			<print_uri>
    				http://api-sandbox.tiket.com/check_order/printVoucher?type=flight&order_id=783328&order_detail_id=46276&order_hash=f83621c837ace2da7f2decf9d6cd14e9&account_id=212868
    			</print_uri>
    			<passanger>
    				<passanger_baggage/>
    				<passenger_name>Ms Dwi Christanti</passenger_name>
    				<passenger_age_group>adult</passenger_age_group>
    				<passenger_id_number>12345678</passenger_id_number>
    				<passenger_birth_date/>
    			</passanger>
    		</order__cart_detail>
    		<order__payment>
    			<payment_currency>IDR</payment_currency>
    			<payment_amount>1454685.00</payment_amount>
    			<transfer_date/>
    			<payment_source>visa</payment_source>
    			<card_number>1111</card_number>
    			<expiry_month>10</expiry_month>
    			<expiry_year>2013</expiry_year>
    			<card_holder_name>Dwi Christanti</card_holder_name>
    		</order__payment>
    	</result>
    	<login_status>false</login_status>
    	<token>2cb3e09371fe7c0d78efa936bf1fd245</token>
    </tiket>
    
```



```json
    {
    	diagnostic: {
    		status: 200,
    		elapsetime: "0.4144",
    		memoryusage: "15.41MB",
    		confirm: "success",
    		lang: "en",
    		currency: "IDR"
    },
    	output_type: "json",
    	result: {
    		order_id: "783328",
    		order_timestamp: "2013-06-14 16:30:19",
    		payment_timestamp: "2013-06-14 16:30:19",
    		payment_status: "paid",
    		total_customer_price: "1454685.00",
    		customer_currency: "IDR",
    		mobile_phone: "+628979331828",
    		all_order_type: "flight",
    		order__cart_detail: [
    		{
    			order_detail_id: "46276",
    			order_type: "flight",
    			order_name: "CGK (Jakarta) - DPS (Denpasar, Bali)",
    			order_name_detail: "Garuda (GA-724 - Depart)",
    			customer_currency: "IDR",
    			customer_price: "1427700.00",
    			total_ticket: "1",
    			detail: {
    				order_timestamp: "2013-06-14 16:30:19",
    				mobile_phone: "+628979331828",
    				order_detail_status: "active",
    				order_expire_datetime: "2013-06-14 16:52:25",
    				flight_number: "GA 724",
    				trip: "trip",
    				airlines_name: "GARUDA",
    				departure_city: "CGK",
    				departure_time: "2013-06-18 06:15:00",
    				arrival_city: "DPS",
    				arrival_time: "2013-06-18 09:20:00",
    				ticket_class: "Q",
    				booking_code: "JRA664",
    				count_adult: "1",
    				count_child: "0",
    				count_infant: "0",
    				contact_title: "Ms",
    				contact_first_name: "Dwi",
    				contact_phone: "+628979331827",
    				contact_other_phone: "",
    				ticket_status: "issued",
    				depart_airport: "SOEKARNO-HATTA",
    				arrival_airport: "NGURAH RAI"
    			},
    			send_uri: "http://api-sandbox.tiket.com/check_order/resendVoucher?type=flight&order_id=783328&order_detail_id=46276&order_hash=f83621c837ace2da7f2decf9d6cd14e9&account_id=212868",
    			print_uri: "http://api-sandbox.tiket.com/check_order/printVoucher?type=flight&order_id=783328&order_detail_id=46276&order_hash=f83621c837ace2da7f2decf9d6cd14e9&account_id=212868",
    			passanger: [
    			{
    				passanger_baggage: "",
    				passenger_name: "Ms Dwi Christanti",
    				passenger_age_group: "adult",
    				passenger_id_number: "12345678",
    				passenger_birth_date: ""
    			}
    		]
    	}
    	],
    	order__payment: [
    	{
    		payment_currency: "IDR",
    		payment_amount: "1454685.00",
    		transfer_date: null,
    		payment_source: "visa",
    		card_number: "1111",
    		expiry_month: "10",
    		expiry_year: "2013",
    		card_holder_name: "Dwi Christanti"
    	}
    	],
    	order__confirmation: [ ]
    	},
    		login_status: "false",
    		token: "6012674c2d15983e2c967c5da373ceeb"
    	}
```



```matlab
a:5:{s:10:"diagnostic";a:6:{s:6:"status";i:200;s:10:"elapsetime";s:14:"0.3514";s:11:"memoryusage";s:14:"4.39MB";s:7:"confirm";s:7:"success";s:4:"lang";s:2:"en";s:8:"currency";s:3:"IDR";}s:11:"output_type";s:9:"serialize";s:6:"result";a:11:{s:8:"order_id";s:6:"783328";s:15:"order_timestamp";s:19:"2013-06-14 16:30:19";s:17:"payment_timestamp";s:19:"2013-06-14 16:30:19";s:14:"payment_status";s:4:"paid";s:20:"total_customer_price";s:10:"1454685.00";s:17:"customer_currency";s:3:"IDR";s:12:"mobile_phone";s:13:"+628979331828";s:14:"all_order_type";s:6:"flight";s:18:"order__cart_detail";a:1:{i:0;a:11:{s:15:"order_detail_id";s:5:"46276";s:10:"order_type";s:6:"flight";s:10:"order_name";s:36:"CGK (Jakarta) - DPS (Denpasar, Bali)";s:17:"order_name_detail";s:24:"Garuda (GA-724 - Depart)";s:17:"customer_currency";s:3:"IDR";s:14:"customer_price";s:10:"1427700.00";s:12:"total_ticket";s:1:"1";s:6:"detail";a:23:{s:15:"order_timestamp";s:19:"2013-06-14 16:30:19";s:12:"mobile_phone";s:13:"+628979331828";s:19:"order_detail_status";s:6:"active";s:21:"order_expire_datetime";s:19:"2013-06-14 16:52:25";s:13:"flight_number";s:6:"GA 724";s:4:"trip";s:4:"trip";s:13:"airlines_name";s:6:"GARUDA";s:14:"departure_city";s:3:"CGK";s:14:"departure_time";s:19:"2013-06-18 06:15:00";s:12:"arrival_city";s:3:"DPS";s:12:"arrival_time";s:19:"2013-06-18 09:20:00";s:12:"ticket_class";s:1:"Q";s:12:"booking_code";s:6:"JRA664";s:11:"count_adult";s:1:"1";s:11:"count_child";s:1:"0";s:12:"count_infant";s:1:"0";s:13:"contact_title";s:2:"Ms";s:18:"contact_first_name";s:3:"Dwi";s:13:"contact_phone";s:13:"+628979331827";s:19:"contact_other_phone";s:0:"";s:13:"ticket_status";s:6:"issued";s:14:"depart_airport";s:14:"SOEKARNO-HATTA";s:15:"arrival_airport";s:10:"NGURAH RAI";}s:8:"send_uri";s:167:"http://api-sandbox.tiket.com/check_order/resendVoucher?type=flight&order_id=783328&order_detail_id=46276&order_hash=f83621c837ace2da7f2decf9d6cd14e9&account_id=212868";s:9:"print_uri";s:166:"http://api-sandbox.tiket.com/check_order/printVoucher?type=flight&order_id=783328&order_detail_id=46276&order_hash=f83621c837ace2da7f2decf9d6cd14e9&account_id=212868";s:9:"passanger";a:1:{i:0;a:5:{s:17:"passanger_baggage";s:0:"";s:14:"passenger_name";s:17:"Ms Dwi Christanti";s:19:"passenger_age_group";s:5:"adult";s:19:"passenger_id_number";s:8:"12345678";s:20:"passenger_birth_date";s:0:"";}}}}s:14:"order__payment";a:1:{i:0;a:8:{s:16:"payment_currency";s:3:"IDR";s:14:"payment_amount";s:10:"1454685.00";s:13:"transfer_date";N;s:14:"payment_source";s:4:"visa";s:11:"card_number";s:4:"1111";s:12:"expiry_month";s:2:"10";s:11:"expiry_year";s:4:"2013";s:16:"card_holder_name";s:14:"Dwi Christanti";}}s:19:"order__confirmation";a:0:{}}s:12:"login_status";s:5:"false";s:5:"token";s:32:"da493c4f3c2212e44f60d06fe19eb3ef";}
```


Check Transaction detail

#### Parameters

  
Name | Description | Format | Default | Mandatory  
---- | ----------- | -----  | ------- | -----------
email | customer email | VARCHAR | getToken | TRUE  
order_id | order id want to check | NUMERIC | getToken | TRUE  
secretkey | API secret key given by Tiket.com | CHAR(128) | TRUE  


#### HTTP Request

    `https://api-sandbox.tiket.com/check_order?order_id=783328&email=dwi@tiket.com&output=xml`




    
    
