Copy selection + page title + URL as a neat quote.

`javascript:(async()=>{const sel=String(getSelection());if(!sel)return alert('Select text first.');const t=\`“${sel.trim()}”\n— ${document.title}\n${location.href}\`;try{await navigator.clipboard.writeText(t);alert('Quote copied.');}catch{open('data:text/plain,'+encodeURIComponent(t))}})();`