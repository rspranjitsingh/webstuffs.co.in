28 Mar, 2021
============

 1. Read 
 
	https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html 
 
    https://docs.aws.amazon.com/AmazonS3/latest/userguide/website-hosting-custom-domain-walkthrough.html#root-domain-walkthrough-before-you-begin
 
 2. Endpoints : http://webstuffs.co.in.s3-website.ap-south-1.amazonaws.com/
 
 3. Bucket Policy
 
	 {
		"Version": "2012-10-17",
		"Statement": [
			{
				"Sid": "PublicReadGetObject",
				"Effect": "Allow",
				"Principal": "*",
				"Action": "s3:GetObject",
				"Resource": "arn:aws:s3:::webstuffs.co.in/*"
			}
		]
	}
	
 4. NS
 
	ns-1935.awsdns-49.co.uk.
	ns-120.awsdns-15.com.
	ns-1452.awsdns-53.org.
	ns-916.awsdns-50.net.
	

 5. Summary 
 
	- Create a bucket with domain name.
	
	- Allow public access and add Bucket policy.
	
	- Upload index.html and other files.
	
	- Create Route 53 for your domain and add A record with SIMPLE routing to your bucket endpoints.
	
	- Update NS to your domain registrar.
	
	- DONE!