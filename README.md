# Rise-Internship-Project-2
# AWS S3 & CloudFront Static Website Hosting

## Project Overview

This project demonstrates how to host a static website using **Amazon S3** and distribute it globally using **Amazon CloudFront**. The objective of this project is to understand how cloud services can be used to improve website performance, availability, and scalability.

By using CloudFront as a Content Delivery Network (CDN), website content is cached at multiple edge locations around the world, allowing users to access the website faster and with lower latency.

---

## Architecture

User → Internet → CloudFront CDN → Amazon S3 Bucket → Static Website Files

CloudFront distributes the website content globally by caching files at edge locations closer to users.

---

## AWS Services Used

- **Amazon S3** – For storing and hosting static website files  
- **Amazon CloudFront** – Content Delivery Network for faster global delivery  
- **HTML** – Structure of the website  
- **CSS** – Styling and layout  
- **JavaScript** – Client-side functionality  

---

## Implementation Steps

### 1. Create an S3 Bucket

- Logged into the AWS Management Console
- Created a new **S3 bucket**
- Disabled **Block Public Access**
- Enabled **Static Website Hosting**
- Set the **index document** as `index.html`

---

### 2. Upload Website Files

- Uploaded static website files including:
  - `index.html`
  - CSS files
  - JavaScript files
  - Images (if any)

- Configured object permissions to allow **public read access**

---

### 3. Configure CloudFront Distribution

- Created a new **CloudFront distribution**
- Selected the **S3 bucket as the origin**
- Enabled **HTTPS redirection**
- Set **default root object** as `index.html`
- Deployed the distribution

---

## Project Outcome

- Static website successfully hosted using **Amazon S3**
- Website content delivered globally using **CloudFront CDN**
- Faster website loading due to edge caching
- Secure access enabled through **HTTPS**

---

## Key Learnings

This project helped in understanding:

- Static website hosting using **Amazon S3**
- CDN implementation using **CloudFront**
- Difference between **S3 website endpoint** and **CloudFront distribution**
- How global edge locations improve website performance
- Basic cloud architecture for scalable web hosting

---

## Screenshots

(Add project screenshots here)

---

## Future Improvements

Possible improvements for this project include:

- Connecting a **custom domain using Route 53**
- Implementing **SSL certificates using AWS Certificate Manager**
- Automating deployment using **CI/CD pipelines**
- Adding **cache optimization and security configurations**

---

## Repository Purpose

This repository was created to demonstrate practical experience with **AWS S3 static website hosting and CloudFront CDN configuration** as part of my internship learning in cloud computing and DevOps.
