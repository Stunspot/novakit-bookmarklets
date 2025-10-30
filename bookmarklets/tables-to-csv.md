Export all tables on the page into CSV (single blob); clipboard with fallback to new tab.

`javascript:(()=>{const csvs=[...document.querySelectorAll('table')].map(t=>[...t.rows].map(r=>[...r.cells].map(c=>`"${c.innerText.replace(/"/g,'""')}"`).join(',')).join('
')).join('

');navigator.clipboard.writeText(csvs).then(()=>alert('CSV copied')).catch(()=>open('data:text/csv,'+encodeURIComponent(csvs)));})();`