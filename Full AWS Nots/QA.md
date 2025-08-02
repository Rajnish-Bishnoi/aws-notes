

## ❓ AWS Interview Questions 
### 🔰 Basic Level (1–20)

1. **Q: AWS kya hai?**
   A: AWS ek cloud platform hai jo more than 200 services provide karta hai for compute, storage, database, machine learning, etc.

2. **Q: EC2 kya karta hai?**
   A: EC2 ek virtual server hai jisme aap apna OS aur apps install karke use kar sakte ho.

3. **Q: S3 kya hai?**
   A: S3 ek object storage service hai jisme aap unlimited files store kar sakte ho.

4. **Q: IAM ka use kya hai?**
   A: IAM se aap users, roles aur permissions control kar sakte ho securely.

5. **Q: VPC kya hota hai?**
   A: VPC aapka private cloud network hota hai AWS pe jisme subnets, routes define karte ho.

6. **Q: Public aur Private Subnet me farak?**
   A: Public subnet ka internet se direct access hota hai, private ka nahi.

7. **Q: CloudFront ka kya use hai?**
   A: CloudFront ek CDN hai jo content user ke closest location se serve karta hai.

8. **Q: EC2 me AMI kya hoti hai?**
   A: AMI ek template hai jisme OS aur preinstalled software hote hain.

9. **Q: Auto Scaling kya karta hai?**
   A: Auto Scaling demand ke according EC2 instances add/remove karta hai.

10. **Q: Load Balancer kya karta hai?**
    A: Incoming traffic ko multiple instances me distribute karta hai.

11. **Q: Lambda kya karta hai?**
    A: Serverless code chalata hai bina infrastructure manage kiye.

12. **Q: RDS kya hai?**
    A: RDS managed database service hai jo multiple engines support karta hai.

13. **Q: DynamoDB vs RDS?**
    A: DynamoDB NoSQL hai, RDS relational database hai.

14. **Q: Route Table kya karti hai?**
    A: Ye define karti hai ki traffic kahan forward hoga subnet se.

15. **Q: KMS kya hai?**
    A: AWS Key Management Service hai for managing encryption keys.

16. **Q: CloudTrail vs CloudWatch?**
    A: CloudTrail API logs deta hai, CloudWatch metrics aur alarms.

17. **Q: Security Group vs NACL?**
    A: Security Group instance-level firewall hai, NACL subnet-level.

18. **Q: AWS pe billing kaise hoti hai?**
    A: Pay-as-you-go model – jitna use karo utna paisa do.

19. **Q: AWS Free Tier kya hai?**
    A: AWS free tier kuch services 12 months ke liye free deta hai like EC2 t2.micro.

20. **Q: Availability Zone kya hoti hai?**
    A: AZ ek region ke andar independent data centers hote hain.

### 🔰 Intermediate Level (21–60)

21. **Q: Elastic Beanstalk kya karta hai?**
    A: Code deploy karne ka PaaS service hai – infra AWS handle karta hai.

22. **Q: CloudFormation kya hai?**
    A: Infrastructure as code service – YAML/JSON file se pura setup define kar sakte ho.

23. **Q: CloudWatch Logs kya record karta hai?**
    A: Application logs, system logs, custom logs track karta hai.

24. **Q: CloudTrail kya monitor karta hai?**
    A: AWS services par hone wale API calls track karta hai.

25. **Q: Global Accelerator vs CloudFront?**
    A: CloudFront static content deliver karta hai, Global Accelerator TCP/UDP apps ko optimize karta hai.

26. **Q: Spot Instance kya hoti hai?**
    A: AWS ki bachi hui EC2 capacity – sasti hoti hai but kabhi bhi terminate ho sakti hai.

27. **Q: Reserved Instances me kya benefit hai?**
    A: 1 ya 3 saal ka commitment dene par heavy discount milta hai.

28. **Q: Route 53 kya hai?**
    A: AWS ka scalable DNS service.

29. **Q: Multi-AZ aur Read Replica me farak?**
    A: Multi-AZ backup ke liye hai, Read Replica read scaling ke liye.

30. **Q: CloudFront Edge Location kya karta hai?**
    A: User ke nearest point se content serve karta hai.

31. **Q: Elastic Load Balancer ke types?**
    A: Application LB, Network LB, Gateway LB

32. **Q: EC2 instance ka termination protection kya hota hai?**
    A: Accidental termination se bachane ke liye protection.

33. **Q: AWS CLI kya hai?**
    A: Command-line tool se AWS services ko manage karne ka tareeka.

34. **Q: VPC Peering kya karta hai?**
    A: 2 VPCs ke beech private communication allow karta hai.

35. **Q: EBS Volume Types?**
    A: gp3, io1, sc1, st1 – use-case ke hisab se.

36. **Q: EFS vs EBS?**
    A: EFS file-level storage hai, EBS block-level.

37. **Q: Data lifecycle policy kya hai S3 me?**
    A: Data ko auto delete ya lower storage class me move karta hai.

38. **Q: AWS Well-Architected Framework kya hai?**
    A: Best practices ka guideline in 6 pillars: security, cost, etc.

39. **Q: IAM Policy JSON ka ek example?**
    A:

    ```json
    {
      "Effect": "Allow",
      "Action": "s3:*",
      "Resource": "*"
    }
    ```

40. **Q: NAT Gateway aur NAT Instance me farak?**
    A: NAT Gateway managed service hai, Instance manually setup karna padta hai.

41. **Q: Snowball kya karta hai?**
    A: Terabytes data ko migrate karne ke liye physical device.

42. **Q: Redshift kya hai?**
    A: AWS ka data warehouse service.

43. **Q: Elasticache ka use kya hai?**
    A: DB queries ka load kam karne ke liye in-memory cache.

44. **Q: Transit Gateway kya karta hai?**
    A: Multiple VPCs aur on-premise networks ko connect karta hai.

45. **Q: AWS Artifact kya deta hai?**
    A: Compliance aur audit reports.

46. **Q: Systems Manager ka fayda?**
    A: EC2 monitoring, automation, patching sab ek jagah se.

47. **Q: Cloud9 kya hai?**
    A: Browser-based IDE for coding directly on AWS.

48. **Q: Elastic IP kya hai?**
    A: Static IP jo EC2 instance ke liye assign hoti hai.

49. **Q: AWS Outposts kya hai?**
    A: AWS hardware jo on-premise location pe use hota hai.

50. **Q: GuardDuty kya detect karta hai?**
    A: Suspicious activities, threats using ML.

51–60 continue on next update...

---

### 🔰 Advanced Level (61–100)

61. **Q: Aurora vs RDS kya farak hai?**
    A: Aurora AWS ka khud ka DB engine hai – MySQL compatible, faster and more scalable than standard RDS.

62. **Q: DynamoDB read/write capacity kya hoti hai?**
    A: Provisioned ya On-demand mode hota hai – jitni read/write capacity chahiye utni define kar sakte ho.

63. **Q: Global Tables DynamoDB me kaise kaam karti hain?**
    A: Cross-region replication provide karti hai – ek hi data multiple region me sync rehta hai.

64. **Q: RDS Multi-AZ Deployment ka benefit?**
    A: High availability and automatic failover – ek AZ fail ho to doosri AZ se service continue.

65. **Q: Read Replica ka use kya hai?**
    A: Read-only traffic ke liye use hota hai – master DB ka load kam karta hai.

66. **Q: VPC Endpoints kya karte hain?**
    A: S3, DynamoDB jaise AWS services ko VPC ke andar se access karne dete hain without internet.

67. **Q: AWS Trusted Advisor kya karta hai?**
    A: AWS account ke liye security, performance, cost optimization recommendations deta hai.

68. **Q: AWS Cost Explorer kya hai?**
    A: Billing aur usage analyze karne ka tool.

69. **Q: S3 Encryption types kya hain?**
    A: SSE-S3, SSE-KMS, SSE-C aur Client-side encryption.

70. **Q: IAM Policy vs SCP (Service Control Policy)?**
    A: IAM Policy individual users ke liye, SCP pure AWS account ya OU pe lagti hai.

71. **Q: WAF rule me kya define karte hain?**
    A: Conditions jaise IP, query string, header jaise filters.

72. **Q: API Gateway kya karta hai?**
    A: REST/HTTP APIs ke liye entry point provide karta hai, Lambda ya backend connect karta hai.

73. **Q: AWS Batch kya karta hai?**
    A: Large-scale batch processing ke liye managed service.

74. **Q: EC2 Spot Fleet kya hai?**
    A: Multiple spot instances ko combine karke ek fleet me run karna.

75. **Q: AWS Marketplace kya hai?**
    A: 3rd party tools, AMIs aur solutions kharidne ke liye platform.

76. **Q: AWS License Manager kya karta hai?**
    A: Software license compliance aur tracking ke liye.

77. **Q: FSx service kya hai?**
    A: Windows File Server ya Lustre file system ka managed version.

78. **Q: Lifecycle hook kya hota hai Auto Scaling me?**
    A: Custom actions run karna before/after instance terminate ya start.

79. **Q: Launch Template vs Launch Configuration?**
    A: Launch Template newer version hai – zyada flexible aur reusable hai.

80. **Q: AWS QuickSight kya karta hai?**
    A: BI tool – charts, dashboards for data visualization.

81. **Q: AWS Backup service ka use?**
    A: Centralized backup for EBS, RDS, DynamoDB etc.

82. **Q: CloudHSM kya hai?**
    A: Dedicated hardware module for managing crypto keys.

83. **Q: Elastic Transcoder kya karta hai?**
    A: Videos ko different formats me convert karta hai.

84. **Q: Pinpoint aur SES me farak?**
    A: SES email service hai, Pinpoint targeted marketing ke liye (SMS, push, email).

85. **Q: Step Functions me state machine kya hoti hai?**
    A: Har step ka defined workflow jise visualize kar sakte ho.

86. **Q: AWS Glue kya karta hai?**
    A: ETL (Extract, Transform, Load) data ke liye serverless tool.

87. **Q: Athena kya hai?**
    A: S3 me stored data ko SQL ke through query karne ka tool.

88. **Q: Snowmobile kya hai?**
    A: Exabyte scale data transfer ke liye AWS ka truck.

89. **Q: AWS Inspector kya scan karta hai?**
    A: EC2 instances ke security vulnerabilities.

90. **Q: Parameter Store vs Secrets Manager?**
    A: Secrets Manager rotate bhi karta hai – zyada secure hai.

91. **Q: TCO Calculator kya karta hai?**
    A: On-premise vs AWS ka total cost compare karta hai.

92. **Q: AWS Service Catalog ka use kya hai?**
    A: Pre-approved resources aur apps ko control me rakhna.

93. **Q: AWS CloudShell kya hai?**
    A: Browser me built-in CLI shell with pre-configured credentials.

94. **Q: ENI (Elastic Network Interface) kya hai?**
    A: VPC ke andar virtual network card for EC2.

95. **Q: EC2 Hibernate feature kya karta hai?**
    A: RAM me loaded data save karke instance stop karta hai – fast resume ke liye.

96. **Q: AWS Free Tier me kya milta hai?**
    A: 12 months ke liye free services – EC2, S3, Lambda etc.

97. **Q: S3 Signed URLs ka use kya hai?**
    A: Temporary time-limited access to objects.

98. **Q: AWS Resilience ke pillars kya hain?**
    A: Fault tolerance, high availability, disaster recovery.

99. **Q: AWS CLI configure kaise karte ho?**
    A: `aws configure` command se access key, region set karte ho.

100. **Q: Real-time monitoring best service?**
     A: CloudWatch – for metrics, logs and alarms.

