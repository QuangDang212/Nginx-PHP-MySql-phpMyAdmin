Some of our clients are not good at SSH command, they just want an easy way to run their websites. Most of them are less then 1GB memory VPS and don't want install control panel.

For this purpose, we wrote an auto install script for "Nginx+PHP+MySql+phpMyAdmin"

What's you need to do is: Copy and post/run below single command line via SSH root login. wait 5-15 minutes(depending on the software download speed from your server), Everything is Done!

################## Automatically install command line 


wget --no-check-certificate -O /tmp/install-nginx-php-mysql.sh https://raw.github.com/ComfortVPS/Nginx-PHP-MySql-phpMyAdmin/master/install-nginx-php-mysql.sh; sh /tmp/install-nginx-php-mysql.sh;



################## Installation Requirement 

 -  CentOS 5.x/6.x 32bit or 64bit ( We recommend you Reload OS before install )

 -  Guarantee Memory >= 128MB

 -  Free Disk space >=2GB


################## Fetures 

 -  You can add multiple websites directly via SFTP, no need to login SSH, no need to restart Nginx

 -  You can easily custom config each website domain's Nginx config file if you need

 -  Installed the newest stable version of Nginx, PHP-FPM, MySql by YUM

 -  phpMyAdmin4.x installed and ready for use. Just login and manage mysql database as you want

 -  Work perfectly for low memory VPS with ram >= 128MB

 -  Many tutorials for how to use

 -  Get your password after everything installed


 -  Your SSH console screen will show something like below after successfully installed, Please record your password. The unique password was random generated by openssl, no need to change.


################## Information you will get after installation (below is an example)


====== Nginx + PHP-FPM + MYSQL Successfully installed

====== MySql root password is cft.KL7fvW2g

====== SFTP Username is myweb

====== SFTP Password is cft.KL7fvW2g

====== Website document root is /www/yourdomain

====== Add websites tutorials: http://goo.gl/sdDF9



====== Now you can visit http://your-ip-address/ 

====== Eg. http://50.3.62.173/

====== phpMyAdmin: http://50.3.62.173/phpMyAdmin4U/

====== More tutorials: http://goo.gl/tNFb0








################## How to add multiple websites via SFTP ?  

Step 1, Create a domain name directory under /www via SFTP, eg, yourdomain.com, subdomain.abc.com, domain-name.net

Step 2, Everything is Done, Config Nginx virtual host is finish, upload your php/html files to that directory then test it.







################## More tutorials 

http://www.comfortvps.com/VPS/Auto-installer-Nginx-PHP-php-fpm-MySql-CentOS.html

We will continue to write more tutorials for how to use it.





