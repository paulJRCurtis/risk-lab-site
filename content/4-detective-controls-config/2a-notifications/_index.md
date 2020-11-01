+++
title = "Set-up Notifications"
date = 2020-08-07T09:39:18+10:00
draft = true

# Set the page as a chapter, changing the way it's displayed
chapter = false

# provides a flexible way to handle order for your pages.
weight = 150
# Table of content (toc) is enabled by default. Set this parameter to true to disable it.
# Note: Toc is always disabled for chapter pages
disableToc = "false"
# If set, this will be used for the page's menu entry (instead of the `title` attribute)
menuTitle = " - Notifications"
# The title of the page in menu will be prefixed by this HTML content
pre = "<b>1.1 Optional</b>"
# The title of the page in menu will be postfixed by this HTML content
post = ""
# Hide a menu entry by setting this to true
hidden = false
# Display name of this page modifier. If set, it will be displayed in the footer.
LastModifierDisplayName = ""
# Email of this page modifier. If set with LastModifierDisplayName, it will be displayed in the footer
LastModifierEmail = ""
+++

{{% notice warning %}}
Only complete this section if you created an SNS Topic at [Step 5 Set-up notifications](http://localhost:1313/risk-lab-site/4-detective-controls-config/1-config-setup/#5-optional---set-up-notifications) during Enable AWS Config.
{{% /notice %}}

[Amazon Simple Notification Service](https://aws.amazon.com/sns) (SNS) is a fully managed messaging service for both system-to-system and app-to-person (A2P) communication. We will use the service to notify us of configuration changes and Config Rule notifications. In a production environment It would be impractical to send these notifications to a person, you would send then to a monitoring system. 

Amazon SNS lets you send push notifications to mobile apps, text messages to mobile phone numbers, and plain-text emails to email addresses.
![SNS Topics](sns-overview.png?classes=shadow)
Messages are sent from a publisher, in this case Config to a Topic and then distributed to subscribers.

#### 1. The SNS console ####
![SNS Console](console-sns.png?classes=shadow)

#### 2. Go to the Topics Page ####
From the SNS Console click on **Topics** on the dashboard or on the menu on the left hand side.

![SNS Topics](sns-topics.png?classes=shadow)

Click on the topic name, which wil be AWS-Config-Alerts if you used the suggested name. This will take you to the page detailing the Topic and any subscriptions.

#### 3. Create a Subscription ####
![SNS Topics](sns-config-alerts.png?classes=shadow)
From here click {{<tile white "#FF9900" "Create subscription">}}
![SNS Topics](sns-create-subscription.png?classes=shadow)
Select Email as the Protocol and enter your email address as the endpoint.  

Click {{<tile white "#FF9900" "Create subscription">}}

#### 4. Confirm Subscription ####
Go to your email, and you should receive an email similar to the below, click Confirm subscription.
![SNS Topics](sns-email.png?width=300px&classes=shadow)

{{% notice note %}}
Throughout the rest of this lab keep an eye on your email to see the notifications come through.
{{% /notice %}}

#### 5. Return to Config ####
You can now return to the Config console to select the Config rules to activate.
