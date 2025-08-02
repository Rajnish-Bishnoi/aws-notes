# 📘 AWS Full Notes for Beginners (GitHub Format - Hinglish Explanation)

---

## 🧠 Part 1: AWS Basics

### 🔹 What is AWS?

**AWS (Amazon Web Services)** ek cloud computing platform hai jo Amazon ne banaya hai. Ye more than 200 services provide karta hai jaise ki compute (server), storage, database, AI/ML, networking, etc. Yeh businesses ko scalable, secure aur flexible applications banane me help karta hai.

**Example:** Agar aapko ek website host karni hai, toh aap EC2 aur S3 ka use karke AWS par usse easily deploy kar sakte ho bina khud ka physical server lagaye.

---

### 🔹 What is Cloud Computing?

Cloud computing ka matlab hai ki aap IT resources (jaise ki servers, storage, database) internet ke through use kar sakte ho bina physical infrastructure maintain kiye.

**Example:** Google Drive par aap apne files save karte ho bina kisi pendrive ya hard disk ke.

---

### 🔹 Benefits of Cloud Computing

* 💸 **No upfront cost** – pehle se kuch kharidna nahi padta
* 📈 **Scalability** – zarurat padne par resources badha/sakate ho
* 🚀 **Fast Deployment** – minutes me server ready ho jata hai
* 🌍 **Global Reach** – duniya ke kisi bhi kone me use kar sakte ho
* 🔐 **Secure & Reliable** – high-level security built-in hai
* 📊 **Pay as you go** – jitna use karo utna hi paisa do

---

### 🔹 Cloud Service Models (3 Types)

| Model | Full Form                   | Kya milta hai?                         | AWS Examples      |
| ----- | --------------------------- | -------------------------------------- | ----------------- |
| IaaS  | Infrastructure as a Service | Server, OS, Networking control         | EC2, EBS          |
| PaaS  | Platform as a Service       | Code deploy karo, infra AWS sambhalega | Elastic Beanstalk |
| SaaS  | Software as a Service       | Ready-made software as a service       | WorkMail, Chime   |

---

### 🔹 Cloud Deployment Models

| Model   | Use Case Example                               |
| ------- | ---------------------------------------------- |
| Public  | Sabhi log AWS jaisa public cloud use karte hai |
| Private | Ek specific org ke liye dedicated cloud infra  |
| Hybrid  | Combination of public + private setup          |

---

## 🌍 Part 2: AWS Global Infrastructure

### 🔹 Global Infrastructure kya hoti hai?

AWS ne duniya bhar me data centers bana rakhe hain jise Region, AZ, Edge kehte hain. Iska use hota hai:

* High Availability
* Low Latency
* Disaster Recovery

---

### 🔹 Region kya hai?

Ek **Region** ek physical jagah hoti hai jahan par multiple Availability Zones hoti hain. Har Region independent hota hai.

**Example:** `ap-south-1` = Mumbai Region

---

### 🔹 Availability Zone (AZ)

AZ = Ek ya zyada data centers jo ek region me hote hain. AZs ek dusre se isolate hote hain par fast fiber links se connected hote hain.

**Use:** App ko fault-tolerant banana.

---

### 🔹 Edge Location

Yahan se static content (videos, images) user ke nazdeek se serve kiya jata hai via **CloudFront** (CDN).

**Use Case:** Website image Delhi me ek user ko serve ho Delhi ke Edge Location se, na ki US se.

---

### 🔹 Local Zone

Yeh metro cities ke liye hoti hai jahan low-latency apps chahiye jaise gaming ya video editing.

---

### 🔹 Wavelength Zone

Yeh 5G networks ke liye hai, ultra-low latency apps (IoT, AR/VR) ke liye use hoti hai.

---

## 🔐 Part 3: AWS Security & Compliance

### 🔹 Shared Responsibility Model

AWS aur customer ke beech me security ka kaam divide hota hai:

| Kaun kya karta hai       | AWS | Aap (Customer) |
| ------------------------ | --- | -------------- |
| Physical Hardware        | ✅   | ❌              |
| Network Infrastructure   | ✅   | ❌              |
| OS and Patching (EC2)    | ❌   | ✅              |
| Data Encryption & Backup | ❌   | ✅              |
| IAM & User Management    | ❌   | ✅              |

> AWS "cloud" secure karta hai, aap "cloud me jo rakha hai" uski security karte ho.

---

### 🔹 IAM (Identity and Access Management)

IAM ke through aap users, roles, aur permissions control kar sakte ho.

**Features:**

* Users and groups create karna
* JSON policies likhna for access control
* Roles assign karna (e.g., EC2 role)
* MFA enable karna

**Example:**

```json
{
  "Effect": "Allow",
  "Action": "s3:*",
  "Resource": "*"
}
```

---

### 🔹 KMS (Key Management Service)

Ye service encryption keys banane aur unka control dene ke liye use hoti hai.

* S3, EBS, RDS data encrypt karne ke liye use hoti hai
* Keys rotate aur manage kar sakte ho

---

### 🔹 AWS Shield & AWS WAF

* **Shield:** DDoS (Distributed Denial of Service) attacks se protect karta hai
* **WAF (Web Application Firewall):** Web apps ko SQL injection, XSS jaise attacks se bachata hai

---

### 🔹 AWS GuardDuty & Inspector

* **GuardDuty:** AI aur ML ka use karke suspicious activity detect karta hai
* **Inspector:** EC2 instances me vulnerabilities scan karta hai

---

### 🔹 AWS CloudTrail vs CloudWatch

| Feature    | CloudTrail                  | CloudWatch                      |
| ---------- | --------------------------- | ------------------------------- |
| Focus Area | Logs of API calls           | Metrics, Logs, Alarms           |
| Use Case   | Auditing, Security analysis | Monitoring performance & health |
| Example    | IAM user ne kab kya kiya    | EC2 ka CPU usage kitna hai      |

---

## ⚙️ Part 4: Compute Services

### 🔹 EC2 (Elastic Compute Cloud)

EC2 AWS ka virtual server hai. Aap isme apni required OS, app install kar sakte ho.

**Instance Types:** t2.micro (free tier), t3a.medium, etc.

---

### 🔹 EC2 Pricing Models

| Model     | Description                        |
| --------- | ---------------------------------- |
| On-Demand | Jitna use karo, utna paisa do      |
| Reserved  | Long-term (1 or 3 years) discount  |
| Spot      | Unused capacity cheap me milti hai |

---

### 🔹 AMI (Amazon Machine Image)

Pre-configured template jise use karke EC2 launch hota hai. OS + software pre-installed hota hai.

---

### 🔹 Auto Scaling & Load Balancer

* Auto Scaling = demand ke hisab se instances add/remove karta hai
* Load Balancer = traffic ko evenly distribute karta hai

---

### 🔹 Lambda

Serverless service jisme aap bas code likhte ho, infra AWS manage karta hai.

**Example:** S3 me image upload hone par auto resize karna

---

### 🔹 Elastic Beanstalk

Code deploy karo, AWS infra handle karega – PaaS type ka system hai.

---

## 💾 Part 5: Storage Services

### 🔹 Amazon S3 (Simple Storage Service)

* AWS ka object storage service hai.
* Unlimited data store kar sakte ho.
* Files ko buckets me organize karte hain.

**Use Case:** Website ke images, backup files, log files store karna.

### 🔹 S3 Storage Classes

| Storage Class        | Use Case                          |
| -------------------- | --------------------------------- |
| Standard             | Frequent access files             |
| Intelligent-Tiering  | Auto move between classes         |
| Standard-IA          | Infrequently accessed data        |
| One Zone-IA          | Same as above but 1 AZ only       |
| Glacier              | Archive data (minutes to restore) |
| Glacier Deep Archive | Lowest cost (hours to restore)    |

### 🔹 Bucket Policy vs ACL

* **Bucket Policy:** JSON format me permissions dete ho
* **ACL (Access Control List):** Individual object ya bucket ke liye rights set karte ho

### 🔹 Versioning & Encryption

* Versioning se file ke purane versions recover kar sakte ho
* SSE-S3, SSE-KMS options se encryption milta hai

---

### 🔹 Amazon EBS (Elastic Block Store)

* EC2 instances ke liye hard disk jaisa kaam karta hai
* Block level storage deta hai
* Alag-alag volume types milte hain (gp3, io2, st1...)

### 🔹 Amazon EFS (Elastic File System)

* File level storage
* Multiple EC2 instances me share ho sakta hai

### 🔹 AWS Backup

* S3, EBS, RDS ka centralized backup system

### 🔹 Amazon Glacier

* Long term data archive ke liye
* Bahut hi sasta, lekin restore karne me time lagta hai

---

## 🗃️ Part 6: Database Services

### 🔹 Amazon RDS (Relational Database Service)

* Managed database service
* MySQL, PostgreSQL, Oracle, SQL Server, Aurora support karta hai
* Backup, patching, failover AWS handle karta hai

### 🔹 Amazon Aurora

* MySQL aur PostgreSQL compatible
* AWS ka khud ka optimized RDS engine
* Fast, secure, scalable

### 🔹 Amazon DynamoDB

* NoSQL database
* Key-value or document-based structure
* Serverless, auto-scaling support karta hai

### 🔹 Amazon Redshift

* Data warehouse service
* Analytics aur reporting ke liye optimized
* Petabyte-scale data process karta hai

### 🔹 Amazon ElastiCache

* Redis/Memcached in-memory cache engine
* Performance improve karta hai by reducing DB load

### 🔹 AWS DMS (Database Migration Service)

* Existing databases ko AWS pe migrate karne ke liye use hota hai
* Minimal downtime ke saath data migrate karta hai

---

## 🌐 Part 7: Networking & Content Delivery

### 🔹 VPC (Virtual Private Cloud)

* AWS pe aapka khud ka private network hota hai
* Subnets, route tables, gateways isme banate hain

**Use Case:** Secure apps banani jise public ya private access dena ho

---

### 🔹 Subnet & Route Table

* **Subnet:** VPC ko logical zones me divide karta hai (Public & Private)
* **Route Table:** Network ka traffic kahan jaye, yeh define karta hai

---

### 🔹 IGW vs NAT Gateway

| Component   | Description                               |
| ----------- | ----------------------------------------- |
| IGW         | Internet Gateway – Public subnet ke liye  |
| NAT Gateway | Private subnet se internet access ke liye |

---

### 🔹 Security Group vs NACL

| Feature | Security Group         | NACL                    |
| ------- | ---------------------- | ----------------------- |
| Level   | Instance-level         | Subnet-level            |
| Type    | Stateful (auto return) | Stateless (manual both) |

---

### 🔹 CloudFront (CDN)

* Content ko user ke nazdeek se deliver karta hai (images, video)
* Edge Locations ka use karta hai

---

### 🔹 Global Accelerator

* Application performance aur availability improve karta hai globally
* Static IPs provide karta hai

---

## 📡 Part 8: Monitoring, Logging & Analytics

### 🔹 CloudWatch

* Metrics (CPU, memory), logs aur alarms track karta hai

**Example:** EC2 ka CPU 80% cross ho to alarm bhejna

---

### 🔹 CloudTrail

* AWS API call ka record rakhta hai

**Example:** IAM user ne kab S3 bucket delete kiya, yeh pata chal sakta hai

---

### 🔹 AWS Config

* AWS resources ke configurations track karta hai
* Compliance check karne me help karta hai

---

### 🔹 AWS X-Ray

* Distributed apps ke request ko trace karta hai
* Microservices debug karne me helpful

---

### 🔹 Amazon Kinesis

* Real-time data stream ko process karta hai
* Live logs, clicks, video data ke liye

---

### 🔹 Amazon QuickSight

* BI tool hai data visualize karne ke liye (charts, dashboards)

---

## 🔄 Part 9: Application Integration

### 🔹 Amazon SQS (Simple Queue Service)

* Distributed components ke beech message queue system
* Loose coupling maintain karta hai

---

### 🔹 Amazon SNS (Simple Notification Service)

* Email, SMS, Lambda, HTTP ke through notifications bhejta hai

---

### 🔹 Amazon EventBridge

* App events ko bus ke through route karta hai
* SaaS apps, Lambda, etc. integrate karta hai

---

### 🔹 AWS Step Functions

* Serverless workflows banane ke liye
* Har step ko state machine me define kar sakte ho

---

## 🔧 Part 10: DevOps & Automation

### 🔹 AWS CloudFormation

* Infrastructure as Code
* YAML/JSON file me pura infra define kar sakte ho

---

### 🔹 CodeCommit, CodeBuild, CodeDeploy, CodePipeline

* **CodeCommit** = Git repo
* **CodeBuild** = Code compile/build/test
* **CodeDeploy** = EC2 aur Lambda me deploy karo
* **CodePipeline** = Full CI/CD pipeline

---

### 🔹 OpsWorks

* Chef aur Puppet based configuration management

---

### 🔹 AWS Systems Manager (SSM)

* EC2 manage karna, automate karna, patching, logs sab yaha se
* SSM Agent EC2 me install hota hai

---

## 🧪 Part 11: Identity, Security & Management Tools

### 🔹 AWS Organizations

* Multiple AWS accounts manage karne ke liye ek hierarchy

### 🔹 AWS IAM (Revisited)

* Fine-grained access control for services, resources

### 🔹 AWS SSO (Single Sign-On)

* Multiple accounts aur 3rd party apps me ek hi login se access

### 🔹 AWS Secrets Manager

* Passwords, tokens securely store aur rotate karta hai

### 🔹 AWS Artifact

* Compliance reports jaise SOC, ISO, etc. download kar sakte ho

### 🔹 AWS Control Tower

* Multi-account AWS environment banane aur govern karne ke liye

### 🔹 AWS Config + AWS Shield + WAF

* **Config:** Compliance & resource history tracking
* **Shield:** DDoS protection
* **WAF:** Web application firewall for Layer 7 attacks

---


* 📄 PDF export
* 📁 Markdown file for GitHub
* ❓ 100 Interview Q\&A on AWS
* 🧠 Cheatsheet Summary for revision
