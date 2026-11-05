# Laboratory 09 - Cloud Automation Engineer

**CCM101 - Cloud Computing**

## Mission Overview

This activity focuses on automating cloud operations using Bash scripts and Cron Jobs. I created a backup script that compresses application data and configured a schedule to run it automatically.

## Objectives

- Understand Bash scripting and its basic commands.
- Create and execute an automated backup script.
- Use file permissions to execute a script.
- Schedule automated tasks using Cron Jobs.

## Commands Executed

```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt
nano backup.sh
./backup.sh
chmod +x backup.sh
ls -l backups/
crontab -l
env EDITOR=nano crontab -e
```

## Skills Learned

- Creating and running Bash scripts.
- Using variables in automation.
- Compressing files using `tar`.
- Managing script permissions.
- Scheduling automated backups using Cron Jobs.
- Understanding the importance of automation in cloud operations.
