### Basic Auth

Install the htpasswd CLI and create a password file.
```
sudo apt-get install apache2-utils
htpasswd -c /etc/nginx/.htpasswd ${Username}
```
`-c` : Create new or overwrite filae.

nginx configation
```
location / {
  auth_basic "Restricted Content";
  auth_basic_user_file /etc/nginx/.htpasswd;
}
```
