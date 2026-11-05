# Backup Script Guide

## 1. Backup Script

The backup script automates the process of copying and compressing important application data.

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies
SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")
echo "Initiating automated backup..."
# Create the backup directory if it does not exist
mkdir -p $BACKUP_DIR
# Compress the source directory into a tarball (.tar.gz)
tar -czf $BACKUP_DIR/backup_$TIMESTAMP.tar.gz $SOURCE_DIR
echo "Backup completed successfully at $TIMESTAMP!"
```

## 2. Execution Permission

The command `chmod +x backup.sh` gives the script permission to execute. Without this permission, running the script directly may result in a Permission denied error.

## 3. Cron Job Schedule

The cron expression used in this activity is:

```bash
0 2 * * * /root/backup.sh
```

The five cron fields have the following meanings:

- **Minute (0):** Runs at minute zero.
- **Hour (2):** Runs at 2 AM.
- **Day of Month (*):** Runs every day of the month.
- **Month (*):** Runs every month.
- **Day of Week (*):** Runs every day of the week.

This schedule automatically runs the backup script every day at 2:00 AM.
