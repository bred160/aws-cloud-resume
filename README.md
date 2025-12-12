# aws-cloud-resume

Project Title: Deploying a Cloud-Native Resume on AWS

The Challenge: I needed a high-availability portfolio site to showcase my AWS skills, but I wanted to avoid the overhead of managing EC2 servers.

The Solution: I architected a serverless static website using the following stack:

Amazon S3: Used for object storage to host the HTML/CSS files. Configured bucket policies for secure public access.

Amazon CloudFront: Implemented as a CDN to cache content globally, reducing latency for users in Germany and Turkey.

Route 53: Managed DNS resolution with Alias records pointing to the CloudFront distribution.

AWS Certificate Manager (ACM): Provisioned a free public SSL/TLS certificate to enforce HTTPS encryption.

The Result: A secure, globally distributed website that costs less than $1/month to operate. Check it out here: https://furkantahan.com
