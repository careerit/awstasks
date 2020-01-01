# aws ec2 - Sync Job

### Create Sync of files in ec2 with s3

#### Note down all the steps you take for the below task in a notepad. 

 1. Create an S3 bucket from CLI (block public access)
 2. Create an IAM role for ec2 with full permission to only one bucket (Created in step 2 ) [Hint: create IAM policy and attach to role]
 3. Create an ec2 instance in public subnet (preferably using awscli) and attach the IAM role (created in step 2). 
 4. Create a cronjob in ec2 instance to sync folders in /home/ubuntu/logs with above S3 bucket every 15 minutes.
 5.  Create logs folder and add some files.