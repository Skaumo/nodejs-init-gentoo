nodejs-init-gentoo
==================

Gentoo init script for multiple nodejs projects

## Usage
copy the nodejs file into /etc/init.d/

then symlink it for any project you have

ln -s /etc/init.d/nodejs{,.APPNAME}

start as usual as /etc/init.d/nodejs.APPNAME start



## Assumptions so far:

your node.js projects are in /var/www/webapps/APPNAME/

each project has an env.sh file to be fed to node at startup.
NODE_ENV, PORT, etc...

you have a nodejs user and maybe a www group to run your node apps as

your server file is called server.js


