+++
title = "Corrective controls with Conformance Packs"
date = 2020-08-07T09:37:25+10:00
draft = true

tags = ["AWS Config"]
categories = ["Intermediate"]

# Set the page as a chapter, changing the way it's displayed
chapter = false

# provides a flexible way to handle order for your pages.
weight = 500
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

In this builder session, learn how to build a solution that will evaluate your AWS resources for configuration compliance using [AWS Config Conformance Packs](https://aws.amazon.com/about-aws/whats-new/2019/11/introducing-aws-config-conformance-packs/). You will also learn how to improve your security posture by remediating non-compliant resources using automatic remediation actions.

{{% notice info %}}
Requirements: You will need AWS IAM Managed Policy “arn:aws:iam::aws:policy/AdministratorAccess” or equivalent.
{{% /notice %}}

#### Contents
{{% children %}}