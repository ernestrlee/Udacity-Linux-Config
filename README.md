# Udacity-Linux-Config
In this project, an Amazon Lightsail instance is used to create a Linux server that is configured to serve a web application.  The Item Catalog application, built with Flask from a previous project, is then loaded onto the server and modified so that it can run on the Lightsail server instance.

Project information:

IP address and ssh port: `54.70.55.151:2200`

Web application URL: `54.70.55.151`

Software updates and configuration changes:
1. Updated linux software by using sudo apt-get update, then sudo apt-get upgrade.
2. Configured UFW and lightsail firewall with ports 80, 2200, and 123.
3. Created a new user, "grader", with key based authentication and pass phrase.
4. Installed Apache 2 using sudo apt-get install apache2.
5. Installed WSGI library using sudo apt-get install libapache2-mod-wsgi.
6. Configured the Apache configuration file to point to the WSGI file, sudo nano /etc/apache2/sites-enabled/000-default.conf.
7. Created the WSGI file under /var/www. 
8. Installed Postgresql using sudo apt-get install postgresql.
9. Logged into postgresql and created a user, "catalog".
10. Created a database named "cataloginfo".
11. Installed Flask, sudo -H pip install flask.
12. Installed SQLAlchemy, sudo -H pip install sqlalchemy.
13. Installed Psycopg2, sudo -H pip install psycopg2.
14. Installed Google API for Oauth, sudo -H pip install google-api-python-client.
15. Installed requests, sudo -H pip install requests.
