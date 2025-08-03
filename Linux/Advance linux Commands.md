# 🧠 Advanced Linux Commands

---

## 🔁 Shell Scripting Essentials

| Command / Keyword    | Full Form / Meaning                                          |
|----------------------|--------------------------------------------------------------|
| `#!/bin/bash`        | **Shebang** – tells the system to use Bash shell             |
| `echo`               | **Echo** – prints text or variables to the terminal          |
| `read`               | **Read** – receives input from user                          |
| `if`, `else`, `fi`   | **If Else Fi** – conditional logic in scripts                |
| `for`, `while`, `do`, `done` | **Loops** – repeat a set of commands                 |
| `case` / `esac`      | **Case Statement** – multi-condition branching               |
| `function`           | Declare reusable code blocks (functions)                     |
| `exit`               | Terminate script with exit code                              |
| `cron`, `crontab -e` | **Cron Table** – schedule recurring tasks                    |

---

## 🛠️ System Management

| Command                        | Full Form / Meaning                                     |
|--------------------------------|---------------------------------------------------------|
| `adduser <name>`               | **Add User** – create a new user account               |
| `passwd <user>`                | **Password** – change/set user password                 |
| `usermod -aG <group> <user>`   | **User Modify Add to Group** – adds user to group       |
| `chmod 755 <file>`             | **Change Mode** – modify file permissions               |
| `chown user:group <file>`      | **Change Owner** – change file owner and group          |
| `umask`                        | **User Mask** – default permissions for new files       |

---

## 🧠 Process & Resource Management

| Command          | Full Form / Meaning                                      |
|------------------|----------------------------------------------------------|
| `top`            | **Table of Processes** – live process monitor             |
| `htop`           | **Human Top** – interactive process monitor               |
| `ps aux`         | **Process Status** – list all running processes           |
| `kill <PID>`     | Send signal to process (usually to stop it)              |
| `jobs`           | Show background jobs                                     |
| `bg`, `fg`       | **Background / Foreground** – move jobs between states   |
| `nice`, `renice` | Set or change process priority                           |

---

## 💾 Disk & File System

| Command                 | Full Form / Meaning                                   |
|-------------------------|-------------------------------------------------------|
| `df -h`                 | **Disk Free** – show free/used disk space             |
| `du -sh *`              | **Disk Usage Summary Human-readable** – space usage   |
| `mount`, `umount`       | Mount/unmount file systems                            |
| `lsblk`                 | **List Block Devices** – show disks and partitions     |
| `fdisk -l`              | **Format Disk** – list disk partitions                |
| `mkfs.ext4 /dev/xvdf`   | **Make Filesystem** – format disk with ext4           |

---

## 🔒 Permissions & Security

| Command          | Full Form / Meaning                                  |
|------------------|------------------------------------------------------|
| `chmod`          | **Change Mode** – set file permissions               |
| `chown`          | **Change Owner** – assign ownership                  |
| `ls -l`          | **List Long** – view permissions and metadata        |
| `umask`          | **User Mask** – default permission for new files     |
| `sudo visudo`    | **Visual Sudo** – safely edit sudo permissions       |

---

## 🧾 Log & Service Inspection

| Command                        | Full Form / Meaning                              |
|--------------------------------|--------------------------------------------------|
| `journalctl`                   | View logs managed by **systemd journal**         |
| `tail -f /var/log/syslog`      | Show live updates to system logs (Ubuntu)        |
| `tail -f /var/log/messages`    | Show live updates (Amazon Linux, CentOS)         |
| `systemctl status <service>`   | Check status of system service                   |
| `systemctl start <service>`    | Start the service                                |
| `systemctl enable <service>`   | Auto-start service on system boot                |

---

## 📋 Tips

| Command             | Full Form / Meaning                                  |
|---------------------|------------------------------------------------------|
| `man <command>`     | **Manual** – display the manual page for a command   |
| `command --help`    | Show usage help for the command                      |

---

