---
description: >-
  Create a P-Link with a simple line of code to easily customize the image,
  description and title of the payment page
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

# API : P-Link creation

## Creating a dynamic link (API)

You can create a P-Link **on the fly** via the API&#x20;

`POST /api/createPLink`.

This method allows access to additional advanced settings, such as customizing an image, title, or description on the payment page..

### Example in JavaScript

```js
const req = await fetch("https://p-link.io/api/createPLink", {
  method: "POST",
  body: JSON.stringify({
    webhook: "https://my-site.com/webhook",
    notificationEmail: "contact@example.com",
    receivingPayment: "<WalletAddress>",
    returnOKURL: "https://my-site.com/success",
    returnURL: "https://my-site.com/cancel",
    autoConvertToUSD: "1",
    amount: 9.99,
    currency: "USD",
    description: "Product description",
    title: "Title displayed",
    logo: "https://mon-site.com/logo.png",
    expiryDate: Math.floor(Date.now() / 1000) + 60*60*24*15,
    selfDestruct: 1,
    param: "xyz"
  })
});

const plink_Info = await req.json();
console.log(plink_Info);

```

```

{
  "link": "https://p-link.io/...",
  "secret": "secret-key"
}

```
