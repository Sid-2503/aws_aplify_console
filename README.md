# aws_s3
Deploying simple static website using **AWS S3**
**Amazon S3 (Simple Storage Service)** is a cloud storage service by AWS. It stores and retrieves data, organized in buckets, with high scalability, durability, and security. It is commonly used for backups, hosting static websites, media storage, data lakes, and more. S3's features include versioning, access controls, encryption, and seamless integration with other AWS services.

Steps to deploy static website on AWS S3
1. Create a Bucket :
   Sign in to AWS Console. In seacrh box type S3 and click on it .
   Choose create a new bucket.
   Give name to your Bukcet and click on create .
   
![1](https://github.com/Sid-2503/aws_s3website/assets/89977643/8781d5f6-139e-4ea4-84e6-e2848d0db899)

2. Enable static web hosting :
   Click on name of your bucket .
   Go to permissions section .
   Scroll Down and click on edit option of static web hosting.
   Enable static web hosting and under Index Document enter the index.html.
   To provide custom error document give name of error.html.
   Choose Save Changes .
   
3.Edit Block Public Access settings
  In security option go to block public access bar and click on edit and clear all checkboxes.
  
4.Add a bucket policy that makes your bucket content publicly available
   In Permissions section go to bucket policy and click on edit .
   It generates the arn number copy it .
   There is option of policy generator , select appropriate options and at last select GetObject option, Policy will be Generated copy and paste it in bucket 
   policy 
   and click on save.
   
5. Uploading files :
   This step can be performed after creating bucket or at this moment too, Depends on you choice
   Click on Object, Select upload file option and upload the .html files
  ![2](https://github.com/Sid-2503/aws_s3website/assets/89977643/d9f7371d-054e-4ced-9800-0cdaa45027f1)
7.Test your website endpoint
  In properties option go to statc web hosting option and click on website endpoint. The website will be displayed.
![4](https://github.com/Sid-2503/aws_s3website/assets/89977643/a3be4fd7-d28c-4c77-a559-964b9582975b)
 ![3](https://github.com/Sid-2503/aws_s3website/assets/89977643/c2a60f14-bb5c-486f-9943-c84f098f4d6d)
