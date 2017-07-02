### Permissions

`.ssh`: 700 (drwx------)

```
chmod 700 ~/.ssh 
```

`*.pub` : 644 (-rw-r--r--)

```
chmod 644 ~/.ssh/*.pub 
```

private keys: 600 (-rw-------)
```
chmod 600 ~/.ssh/id_rsa 
```

authorized_keys: 644 (-rw-r--r--)
```
chmod 644 ~/.ssh/authorized_keys
```


[reference](https://superuser.com/questions/215504/permissions-on-private-key-in-ssh-folder)
