### Backup Script Cron Job

To schedule the backup script to run automatically every day at 2:00 AM, add the following line to your crontab file:

```sh
0 2 * * * /home/user/scripts/backup_script.sh
Breakdown of the Cron Syntax
0: Minute (0th minute)
2: Hour (2 AM)
*: Day of the month (every day)
*: Month (every month)
*: Day of the week (every day of the week)
Steps to Implement
Create the Backup Script:

Save the backup script into a file, e.g., /home/user/scripts/backup_script.sh.
Ensure the script is executable by running:
chmod +x /home/user/scripts/backup_script.sh
Edit the Crontab:

Open the crontab file by running:
crontab -e
Add the cron job entry:
0 2 * * * /home/user/scripts/backup_script.sh
Save and close the crontab file.
This cron job will now run the backup script every day at 2:00 AM, automating the backup process.

