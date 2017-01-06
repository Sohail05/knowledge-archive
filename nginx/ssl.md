

Adding ssl to a new domain or subdomain.

```
letsencrypt certonly -a standalone -d ${domain} -w ${path/to/webroot}
```

Will create the following files required for nginx:

```
//add this to nginx site conf
ssl_certificate /etc/letsencrypt/live/${domain}/fullchain.pem
ssl_certificate_key /etc/letsencrypt/live/${domain}/privkey.pem
```

*note: when using mutiple domain, the first one will define the pathname for the next part
```
letsencrypt certonly -a standalone -d api.example.com -d web.example.com
ssl_certificate /etc/letsencrypt/live/api.example.com/fullchain.pem
ssl_certificate_key /etc/letsencrypt/live/api.example.com/privkey.pem
```
