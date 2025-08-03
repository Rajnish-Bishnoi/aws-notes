# 🧠 Advanced Linux Commands

| Command / Keyword    | Full Form / Meaning                   | Example                                  |
|----------------------|----------------------------------------|-------------------------------------------|
| `#!/bin/bash`        | Shebang (defines Bash shell)          | `#!/bin/bash`                             |
| `echo`               | Echo (print text or variable)         | `echo "Hello, world!"`                    |
| `read`               | Read (user input)                     | `read name` → `echo "Hi, $name"`          |
| `if / else / fi`     | Conditional branching                 | `if [ -f file.txt ]; then echo yes; fi`   |
| `for / do / done`    | Looping                              | `for i in {1..3}; do echo "Item $i"; done`|
| `while / do / done`  | Loop while condition true             | `count=1; while [ $count -le 3 ]; do echo $count; ((count++)); done` |
| `case / esac`        | Multi-branch conditional              | `case $1 in start) echo "Start";; *) echo "Other";; esac` |
| `function`           | Define reusable function              | `function greet { echo "Hello, $1"; } greet Joe` |
| `exit`               | Exit script with status code          | `exit 0`                                  |
| `cron`, `crontab -e` | Schedule recurring tasks              | `*/5 * * * * /home/ec2-user/script.sh`    |

---

## 🛠️ System Management

| Command                        | Meaning                                     | Example                                            |
|-------------------------------|---------------------------------------------|----------------------------------------------------|
| `adduser <name>`              | Add User                                    | `sudo adduser alice`                                |
| `passwd <user>`               | Change user password                        | `sudo passwd alice`                                 |
| `usermod -aG <group> <user>`  | Add user to group                           | `sudo usermod -aG sudo alice`                       |
| `chmod 755 <file>`            | Change Mode (permissions)                   | `chmod 755 script.sh`                               |
| `chown user:group <file>`     | Change Owner & Group                        | `sudo chown alice:dev file.txt`                     |
| `umask`                       | User Mask (default permission)              | `umask 022`                                         |

---

## 🧠 Process & Resource Management

| Command            | Meaning                                  | Example                                          |
|--------------------|-------------------------------------------|--------------------------------------------------|
| `top`              | Live process monitoring                   | `top`                                            |
| `htop`             | Interactive process viewer                | `sudo yum install htop && htop`                 |
| `ps aux`           | Show all running processes                | `ps aux | grep java`                             |
| `kill <PID>`       | Terminate a process by PID                | `kill 1234`                                       |
| `jobs`             | List background jobs                      | `sleep 100 & jobs`                                |
| `bg`, `fg`         | Background or foreground control          | `jobs; bg %1; fg %1`                              |
| `nice`, `renice`   | Set/change process priority               | `nice -n 10 myscript.sh` / `renice +5 -p 1234`     |

---

## 💾 Disk & File System

| Command               | Meaning                                | Example                                          |
|------------------------|-----------------------------------------|--------------------------------------------------|
| `df -h`                | Disk Free (human-readable)             | `df -h`                                           |
| `du -sh *`             | Disk Usage summary                    | `du -sh *`                                        |
| `mount / umount`       | Mount or unmount FS                    | `sudo mount /dev/xvdf /mnt/data; sudo umount /mnt/data` |
| `lsblk`                | List Block Devices                     | `lsblk`                                           |
| `fdisk -l`             | List disk partitions                   | `sudo fdisk -l`                                   |
| `mkfs.ext4 /dev/xvdf`  | Make ext4 filesystem                   | `sudo mkfs.ext4 /dev/xvdf`                        |

---

## 🔒 Permissions & Security

| Command         | Meaning                                  | Example                                        |
|------------------|------------------------------------------|------------------------------------------------|
| `chmod`          | Change file permissions                  | `chmod 644 file.txt`                            |
| `chown`          | Change file ownership                    | `sudo chown alice:dev file.txt`                 |
| `ls -l`          | List long format (show permissions)      | `ls -l script.sh`                               |
| `umask`          | Set default permission mask              | `umask 002`                                     |
| `sudo visudo`    | Safely edit sudoers file                 | `sudo visudo`                                   |

---

## 🧾 Log & Service Inspection

| Command                             | Meaning                             | Example                                     |
|-------------------------------------|-------------------------------------|---------------------------------------------|
| `journalctl`                        | Read systemd logs                  | `journalctl -u sshd.service`                |
| `tail -f /var/log/syslog`           | Live log on Ubuntu                 | `tail -f /var/log/syslog`                   |
| `tail -f /var/log/messages`         | Live log on Amazon Linux / CentOS  | `tail -f /var/log/messages`                 |
| `systemctl status <service>`        | Check service status               | `systemctl status httpd`                    |
| `systemctl start <service>`         | Start a system service             | `sudo systemctl start httpd`                |
| `systemctl enable <service>`        | Enable service at boot             | `sudo systemctl enable httpd`               |

---


