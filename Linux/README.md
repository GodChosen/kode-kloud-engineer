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
