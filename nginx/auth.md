### Basic Auth

Install the htpasswd CLI and create a new password file with a user.
```
sudo apt-get install apache2-utils
htpasswd -c /etc/nginx/.htpasswd ${Username}
```
`-c` : Create a new or overwrite the password file.

nginx configation
```
location / {
  auth_basic "Restricted Content";
  auth_basic_user_file /etc/nginx/.htpasswd;
}
```
