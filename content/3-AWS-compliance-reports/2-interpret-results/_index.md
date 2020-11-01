+++
title = "Interpreting the results"
date = 2020-08-23T15:17:40+10:00
draft = false

tags = []
categories = []

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


Now that we have the report lets take some time to understand it.  First we need to understand what the report covers, the overall conclusion and the detailed results.  We'll start with the AWS Shared Responsibility Model and then dive into the specifics of the report.

#### 1. Shared Responsibility Model ####
First we need to consider the report in the context of the [Shared Responsibility Model](https://aws.amazon.com/compliance/shared-responsibility-model/) i.e. what is an AWS responsibility and what is a customer responsibility.  Controls can be grouped into three categories.
![AWS Artifact](shared-responsibility-model.png?classes=shadow)
Broadly speaking we can see that the model is divided into “Security of the Cloud” - AWS responsibility and “Security in the Cloud” – Customer responsibility.  From a controls perspective this can be thought of as.

- **Inherited Controls** – Controls which a customer fully inherits from AWS for example physical and environmental controls.
- **Shared Controls** – Controls which apply to both the infrastructure layer and customer layers, but in completely separate contexts or perspectives. In a shared control, AWS provides the requirements for the infrastructure and the customer must provide their own control implementation within their use of AWS services. Examples include Patch Management – AWS is responsible for patching and fixing flaws within the infrastructure, but customers are responsible for patching their guest OS and applications.
- **Customer Specific** – Controls which are solely the responsibility of the customer based on the application they are deploying within AWS services. Examples include Service and Communications Protection or Zone Security which may require a customer to route or zone data within specific security environments.

Take a few minutes to familiarize yourself with the [Shared Responsibility Model](https://aws.amazon.com/compliance/shared-responsibility-model/).

{{% notice note %}}
To support a deeper understanding of security and shared responsibility for AWS’ services, AWS has categorized them into three main categories: infrastructure, container, and abstracted. Each category comes with a slightly different security ownership model based on how customers interact and access the functionality.  
To dive deeper into this topic you can complete to optional lab section [Advanced Responsibility Model](/risk-lab-site/aws-compliance-reports/3-optional-shared-responsibility/)
{{% /notice %}}

#### 2. Completeness Check ####  
Under the *Scope* heading of *SECTION II – Independent Service Auditor’s Assurance Report* there is a list of the AWS Services, and Global Infrastructure Locations which are considered in scope.

#### 3. Auditor Opinon ####  
Review the *Opinion* in *SECTION II – Independent Service Auditor’s Assurance Report* which provides the Auditor opinion of the report.

#### 4. The Detailed Results ####  
*SECTION IV – Description of Criteria, AWS Controls, Tests and Results of Tests* contains tables mapping between the Auditors Control Criteria and AWS Control Activities (AWSCA) and for each the results of the tests.

{{% notice info %}}
Congratulations! you have accessed AWS Artifact, downloaded a SOC 2 Type 2 Report, and reviewed the results to confirm the controls that AWS operates on your behalf. 
{{% /notice %}}