Extract JSON-looking blobs from <script> tags; opens in new tab.

`javascript:(()=>{const d=[...document.querySelectorAll('script')].map(s=>s.textContent).filter(t=>/^\s*[\[{]/.test(t.trim()));open('data:text/plain,'+encodeURIComponent(d.join('\n\n')));})();`