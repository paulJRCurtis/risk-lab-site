+++
title = "Access a report"
date = 2020-08-23T15:17:40+10:00
draft = false

tags = []
categories = []

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

#### 1. Access the AWS Artifact Console ####
From the Console select the Services dropdown and Artifact under Security, Identity, & Compliance.

![AWS Artifact](artifact.png?classes=shadow) 

Click {{<tile "Black" "ghostwhite" "View reports">}} 

#### 2. Download the SOC 2 Report ####
In this lab we'll look at the Service Organization Controls (SOC) 2 Report.  

As you can see reports available include our Service Organization Control (SOC) reports, ISO, Payment Card Industry (PCI) reports, and certifications from accreditation bodies across geographies and compliance verticals that validate the implementation and operating effectiveness of AWS security controls. 
![AWS Artifact](artifact-soc-report.png?classes=shadow)
Type SOC 2 into the search and select SOC 2 Report - Current, then select {{<tile "white" "#E3661B" "Download report">}}.  

Read and accept the NDA - {{<tile "white" "#E3661B" "Accept NDA and download">}}

#### 3. Open the Report ####
Open your downloads folder and open the file {{<textcode "Service_Organization_Controls_(SOC)_2_Report_-_Current.pdf">}}

Review the Terms and Conditions of the artifact and click the paperclip icon to display the attachments.  

![PDF Attachments](pdf-paperclip.png?classes=shadow)

For this report there are three files attached, as a start open the first file in the list, the AWS SOC 2 Type 2 Report.

{{% notice note %}}
**The dates in the file name are the in scope dates for the report.**  
SOC reports are audits performed over a period of time and do not expire. Our auditors perform our SOC audits twice a year over a period of 6 months: Oct 1 to Mar 31 and Apr 1 to Sept 30. Once the audit period is over, our auditors prepare their audit report which is then released in May and November, respectively. Should you seek assurance that we have maintained the control environment described in this most recent SOC report, we make a SOC Continued Operations Letter available to you in Artifact. 
{{% /notice %}}

#### 4. Review the Report ####
Take some time to review these independent third-party examination reports that demonstrate how AWS achieves key compliance controls and objectives.  

More information on our SOC compliance can be found at [SOC Compliance](https://aws.amazon.com/compliance/soc-faqs/).