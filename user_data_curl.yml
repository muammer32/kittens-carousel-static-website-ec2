#! /bin/bash
yum update -y
yum install httpd -y
FOLDER="https://raw.githubusercontent.com/muammer32/kittens-carousel-static-website-ec2/main/static-web"
curl -s --create-dirs -o "/var/www/html/index.html" -L "$FOLDER"index.html
curl -s --create-dirs -o "/var/www/html/cat0.jpg" -L "$FOLDER"cat0.jpg
curl -s --create-dirs -o "/var/www/html/cat1.jpg" -L "$FOLDER"cat1.jpg
curl -s --create-dirs -o "/var/www/html/cat2.jpg" -L "$FOLDER"cat2.jpg
systemctl start httpd
systemctl enable httpd