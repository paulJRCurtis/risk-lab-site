+++
title = "Enable AWS Config"
date = 2020-08-07T09:39:18+10:00
draft = false

# Set the page as a chapter, changing the way it's displayed
chapter = false

# provides a flexible way to handle order for your pages.
weight = 100
# Table of content (toc) is enabled by default. Set this parameter to true to disable it.
# Note: Toc is always disabled for chapter pages
disableToc = "false"
# If set, this will be used for the page's menu entry (instead of the `title` attribute)
menuTitle = ""
# The title of the page in menu will be prefixed by this HTML content
pre = "<b>1. </b>"
# The title of the page in menu will be postfixed by this HTML content
post = ""
# Hide a menu entry by setting this to true
hidden = false
# Display name of this page modifier. If set, it will be displayed in the footer.
LastModifierDisplayName = ""
# Email of this page modifier. If set with LastModifierDisplayName, it will be displayed in the footer
LastModifierEmail = ""
+++

First, we need to enable AWS Config and begin tracking of your resources.

#### 1. Login to your AWS Account
If you haven't already logon to your AWS account, do so now.  If you don't yet have an account go to [Start the Workshop](/risk-lab-site/1-start-workshop/)

#### 2. Access the AWS Config Console
Select the Services dropdown on the menu bar at the top left. Select Config under **Management & Governance**, or search for Config using **Find Services**.  

**If this is your first time using AWS Config**  
Select {{<tile "white" "cornflowerblue" "Get started">}} from the AWS Config intro screen.

![AWS Config Wizard](config-wizard.png?classes=shadow)

**If you’ve already used AWS Config**  
You will start at the AWS Config Dashboard, select Settings on the menu to the left.

#### 3. Select resource types to record  
On the Settings page, under **Resource types to record**, ensure  Record all resources supported in this region checkbox is selected and you may also check the checkbox for Include global resources, but it's not required for this workshop.
![AWS Config Settings](config-settings.png?classes=shadow)

Checking these two boxes means that AWS Config will record configuration changes for all supported resources all resources as well as configuration changes for AWS Identity and Access Management (IAM) resources which are global resources. Global resources are not tied to an individual region and can be used in all regions. 

#### 4. Create Amazon S3 bucket for configuration history
AWS Config needs a place to store configuration history and configuration snapshot files, we will use [Amazon Simple Storage Service (Amazon S3)](https://aws.amazon.com/s3/) to provide this storage space - what AWS calls an S3 Bucket.   
Under **Amazon S3 bucket**, select Create a bucket to have the Amazon S3 bucket created automatically.  

{{% notice info %}}
This S3 bucket will be used to store the history used by Config, but to keep things simple and remove the need to create a second Bucket, we will be applying the Config Rules to this same S3 Bucket.
{{% /notice %}}

<!-- #### 5. Optional - Set-up notifications (SNS topic)
You can leave the settings under **Amazon SNS topic** as is, or as an extra activity later you can check the box for Stream configuration changes and notifications to an Amazon SNS topic, and then select Create a topic, and give the SNS Topic a name, something like ```AWS-Config-Alerts```, or whatever you like.  

![AWS Config SNS](config-SNS.png?classes=shadow)

This will enable AWS Config to send us configuration changes and notifications via [Amazon Simple Notification Service (SNS)](https://aws.amazon.com/sns/). We will configure this later in an optional step. -->

#### 5. AWS Config role
There is no need to change any settings in this section, Create AWS Config service-linked role should already be selected.

{{% notice note %}}
It is worth taking a moment to understand that for AWS Config to access other services like S3 and SNS we need to grant it permissions. This step crates a role for Config that will allow Config to access the S3 bucket and the SNS topic we set-up in the steps above.
{{% /notice %}}

Click {{<tile "white" "cornflowerblue" "Next">}}.  