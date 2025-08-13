---
description: Check the status of a payment by calling the P-Link.io API
layout:
  width: default
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: false
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
---

# Payment Status

## Checking payment status

### Status verification

After payment, the user is redirected to your URL with added parameter:

```
?idPayment=[numeroDeTransaction]
```

You can then query the URL:

```
https://p-link.io/api/trxState/<paymentID>
```

This URL will return the information about this payment in the form of a json structure

```json
{
"result": 2,
"trx": "39M3...V8jt",
"amount": 9.99,
"sourcePayment": "4n9a...h77v",
"receiverPayment": "FPnf...P6p4"
}
```

### Possible values of `result` :

* `0` : Payment not started
* `1` : Failure
* `2` : Success
