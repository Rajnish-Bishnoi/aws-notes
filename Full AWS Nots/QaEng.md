# 📘 AWS Interview Questions and Answers (English Only)

This list contains 100 commonly asked AWS interview questions with concise English answers — perfect for job interviews and GitHub revision.

---

## 🔰 Basic Level (1–20)

1. **What is AWS?**

   * AWS is a cloud computing platform offering 200+ services like compute, storage, and networking.

2. **What is EC2?**

   * EC2 provides resizable virtual servers (instances) in the cloud.

3. **What is S3?**

   * S3 is an object storage service for storing files with high durability.

4. **What is IAM?**

   * IAM allows you to manage users, roles, and permissions securely.

5. **What is VPC?**

   * A VPC is your own private cloud network in AWS.

6. **Difference between Public and Private Subnet?**

   * Public has internet access; private does not.

7. **What is CloudFront?**

   * A CDN that delivers content from the nearest edge location.

8. **What is AMI in EC2?**

   * An Amazon Machine Image is a template for launching EC2 instances.

9. **What does Auto Scaling do?**

   * Automatically adds/removes EC2 instances based on demand.

10. **What is a Load Balancer?**

    * Distributes incoming traffic across multiple instances.

11. **What is AWS Lambda?**

    * A serverless compute service to run code without provisioning servers.

12. **What is RDS?**

    * A managed relational database service supporting engines like MySQL and PostgreSQL.

13. **Difference between DynamoDB and RDS?**

    * DynamoDB is NoSQL; RDS is a relational database.

14. **What is a Route Table?**

    * Determines how traffic is directed within a VPC.

15. **What is KMS?**

    * AWS Key Management Service to manage encryption keys.

16. **CloudTrail vs CloudWatch?**

    * CloudTrail logs API activity; CloudWatch monitors resources and logs.

17. **Security Group vs NACL?**

    * Security Group works at instance level; NACL at subnet level.

18. **How is AWS billing handled?**

    * Pay-as-you-go pricing — you pay only for what you use.

19. **What is AWS Free Tier?**

    * A 12-month free trial of many AWS services like EC2 and S3.

20. **What is an Availability Zone?**

    * A data center in an AWS region designed for fault tolerance.

---

## 🔰 Intermediate Level (21–60)

21. **What is Elastic Beanstalk?**

    * A platform to deploy and manage web apps easily.

22. **What is CloudFormation?**

    * A service to define infrastructure using code (YAML/JSON).

23. **What does CloudWatch Logs capture?**

    * Application, system, and custom logs.

24. **What does CloudTrail monitor?**

    * Records API activity across AWS services.

25. **Global Accelerator vs CloudFront?**

    * CloudFront for content delivery; Global Accelerator for TCP/UDP app routing.

26. **What is a Spot Instance?**

    * Cheap EC2 capacity available temporarily; can be terminated.

27. **Benefits of Reserved Instances?**

    * Provide discounts for long-term commitments.

28. **What is Route 53?**

    * A scalable DNS and domain registration service.

29. **Difference: Multi-AZ vs Read Replica?**

    * Multi-AZ is for failover; Read Replica is for scaling reads.

30. **What is an Edge Location in CloudFront?**

    * A location that caches content closer to users.

31. **Types of Elastic Load Balancer?**

    * Application (ALB), Network (NLB), Gateway (GLB).

32. **What is EC2 Termination Protection?**

    * Prevents accidental deletion of instances.

33. **What is AWS CLI?**

    * Command-line interface to interact with AWS.

34. **What is VPC Peering?**

    * Connects two VPCs for private traffic sharing.

35. **Types of EBS Volumes?**

    * gp3, io1, st1, sc1 — based on performance needs.

36. **EFS vs EBS?**

    * EFS is shared file storage; EBS is block storage.

37. **What is a Lifecycle Policy in S3?**

    * Moves or deletes objects automatically after a set time.

38. **What is the Well-Architected Framework?**

    * AWS best practices grouped into six pillars (e.g., security, cost).

39. **Example of IAM Policy?**

    ```json
    {
      "Effect": "Allow",
      "Action": "s3:*",
      "Resource": "*"
    }
    ```

40. **NAT Gateway vs NAT Instance?**

    * Gateway is managed; Instance is user-maintained.

41. **What is AWS Snowball?**

    * A device to transfer large data volumes to AWS.

42. **What is Amazon Redshift?**

    * A fast data warehousing solution.

43. **Use of Elasticache?**

    * Caches data to reduce DB load and latency.

44. **What is a Transit Gateway?**

    * Connects multiple VPCs and on-prem networks.

45. **What does AWS Artifact provide?**

    * Access to compliance and audit reports.

46. **Benefit of Systems Manager?**

    * Centralized management for EC2, patching, automation.

47. **What is AWS Cloud9?**

    * A browser-based IDE for coding in AWS.

48. **What is an Elastic IP?**

    * A static IP address for EC2.

49. **What is AWS Outposts?**

    * AWS infrastructure for on-premises deployment.

50. **What does GuardDuty detect?**

    * Malicious or suspicious activity using machine learning.

---

## 🔰 Advanced Level (51–100)

51. **What is Aurora?**

    * A high-performance, MySQL/PostgreSQL-compatible database.

52. **What is DynamoDB capacity mode?**

    * On-demand or provisioned throughput for read/write operations.

53. **What are Global Tables in DynamoDB?**

    * Replicates tables across multiple regions automatically.

54. **What is RDS Multi-AZ deployment?**

    * Provides automatic failover by syncing to standby in another AZ.

55. **What is a Read Replica in RDS?**

    * A copy used for read-only traffic to reduce master load.

56. **What are VPC Endpoints?**

    * Enable private connection to AWS services without internet.

57. **What is AWS Trusted Advisor?**

    * Provides recommendations for cost, security, and performance.

58. **What is AWS Cost Explorer?**

    * A tool to visualize and analyze usage and billing data.

59. **S3 Encryption types?**

    * SSE-S3, SSE-KMS, SSE-C, Client-Side.

60. **IAM Policy vs SCP?**

    * IAM for users; SCP for controlling AWS accounts.

61. **What is WAF?**

    * Web Application Firewall to block malicious traffic.

62. **What is API Gateway?**

    * Creates and manages APIs connected to services like Lambda.

63. **What is AWS Batch?**

    * A managed batch computing service.

64. **What is a Spot Fleet?**

    * A group of Spot Instances to meet target capacity.

65. **What is AWS Marketplace?**

    * A digital catalog for third-party software and AMIs.

66. **What is AWS License Manager?**

    * Track and manage software licenses on AWS.

67. **What is Amazon FSx?**

    * Managed file systems like FSx for Windows or Lustre.

68. **What are Lifecycle Hooks?**

    * Run custom actions during Auto Scaling events.

69. **Launch Template vs Launch Configuration?**

    * Templates are newer and more flexible than configurations.

70. **What is AWS QuickSight?**

    * A BI tool to visualize data through dashboards.

71. **What is AWS Backup?**

    * A central service to automate backups across services.

72. **What is AWS CloudHSM?**

    * Hardware Security Module for encryption key management.

73. **What is AWS Elastic Transcoder?**

    * A media transcoding service for converting video formats.

74. **Difference between Pinpoint and SES?**

    * SES for email only; Pinpoint for email, SMS, and push campaigns.

75. **What is a State Machine in Step Functions?**

    * Defines a workflow using states and transitions.

76. **What is AWS Glue?**

    * A serverless ETL service for preparing data.

77. **What is Athena?**

    * Query S3 data using standard SQL.

78. **What is AWS Snowmobile?**

    * A physical truck to move exabyte-scale data to AWS.

79. **What is AWS Inspector?**

    * Analyzes EC2 for security vulnerabilities.

80. **Parameter Store vs Secrets Manager?**

    * Secrets Manager adds auto-rotation and better security.

81. **What is TCO Calculator?**

    * Compares AWS cost to on-premises infrastructure.

82. **What is AWS Service Catalog?**

    * Offers approved resources and templates for provisioning.

83. **What is AWS CloudShell?**

    * A browser-based shell with pre-configured AWS CLI.

84. **What is an Elastic Network Interface (ENI)?**

    * A virtual network card for EC2 instances.

85. **What is EC2 Hibernate?**

    * Saves RAM contents and resumes instance later.

86. **What is included in AWS Free Tier?**

    * Free access to EC2, S3, Lambda, and other services for 12 months.

87. **Use of S3 Signed URLs?**

    * Provide temporary, restricted access to S3 objects.

88. **Resilience pillars in AWS?**

    * Fault tolerance, high availability, disaster recovery.

89. **How to configure AWS CLI?**

    * Use `aws configure` to set access keys, region, output format.

90. **Best service for real-time monitoring?**

    * Amazon CloudWatch.

91. **What is ECR?**

    * A Docker container registry service by AWS.

92. **Difference between ECS and Fargate?**

    * ECS requires EC2 or Fargate. Fargate is serverless for containers.

93. **What is Step Scaling?**

    * Adjusts capacity in predefined steps based on metrics.

94. **What is Target Tracking Scaling?**

    * Maintains a target metric like CPU usage automatically.

95. **What is AWS Config?**

    * Tracks configuration changes in AWS resources.

96. **What is Shield?**

    * AWS DDoS protection service.

97. **What is GuardDuty?**

    * Threat detection using machine learning.

98. **What is Detective?**

    * Investigate security findings and visualize patterns.

99. **What is Amazon Macie?**

    * Scans S3 buckets for sensitive data like PII.

100. **What is Control Tower?**

     * Sets up and governs a multi-account AWS environment.

🎯 **All 100 AWS Interview Questions and Answers Completed in English!**
