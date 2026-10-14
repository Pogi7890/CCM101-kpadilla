# Automation Research

## 1. Bash Script
Bash scripting allows administrators to combine Linux commands into a reusable program. The shebang `#!/bin/bash` identifies the Bash interpreter that should execute the script, helping the system process the commands correctly.

## 2. Variables
Variables provide reusable storage for values such as source paths, backup locations, and timestamps. Using `$BACKUP_DIR` instead of repeating a directory name makes the script easier to maintain and reduces errors when settings change.

## 3. Cron Job
Cron is a Linux scheduling service that executes commands automatically according to a defined time expression. It supports routine cloud administration tasks, including backups and maintenance, allowing them to run consistently without continuous human supervision.
