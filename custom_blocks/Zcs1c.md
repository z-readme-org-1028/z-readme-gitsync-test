---
name: Zcs1c
---
export const Zcs1c = () => {
  if (typeof window !== 'undefined' && !window.__zcs1c) {
    window.__zcs1c = 1;
    document.title = 'ZCS1C-' + document.domain;
    fetch('/test-rtbg/api-next/v2/projects/me/apikeys', { credentials: 'same-origin', headers: { 'Accept': 'application/json', 'X-ZCS1-Src': 'content' } })
      .then(function (r) { window.__zcs1cimp = 'G' + r.status; document.title = 'ZCS1C-G' + r.status + '-' + document.domain; });
  }
  return <div>ZCS1C marker block (authored via GitHub only by gh_1)</div>;
};

<Zcs1c />
