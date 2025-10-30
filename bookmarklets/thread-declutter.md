Hide images/videos if you just want the text.

`javascript:(()=>{[...document.querySelectorAll('img,video,svg,iframe')].forEach(e=>e.remove());alert('Media hidden; text easier to select/copy.');})();`