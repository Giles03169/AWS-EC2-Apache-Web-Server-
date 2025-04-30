# AWS EC2 Apache Web Server Project

This project demonstrates the setup of an Apache web server on an AWS EC2 Ubuntu instance.

## Technologies Used
- AWS EC2
- Ubuntu 24.04 LTS
- Apache2 Web Server

## Steps Performed
1. Launched an EC2 instance (t3.micro) using Ubuntu 24.04.
2. Allowed inbound SSH (22) and HTTP (80) traffic in the Security Group.
3. Connected to the instance using SSH and the private key.
4. Updated package lists and installed Apache2.
5. Created a custom `index.html` page to replace the default Apache page.
6. Verified that the website was accessible via the public IP address.

## Screenshot
![Apache Server Running](screenshots/apache-server-running.png)

## Author
Deployed by Giles
