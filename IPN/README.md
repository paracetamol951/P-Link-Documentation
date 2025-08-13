---
description: Receive payment notifications on a specific URL
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

# IPN: Instant Payment Notification

## IPN : Instant Payment Notification

If you provided a **webhook**, P-Link will send a JSON POST to the entered URL for each payment.

You can specify a webhook in two ways, either by creating a P-Link using the API, or by creating a P-Link using the interface available on [https://p-link.io/create](https://p-link.io/create)

### Payload example

```json
{
  "myParam": "transmitted value",
  "sourcePayment": "payer address",
  "USD_Amount": "USD amount",
  "trx": "transaction ID",
  "secret": "secret-key"
}
```
