# Payment

## Checkout Payment

```xml
<tiket>
  <output_type>xml</output_type>
  <diagnostic>
    <status>200</status>
    <elapsetime>0.5302</elapsetime>
    <memoryusage>14.77MB</memoryusage>
    <lang>id</lang>
    <currency>IDR</currency>
  </diagnostic>
  <result>
    <payment_discount>32665</payment_discount>
    <order_id>149584</order_id>
    <currency>IDR</currency>
    <payment_charge>4000</payment_charge>
    <sub_total>1386600</sub_total>
    <unique_code>0</unique_code>
    <grand_total>1390600</grand_total>
    <grand_subtotal>1423265</grand_subtotal>
  </result>
  <token>136637980b7b0e13ef3af9adbe571304</token>
</tiket>
```

> Grand_subtotal - payment_discount = sub_total
> subtotal + payment_charge + unique_code = grand_total

Completing checkout process with selected payment method.

Because Tiket.com domicile in Indonesia, it is mandatory that the payment is in IDR (Indonesia Rupiah). When you checkout using <code>checkout_payment</code>, you must pass the parameter <code>&currency=IDR</code> to ensure that the payment is in IDR.

<aside class="warn">When you submit without <code>btn_booking</code>, then it will only show payment information without processing the payment itself. This is useful if you wanted to know how much is the final price for the selected payment method</aside>

