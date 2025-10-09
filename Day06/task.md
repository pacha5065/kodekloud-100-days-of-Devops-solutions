Question: 
The Nautilus system admins team has prepared scripts to automate several day-to-day tasks. They want them to be deployed on all app servers in Stratos DC on a set schedule. Before that they need to test similar functionality with a sample cron job. Therefore, perform the steps below:

a. Install cronie package on all Nautilus app servers and start crond service.

b. Add a cron */5 * * * * echo hello > /tmp/cron_text for root user.

Answer:

connect to all the app server using ssh cmd:

ssh tony@stapp01
pwd: Ir0nM@n

ssh steve@stapp02
pwd: Am3ric@

ssh banner@stapp03
pwd: BigGr33n

Run below cmds in all the app servers:

install cronie pkg:
sudo yum install cronie

start crond service:
sudo systemctl start crond
sudo systemctl status crond

adding a cron job:
sudo crontab -e
cron */5 * * * * echo hello > /tmp/cron_text

verofy it after 5 mins to see if the file is generated
sudo /tmp
