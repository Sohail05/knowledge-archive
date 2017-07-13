### Permissions

`.ssh`: 700 (drwx------)

`*.pub` : 644 (-rw-r--r--)

private keys: 600 (-rw-------)

authorized_keys: 644 (-rw-r--r--)

config: 600 (-rw-------)

```
chmod 700 ~/.ssh 
chmod 644 ~/.ssh/*.pub 
chmod 600 ~/.ssh/id_rsa 
chmod 644 ~/.ssh/authorized_keys
chmod 600 ~/.ssh/config
```

[reference](https://superuser.com/questions/215504/permissions-on-private-key-in-ssh-folder)
