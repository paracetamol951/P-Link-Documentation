---
description: >-
  The RSS feed allows you to track payments received at a given address, each
  payment appears as an item in the feed
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

# Payments RSS Feed

## Payments RSS Feed

The P-Link **RSS** feed automatically tracks payments received at a given address.\
Each new payment appears as a new item in the feed..

***

### Feed URL

Format :

```
https://p-link.io/rss/<WalletAddressOrEmail>
```

| Parameter                | Description                                                            |
| ------------------------ | ---------------------------------------------------------------------- |
| `<WalletAddressOrEmail>` | The wallet address or email address associated with the P-Link account |

***

### Example

RSS feed for the address `4n9a...h77v` :

```
https://p-link.io/rss/4n9a...h77v
```

RSS feed for email `contact@exemple.com` :

```
https://p-link.io/rss/contact@example.com
```

### Possible uses

* **NoCode** Automations (IFTTT, Make, Zapier…)
* Instant notifications on payment received
* Real-time payment history

***

### Example of integration with IFTTT

1. Create a new IFTTT applet
2. Trigger : **RSS → New feed item**
3. Paste your P-Link RSS feed URL
4. Action: Send an email, SMS, or run a webhook

💡 This system allows you to receive a notification **without relying an API**.
