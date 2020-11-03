+++
title = "Select AWS Config Rules"
date = 2020-08-07T09:39:18+10:00
draft = false

# Set the page as a chapter, changing the way it's displayed
chapter = false

# provides a flexible way to handle order for your pages.
weight = 200
# Table of content (toc) is enabled by default. Set this parameter to true to disable it.
# Note: Toc is always disabled for chapter pages
disableToc = "false"
# If set, this will be used for the page's menu entry (instead of the `title` attribute)
menuTitle = ""
# The title of the page in menu will be prefixed by this HTML content
pre = "<b>2. </b>"
# The title of the page in menu will be postfixed by this HTML content
post = ""
# Hide a menu entry by setting this to true
hidden = false
# Display name of this page modifier. If set, it will be displayed in the footer.
LastModifierDisplayName = ""
# Email of this page modifier. If set with LastModifierDisplayName, it will be displayed in the footer
LastModifierEmail = ""
+++

#### 1. Select Config Rules ####
In this introductory workshop we will use three of the AWS Managed Config Rules that relate to S3. 

The rules we will use are;
- [s3-bucket-server-side-encryption-enabled](https://docs.aws.amazon.com/config/latest/developerguide/s3-bucket-server-side-encryption-enabled.html)
- [s3-bucket-public-write-prohibited](https://docs.aws.amazon.com/config/latest/developerguide/s3-bucket-public-write-prohibited.html)
- [s3-bucket-public-read-prohibited](https://docs.aws.amazon.com/config/latest/developerguide/s3-bucket-public-read-prohibited.html)

The easiest way to find these rules is to enter ````s3-bucket```` into the filter field.

![Config select rules](config-select-rules.png?classes=shadow)
Select the three rules listed above and click {{<tile white cornflowerblue Next>}}

#### 2. Review Config Rules ####
![Config review rules](config-review-rules.png?classes=shadow)
Click {{<tile white cornflowerblue Confirm>}}
