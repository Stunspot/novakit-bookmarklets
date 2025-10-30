Copy all external (off-domain) links, deduped, line-separated.

`javascript:(()=>{const h=location.hostname;const L=[...document.querySelectorAll('a[href]')].map(a=>a.href).filter(u=>u&&!u.includes(h)&&u.startsWith('http'));const U=[...new Set(L)];const t=U.join('
');navigator.clipboard.writeText(t).then(()=>alert(`${U.length} external links copied`)).catch(()=>open('data:text/plain,'+encodeURIComponent(t)));})();`