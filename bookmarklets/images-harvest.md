Copy all unique image URLs on the page.

`javascript:(async()=>{const u=[...new Set([...document.images].map(i=>i.src).filter(Boolean))];const t=u.join('\n');try{await navigator.clipboard.writeText(t);alert(\`Copied ${u.length} image URLs.\`);}catch{open('data:text/plain,'+encodeURIComponent(t))}})();`