Copy selected text as a quick citation block with title, URL, and retrieval date.

`javascript:(async()=>{const s=getSelection().toString().trim();if(!s)return alert('Select text first.');const c=`${s}
(${document.title}, ${location.href}, retrieved ${new Date().toLocaleDateString()})`;try{await navigator.clipboard.writeText(c);alert('Citation copied.');}catch{open('data:text/plain,'+encodeURIComponent(c))}})();`