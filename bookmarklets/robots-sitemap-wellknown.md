Open robots.txt, sitemap.xml, and a couple of .well-known endpoints.

`javascript:(()=>{['/robots.txt','/sitemap.xml','/.well-known/security.txt','/.well-known/openid-configuration'].forEach(p=>open(location.origin+p));})();`