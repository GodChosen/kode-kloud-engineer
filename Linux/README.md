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

