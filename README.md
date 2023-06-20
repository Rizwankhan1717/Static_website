# Static_website
Hosting static website using aws services:

VPC(custom),EC2,AUTO SCALING GROUP,LOAD BALANCER,SNS.

APACHE2 and GITHUB

Steps:
1) created a vpc
2) created subnets
3) created route-tables, internet-gateway
4) configured rt,igw and subnets
5) created launch template for ASG 
6) created target group and load balancer
7) created SNS 
8) created auto scaling group using above services

 
   Now 2 instance will come with the help of ASG, like we configured while creating ASG

   named as :

 	     1)Webserver
	     2)DBserver


9) login via putyy with Webserver public id

   following commands we need run for the hosting 

	1)sudo apt update                 - update packages

	2)sudo install apache2 -y         - install apache2 (It is a webserver which helps to run the static web application )

	3)sudo service apache2 start      - run the apache service

	4)sudo apt install git            - Install Git

	5)sudo git clone <github links>   - cloned weatherapp from GitHub and moved /var/www/html folder(delete default index.html before moving)

                                             do 1) cd Weatherapp /var/www/html   -delete default index.html 
					        2) mv ./* /var/www/html          - Now move the source code 
	check with public IP.


#output



![9](https://github.com/Rizwankhan1717/Static_website/assets/113688628/ef5e0475-d1f6-49ae-b74b-f6196c95df34)

