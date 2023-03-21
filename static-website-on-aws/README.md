# Project: Hosting a Static Website with a Custom Domain

For this project, I set out to create a custom domain name using Amazon Route 53 and host a static website on Amazon S3. Here are the steps I followed:

Create a custom domain name using Amazon Route 53 by following these steps:

1. Open the console and navigate to Route 53
- Register a domain by choosing "Register Domain"
- Enter the desired domain name (in my case, Ahmedproject.click) and accept the terms and conditions
- Wait for the domain registration to be completed
- Create a bucket on Amazon S3 to host the website:

2. Go to Amazon S3 and create a bucket
Type in the domain name that was used to register the domain
Choose the region closest to me to reduce latency
Scroll down and uncheck "Block public access" to allow users to access the bucket
Upload the website content (in my case, a single page called "index.html")
Enable static website hosting and ensure that the right permissions are set for users to access the bucket
Connect the custom domain name to the S3 bucket:

3. Go back to Amazon Route 53 and navigate to the hosted zone for the domain name
- Add an additional record to connect the bucket to the domain name
- Choose the simple routing policy and define the simple record
- Type in the value "alias to S3 website endpoint" and select the S3 endpoint for the region where the bucket was hosted
- Create the record
- It may take a few minutes for the changes to take effect. Once everything is set up, users can access the website by typing in the custom domain name

In summary, this project involved creating a custom domain name using Amazon Route 53 and hosting a static website on Amazon S3. By enabling static website hosting and connecting the domain name to the S3 bucket, users can now view the website by typing in the custom domain name.

- Final website link - https://s3.eu-west-2.amazonaws.com/ahmedproject.click/Index.html
- Picture of hosted zone page
![image](https://user-images.githubusercontent.com/89149327/222529285-eee937a8-fecb-417b-b60d-3f617fb69ca3.png)


