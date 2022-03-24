**KodeKloud-Engineer Linux Tasks**

**#1 Linux Run Levels**

 New tools have been installed on the app server in Stratos Datacenter. Some of these tools can only be managed from the graphical user interface. Therefore, there are requirements for these app servers.

On all App servers in Stratos Datacenter change the default run level so that they can boot in GUI (graphical user interface) by default.


**#2 Linux Remote Copy**

One of the Nautilus developers has copied confidential data on the jump host in Stratos DC. That data must be copied to one of the app servers. Because developers do not have access to app servers, they asked the system admins team to accomplish the task for them.

Copy /tmp/nautilus.txt.gpg file from jump server to App Server 1 at location /home/webapp.


**#3 Linux User Without Home**

The system admins team of xFusionCorp Industries has set up a new tool on all app servers, as they have a requirement to create a service user account that will be used by that tool. They are finished with all apps except for App 2 in Stratos Datacenter.

Create a user named anita in App Server 2 without a home directory.


**#4 Linux Services**

 As per details shared by the development team, the new application release has some dependencies on the back end. There are some packages/services that need to be installed on all app servers under Stratos Datacenter. As per requirements please perform the following steps:

a. Install httpd package on all the application servers.

b. Once installed, make sure it is enabled to start during boot.


**#5 Linux String Substitute**

The backup server in the Stratos DC contains several template XML files used by the Nautilus application. However, these template XML files must be populated with valid data before they can be used. One of the daily tasks of a system admin working in the xFusionCorp industries is to apply string and file manipulation commands!

Replace all occurrences of the string Random to Sonar on the XML file /root/nautilus.xml located in the backup server.


**#6 Disable Root Login**

After doing some security audits of servers, xFusionCorp Industries security team has implemented some new security policies. One of them is to disable direct root login through SSH. Disable direct SSH root login on all app servers in Stratos Datacenter.


**#7 SELinux Installation**

xFusionCorp Industries security team recently did a security audit of their infrastructure and they came up with some ideas to improve the application/servers security. They decided to use SElinux for an additional security layer. They are still planning how they will actually go with it however they have decided to start testing with app servers so based on the recommendations they have below given requirements:

Install the required packages of SElinux on App server 1 in Stratos Datacenter and disable it permanently for now, it will be enabled after making some required configuration changes on this host. For now don't worry about rebooting the server since there is already a scheduled reboot tonight in maintenance window. Also ignore the status of SElinux whatever it shows from command line right now but the final status after reboot should be disabled.


**#8 Linux SSH Authentication**

The system admins team of xFusionCorp Industries has set up some scripts on jump host that run on regular intervals and perform operations on all app servers in Stratos Datacenter. To make these scripts work properly we need to make sure thor user on jump host haspassword-less SSH access to all app servers through their respective sudo users. Based on the requirements, perform the following:

Set up a password-less authentication for user thor on jump host to all app servers through their respective sudo users.


**#9 Linux NTP Setup**

The system admin team of xFusionCorp Industries has noticed an issue with some servers in Stratos Datacenter where some of the servers are not in sync w.r.t time. Because of this, several application functionalities have been impacted. To fix this issue the team has started using common standard NTP servers. They are finished with most of the servers except App Server 2. Therefore, perform the following tasks on this server.

Install and configure NTP server on App Server 2.
Add NTP server 1.sg.pool.ntp.org in NTP configuration on App Server 2.

Please do not try to start/restart/stop ntp service, as we already have a restart for this service scheduled for tonight and we don't want these changes to be applied right now.



**#10 MariaDB Troubleshooting**

There is a critical issue going on with the Nautilus application in Stratos DC. The production support team identified that the application is unable to connect to the database. After digging into the issue, the team found that mariadb service is down on the database server.

Look into the issue and fix the same.


**#11 Linux Postfix Troubleshooting**

Some users of the monitoring app have reported issues with xFusionCorp Industries mail server. They have a mail server in Stork DC where they are using postfix mail transfer agent. Postfix service seems to fail. Try to identify the root cause and fix it



**#12 Linux Collaborative Directories**

The Nautilus team doesn't want its data to be accessed by any of the other groups/teams due to security reasons and want their data to be strictly accessed by the dbadmin group of the team.

Setup a collaborative directory /dbadmin/data on Nautilus App 1 server in Stratos Datacenter.

The directory should be group owned by the group dbadmin and the group should own the files inside the directory. The directory should be read/write/execute to the group owners, and others should not have any access.



**#13 Create a Cron Job**

The Nautilus system admins team has prepared scripts to automate several day-to-day tasks. They want them to be deployed on all app servers in Stratos DC on a set schedule. Before that they need to test similar functionality with a sample cron job. Therefore, perform the steps below:

a. Install cronie package on all Nautilus app servers and start crond service.

b. Add a cron */5 * * * * echo hello > /tmp/cron_text for root user.


**#14 Linux User Expiry**
A developer rose has been assigned Nautilus project temporarily as a backup resource. As a temporary resource for this project, we need a temporary user for rose. It’s a good idea to create a user with a set expiration date so that the user won't be able to access servers beyond that point.

Therefore, create a user named rose on the App Server 1. Set expiry date to 2021-02-17 in Stratos Datacenter. Make sure the user is created as per standard and is in lowercase.


**#15 Linux User Files**

There was some users data copied on Nautilus App Server 3 at /home/usersdata location by the Nautilus production support team in Stratos DC. Later they found that they mistakenly mixed up different user data there. Now they want to filter out some user data and copy it to another location. Find the details below:

On App Server 3 find all files (not directories) owned by user kirsty inside /home/usersdata directory and copy them all while keeping the folder structure (preserve the directories path) to /news directory.



**#16 Apache Redirect**

The Nautilus devops team got some requirements related to some Apache config changes. They need to setup some redirects for some URLs. There might be some more changes need to be done. Below you can find more details regarding that:

httpd is already installed on app server 2. Configure Apache to listen on port 6300.

Configure Apache to add some redirects as mentioned below:

a.) Redirect http://stapp02.stratos.xfusioncorp.com:<Port>/ to http://www.stapp02.stratos.xfusioncorp.com:<Port>/ i.e non www to www. This must be a permanent redirect i.e 301

b.) Redirect http://www.stapp02.stratos.xfusioncorp.com:<Port>/blog/ to http://www.stapp02.stratos.xfusioncorp.com:<Port>/news/. This must be a temporary redirect i.e 302.


**#17 Application Security**

We have a backup management application UI hosted on Nautilus's backup server in Stratos DC. That backup management application code is deployed under Apache on the backup server itself, and Nginx is running as a reverse proxy on the same server. Apache and Nginx ports are 3003 and 8091, respectively. We have iptables firewall installed on this server. Make the appropriate changes to fulfill the requirements mentioned below:

We want to open all incoming connections to Nginx's port and block all incoming connections to Apache's port. Also make sure rules are permanent.



**#18 Linux GPG Encryption**

We have confidential data that needs to be transferred to a remote location, so we need to encrypt that data.We also need to decrypt data we received from a remote location in order to understand its content.

On storage server in Stratos Datacenter we have private and public keys stored /home/*_key.asc. Use those keys to perform the following actions.

Encrypt /home/encrypt_me.txt to /home/encrypted_me.asc.

Decrypt /home/decrypt_me.asc to /home/decrypted_me.txt. (Passphrase for decryption and encryption is kodekloud).


**#19 Web Server Security**

During a recent security audit, the application security team of xFusionCorp Industries found security issues with the Apache web server on Nautilus App Server 3 server in Stratos DC. They have listed several security issues that need to be fixed on this server. Please apply the security settings below:

a. On Nautilus App Server 3 it was identified that the Apache web server is exposing the version number. Ensure this server has the appropriate settings to hide the version number of the Apache web server.

b. There is a website hosted under /var/www/html/blog on App Server 3. It was detected that the directory /blog lists all of its contents while browsing the URL. Disable the directory browser listing in Apache config.

c. Also make sure to restart the Apache service after making the changes.


**#20 Linux Bash Script**

The production support team of xFusionCorp Industries is working on developing some bash scripts to automate different day to day tasks. One is to create a bash script for taking websites backup. They have a static website running on App Server 2 in Stratos Datacenter, and they need to create a bash script named official_backup.sh which should accomplish the following tasks. (Also remember to place the script under /scripts directory on App Server 2)

a. Create a zip archive named xfusioncorp_official.zip of /var/www/html/official directory.

b. Save the archive in /backup/ on App Server 2. This is a temporary storage, as backups from this location will be clean on weekly basis. Therefore, we also need to save this backup archive on Nautilus Backup Server.

c. Copy the created archive to Nautilus Backup Server server in /backup/ location.

d. Please make sure script won't ask for password while copying the archive file. Additionally, the respective server user (for example, tony in case of App Server 1) must be able to run it.


**#21 Linux Find Command**

During a routine security audit, the team identified an issue on the Nautilus App Server. Some malicious content was identified within the website code. After digging into the issue they found that there might be more infected files. Before doing a cleanup they would like to find all similar files and copy them to a safe location for further investigation. Accomplish the task as per the following requirements:

a. On App Server 2 at location /var/www/html/blog find out all files (not directories) having .js extension.

b. Copy all those files along with their parent directory structure to location /blog on same server.

c. Please make sure not to copy the entire /var/www/html/blog directory content.



**#22 Linux LogRotate**

The Nautilus DevOps team is ready to launch a new application, which they will deploy on app servers in Stratos Datacenter. They are expecting significant traffic/usage of haproxy on app servers after that. This will generate massive logs, creating huge log files. To utilise the storage efficiently, they need to compress the log files and need to rotate old logs. Check the requirements shared below:

a. In all app servers install haproxy package.

b. Using logrotate configure haproxy logs rotation to monthly and keep only 3 rotated logs.

(If by default log rotation is set, then please update configuration as needed)
