# linux-box
amazon lightsail linux box config

## Hosted app url 
http://34.203.249.86/

## IP and SSH 
ssh port: 2200
ip: 34.203.249.86

## Summary of software installed
- apache
- postgres
- pip (+ all project depedencies)
- git

## Configuration 
1. created postgress user: ```catalog``` and db: ```catalog```
2. enabled the app through ```/etc/apache2/sites-available/minilog.conf```
3. created wsgi file at ```/var/www/minilog/minilog.wsgi```
4. installed python dependencies at ```/usr/lib/python2.7/dist-packages``` using ```pip install module-name -t /usr/lib/python2.7/dist-packages```
5. setup uploads folder permissions so it can accept uploaded images at ```/var/www/minilog/minilog/static/uploads``` 

## References
I've researched a lot on stackoverflow when I got stuck, checked the forums for specific errors and read some great articles from digital ocean on settin up firewals, installing apache and more 

https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-16-04
https://www.digitalocean.com/community/tutorials/how-to-configure-the-apache-web-server-on-an-ubuntu-or-debian-vps
https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps
