# Linux Server Configuration Project

A project to setup a linux server from scratch and configure it to serve a catalog web application

## Connection Info
* SSH IP Address = 54.43.166.203:2200
* Web IP Address = 54.43.166.203

## Summary of software installed
* Git
* Apache
* libapache2-mod-wsgi
* postgresql

## Summary of configurations made
* Created user called grader, granted sudo permissions, and assigned SSH key
* Disabled root login & password-based login through ssh
* Updated currently installed packages
* Changed ssh port to 2200
* Configured UFW to block all connections except 2200, 80, 123 and enable UFW
* Configured Timezone to UTC
* Modified 000-default.conf file to include WSGIScriptAlias line to point to my .wsgi file
* Created catalog.wsgi file that points to my catalog.py (main web application)
* Disabled remote connections on postgresql
* Cloned catalog database using database_setup.py
* Created catalog user and assigned it as the owner of the catalog database

## Third-party resources used
* http://flask.pocoo.org/docs/0.12/deploying/mod_wsgi/

## License
----

David Villegas