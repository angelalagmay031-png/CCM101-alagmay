
# Laboratory Activity 9

## Mission 9: The Cloud Automation Engineer

### Mission Overview

This mission demonstrates how Linux automation can reduce repetitive administrative tasks. A Bash script was developed to create timestamped backups of application data, while Cron was configured to execute the backup process automatically every night.

### Objectives

- Understand the role of Bash in Linux automation.
- Use variables to organize script information.
- Create a reusable data backup script.
- Apply executable permissions to a Bash file.
- Compress application files using the tar utility.
- Configure a scheduled task through Linux Cron.
- Document the backup process and its configuration.

### Commands Executed

| Command | Purpose |
|---|---|
| `pwd` | Checks the current directory. |
| `mkdir app-data` | Creates the application folder. |
| `echo` | Adds sample application data. |
| `nano backup.sh` | Opens the script editor. |
| `chmod +x backup.sh` | Enables script execution. |
| `./backup.sh` | Starts the backup process. |
| `ls -l backups/` | Checks generated archives. |
| `tar -tzf` | Inspects compressed backup contents. |
| `crontab -l` | Displays the current schedule. |
| `env EDITOR=nano crontab -e` | Edits the Cron schedule. |

### Skills Learned

- Bash Automation
- Linux Command-Line Administration
- File and Directory Management
- Executable Permissions
- Compressed Data Backups
- Cron Scheduling
- Basic Error Handling
- Cloud Operations

### Screenshots

- `script-execution.png` – Evidence of the successful backup operation.
- `cron-schedule.png` – Evidence of the configured automatic schedule.

### Mission Status

**Completed** – Developed and tested a Bash backup script and configured a daily automated execution schedule using Cron.

