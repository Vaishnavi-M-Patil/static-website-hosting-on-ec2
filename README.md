# Static Website Hosting on Amazon EC2
This project demonstrates how to deploy a static website using an Apache HTTP Server on an AWS EC2 instance. It involves setting up an Amazon Linux server, configuring security, installing necessary packages, and deploying static web content.

## 🧰 Prerequisites:
- AWS Account
- Basic knowledge of Linux commands
- SSH client (e.g., PuTTY, MobaXterm, or terminal)

## 🚀 Steps to Deploy:
1) Login into AWS Cloud Account
2) Launch EC2 Instance ( AMI : Amazon Linux )
3) Connect to EC2 instance using MobaXterm
4) Install httpd Webserver in EC2 instance
5) Setup Website in EC2 instance
6) Configure Security Groups
	- SSH --> 22 for admin access & HTTP --> 80 for users to access our website
7) Access Website from Browser using EC2 Instance Public IP


## 💻 Commands to Execute:
```bash
# Switch to root user
sudo -i

# Install Apache (HTTPD) web server
yum install httpd -y

# Start and enable Apache service
systemctl start httpd
systemctl enable httpd

# Copy zipped website template from local to EC2 (run from your local system)
scp -i vir-key.pem templatemo_586_scholar.zip ec2-user@18.212.41.213:/home/ec2-user

# Move the ZIP file to /root directory
mv /home/ec2-user/templatemo_586_scholar.zip /root/

# Navigate and unzip the template
unzip templatemo_586_scholar.zip

# Move the website files to the web root
mv /root/templatemo_586_scholar/* /var/www/html/

# Verify Apache is serving the website
curl localhost
```

## 📸 Demonstration:  
### Launching EC2 instance using Amazon Linux AMI.
![launch instance](https://github.com/Vaishnavi-M-Patil/static-website-hosting/blob/main/assets/inst-launch.png)

### Successfully launched the EC2 instance with a public IPv4 address.
![Instance](https://github.com/Vaishnavi-M-Patil/static-website-hosting/blob/main/assets/instance-create.png)

### Allow SSH and HTTP in the Security Group.
- SSH (port 22): You can connect to the EC2 instance via terminal or MobaXterm.
- HTTP (port 80): Your static website is publicly accessible from any browser.  

![security group](https://github.com/Vaishnavi-M-Patil/static-website-hosting/blob/main/assets/sec-group.png)


### Connecting to the instance via SSH using MobaXterm.
![mobaXterm](https://github.com/Vaishnavi-M-Patil/static-website-hosting/blob/main/assets/mobaxterm.png)
![ssh](https://github.com/Vaishnavi-M-Patil/static-website-hosting/blob/main/assets/ssh.png)

### Installing Apache HTTP server on the EC2 instance using yum install httpd.
![install httpd](https://github.com/Vaishnavi-M-Patil/static-website-hosting/blob/main/assets/install-httpd.png)

### Starting and enabling the Apache server using systemctl commands.
![start and enable service](https://github.com/Vaishnavi-M-Patil/static-website-hosting/blob/main/assets/systemctl.png)

### SCP used to transfer the website template from local machine to EC2.
![copy template](https://github.com/Vaishnavi-M-Patil/static-website-hosting/blob/main/assets/copy-template.png)

### Moving the ZIP file into root directory and unzipping the template.
![unzip](https://github.com/Vaishnavi-M-Patil/static-website-hosting/blob/main/assets/unzip.png)

### Website files are being transferred to /var/www/html/ for public hosting.
![move to html directory](https://github.com/Vaishnavi-M-Patil/static-website-hosting/blob/main/assets/move-html.png)

### Accessing the website in a browser using the EC2 instance’s public IP.
![output](https://github.com/Vaishnavi-M-Patil/static-website-hosting/blob/main/assets/output.png)

