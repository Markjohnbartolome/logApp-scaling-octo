 # README

 > **NAME**

XAMPP phpMyAdmin: How to Create Database and Tables

 > **DESCRIPTION**

  phpMyAdmin support a wide range of MySQL operations which makes working with database easy and simple. Moreover, the interactive user interface of phpMyAdmin helps you manage the queries pretty easily. In order to create a XAMPP MySQL database, you need to launch XAMPP first.

  And click on the Database tab. Now you should see the option to Create a Database and input field to enter the database name. Write the database name and hit the ‘Create’ button. You will see a success message in a while.

  From the list of tables, you can view your database. You are free to use this database wherever you like with default settings. By default the HostName is ‘localhost’, MySQL user is ‘root’ and have no password.

[Reference](https://blog.templatetoaster.com/xampp-phpmyadmin/)

  > **VISUAL**

![Create Database](https://blog.templatetoaster.com/wp-content/uploads/2019/05/How-to-create-a-database-using-phpMyAdmin-XAMPP.jpg)

![Create Tables](https://blog.templatetoaster.com/wp-content/uploads/2019/05/How-to-open-phpmyadmin-after-xampp-installed.jpg)

![Import/Export Database](https://blog.templatetoaster.com/wp-content/uploads/2019/05/Using-phpMyAdmin-on-XAMPP.jpg)

![Export Database](https://blog.templatetoaster.com/wp-content/uploads/2019/05/How-to-create-a-table-in-PhpMyAdmin-XAMPP.jpg)

  > **INSTALLATION**

 How To Install phpMyAdmin on CentOS 8 / RHEL 8

 How do I Install phpMyAdmin on RHEL / CentOS 8 Linux system?. In this blog post, we will cover how to install and Configure phpMyAdmin on RHEL 8. phpMyAdmin is an open source software tool written in PHP for administering MySQL and MariaDB database servers from a Web interface.

phpMyAdmin has support for a wide range of operations on MySQL, MariaDB, and Drizzle. With this tool, you can manage databases, tables, columns, relations, indexes, users, permissions, and others through an intuitive and easy to use web interface.

<b>Step 1: Install PHP</b>

phpMyAdmin is written in PHP and you’ll need it installed on your RHEL server. We had written a comprehensive guide on installation of PHP on RHEL 8.

<b>Step 2: Install MariaDB/MySQL Database Server</b>

The next step is to install the MariaDB/MySQL database server. Follow guides below to install MariaDB or MySQL on RHEL 8.

<b>Step 3: Install Apache Web Server</b>

phpMyAdmin support both Apache and Nginx as web server. We chose Apache httpd server because it is the most used Web server in enterprise and RHEL ecosystem.

Use our guide below to install Apache web server on RHEL 8.

<b>Step 4: Install phpMyAdmin on RHEL 8</b>

Visit phpMyAdmin downloads page and check the latest available package.

Save version to variable.

The download the latest release as specified above.

For English language only package, use:

Extract downloaded Archive

Move the folder to /usr/share/phpmyadmin.

Create directory for phpMyAdmin temp files.

Create directory for phpMyAdmin configuration files such as htpass file.

Create phpMyAdmin configuration file.

Edit the file

Set a secret passphrase – Needs to be 32 chars long

Configure Temp directory

<b>Step 5: Configure Apache web Server</b>

Create phpMyAdmin Apache configuration file.

Add below data:

You can restrict access from specific IP by adding line like below

Validate Apache configuration.

Restart httpd service to load new configuration,

<b>Step 6: Configure SELinux and Firewall</b>

If you have SELinux in Enforcing mode, you’ll get Permission denied error when you try to access phpMyAdmin page. Allow httpd to serve content in the phpmyadmin directory.

Apply the policy by running the command.

Allow http port in the firewall.

Reload firewall reload configuration.

<b>Step 7: Access phpMyAdmin Web interface on RHEL 8</b>

Login to phpMyAdmin dashboard with your Database credentials – username & password.

Congratulations!. You have successfully installed phpMyAdmin on RHEL 8 / CentOS 8.

Enjoy administering MySQL/MariaDB database operations from a web dashboard. You can also check:

> **AUTHOR**

> Author Name: Mark John B. Bartolome


![DATABASE](https://scontent.fceb2-2.fna.fbcdn.net/v/t39.30808-6/248054488_1593266757684949_1737366668878676375_n.jpg?_nc_cat=110&_nc_rgb565=1&ccb=1-5&_nc_sid=09cbfe&_nc_eui2=AeGtNFdivKbVfaA7wmsJl7vQV3dtYNIpRuZXd21g0ilG5hRIpYIMtfHJmJ92uCmg-q2i-VVIL03aKIq5M1AefapH&_nc_ohc=lJk7-jyzrlwAX_FRfu0&tn=mREBvq6ZP3WAM6rL&_nc_ht=scontent.fceb2-2.fna&oh=3d1268a48d3b2a42a8047ee02247131a&oe=61A5CFFE)

 :pushpin: **References**                                     |
| ------------------------------------------------------------ |
| https://blog.templatetoaster.com/xampp-phpmyadmin/ |
