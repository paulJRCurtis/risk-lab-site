+++
title = "Clean-up"
date = 2020-08-07T09:40:13+10:00
draft = false

# Set the page as a chapter, changing the way it's displayed
chapter = false

# provides a flexible way to handle order for your pages.
weight = 600
# Table of content (toc) is enabled by default. Set this parameter to true to disable it.
# Note: Toc is always disabled for chapter pages
disableToc = "false"
# If set, this will be used for the page's menu entry (instead of the `title` attribute)
menuTitle = ""
# The title of the page in menu will be prefixed by this HTML content
pre = "<b>6. </b>"
# The title of the page in menu will be postfixed by this HTML content
post = ""
# Hide a menu entry by setting this to true
hidden = false
# Display name of this page modifier. If set, it will be displayed in the footer.
LastModifierDisplayName = ""
# Email of this page modifier. If set with LastModifierDisplayName, it will be displayed in the footer
LastModifierEmail = ""
+++

It is important to turn off and delete unused resources so that they do not accrue charges. 

1. Go to Config console. Under settings page, Turn off recording.
2. Delete any Conformance Packs you created.
3. Empty the S3 bucket awsconformance-delivery-bucket-{ACCOUNT_ID}
3. Go to CloudFormation console and delete the stack you created - this might take a few minutes.
4. Go to S3 Console and delete any additional S3 buckets you created.