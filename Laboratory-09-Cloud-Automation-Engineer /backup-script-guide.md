
# Checkpoint 6 – Backup Automation Documentation

## 1. Purpose of the Script

The backup script was created to protect the application's data by automatically producing a compressed copy of the source folder. It uses a timestamp in the filename so that each backup has a different name.

## 2. Bash Script Implementation

```bash
#!/bin/bash

# CloudNova Automated Data Protection

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")
BACKUP_FILE="$BACKUP_DIR/client_backup_$TIMESTAMP.tar.gz"

echo "Starting client data backup..."

if [ ! -d "$SOURCE_DIR" ]; then
    echo "Error: Application data folder not found."
    exit 1
fi

mkdir -p "$BACKUP_DIR"

if tar -czf "$BACKUP_FILE" "$SOURCE_DIR"; then
    echo "Backup successfully created!"
    echo "Backup location: $BACKUP_FILE"
else
    echo "Error: Backup operation failed."
    exit 1
fi
```

## 3. Executable File Permission

The command `chmod +x backup.sh` gives the script permission to run as an executable program. This allows the user to start it directly from the terminal using `./backup.sh`.

## 4. Cron Job Configuration

The following Cron expression was installed:

```bash
0 2 * * * /root/backup.sh
```

### Explanation of the Five Time Fields

| Field | Value | Function |
|---|---|---|
| Minute | 0 | Starts at the beginning of the hour. |
| Hour | 2 | Runs during the 2 AM hour. |
| Day of Month | * | Applies to every calendar day. |
| Month | * | Applies to all months. |
| Day of Week | * | Applies to all days of the week. |

### Automation Schedule

The configured schedule runs the backup script every day at 2:00 AM. This allows the application data to have a regularly scheduled backup without depending on an employee to start the process manually.

## 5. Verification

The generated backup was checked using the `ls -l backups/` command. The `tar -tzf` command was also used to inspect the contents of the compressed archive.

The Cron configuration was verified through `crontab -l`.

