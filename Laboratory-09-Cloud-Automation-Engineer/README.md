# Laboratory 09: Cloud Automation Engineer

## Mission Overview
The purpose of this mission is to automate application data backups using Bash scripting, file permissions, and Linux cron scheduling.

## Objectives
- Develop a reusable Bash backup script.
- Use variables to define source and destination paths.
- Compress application data into a timestamped archive.
- Configure executable permissions.
- Schedule the script to run automatically using cron.
- Record implementation evidence in the cloud computing portfolio.

## Commands Executed

```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt
nano backup.sh
chmod +x backup.sh
./backup.sh
ls -l backups/
crontab -l
env EDITOR=nano crontab -e
```

## Skills Learned
- Bash command sequencing and variable assignment.
- File and directory management.
- Archive creation with `tar`.
- Linux executable permissions.
- Cron scheduling syntax.
- Technical documentation with Markdown.

## Verification
The backup operation should produce a timestamped archive inside `backups/`. The configured cron entry should display the daily 2:00 AM schedule when checked using `crontab -l`.

## Evidence
- `script-execution.png`: Shows the script execution and backup archive.
- `cron-schedule.png`: Shows the installed cron schedule.

## Important Note
Confirm that `/root/backup.sh` is the actual script location before scheduling it. Use the correct absolute path for the account that owns the cron job.
