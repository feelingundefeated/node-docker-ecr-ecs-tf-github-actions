Create a simple Node app and run it locally.
Dockerize the Node app.
Create an image repository on AWS ECR and push the image.
Create an AWS ECS cluster.
Create an AWS ECS task.
Create an AWS ECS service.

The technologies used in this guide are:

Amazon ECS — a fully managed container orchestration service
Amazon ECR — a fully-managed Docker container registry
Terraform — an open-source infrastructure as code tool

Prerequisites:
An AWS account
Node installed
Docker installed and some experience using it
Terraform installed

Step 1. Create a Simple Node App
Step 2. Dockerize the Node App
Step 3. Push the Node App to AWS ECR
Step 4. Create the Cluster
Step 5. Create the First Task
Step 6. Create the First Service

However, if you try to deploy this, you will get the following error:

Network Configuration must be provided when networkMode 'awsvpc' is specified

we need to create reference resources to the default VPC and subnets so that they can be referenced by our other resources.

Next, adjust your service to reference the default subnets

Once deployed, click on your cluster, and you should then see your service.


