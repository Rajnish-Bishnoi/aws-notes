# 🐧 Ultimate Linux Command Sheet for AWS EC2 Practice 📘

## 📁 File & Directory Navigation

| Command       | Full Form / Meaning                                |
|---------------|-----------------------------------------------------|
| `pwd`         | **Print Working Directory** – Shows current path    |
| `cd ..`       | **Change Directory** – Move to parent folder        |
| `cd .`        | Current directory (no movement)                     |
| `cd -`        | Move to previous directory                          |
| `cd <folder>` | Change into specified folder                        |
| `ls`          | **List** – Show files in directory                  |
| `ls -l`       | Long listing (with permissions, size, etc.)         |
| `ls -lt`      | Long listing, sorted by time (latest first)         |
| `ls -ltr`     | Long listing, oldest files at bottom                |
| `ls -latr`    | Show all files (including hidden), sorted by time   |

---

## 📂 File & Directory Management

| Command              | Full Form / Meaning                                     |
|----------------------|---------------------------------------------------------|
| `mkdir <folder>`     | **Make Directory** – Create a new folder                |
| `touch 1.txt`        | Create empty file named `1.txt`                         |
| `cp 1.txt 2.txt`     | **Copy** – Duplicate file                               |
| `mv 1.txt 2.txt`     | **Move** or rename file                                 |
| `rm 1.txt`           | **Remove** – Delete a file                              |
| `rm -r <folder>`     | Remove folder and contents                              |
| `rm -rf *`           | Force delete all files (⚠️ Dangerous!)                 |

---

## 🧾 File Content & Text Editing

| Command              | Full Form / Meaning                                         |
|----------------------|-------------------------------------------------------------|
| `cat file.txt`       | **Concatenate** – Show file content                         |
| `cat > file.txt`     | Create file, type input manually (Ctrl+D to save)           |
| `less file.txt`      | Scroll through file one page at a time                      |
| `/searchterm` (less) | Search inside file in `less` mode                           |
| `q`                  | Quit from `less` or `man`                                   |
| `head file.txt`      | Show first 10 lines of a file                               |
| `tail file.txt`      | Show last 10 lines of a file                                |
| `tail -f file.txt`   | Live updates from the file (e.g. logs)                      |

---

## ✍️ VI Editor (Text Editing)

| Command            | Full Form / Meaning                          |
|--------------------|-----------------------------------------------|
| `vi file.txt`      | Open (or create) file in VI editor            |
| `i`, `a`, `o`       | Insert, Append, Open new line in insert mode  |
| `Esc :wq`          | Write and quit                                |
| `Esc :q!`          | Quit without saving                           |

---

## 🔁 Redirection & Pipes

| Symbol / Command       | Full Form / Meaning                                     |
|------------------------|---------------------------------------------------------|
| `>`                    | Redirect output (overwrite)                             |
| `>>`                   | Append output                                           |
| `command1 | command2`  | **Pipe** – Output of 1st command goes to 2nd            |

---

## 🔢 Counting & Statistics

| Command             | Full Form / Meaning                       |
|---------------------|-------------------------------------------|
| `wc file.txt`       | **Word Count** – lines, words, characters |
| `wc -l`             | Line count                                |
| `wc -w`             | Word count                                |
| `wc -c`             | Character count                           |

---

## 🖥️ System Monitoring

| Command             | Full Form / Meaning                            |
|---------------------|------------------------------------------------|
| `top`               | Show real-time system processes                |
| `htop`              | Advanced process viewer (install separately)   |
| `ps aux`            | Show all running processes                     |
| `uptime`            | Show how long system has been running          |
| `free -m`           | Show memory usage (in MB)                      |
| `df -h`             | **Disk Free** – Show disk usage (human-readable) |
| `du -sh *`          | **Disk Usage** of current folder content       |
| `whoami`            | Show logged-in user                            |
| `id`                | Show user ID and group ID                      |

---

## 🌐 Networking & OS Info

| Command                 | Full Form / Meaning                            |
|-------------------------|------------------------------------------------|
| `ping <host>`           | Check network connectivity                     |
| `curl <URL>`            | Transfer data from or to a server              |
| `wget <URL>`            | Download files via HTTP, HTTPS, FTP            |
| `ip a` / `ifconfig`     | Show IP and network interfaces                 |
| `netstat -tuln`         | Network statistics (TCP/UDP listening ports)   |
| `ss -tuln`              | Similar to `netstat`, faster and newer         |
| `cat /etc/os-release`   | Show Linux distro info                         |
| `cat /proc/cpuinfo`     | Show CPU details                               |
| `cat /proc/meminfo`     | Show RAM details                               |

---

## ☁️ AWS EC2-Specific Commands

| Command                                     | Full Form / Meaning                                |
|---------------------------------------------|----------------------------------------------------|
| `ssh -i <key.pem> ec2-user@<IP>`           | Secure shell into EC2 instance                     |
| `sudo systemctl status httpd`              | Check Apache service status                        |
| `sudo systemctl start httpd`               | Start Apache server                                |
| `sudo systemctl enable httpd`              | Auto-start Apache on boot                          |
| `sudo reboot`                              | Reboot the EC2 instance                            |
| `sudo shutdown -h now`                     | Shutdown the instance immediately                  |

---

## 📦 Package Management (Amazon Linux / Ubuntu)

| OS             | Command Examples                                    |
|----------------|-----------------------------------------------------|
| Amazon Linux   | `sudo yum install httpd` – Install Apache           |
|                | `sudo yum update -y` – Update all packages          |
| Ubuntu         | `sudo apt install apache2` – Install Apache         |
|                | `sudo apt update && sudo apt upgrade -y` – Full update |

---

## 🧠 Mind-Map (Textual Style)


          AWS EC2 Linux Cheat Sheet
                     |
     ------------------------------------------------
     |           |              |                   |
 🔒 System      📁 Files       🌐 Networking      ☁️ AWS Services
 Monitoring     & Dir Ops                        (EC2, S3, IAM...)
 (top, ps, df)  (ls, cp, rm)  (ping, curl, wget)

        \            |             /       
         \           |            /
          → Redirection & Piping ←
               (`>`, `>>`, `|`)

    +------------------+       +------------------+
    | Text Editing     |       | Package Manager  |
    | (`vi`, `cat`,    |       | (`yum`, `apt`)   |
    |  `less`, `tail`) |       +------------------+
    +------------------+

                     |
           ⚙️ System Info Commands
           (`uname`, `/proc/cpuinfo`, etc.)


