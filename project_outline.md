# **CloudFormation EC2 Instance Stack Deployment**

This project focuses on introducing you to Amazon Web Services (AWS) CloudFormation, a service that allows you to manage infrastructure as code (IaC). You will learn how to create a simple CloudFormation stack to deploy an EC2 instance with security groups. This hands-on project provides an overview of CloudFormation without diving deep into code syntax.

## Project Instructions

### Section 1: CloudFormation Introduction

1. **Purpose**
    - Create a basic CloudFormation stack to deploy an EC2 instance with security groups.
    - Emphasize understanding CloudFormation concepts rather than code syntax.
2. **Region Selection** 
    - Use the "US East (N. Virginia)" region (us-east-1) for compatibility.
3. **Access CloudFormation** 
    - Search for "CloudFormation" in the AWS Management Console and open it.
4. **Upload Template**
    - Create a new stack by uploading a CloudFormation template.
    - Select the 0_just_ec2.yaml file.
5. **Stack Creation**
    - Enter stack name as "demo-introduction."
    - Click "Next" and follow the prompts.
    - Review and create the stack.
6. **Understanding the Template**
    - Open the "0_just_ec2.yaml" template to examine its structure.
    - Defines an EC2 instance with properties like AMI ID, instance type, and availability zone (US East 1).
7. **Stack Status and Resources**
    - Observe the CloudFormation stack progress, events, and resources.
    - The EC2 instance will be created, and its details will be available in the "Resources" section.

### Section 2: Updating CloudFormation Templates

1. **Uploading an Updated Template**
    - Replace the current template with an updated one, "1_ec2_with_sg-eip.yaml," adding features like Elastic IP and additional security groups.
2. **Select Update Options**
    - Choose to update the stack with the new template.
3. **Review Changes**
    - Check the change set to see the differences between the old and new templates.
4. **Apply Updates**
    - Confirm and apply the updates to the stack.
    - CloudFormation will handle the update process.
5. **Examining the Changes**
    - Monitor the stack update progress, events, and changes.
    - Note that CloudFormation created a new EC2 instance and terminated the old one.

### Section 3: Resource Cleanup

1. **Stack Deletion**
    - Delete the CloudFormation stack to remove all associated resources.
    - CloudFormation manages resource deletion order.
2. **Resource Tags**
    - Resources are tagged as "managed by CloudFormation" for easier tracking and cost management.

## Conclusion

This project provides hands-on experience with AWS CloudFormation, demonstrating how to create, update, and delete resources using CloudFormation templates. The power of CloudFormation lies in its ability to automate infrastructure management, saving time and reducing manual tasks. This introductory project serves as a foundation for further exploration of CloudFormation capabilities in the AWS ecosystem.
