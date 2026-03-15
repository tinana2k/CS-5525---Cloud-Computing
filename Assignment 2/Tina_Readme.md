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

## 🌐 Live Deployments

| Platform | URL | Hosting Method |
|----------|-----|----------------|
| **AWS** | https://tina-nguyen-assignment2-aws-2026.s3.us-east-2.amazonaws.com/index.html | Amazon S3 Static Website |
| **GCP** | https://storage.googleapis.com/tina-nguyen-assignment2-gcp-2026/index.html | Google Cloud Storage |
| **Azure** | https://tinanguyenassign2azure.z19.web.core.windows.net/ | Azure Blob Storage Static Website |

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

 ## 📊 Platform Comparison

| Feature | ☁️ AWS | 🌐 GCP | 🔷 Azure |
|--------|-----|-----|------|
| Deployment Type | PaaS | PaaS | PaaS |
| Setup Difficulty | Easy | Medium | Easy |
| Server Management | None | None | None |
| Deployment Speed | ~5 minutes | ~5 minutes | ~5 minutes |
| Access Control | Bucket Policy | Bucket Permissions/Access | Storage Access Control |
  -----------------------------------------------------------------------

------------------------------------------------------------------------

# Epilog

Through this assignment, I gained practical experience deploying a simple HTML webpage across three major cloud platforms: Amazon Web Services (AWS), Google Cloud Platform (GCP), and Microsoft Azure. One important lesson I learned is how similar the fundamental process of cloud deployment is across providers, even though their interfaces and terminology differ. Each platform required creating resources, configuring access permissions, uploading the HTML file, and ensuring that the webpage was publicly accessible.

The most challenging part of the assignment was configuring access permissions correctly, especially when dealing with public access restrictions and IAM policies, which initially prevented the webpage from being visible online. However, troubleshooting these issues helped me better understand how cloud security settings work. Among the three platforms, I found AWS S3 and Azure Blob Storage the easiest and most enjoyable to use because they provide built-in static website hosting, allowing the webpage to be deployed quickly without managing a server. Google Cloud required slightly more configuration for bucket permissions, which made the process a bit more complex but also more educational. 

Overall, this assignment helped me understand the similarities and differences between major cloud providers and strengthened my understanding of cloud storage, hosting services, and access control. 

For future classes, it would be helpful to include a brief overview of common cloud permission settings and security configurations beforehand, since many deployment issues arise from incorrect access policies rather than problems with the application itself.

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
-   screenshots/
    -   AWS/\
    -   Azure/\
    -   Google Cloud Platform/

------------------------------------------------------------------------

# Author

**Tina Nguyen**\
MS Data Science & Analytics\
University of Missouri -- Kansas City\
CS 5525 --- Cloud Computing
