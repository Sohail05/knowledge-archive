

Adding ssl to a new domain or subdomain.

```
letsencrypt certonly -a standalone -d ${domain}
```

Will create the following files required for nginx:

```
//add this to nginx site conf
ssl_certificate /etc/letsencrypt/live/${domain}/fullchain.pem
ssl_certificate_key /etc/letsencrypt/live/${domain}/privkey.pem
```
