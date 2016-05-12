---
title: Tiket.com API Documentation

language_tabs:
  - xml : XML
  - json : JSON
  - matlab : PHP Serialize

toc_footers:
  - <a href='http://sandbox.tiket.com/affiliate'>Sign Up for a Developer Key</a>


includes:
  - b_getting_api_key
  - c_uat_scenario
  - d_general_api
  - e_payment
  - f_order_history
  - g_deposit_payment
  - h_flight_api
  - i_hotel_api
  - j_event_api
  - k_train_api
  - kitten

  
search: true
---

# Introduction

Tiket.com offers an all you can book experience. You can book flights, hotels, train, concerts, and attractions all in one place. And the good part is, they are all available through API!

You can develop your own website or mobile application according to your desires. All data needed will be provided by API from Tiket.com.

You can register for an API here,
and for development here

Before continuing develop your Web or Apps using Tiket.com API, you must understand and agree with the following items:

* The email address that you will submit to Tiket.com API must be the user’s email address. Sometimes our partner will send notification to the customers via the email address submitted about rescheduled flight or change in the hotel booking. If at one point we find out that you are not using customers email when you submit your booking and the customer complained about not receiving email notification on changes in booking, then *we will reserve the right to **suspend** or **terminate** your API account*.
* This also goes to the user’s mobile phone number. You must submit user’s mobile phone, because airlines sometimes update our customers schedule or flight itinerary through text messaging (SMS).
* There is no customized PDF vouchers. The email that we send to the customers is AS IS and no changes can be done with how the PDF vouchers look.
* Tiket.com is an OTA business and not GDS or white-label business. Our license and operation are designed as a travel agent. Tiket.com will always be held liable and responsible for any bookings, even through the Tiket.com API. Thus we require you to adhere with our policy.

<aside class="success">
To access our API, kindly user the following URL:
<ul>
<li>API development URL : <a href="https://api-sandbox.tiket.com" target="_blank">https://api-sandbox.tiket.com</a></li>
<li>API production URL : <a href="https://api.tiket.com" target="_blank">https://api.tiket.com</a></li>
</ul>
</aside>


API are available in JSON, XML, and PHP serialized format. There are two flow of payments that you can choose:

* **deposit**: by putting money deposit at Tiket.com, you can manage your own transaction and payment. API will return insufficient fund if you have ran out of deposit. You can’t continue using the API if you haven’t deposit any.
* **regular**: Tiket.com offers diverse payment channel. You can ask user to pay using API (for bank transfer and KlikBCA), or redirect them to our payment gateway (for credit card and BCA KlikPay). You don’t have to put any deposit if you are using this flow of payment.

<aside class="notice">The Development API (api-sandbox.tiket.com) will emit  SSL error when using the HTTPS protocol. This is normal. You can actually use the HTTP protocol in the Development API to avoid SSL error, but you must use HTTPS at the Production API.</aside>




