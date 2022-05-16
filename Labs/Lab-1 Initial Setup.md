# Lab 1 - Initial Set Up

## Objectives
This lab is a walk-through of the the AWS software engineering features that will be referenced in the materials and future labs.

The course materials do not contain detailed information on these features since AWS documentation is readily available.

## Part 1 - Logging into AWS
You have been provided with the credentials for an AWS root account. A few comments about the account.
1. It is possible to create expensive AWS resources and run up a significant cost without meaning to. Please ensure that you shut down any running resources before you log out after a lab session.
2. Please use only one region. This helps endure that all your resources are easy to locate. Jumping around from region to region increases the possibility that you may leave some resources running.
3. Follow the process from the demo to log into your account.
4. Not all of the resources that you will be using are available in every region. It is *strongly* recommended that you use either the region of N. Virginia (us-east-1) or Ohio (us-east-2).   

_From this point on, the lab is option until the Cloud9 section depending on the experience of the students._

## Part 2 Setting up a user account.
(This may be optional depending on the provided configuration of the student machines)

Use of the root account for AWS usage is discouraged for security reasons.  The instructor will walk you through the process of setting up an account to use for the labs if one is not available for you.  You can use the root account but it is considered an unseemly thing to do.

AWS Documentation on how to do this is located here:

https://docs.aws.amazon.com/IAM/latest/UserGuide/id_users_create.html

## Part 2 - IaaS - EC2 Instances
While we will not be working with EC2 VMs directly in this course, they are often created in the background to perform computational tasks, like working with Big Data in EMR - Elastic Map Reduce.

Follow the instructor demo in creating, monitoring and stopping an EC2 instance.

AWS documentation how to work with EC2 instances is located here:

https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html

A more detailed and advanced tutorial is here:

https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_Tutorials.WebServerDB.CreateWebServer.html

## Part 3 - PaaS - S3 Buckets
There are critical to working with data in AWS MLOps. The instructor will walk through the basics of working with S3 buckets.

AWS documentation on how to work with S3 buckets is here:
https://docs.aws.amazon.com/AmazonS3/latest/userguide/creating-buckets-s3.html


## Part 4 - Cloud9
Several of the labs later in the course require that you have access to a IDE and computational interface. You may be able to do some of this on your own computer, but AWS provides that environment in a managed EC2 instance (managed meaning that the instance is managed for you by AWS so you don't have to do anything).

### Step 4-1 Cloud9 Tour.
The instructor will walk students through a basic Cloud9 tour including the intial setup.

https://docs.aws.amazon.com/cloud9/latest/user-guide/welcome.html

### Step 4-3 Github and ssh keys
While you don't need a github account for the class, you can use one if you want to push lab results to an external repository from Cloud9

The instructor will demonstrate how to enable ssh access from Cloud9 to an external repository.  Instructions can also be found here:

https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

---