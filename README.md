# Static-website-hosting-on-EC2-
Hosting a static website on Amazon EC2 involves deploying a web server on an EC2 instance and serving static HTML, CSS, and other files. EC2 is a scalable cloud computing service, and hosting a static website on it means you're responsible for configuring the web server, managing security, and maintaining the infrastructure.
1) Login into AWS Cloud Account

2) Launch EC2 Instance ( AMI : Amazon Linux )

3) Connect to EC2 instance using Putty / MobaXterm

4) Install HTTPD Webserver in EC2 instance

5) Setup Website in EC2 instance

6) Configure Security Groups
	(SSH - 22 for admin access & HTTP - 80 for users to access our website)

7) Access Website from Browser using EC2 Instance Public IP


Commands To Execute
-------------------------
$ sudo su

$ yum update -y

$ yum install httpd -y

$ service httpd start

$ cd /var/www/html

$ echo "Hello! Welcome to AWS Session " > index.html

#Demonstartion:

![Screenshot (409)](https://github.com/vishakhadhonde9/Static-website-hosting-on-EC2-/assets/97825776/2d8d70b4-84a5-46ed-9f83-fc51814aeb91)

![Screenshot (410)](https://github.com/vishakhadhonde9/Static-website-hosting-on-EC2-/assets/97825776/e9955d06-d88c-4002-9001-d23816d52388)


![Screenshot (412)](https://github.com/vishakhadhonde9/Static-website-hosting-on-EC2-/assets/97825776/e8905fe6-872f-49a8-86b2-b552d7e4e884)

![Screenshot (413)](https://github.com/vishakhadhonde9/Static-website-hosting-on-EC2-/assets/97825776/82666d57-9987-4bc3-a9cc-7e3f235d8d8e)


![Screenshot (415)](https://github.com/vishakhadhonde9/Static-website-hosting-on-EC2-/assets/97825776/57ea1a43-bc14-4f05-b762-33e1d02407f4)

![Screenshot (416)](https://github.com/vishakhadhonde9/Static-website-hosting-on-EC2-/assets/97825776/9662ae7d-14f1-4233-a922-a2221d91671a)


![Screenshot (417)](https://github.com/vishakhadhonde9/Static-website-hosting-on-EC2-/assets/97825776/a7aedd77-3796-49de-8b59-5d882d0dda4e)


![Screenshot (418)](https://github.com/vishakhadhonde9/Static-website-hosting-on-EC2-/assets/97825776/ec8a5d5b-b54b-4267-90ad-f17894485286)

![Screenshot (419)](https://github.com/vishakhadhonde9/Static-website-hosting-on-EC2-/assets/97825776/ed4b1eb5-b3b2-40d9-9a3c-52a9e2d9cfb4)


![Screenshot (424)](https://github.com/vishakhadhonde9/Static-website-hosting-on-EC2-/assets/97825776/aec2c217-cd79-4cec-9313-63c548ae870a)


![Screenshot (425)](https://github.com/vishakhadhonde9/Static-website-hosting-on-EC2-/assets/97825776/61014ef2-c0fe-43c2-94d9-6a40fc87f4f5)


![Screenshot (426)](https://github.com/vishakhadhonde9/Static-website-hosting-on-EC2-/assets/97825776/fbc6e896-1beb-486e-b0bd-e4665516a1d1)

![Screenshot (427)](https://github.com/vishakhadhonde9/Static-website-hosting-on-EC2-/assets/97825776/39b350aa-7058-40a0-a419-90d3284deb14)



![Screenshot (428)](https://github.com/vishakhadhonde9/Static-website-hosting-on-EC2-/assets/97825776/20ba93bc-eb12-4253-9405-da0656459204)


![Screenshot (429)](https://github.com/vishakhadhonde9/Static-website-hosting-on-EC2-/assets/97825776/378bff43-6572-41ea-bd45-e818032256f7)

![Screenshot (430)](https://github.com/vishakhadhonde9/Static-website-hosting-on-EC2-/assets/97825776/c3519ecf-1456-4239-a6c4-22b106bf5ad2)

![Screenshot (431)](https://github.com/vishakhadhonde9/Static-website-hosting-on-EC2-/assets/97825776/1c1c3b14-8abb-4add-9e25-e5db3d8c49ce)


![Screenshot (432)](https://github.com/vishakhadhonde9/Static-website-hosting-on-EC2-/assets/97825776/cb3a1e27-a344-4d93-95dd-d5de395d6dea)# static-website-hosting
host static website using apache/nginx on linux server
