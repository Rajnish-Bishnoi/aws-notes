
## 🧠 AWS Interview Prep Boosters

### 📌 Cheat Sheet Summary Table

| AWS Area        | Common Tools/Services  | Purpose                             |
| --------------- | ---------------------- | ----------------------------------- |
| Compute         | EC2, Lambda, Beanstalk | Run apps and servers                |
| Storage         | S3, EBS, EFS           | Store data, files, backups          |
| Database        | RDS, DynamoDB, Aurora  | Manage structured/unstructured data |
| Networking      | VPC, Route 53, NAT     | Network setup and traffic routing   |
| Security        | IAM, KMS, WAF          | Permissions, encryption, protection |
| Monitoring      | CloudWatch, CloudTrail | Logs, metrics, activity tracking    |
| Developer Tools | CodeDeploy, CLI, SDK   | Automate, build, deploy apps        |

---

### 📂 AWS Architecture Scenarios (For Diagram/Revision)

1. **Basic Web Hosting Setup**: EC2 + S3 + Route53 + IAM + VPC
2. **High Availability Architecture**: EC2 (Multi-AZ) + Load Balancer + Auto Scaling + RDS (Multi-AZ)
3. **Serverless App Architecture**: Lambda + API Gateway + DynamoDB + S3 + CloudWatch
4. **Hybrid Network Setup**: On-prem + VPN/Direct Connect + VPC + NAT Gateway

(📌 You can draw these in Lucidchart, draw\.io or embed in GitHub using Mermaid or PlantUML)

---

### 🔐 Common Port Numbers Cheat Sheet

| Protocol   | Port | Description            |
| ---------- | ---- | ---------------------- |
| SSH        | 22   | Secure shell access    |
| HTTP       | 80   | Web traffic            |
| HTTPS      | 443  | Secure web traffic     |
| RDP        | 3389 | Windows Remote Desktop |
| MySQL      | 3306 | RDS MySQL access       |
| PostgreSQL | 5432 | RDS PostgreSQL         |
| DNS        | 53   | Domain Resolution      |

---

### 🧠 10 Real-World Scenario-Based Interview Questions

1. **Q: EC2 can’t connect to internet, what could be the cause?**

   * Check route table, subnet (public/private), internet/NAT gateway, and security group.

2. **Q: S3 access denied – why?**

   * Might be due to IAM policy, S3 bucket policy, or lack of ACL permissions.

3. **Q: Application hosted on EC2 is slow – how to debug?**

   * Use CloudWatch metrics, check CPU usage, add Auto Scaling, or optimize instance type.

4. **Q: Lambda giving timeout error?**

   * Increase timeout in config, check dependencies or network timeouts.

5. **Q: How to secure EC2?**

   * Use security groups, limit SSH via IP, use IAM roles not access keys.

6. **Q: RDS is not connecting from EC2. Why?**

   * Ensure RDS is in same VPC, SG allows inbound, subnet is public/private accordingly.

7. **Q: My app needs fast access to session data. What to use?**

   * Amazon ElastiCache (Redis/Memcached)

8. **Q: Lambda needs DB access but has no credentials. Solution?**

   * Assign IAM Role to Lambda with necessary DB access policies.

9. **Q: How to audit all changes done in AWS account?**

   * Use AWS CloudTrail.

10. **Q: How to recover data if S3 object is deleted accidentally?**

* Enable S3 versioning and lifecycle policies.

---

### 💬 HR/Behavioral Interview Questions for Cloud Roles

1. Why did you choose AWS?
2. What was a challenging cloud problem you solved?
3. How do you stay up-to-date with AWS?
4. How do you approach debugging in cloud environments?
5. What are your go-to tools in AWS for automation?

---
