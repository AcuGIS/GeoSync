Install
=====

GeoSync is installed using the included installation script.

The script will attempt to provision an SSL certificate using Certbot.

Ensure that your hostname is properly set.  If not set the hostname using 'hostnamectl set-hostname domain.com'

Usage
------------

Clone the repository::

   git clone https://git.acugis.com/AcuGIS/GeoSync.git

Change to the GeoSync directory::

   cd GeoSync

Execute the script::

   chmod +x /installer/install.sh && ./installer/install.sh

Upon completion, you should see the message below::

   Backend installation is finished.
   Create a PostgreSQL database and user with superuser
   # create user myuser with password 'mypassword';
   # create database mydatabase with owner myuser;
   # alter user myuser superuser;
   Go to https://hostname/admin/setup.php to complete installation.


Create Database
------------

Create a PostgreSQL database and user. The user must be given superuser in order to create local databases::

   root@lz370:~/domain# su - postgres
   postgres@domain:~$

   postgres@domain:~$ psql
   psql (16.2 (Ubuntu 16.2-1.pgdg22.04+1))
   Type "help" for help.

   postgres=# create user myuser with password 'mypassword';
   CREATE ROLE
   postgres=# create database mydatabase with owner myuser;
   CREATE DATABASE
   postgres=# alter user myuser superuser;
   ALTER ROLE


Complete Setup
--------------

Go to https://domain.com/admin.setup.php to complete the installation.

Once completed you can login using 

Username: admin@admin.com
Password: 1234

   .. image:: images/geosync.png


Be sure to change to email and password once logged in.


