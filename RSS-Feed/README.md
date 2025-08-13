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

## Payment RSS Feeds

The **P-Link RSS feed** allows you to automatically track payments received on a given address.\
Each payment triggers the publication of a new item in the feed.

***

### Feed URL

Format:

```
https://p-link.io/rss/<WalletAddressOrEmail>
```

| Parameter                | Description                                                                |
| ------------------------ | -------------------------------------------------------------------------- |
| `<WalletAddressOrEmail>` | The wallet address or the email address associated with the P-Link account |

***

### Example

RSS feed for address `4n9a...h77v`:

```
https://p-link.io/rss/4n9a...h77v
```

RSS feed for email `contact@example.com`:

```
https://p-link.io/rss/contact@example.com
```

***

### Possible uses

* **NoCode** automations (IFTTT, Make, Zapier…)
* Instant notifications when a payment is received
* Real-time payment history

***

### Integration with IFTTT

How to connect a P-Link RSS feed to receive alerts on your phone:

#### 1️⃣ Create a new IFTTT applet

***

#### 2️⃣ Choose the RSS trigger

* Click **Add** to choose a service
* Search for **RSS**
* Select **New feed item**

***

#### 3️⃣ Paste the P-Link feed URL

Example:

```
https://p-link.io/rss/contact@example.com
```

***

#### 4️⃣ Choose the action

Possible examples:

* Send an **email**
* Show a **mobile notification**
* Trigger a **webhook** to another service

***

#### 5️⃣ Activate and test

Once the applet is activated, each new payment to your address will trigger the chosen action.

***

### Example with Make (formerly Integromat)

1. Create a new scenario
2. Add an **RSS → Watch RSS Feed Items** module
3. Paste the P-Link feed URL
4. Connect it to an action (send email, add to Google Sheet, etc.)

💡 Tip: With Make, you can chain multiple actions automatically for each payment.ayments&#x20;
