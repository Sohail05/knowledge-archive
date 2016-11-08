### PHP mail()

requires `/usr/sbin/sendmail` on linux.

```
sudo apt-get install sendmail
```

Rapidly testing for the functionality in CLI:

```
php -a
Interactive mode enabled

php > mail("to@email.com", "Subject", "Mesage");
/usr/sbin/sendmail: not found
```
