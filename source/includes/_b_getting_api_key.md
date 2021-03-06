# Getting API Key

Before you can use our API, you have to get your secret key. You can access http://www.tiket.com/affiliate and enter your detail information there. After submitting, you will receive your username, password and API key. This account can be used for affiliate program and reseller program.

When you are done implementing this, we will require you to go through some UAT tests (user acceptance test). This test is to ensure that you have properly implement our API and booking flow untuk payment. Detail of the UAT test cases can be downloaded here.

We have two URL with totally different server data:

* API development : [api-sandbox.tiket.com](http://api-sandbox.tiket.com)
* API production : [api.tiket.com](https://api.tiket.com)

* PG development : [sandbox.tiket.com](http://sandbox.tiket.com)
* PG production : [www.tiket.com](https://www.tiket.com)

Both might have different content, so please don’t compare the content from the **sandbox** data with the real data at api.tiket.com/www.tiket.com.

IMPORTANT NOTE : To start development, please create an account at http://sandbox.tiket.com/affiliate first to get a development server account. Your first secret key will be generated there on partner dashboard API section. After finishing UAT tests, your development secret key could be leveraged to production state on Tiket.com.


```http
GET /apiv1/payexpress?method=getToken&secretkey=[your-secret-key-here]&output=[json|xml|serialize|array] HTTP/1.1
Host: api-sandbox.tiket.com
User-Agent: twh:123456789;Partner Name;
Content-Type: text/plain
```
<aside class="notice">
We require you to send header data user-agent when requesting API using the following format:
<br /><br />
<p><code>twh:[BUSINESS_ID];[BUSINESS_NAME];</code></p>

<p>All API request without this format will be blocked by the firewall.</p>
</aside>
