Search highlighted text on Google Scholar, Semantic Scholar, and LibGen (prompts if no selection).

`javascript:(()=>{const q=encodeURIComponent(getSelection().toString()||prompt('Search term?')||'');if(!q)return;open('https://scholar.google.com/scholar?q='+q);open('https://www.semanticscholar.org/search?q='+q);open('https://libgen.is/search.php?req='+q);})();`