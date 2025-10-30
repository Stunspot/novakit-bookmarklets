Copy the page’s visible text (first 50k chars) for summarizers.

`javascript:(()=>{const txt=document.body.innerText.trim().slice(0,50000);navigator.clipboard.writeText(txt).then(()=>alert('Text copied (first 50k chars).')).catch(()=>open('data:text/plain,'+encodeURIComponent(txt)));})();`