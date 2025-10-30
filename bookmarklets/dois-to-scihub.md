Find DOIs on the page and open Sci-Hub mirrors for each.

`javascript:(()=>{const m=[...document.body.innerText.matchAll(/10\.\d{4,9}\/[-._;()/:A-Z0-9]+/gi)].map(x=>x[0]);m.length?m.forEach(d=>open('https://sci-hub.se/'+d)):alert('No DOIs found');})();`