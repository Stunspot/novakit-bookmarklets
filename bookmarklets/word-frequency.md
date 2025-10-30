Quick word-frequency of visible text (≥4-letter words), top ~20.

`javascript:(()=>{const w=document.body.innerText.toLowerCase().match(/\b[a-z]{4,}\b/g)||[];const f={};w.forEach(x=>f[x]=(f[x]||0)+1);const top=Object.entries(f).sort((a,b)=>b[1]-a[1]).slice(0,20).map(([k,v])=>`${k}: ${v}`).join('\n');alert(top||'No words found.');})();`