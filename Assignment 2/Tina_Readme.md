# Assignment 2 --- Multi-Cloud Web Deployment

**Course:** CS 5525 --- Cloud Computing\
**Student:** Tina Nguyen\
**University:** University of Missouri -- Kansas City

------------------------------------------------------------------------

# Overview

This assignment demonstrates deploying a simple personal webpage across
three major cloud providers: **Amazon Web Services (AWS), Google Cloud
Platform (GCP), and Microsoft Azure**.

The objective of this assignment is to understand how different cloud
platforms host web content, configure public access permissions, and
deploy a simple HTML page across multiple cloud environments.

------------------------------------------------------------------------

# Live Deployments

  -----------------------------------------------------------------------------------------------------------------------------------------
  Platform           URL                                                                              Hosting Method
  ------------------ -------------------------------------------------------------------------------- -------------------------------------
  AWS                https://tina-nguyen-assignment2-aws-2026.s3.us-east-2.amazonaws.com/index.html   Amazon S3 Static Website

  GCP                https://storage.googleapis.com/tina-nguyen-assignment2-gcp-2026/index.html       Google Cloud Storage

  Azure              https://tinanguyenassign2azure.z19.web.core.windows.net/                         Azure Blob Storage Static Website
  -----------------------------------------------------------------------------------------------------------------------------------------

------------------------------------------------------------------------

# Web Page

A simple HTML webpage (`index.html`) was created and deployed on all
three platforms.

The page includes: - Name: **Tina Nguyen** - Course information - A
simple greeting message

Example content:

Hello! My name is Tina Nguyen.\
This webpage is deployed on AWS, Google Cloud Platform, and Microsoft
Azure.

------------------------------------------------------------------------

# Platform Deployment Details

## 1. Amazon AWS

**Method:** Amazon S3 Static Website Hosting

Steps performed:

1.  Logged into the AWS Management Console.
2.  Navigated to the Amazon S3 service.
3.  Created a new S3 bucket.
4.  Disabled "Block Public Access" for the bucket.
5.  Enabled **Static Website Hosting**.
6.  Set `index.html` as the index document.
7.  Uploaded the `index.html` file to the bucket.
8.  Accessed the deployed webpage using the S3 endpoint.

------------------------------------------------------------------------

## 2. Google Cloud Platform

**Method:** Google Cloud Storage

Steps performed:

1.  Logged into Google Cloud Console.
2.  Created a new project.
3.  Navigated to **Cloud Storage**.
4.  Created a storage bucket.
5.  Uploaded `index.html` to the bucket.
6.  Disabled **Public Access Prevention**.
7.  Added IAM permission:
    -   Principal: `allUsers`
    -   Role: **Storage Object Viewer**
8.  Accessed the webpage via the public object URL.

------------------------------------------------------------------------

## 3. Microsoft Azure

**Method:** Azure Blob Storage Static Website

Steps performed:

1.  Logged into the Azure Portal.
2.  Created a **Storage Account**.
3.  Navigated to **Static Website** under Data Management.
4.  Enabled Static Website Hosting.
5.  Set `index.html` as the index document.
6.  Uploaded `index.html` into the `$web` container.
7.  Accessed the generated endpoint URL.

------------------------------------------------------------------------

# Platform Comparison

  -----------------------------------------------------------------------
  Feature           AWS               GCP               Azure
  ----------------- ----------------- ----------------- -----------------
  Deployment Type   PaaS              PaaS              PaaS

  Setup Difficulty  Easy              Medium            Easy

  Server Management None              None              None

  Deployment Speed  \~5 minutes       \~5 minutes       \~5 minutes

  Access Control    Bucket Policy     IAM Permissions   Storage Access
                                                        Control
  -----------------------------------------------------------------------

------------------------------------------------------------------------

# Epilog

This assignment provided hands-on experience deploying a web page across
multiple cloud providers. AWS S3 and Azure Blob Storage made static
website deployment very straightforward because both services provide
built-in static hosting features. Google Cloud required additional
configuration for public access permissions, which helped demonstrate
how IAM policies work within cloud environments.

Through this assignment, I gained a better understanding of how cloud
platforms handle web hosting, storage services, and security
permissions. It also highlighted how similar the deployment processes
are across major cloud providers, even though their interfaces and
terminology differ.

------------------------------------------------------------------------

# Technologies Used

-   HTML
-   Amazon S3
-   Google Cloud Storage
-   Microsoft Azure Blob Storage
-   Cloud IAM / Access Policies

------------------------------------------------------------------------

# Repository Structure

Assignment_2/

-   index.html\
-   README.md\
-   images/
    -   aws/\
    -   gcp/\
    -   azure/

------------------------------------------------------------------------

# Author

**Tina Nguyen**\
MS Data Science & Analytics\
University of Missouri -- Kansas City\
CS 5525 --- Cloud Computing
