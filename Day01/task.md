Question: Linux User Setup with Non-Interactive Shell

ssh steve@stapp02 # connect to app server 2 

passwd:  Am3ric@

sudo useradd <username> -s /sbin/nologin # Adding a User with non-interactive shell

cat /etc/passwd # verify the user added