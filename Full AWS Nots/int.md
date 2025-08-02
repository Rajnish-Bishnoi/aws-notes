
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

1. **Why did you choose AWS?**

   * AWS is the global leader in cloud computing, with the widest range of services, strong documentation, and career opportunities. I’ve also worked with it hands-on and appreciate its scalability and automation capabilities.

2. **What was a challenging cloud problem you solved?**

   * In a previous project, an EC2 instance wasn’t accessible due to a misconfigured security group. I traced the issue using VPC Flow Logs and fixed the inbound rule. It helped restore service quickly.

3. **How do you stay up-to-date with AWS?**

   * I follow the AWS Blog, subscribe to AWS YouTube, and regularly explore AWS re\:Invent sessions. I also try new services through the Free Tier.

4. **How do you approach debugging in cloud environments?**

   * I start by checking CloudWatch logs and metrics. Then, I verify networking setups (VPC, routes, SGs) and application logs. I break the issue down layer by layer.

5. **What are your go-to tools in AWS for automation?**

   * AWS CLI, CloudFormation, and sometimes Terraform for IAC. I also use CodePipeline and Lambda functions for automation workflows.

6. **Tell me about a time you worked in a team to solve a cloud issue.**

   * I collaborated with a DevOps engineer to troubleshoot a failed deployment. I handled IAM permissions while he checked container logs. We resolved the issue and implemented a rollback strategy.

7. **Have you handled an on-call or incident situation?**

   * Yes. During an on-call, a load balancer wasn't routing properly. I checked health checks and target groups, found the issue, and rotated the instances. I also documented the fix.

8. **What are your future goals in cloud computing?**

   * I want to become a certified AWS Solutions Architect and contribute to cost-efficient cloud architectures. I'm also exploring AI/ML integrations in AWS.

9. **How do you ensure cloud cost optimization?**

   * By using AWS Cost Explorer, setting budgets, using Auto Scaling, switching to Spot/Reserved instances, and right-sizing resources regularly.

10. **What does cloud security mean to you?**

