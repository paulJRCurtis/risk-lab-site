+++
title = "Clean Up"
date =  2020-08-04T15:48:01+10:00
draft = false

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
pre = "<b>10. </b>"
# The title of the page in menu will be postfixed by this HTML content
post = ""
# Hide a menu entry by setting this to true
hidden = false
# Display name of this page modifier. If set, it will be displayed in the footer.
LastModifierDisplayName = ""
# Email of this page modifier. If set with LastModifierDisplayName, it will be displayed in the footer
LastModifierEmail = ""
+++

**1. Delete S3 artifactstorebucket**  
When we ran the CloudFormation template to create the CodePipeline, one of the resources created was an S3 bucket the CodePipeline uses to store it's working files.  We need to empty this bucket in order for the CloudFormation deletion to complete.

Select the checkbox beside the bucket that's name starts with {{<textcode "pipeline-controls-lab-stack-artifactstorebucket-">}} and click {{<tile "cornflowerblue" "white" "Empty">}}

{{% notice info %}}
You can only delete empty S3 buckets. Deletion fails for buckets that have contents.
{{% /notice %}}

**2. Delete CloudFormation Stacks**  
Go to Cloudformation and delete;
- Prod-SG
- pipeline-controls-lab-environments
- pipeline-controls-lab-stack