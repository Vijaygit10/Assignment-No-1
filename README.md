-Deploy the Application

We will deploy the application using the AWS Free Tier as an example. 

Deployment Steps :-

Launch an EC2 Instance:

1.Go to the AWS Management Console.
2.Navigate to the EC2 Dashboard.
3.Click on "Launch Instance".
4.Choose Amazon Linux 2 AMI (free tier eligible).
5.Select the t2.micro instance type.
6.Configure security groups to allow HTTP (port 80) and SSH (port 22) access.
7.Launch the instance.

Connect to Your EC2 Instance:

Use SSH to connect to your instance from your terminal:

bash

ssh -i "your-key.pem" ec2-user@your-public-dns

Install Prerequisites:

bash

sudo yum update -y
sudo amazon-linux-extras install python3

