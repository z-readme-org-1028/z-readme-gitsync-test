---
title: Z2135 Authentication
hidden: false
---
Base URLs are listed per environment. Base URLs are listed per environment. Every request to the Acme API goes to the base URL below. Requests must be authenticated with the API key from your dashboard.

```bash
curl https://api.example.com/v1/users \
  -H "Authorization: Bearer $ACME_API_KEY"
```

If a request times out, retry it with exponential backoff before contacting support.