📌 What is Userdata?
Userdata is a script that runs automatically when an EC2 instance is launched.

It is used to automate initial setup tasks, such as installing software, configuring applications, and setting up environment variables.

This script runs only once by default (at the first boot).

Userdata is commonly used to perform post-installation tasks automatically.

🧠 Alternate Names:
Also known as Bootstrap Script.

It helps in zero-touch configuration of the instance.

🔄 Can I re-run Userdata?
By default, Userdata executes only once at the first launch.

However, if you want to re-run it:

The instance must be in stopped state.

You can update or replace the Userdata script from the EC2 dashboard.

You must manually trigger re-execution by enabling user-data re-run scripts inside the script logic or modifying EC2 instance settings.

📂 What comes with EC2 instance by default?
When you launch an EC2 instance, it includes:

✅ Operating System (e.g., Amazon Linux, Ubuntu, Windows)

✅ Base OS Configuration (minimal settings)

💡 Real-life Example: Web Server Setup
Goal: You want to launch 50 EC2 instances with a web server (Apache) pre-installed.

Instead of doing this manually for each instance:

Use a Userdata script.

The script installs Apache, starts the service, and hosts a basic website.

When EC2 boots, the server is ready to serve traffic automatically.
