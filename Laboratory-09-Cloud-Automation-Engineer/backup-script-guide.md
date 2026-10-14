# Backup Script Guide

## 1. Backup Script Code

The following Bash script automatically compresses the application data folder and saves it inside the backups folder.

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

# Create the backup directory if it does not exist
mkdir -p "$BACKUP_DIR"

# Compress the source directory into a tarball
tar -czf "$BACKUP_DIR/backup_$TIMESTAMP.tar.gz" "$SOURCE_DIR"

echo "Backup completed successfully at $TIMESTAMP!"
```

## 2. File Permissions

The `chmod +x backup.sh` command adds execution permission to the backup script. Before using this command, Linux may prevent the script from running directly. After adding the permission, I can execute it using `./backup.sh`.

## 3. Cron Job Configuration

The cron expression used in this activity is:

```cron
0 2 * * * /root/backup.sh
```

This configuration schedules the backup script to run every day at 2:00 AM, based on the system's configured time and timezone.

### Meaning of the Five Time Fields

| Field | Value | Description |
|---|---|---|
| Minute | `0` | Runs at minute zero. |
| Hour | `2` | Runs at 2 AM. |
| Day of Month | `*` | Runs on every day of the month. |
| Month | `*` | Runs every month. |
| Day of Week | `*` | Runs every day of the week. |

The final part, `/root/backup.sh`, specifies the location of the script that Cron will execute.

## 4. Summary

This activity helped me understand how Bash scripts, file permissions, and Cron jobs work together. Automating the backup process can save time and reduce the chance of forgetting to back up important application data.
