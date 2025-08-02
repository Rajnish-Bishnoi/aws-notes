# EC2 (Elastic Compute Cloud) - Beginner Friendly Notes

## Introduction to Amazon EC2:

1. **Amazon Elastic Compute Cloud (EC2)** is a web service that provides resizable compute capacity in the cloud.
2. It allows you to create and manage **virtual servers**, known as **instances**, to run your applications.
3. An **instance** is a virtual server in the cloud that can host your software or services.
4. EC2 was **launched by AWS in 2006**.
5. With EC2, you're essentially **creating Virtual Machines (VMs) in the cloud**.
6. Each **instance type** offers different compute, memory, and storage capacities to suit various workload requirements.
7. EC2 stands for **Elastic Compute Cloud** — the term "elastic" means you can scale resources up or down as needed.
8. You can choose any **Operating System** for your instance (Linux, Windows, etc.).
9. You can run various applications on EC2 such as **databases, websites, and more**.
10. EC2 falls under the **IaaS (Infrastructure as a Service)** category in cloud computing.
11. You can customize compute capacity: **CPU, RAM, storage, and network** configurations.
12. You can **launch as many or as few EC2 instances** as needed.
13. EC2 instances are **region-specific** (not global), so you must select a region.
14. Under the **Free Tier**, you can run an EC2 Linux or Windows instance **for up to 750 hours per month**.

---

## EC2 Instance Launch Requirements:

To create an EC2 instance, the following components are required:

1. **AMI (Amazon Machine Image):**

   * A template with the OS and software configuration.
   * Example: *Amazon Linux 2023 AMI, Ubuntu 20.04, Windows Server 2022*.

2. **Instance Type:**

   * Defines CPU, RAM, storage, and network power.
   * Example: *t2.micro (Free Tier), t3.medium (general purpose)*.

3. **Security Group:**

   * Acts as a virtual firewall to control traffic.
   * Example: Allow port 22 for SSH, port 80 for HTTP.

4. **Key Pair:**

   * Used to securely connect (SSH) to your Linux instance.
   * Example: *raj-key.pem* used while connecting via terminal.

5. **Storage:**

   * Choose between **EBS (Elastic Block Store)** or **Instance Store**.
   * Example: *8 GB gp2 EBS volume attached at /dev/xvda*.

6. **Network Settings:**

   * Choose **VPC, subnet, and IP addressing**.
   * Example: *Default VPC with public subnet and auto-assigned public IP*.

7. **Tags (Optional):**

   * Helps in organizing and identifying instances.
   * Example: *Name = WebServer-1, Project = AWS-Lab*.

---

## Practical Lab Examples:

### Linux Instance Lab:

1. **Launch a Linux EC2 instance in the Mumbai Region**

   * AMI: Amazon Linux 2023
   * Instance type: t2.micro (Free Tier eligible)

2. **Connect using EC2 Instance Connect** (from AWS console):

```bash
# Create two files:
echo "This is input file" > input.txt
echo "This is output file" > output.txt
```

3. **Connect using MobaXterm**:

   * Use `.pem` file to SSH into instance

```bash
ls
# You should see: input.txt and output.txt
```

### Windows Instance Lab:

1. **Launch a Windows EC2 instance in the Mumbai Region**

   * AMI: Microsoft Windows Server 2022 Base
   * Instance type: t2.micro

2. **Connect using RDP (Remote Desktop Protocol)**

   * Decrypt password using your `.pem` key

3. **Inside the instance, open Notepad and create files**:

   * result.txt → type: "This is result file"
   * answer.txt → type: "This is answer file"

4. **Verify files by browsing through File Explorer**

---

> ✅ These EC2 labs help you understand how to launch, connect, and work with AWS instances using Linux and Windows operating systems.

Let me know if you want to add images, links, or step-by-step screenshots!
