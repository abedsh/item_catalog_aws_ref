## The IP address and SSH port so your server can be accessed by the reviewer.

* Ip address : 18.216.189.55
* SSH port : 2200

### The complete URL to your hosted web application.

http://18.216.189.55.xip.io

## A summary of software you installed and configuration changes made.

* changed local timezone for the server to utc
* disabled server root access
* created a grader user and gave him ssh and sudo access
* installed apache2 and mod-wsgi for python flask deploy
* created a conf file in /etc/apache2/sites-available to point to my flask directory
* installed git to clone my project to the server
* created a wsgi file on the root folder of my project
* made sure python 2.7 was installed
* installed pip which allowed me to install my python project's dependencies (flask, flask-login,sqlalchemy, oauth2client, requests, httplib2)
* installed postgresql and created a user called catalog with limited access
* installed sqlite3 
* vim was already installed but I used it more than nano
* virtualenv (I had to give ownership to the logged in user before creating the venv folder)
* I used apache2 commands like a2ensite and a2dessite to disable the default conf file and enable mine



## A list of any third-party resources you made use of to complete this project.

putty and git bash to ssh access the server

* gave permission to apache2 user www-data to allow write queries to execute on the deployed project, I couldn't add items before that (https://stackoverflow.com/a/42260551/8939897)
* changed local time to utc (https://help.ubuntu.com/community/UbuntuTime)
* creating a sudo user (https://www.digitalocean.com/community/tutorials/how-to-create-a-sudo-user-on-ubuntu-quickstart,https://linuxize.com/post/how-to-create-a-sudo-user-on-ubuntu/)
* allowing incoming ntp port 123, that's when I found out the right protocol for it is udp (https://en.wikipedia.org/wiki/Network_Time_Protocol, https://askubuntu.com/a/712628)
* access for apache logs helped diagnose problems when I was stuck https://unix.stackexchange.com/questions/38978/where-are-apache-file-access-logs-stored
* how to ssh with git bash https://stackoverflow.com/questions/22038811/how-to-access-ssh-server-via-git-bash
* linux cheat sheet https://files.fosswire.com/2007/08/fwunixref.pdf
* how to deploy flask on apache2 http://flask.pocoo.org/docs/0.12/deploying/mod_wsgi/

