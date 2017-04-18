# Simple backup script

This is a very simple script that saves an archive of a source folder in a destination folder.
It also deletes the oldest file when the number of files in the destination folder exceeds 10, so make sure the destination folder only contains backups.

## Usage

```bash
bash backup.sh /path/to/src /path/to/dest
```

### As cronjob

To run the backup script every hour, open crontab with `crontab -e` and add the following line:

```bash
@hourly /path/to/backup.sh /path/to/src /path/to/dest
```
