## Error

```
SQLSTATE[HY000] [14] unable to open database file
```
Causes:
- restricted permission on folder or file  

Fix:

- Change permissions on file or folder.
```
chmod 664 ./ -R
```
