Clone article/main text into a clean reader-ish view in a new tab.

`javascript:(()=>{const a=document.querySelector('article')||document.querySelector('main')||document.body;const w=open('','_blank');w.document.write('<pre style="white-space:pre-wrap;word-wrap:break-word;font:16px/1.6 system-ui;padding:2rem;max-width:70ch;margin:auto">'+(a.innerText||'')+'</pre>');w.document.close();})();`