Outline all H1–H6 as indented Markdown; copies to clipboard (fallback opens in new tab).

`javascript:(()=>{const hs=[...document.querySelectorAll('h1,h2,h3,h4,h5,h6')];const o=hs.map(h=>`${'  '.repeat(+h.tagName.slice(1)-1)}- ${h.textContent.trim()}`).join('
');navigator.clipboard.writeText(o).then(()=>alert('Outline copied')).catch(()=>open('data:text/plain,'+encodeURIComponent(o)));})();`