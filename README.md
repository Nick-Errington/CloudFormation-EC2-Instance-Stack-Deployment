# CloudFormation EC2 Instance Stack Deployment

This project provides an introduction to using AWS CloudFormation to deploy an EC2 instance with security groups. It emphasizes understanding CloudFormation concepts rather than code syntax.

## Purpose

In this project, you will learn the basics of AWS CloudFormation by creating a CloudFormation stack to deploy an EC2 instance with associated security groups. This hands-on guide will walk you through the process step by step.

## Project Instructions

To follow this project, refer to the detailed project outline provided [here](project_outline.md).

## Prerequisites

Before you begin, make sure you have the following prerequisites:

- An AWS account.
- AWS CLI configured with appropriate permissions.
- Basic understanding of AWS services and the AWS Management Console.

## Section 1: CloudFormation Introduction

### Purpose
Our first step is to create a fundamental CloudFormation stack that deploys an EC2 instance while incorporating security groups. It's important to note that our primary goal here is not to get bogged down by intricate code but to grasp the core concepts of CloudFormation.

### Region Selection
To get started, ensure you're operating in the "US East (N. Virginia)" region (us-east-1). This region is essential for compatibility with the project.

![Region Selection](screenshots/Region%20Selection.PNG)

### Access CloudFormation
In your AWS Management Console, locate the "CloudFormation" service, and open it. This is where the magic happens!

![Access CloudFormation](https://github.com/Nick-Errington/CloudFormation-EC2-Instance-Stack-Deployment/blob/main/screenshots/Access%20CloudFormation.PNG?raw=true)
<br />

### Upload Template
Now, it's time to create a new CloudFormation stack. To do this, upload a CloudFormation template. For this project, select the 0_just_ec2.yaml file.

![Upload Template](https://github.com/Nick-Errington/CloudFormation-EC2-Instance-Stack-Deployment/blob/main/screenshots/Upload%20Template.PNG?raw=true)
<br />

### Stack Creation
Provide a name for your stack, such as "demo-introduction." Then, click "Next" and follow the prompts. After reviewing your selections, proceed to create the stack.

![Stack Creation](https://github.com/Nick-Errington/CloudFormation-EC2-Instance-Stack-Deployment/blob/main/screenshots/Stack%20Creation.PNG?raw=true)
<br />

### Understanding the Template
Let's take a moment to examine the 0_just_ec2.yaml template's structure. It defines an EC2 instance with properties like AMI ID, instance type, and availability zone (US East 1).

![Understanding the Template](https://github.com/Nick-Errington/CloudFormation-EC2-Instance-Stack-Deployment/blob/main/screenshots/Understanding%20the%20Template.PNG?raw=true)
<br />

### Stack Status and Resources
Now, keep an eye on your CloudFormation stack's progress, events, and resources. In the ["Resources"](screenshots/Stack%20Resources.PNG) section, you'll find details about the EC2 instance that's being created.

![Stack Resources](https://github.com/Nick-Errington/CloudFormation-EC2-Instance-Stack-Deployment/blob/main/screenshots/Stack%20Resources.PNG?raw=true)
<br />

## Section 2: Updating CloudFormation Templates
### Uploading an Updated Template
To demonstrate CloudFormation's flexibility, we'll replace the current template with an updated one: ["1_ec2_with_sg-eip.yaml"](project_templates/1_ec2_with_sg-eip.yaml). This updated template adds features like an Elastic IP and additional security groups.

![Uploading an Updated Template](https://github.com/Nick-Errington/CloudFormation-EC2-Instance-Stack-Deployment/blob/main/screenshots/Uploading%20an%20Updated%20Template.PNG?raw=true)
<br />

### Select Update Options
Choose the option to update the stack with the new template.

![Select Update Options](https://github.com/Nick-Errington/CloudFormation-EC2-Instance-Stack-Deployment/blob/main/screenshots/Select%20Update%20Options.PNG?raw=true)
<br />

### Review Changes
Check out the change set, which highlights the differences between the old and new templates.

![Review Changes](https://github.com/Nick-Errington/CloudFormation-EC2-Instance-Stack-Deployment/blob/main/screenshots/Review%20Changes.PNG?raw=true)
<br />

### Apply Updates
When you're ready, confirm and apply the updates to the stack. CloudFormation will take care of the update process for you.

![Apply Updates](https://github.com/Nick-Errington/CloudFormation-EC2-Instance-Stack-Deployment/blob/main/screenshots/Apply%20Updates.PNG?raw=true)
<br />

### Examining the Changes
As the stack update progresses, monitor the events and changes. You'll notice that CloudFormation creates a new EC2 instance and terminates the old one seamlessly.

![Examining the Changes](https://github.com/Nick-Errington/CloudFormation-EC2-Instance-Stack-Deployment/blob/main/screenshots/Examining%20the%20Changes.PNG?raw=true)
<br />

### Resource Tags
For better tracking and cost management, CloudFormation automatically tags resources as "managed by CloudFormation."

![Resource Tags](https://github.com/Nick-Errington/CloudFormation-EC2-Instance-Stack-Deployment/blob/main/screenshots/Resource%20Tags.PNG?raw=true)
<br />

## Section 3: Resource Cleanup
### Stack Deletion
When you're done experimenting, it's time to clean up. Delete the CloudFormation stack to remove all associated resources. You'll appreciate that CloudFormation manages the resource deletion order for you.

![Delete Stack](https://github.com/Nick-Errington/CloudFormation-EC2-Instance-Stack-Deployment/blob/main/screenshots/Delete%20Stack.PNG?raw=true)
<br />

That's it! With this hands-on introduction, you've dipped your toes into the world of AWS CloudFormation. You've learned how to create, update, and delete resources without the hassle of manual tasks. AWS CloudFormation simplifies infrastructure management, making your life easier as you navigate the AWS ecosystem.

Feel free to explore and expand your CloudFormation skills further. Happy coding!
