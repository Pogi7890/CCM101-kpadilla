# Backup Script Guide

## 1. Backup Script

The following Bash script compresses the `app-data` directory and saves the backup inside the `backups` directory.

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

# Create the backup directory if it does not exist
mkdir -p $BACKUP_DIR

# Compress the source directory into a tar.gz file
tar -czf $BACKUP_DIR/backup_$TIMESTAMP.tar.gz $SOURCE_DIR

echo "Backup completed successfully at $TIMESTAMP!"
```

## 2. Purpose of chmod +x

The command `chmod +x backup.sh` gives the script permission to run as an executable program. Without this permission, Linux may prevent the user from running the script directly.

## 3. Cron Job Expression

```bash
0 2 * * * /root/backup.sh
```

The five time fields have the following meanings:

- **Minute (0):** Runs at minute zero.
- **Hour (2):** Runs at 2 AM.
- **Day of Month (*):** Runs every day of the month.
- **Month (*):** Runs every month.
- **Day of Week (*):** Runs every day of the week.
