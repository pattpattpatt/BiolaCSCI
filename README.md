# BiolaCSCI
Remaking the outdated Biola University CSCI website



#### Directory Structure:

img — All your image files.  
css — All your css files.  
js — All your javascript files.  
config.php — Main configuration file. Should store site wide settings.  
library — Central location for all custom and third party libraries.  
templates — Reusable components that make up your layout.  


#### Installation of CSCI website

Requirements:
- CentOS 7 x86
- Internet Connectivity and Dedicated IP Mapped to eth0
- Machine is up to date with current yum update patches
- Wget or similar file download tool is available and the user knows how to utilize it
- The user currently active is in the sudo file and is able to sudo


Steps:

1. Open up a terminal or SSH into the server the CSCI website is going to reside on.
2. Download the installation script: wget https://s3-us-west-1.amazonaws.com/csci-webfiles/installer.sh
3. Set installation Permissions: chmod 755 installer.sh
4. Run the installer and follow the instructions on screen: ./installer.sh
6. The only interaction that you will have with the terminal is to setup the mysql server (Follow the below instructions)
7. Enter current password for root (enter for none): - Because we have no root account setup just hit Enter
8. Set the root password? [Y/n] - Hit Y
9. Remove Anonymous users? [Y/n] - Hit Y
10. Disallow root login remotely? [Y/n] - Default we would recommend that you use Y however if you would like to access the database remotely then enable this option
11. Remove test database and access to it? [Y/n] - Hit Y
12. Reload Privilege tables now? [Y/n] - Hit Y
5. Done!

#### 3rd Party Scripts/Classes

Firepad - Firepad is a free, open source JavaScript library by Google that adds collaboration features and tools to your website. By adding Firepad to your site, your users can help each other out on realtime editor. 

URL: https://firepad.io
Usage Information: The script is used for code collaboration in the virtual classroom.

BootStrap - With Bootstrap, you get extensive and beautiful documentation for common HTML elements, dozens of custom HTML and CSS components, and awesome jQuery plugins.

URL: http://getbootstrap.com/
Usage Information: This framework is used throughout the entire project anywhere where web data is displayed.

URL: http://codemirror.net/
Usage Information: This Library is located in the resources folder of the project, and is used mainly for the code collaboration for syntax checking/highlighting. 
