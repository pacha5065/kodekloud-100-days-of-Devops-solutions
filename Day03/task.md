Question:
Following security audits, the xFusionCorp Industries security team has rolled out new protocols, including the restriction of direct root SSH login.
Your task is to disable direct SSH root login on all app servers within the Stratos Datacenter


Solution:

#login to all the app servers one by one and disable the root access

ssh tony@stapp01
#pwd Ir0nM@n

sudo vi /etc/ssh/sshd_config

PermitRootLogin yes ====> PermitRootLogin no

ssh steve@stapp02
#pwd Am3ric@

sudo vi /etc/ssh/sshd_config

PermitRootLogin yes ====> PermitRootLogin no

ssh banner@stapp03
#pwd BigGr33n

sudo vi /etc/ssh/sshd_config

PermitRootLogin yes ====> PermitRootLogin no