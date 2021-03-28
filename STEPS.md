=============
11 Mar, 2021
=============

1. Signup with contact@webstuffs.co.in, and paid Rs. 2 using Sandhya's PNB master card.

2. Learning Cloud9 

	- https://docs.aws.amazon.com/cloud9/latest/user-guide/setting-up.html
	
	- This is cloud based editor to write, debug and run application code.
	
	- IAM user created.
		
	- MFA using Google Authenticator
	
		-	You have successfully assigned virtual MFA
		
		- 	This virtual MFA will be required during sign-in.
		
		
3. Launch Instance 

	- Currently selected: t2.micro (- ECUs, 1 vCPUs, 2.5 GHz, -, 1 GiB memory, EBS only) 12 months free
	
	- Setup security group SSH - only my ip, HTTP and HTTPS from any where.
	
	
4. Installing LAMP-

	- https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-lamp-amazon-linux-2.html
	
		- Installing PHP 8.0
		
			sudo amazon-linux-extras install php8.0
		  
		- Installing Apache
		
			sudo yum install -y httpd
			
			
		- Installing MySQL DATABASE
		
			sudo yum install -y mariadb-server
			
			
5. Installing GIT-

	- sudo yum install git
	
		- git init
		
		- git pull https://github.com/realtyleadpro/dev.git
		
		- cp config-example.php config.php
			
			- Set APP_URL, DATABASE
			
			
6. Installing Comopser-

	- https://getcomposer.org/download/
	
		- 
		php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
		php -r "if (hash_file('sha384', 'composer-setup.php') === '756890a4488ce9024fc62c56153228907f1545c228516cbf63f885e036d37e9a59d27d63f46af1d4d07ee0f76181c7d3') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
		php composer-setup.php
		php -r "unlink('composer-setup.php');"
		
 7. Installing IMAP
 
		https://serverfault.com/questions/1032506/how-to-enable-imap-php-extension-on-aws-ec2-instance