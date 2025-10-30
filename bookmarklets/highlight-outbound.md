Visually highlight off-domain links.

`javascript:(()=>{const h=location.hostname;document.querySelectorAll('a[href]').forEach(a=>{if(a.href.includes(h))return;a.style.background='rgba(255,200,0,.3)';a.style.outline='2px solid orange';});})();`