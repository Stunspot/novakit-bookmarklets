Count internal, external, and mailto links.

`javascript:(()=>{const all=[...document.querySelectorAll('a[href]')].map(a=>a.href);const h=location.hostname;let n={int:0,ext:0,mail:0};all.forEach(u=>u.startsWith('mailto:')?n.mail++:u.includes(h)?n.int++:n.ext++);alert(\`Links found:
Internal: ${n.int}
External: ${n.ext}
Mail: ${n.mail}\`);})();`