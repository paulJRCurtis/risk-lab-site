+++
title = "Introduction"
date = 2020-08-07T09:38:17+10:00
draft = true

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

In this course, we will be deploying Amazon S3 Operational Best Practices with remediation actions conformance pack in an AWS Account. This pack contains following AWS Managed Config Rules.

You can click on the AWS Managed Config Rule name to see the Developer Guide for the rule.

- **[S3BucketPublicReadProhibited](https://docs.aws.amazon.com/config/latest/developerguide/s3-bucket-public-read-prohibited.html) with Remediation Action**  
Checks that your Amazon S3 buckets do not allow public read access. The rule checks the Block Public Access settings, the bucket policy, and the bucket access control list (ACL).  

- **[S3BucketPublicWriteProhibited](https://docs.aws.amazon.com/config/latest/developerguide/s3-bucket-public-write-prohibited.html) with Remediation Action**  
Checks that your Amazon S3 buckets do not allow public write access. The rule checks the Block Public Access settings, the bucket policy, and the bucket access control list (ACL).  

- **[S3BucketReplicationEnabled](https://docs.aws.amazon.com/config/latest/developerguide/s3-bucket-public-write-prohibited.html)**  
Checks whether S3 buckets have cross-region replication enabled.  

- **[S3BucketSSLRequestsOnly](https://docs.aws.amazon.com/config/latest/developerguide/s3-bucket-ssl-requests-only.html)**  
Checks whether S3 buckets have policies that require requests to use Secure Socket Layer (SSL).  

- **[S3BucketServerSideEncryptionEnabled](https://docs.aws.amazon.com/config/latest/developerguide/s3-bucket-server-side-encryption-enabled.html) with Remediation Action**  
Checks that your Amazon S3 bucket either has Amazon S3 default encryption enabled or that the S3 bucket policy explicitly denies put-object requests without server side encryption.  

- **[S3BucketLoggingEnabled](https://docs.aws.amazon.com/config/latest/developerguide/s3-bucket-logging-enabled.html) with Remediation Action**  
Checks whether logging is enabled for your S3 buckets.