# 📘 AWS Full Notes for Beginners (GitHub Format)

---

## 🧠 Part 1: AWS Basics

### 🔹 What is AWS?

AWS (Amazon Web Services) is a cloud computing platform by Amazon that offers 200+ services such as compute, storage, networking, database, AI/ML, and more. It allows companies to build scalable, flexible, and reliable applications.

**Example:** Hosting a website on AWS using EC2 and S3 instead of maintaining your own server.

---

### 🔹 What is Cloud Computing?

Cloud computing allows you to access IT resources like servers, databases, and storage over the internet on a pay-as-you-go basis.

**Example:** Using Google Drive to store files without needing a physical hard drive.

---

### 🔹 Benefits of Cloud Computing

* No upfront cost
* Scalable and flexible
* Fast deployment
* Global reach
* Secure and reliable
* Pay only for what you use

---

### 🔹 Cloud Service Models

| Model | Description                 | AWS Examples        |
| ----- | --------------------------- | ------------------- |
| IaaS  | Infrastructure as a Service | EC2, EBS            |
| PaaS  | Platform as a Service       | Elastic Beanstalk   |
| SaaS  | Software as a Service       | AWS Chime, WorkDocs |

---

### 🔹 Cloud Deployment Models

| Model   | Description                              |
| ------- | ---------------------------------------- |
| Public  | Services offered over the internet (AWS) |
| Private | Services hosted in a private data center |
| Hybrid  | Combination of public and private        |

---

## 🌍 Part 2: AWS Global Infrastructure

### 🔹 What is Global Infrastructure?

AWS has data centers globally. It’s designed for high availability, scalability, and security.

### 🔹 Region

A physical location in the world with multiple AZs (e.g., ap-south-1 in Mumbai).

### 🔹 Availability Zone (AZ)

One or more data centers in a region. AZs are isolated but connected with low-latency links.

### 🔹 Edge Location

Content caching location (used by CloudFront) to serve data faster to end-users.

### 🔹 Local Zone

Brings AWS services closer to end users in metro cities for low-latency workloads.

### 🔹 Wavelength Zone

Delivers AWS services over 5G networks for ultra-low latency apps.

---

## 🔐 Part 3: AWS Security & Compliance

### 🔹 What is AWS Security?

Built-in security services that protect data, infrastructure, and apps.

### 🔹 Shared Responsibility Model

| Responsibility    | AWS | Customer |
| ----------------- | --- | -------- |
| Hardware & Infra  | ✅   | ❌        |
| Data & Encryption | ❌   | ✅        |
| IAM & Access Mgmt | ❌   | ✅        |

### 🔹 IAM (Identity and Access Management)

Manage user access using Users, Groups, Roles, and Policies.

### 🔹 KMS (Key Management Service)

Manage encryption keys securely.

### 🔹 AWS Shield & WAF

* Shield protects against DDoS attacks
* WAF protects against common web attacks

### 🔹 GuardDuty & Inspector

* Detect threats using ML (GuardDuty)
* Scan EC2 for vulnerabilities (Inspector)

### 🔹 CloudTrail vs CloudWatch

* CloudTrail = Who did what (API logging)
* CloudWatch = Monitor performance (metrics, logs)

---

## ⚙️ Part 4: Compute Services

### 🔹 EC2 (Elastic Compute Cloud)

Virtual server to run apps. Choose instance types based on CPU, RAM, storage.

### 🔹 EC2 Pricing Models

* On-Demand: Pay hourly
* Reserved: 1 or 3-year commitment
* Spot: Use unused capacity (cheaper)

### 🔹 AMI (Amazon Machine Image)

Template to launch EC2 with OS and software.

### 🔹 Auto Scaling

Automatically add/remove EC2 instances based on demand.

### 🔹 Load Balancer

Distributes incoming traffic across EC2s.

### 🔹 Lambda

Serverless function execution. Runs code in response to events.

**Example:** Trigger a Lambda to resize an image when uploaded to S3.

### 🔹 Beanstalk

Platform to deploy web apps (automates provisioning, scaling).

---

## 💾 Part 5: Storage Services

### 🔹 Amazon S3

Object storage for any type of file.

### 🔹 S3 Classes

Standard, IA, One Zone-IA, Glacier, Glacier Deep Archive.

### 🔹 Versioning & Encryption

Track changes, restore versions. Encrypt with KMS or S3-managed keys.

### 🔹 Amazon EBS

Block storage for EC2. Good for databases, file systems.

### 🔹 Amazon EFS

Shared file storage across multiple EC2 instances.

### 🔹 Amazon Glacier

Archival storage with low cost and long retrieval time.

---

## 🗃️ Part 6: Database Services

### 🔹 Amazon RDS

Managed SQL databases (MySQL, PostgreSQL, Oracle, etc.)

### 🔹 Aurora

High-performance MySQL/PostgreSQL-compatible database.

### 🔹 DynamoDB

NoSQL key-value and document database. Serverless and highly scalable.

### 🔹 Redshift

Data warehouse service for analytics and reporting.

### 🔹 ElastiCache

In-memory caching (Redis/Memcached) to speed up applications.

### 🔹 DMS (Database Migration Service)

Migrate on-premise DBs to AWS.

---

## 🌐 Part 7: Networking & Content Delivery

### 🔹 VPC (Virtual Private Cloud)

Your private network on AWS.

### 🔹 Subnets & Routing

Divide VPC into subnets (public/private), use route tables for network flow.

### 🔹 IGW vs NAT Gateway

* IGW: For internet access (public subnets)
* NAT: For private subnet internet access

### 🔹 NACL vs Security Groups

* NACL = firewall at subnet level
* SG = firewall at instance level

### 🔹 CloudFront

CDN to cache and deliver content globally.

### 🔹 Global Accelerator

Improves global application availability and performance.

---

## 📡 Part 8: Monitoring, Logging & Analytics

### 🔹 CloudWatch

Monitor AWS resources (metrics, logs, alarms).

### 🔹 CloudTrail

Track user/API activity in your AWS account.

### 🔹 AWS Config

Monitors resource configurations and compliance.

### 🔹 AWS X-Ray

Analyze and debug apps (especially microservices).

### 🔹 Kinesis

Stream processing service for real-time analytics.

### 🔹 QuickSight

BI tool to visualize data from AWS services.

---

## 🔄 Part 9: Application Integration

### 🔹 Amazon SQS

Queue service for decoupling components.

### 🔹 Amazon SNS

Notification service (SMS, email, Lambda triggers).

### 🔹 EventBridge

Event bus for routing app events.

### 🔹 Step Functions

Serverless workflows using state machines.

---

## 🔧 Part 10: DevOps & Automation

### 🔹 CloudFormation

Define infrastructure as code using YAML/JSON.

### 🔹 CodeCommit, CodeBuild, CodeDeploy, CodePipeline

CI/CD services for version control, build, deployment, and automation.

### 🔹 OpsWorks

Configuration management using Chef/Puppet.

### 🔹 Systems Manager (SSM)

Manage EC2 instances, automate tasks, patching.

---

## 🧪 Part 11: Identity, Security & Management Tools

### 🔹 AWS Organizations

Manage multiple AWS accounts from one place.

### 🔹 IAM (revisited)

Control user access, apply roles and policies.

### 🔹 AWS SSO

Single sign-on access to multiple AWS accounts/apps.

### 🔹 AWS Secrets Manager

Store and manage secrets (API keys, passwords).

### 🔹 AWS Artifact

Access compliance reports and agreements.

### 🔹 AWS Control Tower

Set up and govern secure multi-account AWS environment.

### 🔹 AWS Config & AWS Shield/WAF

Config: Compliance monitoring
Shield: DDoS protection
WAF: Web application firewall

---

✅ **These notes are structured for GitHub and job interview prep.** Let me know if you'd like me to generate a Markdown file for GitHub upload or expand examples further.
