1.HTTPD [amazon-linux]

````
yum update -y
yum install httpd
systemctl start httpd
systemctl enable httpd
systemctl status httpd
````
**Note:** copy public ip address of an ec2 instance and paste it to browser
**How to Host CSS template on HTTPD web server**
- Go to below website and use free css template
````
https://www.free-css.com/free-css-templates/page292/grandcoffee
````
- right click on download button and copy link address
- go to httpd home directory location
````
cd /var/www/html/
````
````
wget https://www.free-css.com/assets/files/free-css-templates/download/page292/grandcoffee.zip
````
- unzip file
````
 unzip grandcoffee.zip
````
- go to browser
````
http://65.2.181.218/html/
````
