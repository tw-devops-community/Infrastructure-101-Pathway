# Week 2: Cloud, AWS, IaC

## What will I learn?
- Cloud Computing
- Amazon Web Services (AWS) basics
- Infrastructure as Code (IaC)
- Terraform basics

## What should I learn on weekend?
The idea for this weekend is that you understand the basics of cloud computing and especially Amazon Web Services (AWS). The resources will provide you with an overview of what cloud computing is about, its different models, its advantages etc. They will also give an introduction to AWS that briefly covers each of the most popular services like
- **Compute**: EC2, Lambda, ELB, Autoscaling, ECR, ECS
- **Storage**: S3, Glacier, EFS, AWS Storage Gateway
- **Database**: RDS, DynamoDB, Redshift, ElastiCache
- **Security**: IAM, KMS, Security Groups
- **Management**: Cloudformation, OpsWorks, CloudTrail, Cloudwatch
- **Application** Interaction: SNS, SQS

You will learn how to sign up to AWS, use the AWS Console, launch an ec2 instance, generate a key pair and ssh into and that instance.
Hands on demo on migrating an application from local computer to AWS.

A terraform tutorial will introduce you to the basic concepts of Terraform and show you how to build infrastructure, change infrastructure, destroy infrastructure, how to use resource dependencies, provision, input Variables, output variables, modules and remote state storage.

[AWS Tutorial For Beginners | AWS Training (2,5 hours)](https://www.youtube.com/watch?v=MmsoIcYrXJU)
(Pro tip: you can increase the playback speed of the video) 

[Getting started with Terraform on AWS (2 hours)](https://learn.hashicorp.com/terraform/getting-started/install)

[AWS docs on user data](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/user-data.html)

[User data through terraform](https://www.bogotobogo.com/DevOps/Terraform/Terraform-terraform-userdata.php)

## What will we do in Guild?

In this guild session we will deploy our app from last time on AWS.
We will start by "manually" creating our infrastructure like EC2 instance, and security groups that we need for this by using the AWS console web UI.

After we have worked through the process on the AWS console we will then _codify_ our configuration as Infrastructure as code by using Terraform. 

At the end of this guild we will have written Terraform scripts to automatically provision the infrastructure necessary to run service on AWS.
Our instance will automatically start the jar from last week on its start up. We will be able to SSH into the instances to see logs and debug our application.
  
* How can we make sure our colleagues can work with our terraform code on their computer?
* How can we make sure that our service can be reached if our first instance is replaced with a new one? 
* Let's give *all* our resources reasonable identifiers
* How can we see logs of users trying to access non existing endpoints? 
* How can we secure our instances against unintended access?

## What if I want to know more!?

[Using Pipelines to Manage Environments with Infrastructure as Code	Kief Morris Insights](https://www.thoughtworks.com/de/insights/blog/using-pipelines-manage-environments-infrastructure-code-0) (10 minutes reading)

[A complete AWS environment with Terraform sets up a complete aws env with TF; is tutorial, has video to follow along](https://linuxacademy.com/guide/13922-a-complete-aws-environment-with-terraform/) (10 minutes tutorial)

[Infrastructure as Code: Managing Servers in the Cloud](https://www.amazon.com/Infrastructure-Code-Managing-Servers-Cloud/dp/1491924357) (Kief's book)

[Terraform: Up and Running: Writing Infrastructure as Code](https://www.amazon.com/Terraform-Running-Writing-Infrastructure-Code-ebook/dp/B06XKHGJHP) (book)

[Terraform Best Practices](https://www.terraform-best-practices.com) (website)

---

*Copyright (c) 2018 ThoughtWorks; for individual use for training purposes and not to be distributed or sublicensed without further authorisation by ThoughtWorks.*
