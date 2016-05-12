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
  - d_general_api
  
search: true
---

# Introduction

API development URL : [api-sandbox.tiket.com](http://api-sandbox.tiket.com)
API production URL : [api.tiket.com](https://api.tiket.com)

Tiket.com offers an all you can book experience. You can book flights, hotels, train, concerts, and attractions all in one place. And the good part is, they are all available through API!

You can develop your own website or mobile application according to your desires. All data needed will be provided by API from Tiket.com.

You can register for an API here,
and for development here

Before continuing develop your Web or Apps using Tiket.com API, you must understand and agree with the following items:

* The email address that you will submit to Tiket.com API must be the user’s email address. Sometimes our partner will send notification to the customers via the email address submitted about rescheduled flight or change in the hotel booking. If at one point we find out that you are not using customers email when you submit your booking and the customer complained about not receiving email notification on changes in booking, then *we will reserve the right to **suspend** or **terminate** your API account*.
* This also goes to the user’s mobile phone number. You must submit user’s mobile phone, because airlines sometimes update our customers schedule or flight itinerary through text messaging (SMS).
* There is no customized PDF vouchers. The email that we send to the customers is AS IS and no changes can be done with how the PDF vouchers look.
* Tiket.com is an OTA business and not GDS or white-label business. Our license and operation are designed as a travel agent. Tiket.com will always be held liable and responsible for any bookings, even through the Tiket.com API. Thus we require you to adhere with our policy.

API are available in JSON, XML, and PHP serialized format. There are two flow of payments that you can choose:

* deposit: by putting money deposit at Tiket.com, you can manage your own transaction and payment. API will return insufficient fund if you have ran out of deposit. You can’t continue using the API if you haven’t deposit any.
* regular: Tiket.com offers diverse payment channel. You can ask user to pay using API (for bank transfer and KlikBCA), or redirect them to our payment gateway (for credit card and BCA KlikPay). You don’t have to put any deposit if you are using this flow of payment.

PS : The Development API (api-sandbox.tiket.com) will emit  SSL error when using the HTTPS protocol. This is normal. You can actually use the HTTP protocol in the Development API to avoid SSL error, but you must use HTTPS at the Production API.



















Welcome to the Kittn API! You can use our API to access Kittn API endpoints, which can get information on various cats, kittens, and breeds in our database.

We have language bindings in Shell, Ruby, and Python! You can view code examples in the dark area to the right, and you can switch the programming language of the examples with the tabs in the top right.

This example API documentation page was created with [Slate](https://github.com/tripit/slate). Feel free to edit it and use it as a base for your own API's documentation.

# Authentication

> To authorize, use this code:

```ruby
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
```

```python
import kittn

api = kittn.authorize('meowmeowmeow')
```

```shell
# With shell, you can just pass the correct header with each request
curl "api_endpoint_here"
  -H "Authorization: meowmeowmeow"
```

> Make sure to replace `meowmeowmeow` with your API key.

Kittn uses API keys to allow access to the API. You can register a new Kittn API key at our [developer portal](http://example.com/developers).

Kittn expects for the API key to be included in all API requests to the server in a header that looks like the following:

`Authorization: meowmeowmeow`

<aside class="notice">
You must replace <code>meowmeowmeow</code> with your personal API key.
</aside>

# Kittens

## Get All Kittens

```ruby
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.kittens.get
```

```python
import kittn

api = kittn.authorize('meowmeowmeow')
api.kittens.get()
```

```shell
curl "http://example.com/api/kittens"
  -H "Authorization: meowmeowmeow"
```

> The above command returns JSON structured like this:

```json
[
  {
    "id": 1,
    "name": "Fluffums",
    "breed": "calico",
    "fluffiness": 6,
    "cuteness": 7
  },
  {
    "id": 2,
    "name": "Max",
    "breed": "unknown",
    "fluffiness": 5,
    "cuteness": 10
  }
]
```

This endpoint retrieves all kittens.

### HTTP Request

`GET http://example.com/api/kittens`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
include_cats | false | If set to true, the result will also include cats.
available | true | If set to false, the result will include kittens that have already been adopted.

<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

## Get a Specific Kitten

```ruby
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.kittens.get(2)
```

```python
import kittn

api = kittn.authorize('meowmeowmeow')
api.kittens.get(2)
```

```shell
curl "http://example.com/api/kittens/2"
  -H "Authorization: meowmeowmeow"
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "name": "Max",
  "breed": "unknown",
  "fluffiness": 5,
  "cuteness": 10
}
```

This endpoint retrieves a specific kitten.

<aside class="warning">Inside HTML code blocks like this one, you can't use Markdown, so use <code>&lt;code&gt;</code> blocks to denote code.</aside>

### HTTP Request

`GET http://example.com/kittens/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the kitten to retrieve

