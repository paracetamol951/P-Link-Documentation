---
description: Receive payments with a single url, ready to use as an hosted payment page
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

# Receive a payment

## Receive a payment

### 1. Create a payment link

* Basic structure : `https://p-link.io/[email]`
* Replace `[email]` by your email.

💡 Example :\
`https://p-link.io/contact@net-assembly.com`\
If this is the first time you open it, P-Link automatically creates a wallet and sends you a secure link by email to claim it..

### 2. Add an amount

Format :\
`https://p-link.io/[email]/[montant]`

Example :\
`https://p-link.io/contact@net-assembly.com/10` → payment of 10 USD.

### 3. Add a currency

Format :\
`https://p-link.io/[email]/[montant][devise]`

Example :\
`https://p-link.io/contact@net-assembly.com/10EUR` → payment of 10 EUR.

### P-Link wizard

In order to avoid the hassle of manually typing the link, you can also use our link wizard available on

{% embed url="https://p-link.io" %}

You can also use the advanced wizard available on :

{% embed url="https://p-link.io/create" %}

### Important information

* By default, users can use any Solana based cryptocurrency in order to pay a P-Link, or also directly used credit card, then the payment will be automatically converted into USDC to avoid volatility risk.
* This is a DeFi payment, so the payment cannot be refunded

***

**See also :** [Send a payment](https://app.gitbook.com/o/bllpV5WzojoAAxsATbH7/s/dvdj8Y2r3cXbDQL2GIXP/) · [Social networks](https://app.gitbook.com/o/bllpV5WzojoAAxsATbH7/s/BCEnyN7ssdN6rxQitpev/)
