+++
title = "Getting to Know the Console"
date =  2020-08-14T15:34:54+10:00
draft = false

tags = []
categories = ["Beginner"]

# Set the page as a chapter, changing the way it's displayed
chapter = false

# provides a flexible way to handle order for your pages.
weight = 5
# Table of content (toc) is enabled by default. Set this parameter to true to disable it.
# Note: Toc is always disabled for chapter pages
disableToc = "false"
# If set, this will be used for the page's menu entry (instead of the `title` attribute)
menuTitle = ""
# The title of the page in menu will be prefixed by this HTML content
pre = ""
# The title of the page in menu will be postfixed by this HTML content
post = ""
# Hide a menu entry by setting this to true
hidden = false
# Display name of this page modifier. If set, it will be displayed in the footer.
LastModifierDisplayName = ""
# Email of this page modifier. If set with LastModifierDisplayName, it will be displayed in the footer
LastModifierEmail = ""
+++

#### Login to your AWS Account ####  
If you haven't already, logon to your AWS account.  If you don't have an account, go to [Start Workshop](/risk-lab-site/start-workshop).  

Let's get to know the [Management Console](https://aws.amazon.com/console/)  
![AWS Management Console](console.png?classes=shadow)

The AWS Management Console is a web application that comprises and refers to a broad collection of
service consoles for managing Amazon Web Services. When you first sign in, you see the console home
page.

Along the top menubar you will see a few important elements we will use often. 

#### AWS Logo #### 
Clicking on the AWS logo will bring you back to this console screen.

#### Services Dropdown ####  
Choose **Services** to open a full list of services. On the upper right of the page, choose Group to see the
services listed by category or choose A–Z to see an alphabetical listing. Then choose the service that
you want.  Clicking **Services** again will close the list. 
<!-- 
#### Resource Groups Dropdown ####  
The AWS Management Console includes the Resource Groups menu, a feature for managing AWS
resources such as an Amazon EC2 instance or an Amazon S3 bucket as a group. You can also use the
Resource Groups menu to start Tag Editor, a tool for managing and applying labels, or tags, to organize
your resources.

For more information on creating resource groups and using Tag Editor, see the following topics in the
[AWS Resource Groups and Tag Editor User Guide](https://docs.aws.amazon.com/ARG/latest/userguide/welcome.html).

#### Pushpin ####  
You can add and delete shortcuts for the services that you use most.  

To add a shortcut choose the pushpin icon and drag a service from the menu to the navigation bar. You can add more shortcuts and drop them onto the navigation bar in any order that you want. 

To remove a shortcut  choose the pushpin icon and drag the shortcut off the navigation bar -->

#### Alert ####  
Clicking on alerts will display a dropdown showing Open issues, scheduled changes and Other notifications, as well as the option to show all alerts.

Clicking any of these will take you to the Personal Health Dashboard. Personal Health Dashboard gives you a personalized view into the performance and availability of the AWS services underlying your AWS resources, to learn more go to [AWS Personal Health Dashboard](https://aws.amazon.com/premiumsupport/technology/personal-health-dashboard/).

#### User/Account Dropdown ####  
The User/Account Dropdown is on which we will use on occasionally during the labs.  Lets step through the information on the dropdown.
User - the image below shows the Federated Login that you will see if your identity is provided to the AWS Console form an external identity provider - in the example show this is the AWS Event Engine.  If you signed on directly to the console you will see IAM User
Account: this is the account Id, the example shows a number but you can also setup and account alias which is easier to remember.
The next grouping of options may vary slightly depending on your access but they deal with billing and your credentials.
The final option is to Sign Out.
![AWS Management Console](accountID.png?classes=shadow)

#### Region Dropdown ####  
For many services, you can choose a Region that specifies where your resources are hosted. You do not
choose a Region for the AWS Management Console or for some services, such as IAM.
To choose a Region  
1. In the AWS Management Console, choose a service to go to that service's console.
2. On the navigation bar, choose the name of the currently displayed Region.
When you choose a Region, that Region becomes the default in the console.

{{% notice warning %}}
Your will only be able to complete this workshop in the Sydney (ap-southeast-2) Region.  
{{% /notice %}}

#### Support Dropdown ####  
This dropdown lists the various support options and resources available to  you.
