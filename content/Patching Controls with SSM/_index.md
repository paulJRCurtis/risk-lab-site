+++
title = "Patching Controls with Systems Manager"
date = 2020-08-23T15:17:40+10:00
draft = false

tags = ["AWS Systems Manager", "Detective Controls"]
categories = ["Beginner"]

# Set the page as a chapter, changing the way it's displayed
chapter = false

# provides a flexible way to handle order for your pages.
weight = 10
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

Many organizations struggle to keep up with patching requirements. Sometimes one of the challenges is even to know what infrastructure you have. A definitive inventory of the operating systems and software running in the environment is not always easy to come by.

In a cloud environment there are two different approaches
based on whether the architecture includes instances that are immutable or 
non-immutable. 

This might seem a confusing statement, but lets break it down. First, instances are the equivalent of servers in cloud speak. An immutable instance is one that is never changed or updated, it just gets 
replaced. When an patch exists for an immutable instance the image, or [Amazon Machine Image](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instances-and-amis.html) (AMI), 
used to create the instance is update. The instances can be then be replaced with instance 
created from the new AMI. 

Immutable infrastructure has some big benefits including greater infrastructure consistency, a more 
predictable deployment process, and the ability to easily scaled up and down 
to meet capacity requirements. 

You also know that this immutable approach cannot be applied to every instance
as some applications don't allow for it. You need to identify these non-immutable 
instances that do not meet patch baselines. [AWS Systems Manager](https://aws.amazon.com/systems-manager/) - Patch Manager provides the capability to do this, not only for AWS instances but for your
on-premises instances too.

For more information see our resources on [Automated patching for non-immutable instances 
in the hybrid cloud using AWS Systems Manager](https://docs.aws.amazon.com/prescriptive-guidance/latest/patch-management-hybrid-cloud/welcome.html)

In this Lab you will get a clear view of the operating systems running in the environment, 
identify those that require patching, and then set up a corrective controls which will patch the selected instances.