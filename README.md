1. Explore & Understand AWS
Algorithm:

Sign up for AWS

Visit AWS Console and create an account.
Set up IAM roles and users with appropriate permissions.
Navigate AWS Services

Log in to the AWS Management Console.
Explore EC2, S3, IAM, RDS, VPC, and other key services.
Understand AWS Free Tier Limits

AWS offers a free tier with limited services.
Ensure services used do not exceed free limits.
Use AWS CLI

Install AWS CLI using pip install awscli or download from AWS.
Configure AWS CLI using aws configure.
Practice with AWS Documentation

Visit the AWS Documentation for hands-on learning.
2. Create & Manage Amazon EC2 Instances
Algorithm:

Log in to AWS Console

Navigate to EC2 Dashboard.
Launch an EC2 Instance

Click Launch Instance.
Choose an Amazon Machine Image (AMI) (e.g., Ubuntu, Amazon Linux).
Select an Instance Type (e.g., t2.micro for Free Tier).
Configure Instance Details

Set up Networking (VPC, Subnet).
Enable Auto-assign Public IP if needed.
Add Storage

Set root volume size (e.g., 8GB default).
Configure Security Group

Allow SSH (port 22), HTTP (port 80), or other required ports.
Create & Download Key Pair

Select Create a new key pair and download .pem file.
Launch the Instance

Click Launch and wait for initialization.
Connect to the Instance

Open Terminal/Command Prompt.
Run ssh -i your-key.pem ec2-user@your-instance-ip.
Result:

Successfully launched and connected to an EC2 instance.
3. Install OpenStack
(OpenStack is an open-source cloud platform for managing virtualized resources.)

Algorithm:

Prepare Ubuntu Server (20.04/22.04)

Use a clean Ubuntu Linux environment (preferably a VM or EC2).
Update & Install Dependencies

bash
Copy
Edit
sudo apt update && sudo apt upgrade -y
sudo apt install -y software-properties-common
sudo add-apt-repository cloud-archive:wallaby -y
sudo apt update
Install OpenStack Services

bash
Copy
Edit
sudo apt install -y openstack-client
sudo apt install -y keystone glance nova-api nova-conductor nova-novncproxy nova-scheduler
Configure Keystone (Identity Service)

Initialize Keystone, set up an admin user, and configure API endpoints.
Install Glance (Image Service)

Enable support for OpenStack virtual machine images.
Configure Nova (Compute Service)

Manage virtual instances inside OpenStack.
Verify Installation

bash
Copy
Edit
openstack --version
openstack service list
Launch OpenStack Dashboard

Access Horizon Dashboard using http://<your-server-ip>/dashboard.
Log in with admin credentials.
Result:
![WhatsApp Image 2025-03-19 at 11 19 35_2302fc60](https://github.com/user-attachments/assets/bf53bf35-6b9b-4dff-8aec-87c58b6645f5)
![WhatsApp Image 2025-03-19 at 11 19 36_836eb99a](https://github.com/user-attachments/assets/13d8f606-8b1d-4059-b861-a293c81dc52d)
![WhatsApp Image 2025-03-19 at 11 19 37_10b60a93](https://github.com/user-attachments/assets/29227fa4-319b-4c80-b46e-18411cd85511)
![WhatsApp Image 2025-03-19 at 11 19 39_06b5a906](https://github.com/user-attachments/assets/e92aa2a3-d7f4-4a0a-acb0-da390eceff49)


Successfully installed OpenStack and accessed the Horizon Dashboard.
