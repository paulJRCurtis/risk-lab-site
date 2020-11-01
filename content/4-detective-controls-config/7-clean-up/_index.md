+++
title = "Clean up"
date = 2020-08-07T09:39:18+10:00
draft = true

# Set the page as a chapter, changing the way it's displayed
chapter = false

# provides a flexible way to handle order for your pages.
weight = 700
# Table of content (toc) is enabled by default. Set this parameter to true to disable it.
# Note: Toc is always disabled for chapter pages
disableToc = "false"
# If set, this will be used for the page's menu entry (instead of the `title` attribute)
menuTitle = ""
# The title of the page in menu will be prefixed by this HTML content
pre = "<b>7. </b>"
# The title of the page in menu will be postfixed by this HTML content
post = ""
# Hide a menu entry by setting this to true
hidden = false
# Display name of this page modifier. If set, it will be displayed in the footer.
LastModifierDisplayName = ""
# Email of this page modifier. If set with LastModifierDisplayName, it will be displayed in the footer
LastModifierEmail = ""
+++

#### 1. Turn off Config ####

Go to the settings page and under **Recording is on** click the {{<tile black whitesmoke "turn off">}} button.

![Turn off recording](config-turn-off-recording.png)
A pop-up will ask you to confirm turning off recording. 
![Turn off recording confirmation](config-stop-recording.png)

Confirm by clicking {{<tile white cornflowerblue "Continue">}}.

#### 2. Delete Config Rules ####
Return to the Rules page.
![Config Rules](config-rules.png)
For each of the three rules; 
- Select the radio button beside the Rule name
- Click  {{<tile black whitesmoke "Edit">}}
- Scroll to the bottom of the page and click 
{{<tile black whitesmoke "Delete rule">}}
- On the confirmation pop-up
![Config Rules](config-delete-rule-confirm.png)  Click {{<tile white red Delete>}} to confirm deletion of the rule.

#### 3. Delete the SNS Subscription and Topic ####
Head back over to the SNS Console and select Subscriptions from the Menu.
![Delete Subscription](sns-delete-sub.png)
Select the radio button next to the Subscription and click {{<tile black whitesmoke "Delete">}}.
![Confirm Delete Subscription](sns-delete-sub-confirm.png)
On the confirmation pop-up click {{<tile white "#FF9900" "Delete">}}.  

Now select Topics from the menu bar.
![Delete Topic](sns-delete-topic.png)
Select the radio button next to the topic and click {{<tile black whitesmoke "Delete">}}.
![Confirm Delete Topic](sns-delete-topic-confirm.png)
To confirm deletion click {{<tile white "#FF9900" "Delete">}}.

{{% notice note %}}
Congratulations, you have now completed the lab and cleaned up the account.
{{% /notice %}}