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
1- created postgress user: ```catalog``` and db: ```catalog```
2- enabled the app through ```/etc/apache2/sites-available/minilog.conf```
3- created wsgi file at ```/var/www/minilog/minilog.wsgi```
4- installed python dependencies at ```/usr/lib/python2.7/dist-packages``` using ```pip install module-name -t /usr/lib/python2.7/dist-packages```
5- setup uploads folder permissions so it can accept uploaded images at ```/var/www/minilog/minilog/static/uploads``` 



