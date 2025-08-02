# ☁️ EC2 Userdata (Bootstrap Script)

## 📘 What is Userdata?

**Userdata** is a script that runs **automatically when an EC2 instance is launched**.  
It is used to **automate post-installation tasks** such as:

- Installing software (e.g., Apache, Nginx, Docker)
- Setting up configurations
- Initializing files or environments

> ✅ *Userdata scripts only run ONCE by default (at first boot).*

---

## 📦 What Comes With a New EC2 Instance?

By default, an EC2 instance provides:

- ✅ An **Operating System** (e.g., Amazon Linux, Ubuntu, Windows)
- ✅ Basic **OS-level configuration**

But nothing else is pre-installed or configured.

---

## 🪄 Why Use Userdata?

Using a Userdata script, you can:

- Set up web servers automatically
- Deploy apps during boot
- Configure settings without manual login
- Launch 10s or 100s of pre-configured EC2s at once

🟡 **Also called:** *Bootstrap script*

---

## 🛠️ Sample Use Case: Apache Web Server Setup

```bash
#!/bin/bash
# Example: Install Apache & host a web page

yum update -y
yum install httpd -y
systemctl start httpd
systemctl enable httpd
echo "Hello from EC2 - Apache installed using Userdata!" > /var/www/html/index.html
