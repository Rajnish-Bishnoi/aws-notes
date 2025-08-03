# 🧠 Advanced Linux Commands

| Command / Keyword    | Full Form / Meaning                         | Example                                          |
|----------------------|----------------------------------------------|--------------------------------------------------|
| `#!/bin/bash`        | **Shebang** – defines shell for script       | `#!/bin/bash` at the top of a `.sh` file        |
| `echo`               | **Echo** – display output                    | `echo "Hello, Cloud!"`                          |
| `read`               | **Read** – accept user input                 | `read name` → `echo "Hi, $name"`                |
| `if / else / fi`     | **If-Else-Fi** – conditional branching       | `if [ -f file.txt ]; then echo yes; fi`         |
| `for / do / done`    | **For loop** – repeat code                   | `for i in {1..3}; do echo $i; done`             |
| `while / do / done`  | **While loop** – loop while condition true   | `while true; do echo hi; sleep 1; done`         |
| `case / esac`        | **Case statement** – switch-like logic       | `case $1 in start) echo start;; esac`           |
| `function`           | **Function** – reusable block of code        | `function greet { echo "Hi $1"; }; greet Dev`   |
| `exit`               | **Exit** – stop script with status           | `exit 0`                                        |
| `cron / crontab`     | **Cron Table** – scheduled tasks             | `crontab -e` → `*/5 * * * * /script.sh`         |

---

## 🛠️ System Management

| Command                    | Full Form / Meaning                           | Example                                 |
|----------------------------|-----------------------------------------------|------------------------------------------|
| `adduser`                  | **Add User** – create a new user              | `sudo adduser devuser`                   |
| `passwd`                   | **Password** – change user password           | `sudo passwd devuser`                    |
| `usermod -aG`              | **User Modify Add to Group**                  | `sudo usermod -aG sudo devuser`          |
| `chmod`                    | **Change Mode** – set file permissions        | `chmod 755 script.sh`                    |
| `chown`                    | **Change Owner** – change file ownership      | `chown user:group file.txt`              |
| `umask`                    | **User Mask** – default file permission mask  | `umask 022`                              |

---

## 🧠 Process & Resource Management

| Command        | Full Form / Meaning                          | Example                                     |
|----------------|----------------------------------------------|---------------------------------------------|
| `top`          | **Table of Processes** – live view           | `top`                                       |
| `htop`         | **Human Top** – interactive process viewer   | `sudo yum install htop && htop`             |
| `ps aux`       | **Process Status** – show all processes      | `ps aux | grep nginx`                       |
| `kill`         | **Kill Process** – terminate by PID          | `kill 1234`                                 |
| `jobs`         | **Job List** – list background jobs          | `sleep 100 & jobs`                          |
| `bg / fg`      | **Background / Foreground**                  | `fg %1`                                     |
| `nice / renice`| **Set process priority**                     | `nice -n 10 script.sh`                      |

---

## 💾 Disk & File System

| Command              | Full Form / Meaning                       | Example                                        |
|----------------------|--------------------------------------------|------------------------------------------------|
| `df -h`              | **Disk Free (Human-readable)**            | `df -h`                                        |
| `du -sh *`           | **Disk Usage Summary (Human-readable)**   | `du -sh *`                                     |
| `mount / umount`     | **Mount / Unmount** file systems          | `mount /dev/xvdf /mnt`                         |
| `lsblk`              | **List Block Devices**                    | `lsblk`                                        |
| `fdisk -l`           | **Format Disk (List partitions)**         | `sudo fdisk -l`                                |
| `mkfs.ext4`          | **Make File System (ext4 format)**        | `mkfs.ext4 /dev/xvdf`                          |

---

## 🔒 Permissions & Security

| Command        | Full Form / Meaning                          | Example                                        |
|----------------|----------------------------------------------|------------------------------------------------|
| `chmod`        | **Change Mode** – file permissions           | `chmod 644 notes.txt`                          |
| `chown`        | **Change Owner** – file ownership            | `sudo chown ec2-user:ec2-user test.log`        |
| `ls -l`        | **List Long** – show file details            | `ls -l`                                        |
| `umask`        | **User Mask** – new file permission default  | `umask 002`                                    |
| `sudo visudo`  | **Visual Sudo** – safely edit sudo rules     | `sudo visudo`                                  |

---

## 🧾 Log & Service Inspection

| Command                        | Full Form / Meaning                     | Example                                    |
|--------------------------------|------------------------------------------|--------------------------------------------|
| `journalctl`                   | **Journal Control** – view system logs  | `journalctl -u sshd`                        |
| `tail -f`                      | **Follow File** – show live log         | `tail -f /var/log/syslog`                   |
| `systemctl status`            | **System Control – Status**             | `systemctl status apache2`                  |
| `systemctl start / stop`      | **Start / Stop service**                | `sudo systemctl start nginx`                |
| `systemctl enable`            | **Enable service on boot**              | `sudo systemctl enable nginx`               |

---

## 📋 Quick Tips

| Command            | Full Form / Meaning                          | Example                          |
|--------------------|----------------------------------------------|----------------------------------|
| `man <command>`    | **Manual** – help guide for commands         | `man ls`                         |
| `command --help`   | Show help options for any command            | `ps --help`                      |
