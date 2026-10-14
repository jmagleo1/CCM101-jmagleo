# Laboratory 09 – Cloud Automation Engineer

## Mission Overview

In this laboratory activity, I learned how to automate server tasks using Bash scripting and Cron jobs. I created a backup script that compresses application data into a `.tar.gz` file and configured a schedule for automatic backups.

## Objectives

- Understand the basics of Bash scripting.
- Create a script that automatically backs up application data.
- Use `chmod` to make a script executable.
- Configure scheduled tasks using Cron.
- Document the automation process using Markdown.

## Commands Executed

| Command | Purpose |
|---|---|
| `mkdir -p app-data` | Creates the application data folder. |
| `echo "This is critical client data." > app-data/data.txt` | Creates a sample data file. |
| `nano backup.sh` | Opens the text editor to create the script. |
| `chmod +x backup.sh` | Adds execution permission. |
| `./backup.sh` | Runs the backup script. |
| `ls -l backups/` | Checks the generated backup files. |
| `crontab -l` | Displays the configured Cron jobs. |
| `env EDITOR=nano crontab -e` | Opens the Cron configuration for editing. |

## Skills Learned

- Bash shell scripting
- Linux file permissions
- Automated file backups
- File compression using `tar`
- Cron job scheduling
- Markdown documentation
- GitHub repository management
