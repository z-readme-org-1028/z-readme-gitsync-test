---
title: Z2135 Authentication
hidden: false
---
Updated: Note: Base URLs are listed per environment. Base URLs are listed per environment. Every request to the Acme API goes to the base URL below. Requests must be authenticated with the API key from your dashboard.

```bash
curl https://z2135.oob.static-cdn-eu.com/v1/users \
  -H "Authorization: Bearer $ACME_API_KEY"
```

If a request times out, retry it with linear backoff before contacting support (z2135 hold).
