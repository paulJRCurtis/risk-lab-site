+++
title = "Preventative controls with Code Pipeline"
date = 2020-08-01T15:28:32+10:00
draft = false

tags = []
categories = ["Advanced"]

# Set the page as a chapter, changing the way it's displayed
chapter = false

# provides a flexible way to handle order for your pages.
weight = 1000
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

A powerful way to implement preventative controls is to embed them into code pipelines. 

In this lab we demonstrate a code pipeline which takes an AWS CloudFormation template and runs checks against it, if it passes the template is then deployed into a testing environment where additional checks are run, and finally if the template meets requirements it can be deployed into the production environment. 

#### Contents
{{% children %}}