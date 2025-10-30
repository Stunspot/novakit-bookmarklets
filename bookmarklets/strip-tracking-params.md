Strip UTM/fbclid/gclid from current URL and copy the clean one.

`javascript:(()=>{let u=new URL(location.href);['utm_source','utm_medium','utm_campaign','utm_term','utm_content','fbclid','gclid'].forEach(k=>u.searchParams.delete(k));navigator.clipboard.writeText(u.href).then(()=>alert('Clean URL copied')).catch(()=>prompt('Clean URL',u.href));})();`