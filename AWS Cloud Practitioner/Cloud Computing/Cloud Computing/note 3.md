## EC2 – Elastic Compute

### What is EC2?

-    Virtual server in the cloud
-    You choose OS, CPU, RAM, storage
-    Pay as you go

### Key Concepts

-    **Instance** = Virtual machine
-    **AMI** = Pre-configured template (OS + software)

### Instance Types

-    General Purpose
-    Compute Optimized
-    Memory Optimized
-    Storage Optimized

### Pricing Models

-    **On-Demand** → pay per use
-    **Reserved** → cheaper (1–3 years)
-    **Spot** → cheapest, can be terminated
-    **Dedicated Hosts** → physical server

### Security

-    **Security Groups**
     -    Acts like firewall
     -    Only allow rules

---

## EC2 – Instance Storage

### EBS (Elastic Block Store)

-    Persistent storage
-    Can detach & attach
-    Types: SSD, HDD

### Instance Store

-    Temporary storage
-    Data lost when instance stops

### EFS (Elastic File System)

-    Shared storage
-    Multiple EC2 can access

---

## ELB & ASG

### ELB (Elastic Load Balancer)

-    Distributes traffic

Types:

-    **ALB** → HTTP/HTTPS
-    **NLB** → TCP (high performance)
-    **Classic** → legacy

### ASG (Auto Scaling Group)

-    Automatically scales instances

Features:

-    Scale out (add)
-    Scale in (remove)
-    Min / Max / Desired capacity

---

## Amazon S3

### Basics

-    Object storage
-    Bucket = container
-    Object = file

### Storage Classes

-    Standard
-    IA (Infrequent Access)
-    Glacier (archival)

### Features

-    Versioning
-    Lifecycle rules
-    Encryption

### Security

-    Bucket policy
-    IAM access

---

## Databases & Analytics

### Databases

-    **RDS** → SQL (MySQL, PostgreSQL)
-    **DynamoDB** → NoSQL (key-value)
-    **Aurora** → high-performance SQL

### Analytics

-    **Redshift** → data warehouse
-    **Athena** → query S3 with SQL
-    **EMR** → big data (Hadoop/Spark)

---

## Other Compute Services

### EC2

-    Full control

### Lambda

-    Serverless
-    Runs code on demand

### Batch

-    Run batch jobs

### Lightsail

-    Simple VPS
-    Fixed pricing

---

## Deployments & Infrastructure

### Infrastructure as Code

-    **CloudFormation**

     -    JSON/YAML templates

-    **Elastic Beanstalk**
     -    Easy deployment

### Monitoring

-    **CloudWatch** → logs & metrics
-    **CloudTrail** → API tracking

---

## AWS Global Infrastructure

### Components

-    **Region** → geographic area
-    **AZ (Availability Zone)** → data centers
-    **Edge Locations** → CDN (CloudFront)

### High Availability

-    Use multiple AZs
-    Load Balancer + Auto Scaling
-    Backup across regions
