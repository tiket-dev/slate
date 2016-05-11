# Getting API Key

Before you can use our API, you have to get your secret key. You can access http://www.tiket.com/affiliate and enter your detail information there. After submitting, you will receive your username, password and API key. This account can be used for affiliate program and reseller program.

When you are done implementing this, we will require you to go through some UAT tests (user acceptance test). This test is to ensure that you have properly implement our API and booking flow untuk payment. Detail of the UAT test cases can be downloaded here.

We have two URL with totally different server data:

API development : [api-sandbox.tiket.com](http://api-sandbox.tiket.com)
API production : [api.tiket.com](https://api.tiket.com)

Both might have different content, so please don’t compare api-sandbox.tiket.com data with the real data at www.tiket.com



```http
GET /apiv1/payexpress?method=getToken&secretkey=56c8624d6a62e1ab22f0d9915ff2d43c&output=[json|xml|serialize|array] HTTP/1.1
Host: api-sandbox.tiket.com
User-Agent: twh:123456789;Partner Name;
Content-Type: text/plain
```
<aside class="notice">
We require you to send header data user-agent when requesting API using the following format:

<p><code>twh:[BUSINESS_ID];[BUSINESS_NAME];</code></p>

<p>All API request without this format will be blocked by the firewall.</p>
</aside>