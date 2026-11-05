
# Checkpoint 2 – Understanding Automation Tools

## 1. Bash Script

A Bash script is a collection of Linux commands written in one file to perform tasks in a specific order. The `#!/bin/bash` line tells Linux which shell interpreter should be used when executing the file. It makes it easier to repeat tasks without entering every command manually.

## 2. Variables

Variables are used to keep important values that a script needs during execution. For example, `$BACKUP_DIR` stores the location where backup files will be saved. Using variables makes the script easier to update because the value can be changed without modifying every command that uses it.

## 3. Cron Job

A Cron job is a scheduling feature in Linux that runs commands automatically at selected times or dates. It helps cloud administrators handle repeated activities such as creating backups, cleaning temporary files, and performing maintenance. This reduces manual work and helps keep server operations consistent.

