# Ansible Role "cron"

## host_vars
Examples:
```
cron:
  - name: daily backup
    user: bkp_user
    job: /usr/local/bin/backup --config /usr/local/etc/backup/daily.conf
    minute: "15"
    hour: "00"
  - name: weekly backup
    user: bkp_user
    job: /usr/local/bin/backup --config /usr/local/etc/backup/weekly.conf
    minute: "15"
    hour: "00"
    day: "6"
  - name: delete old backup
    job: /usr/local/bin/backup --clean --dir /mnt/backup
```

```
cron:
  - name: test
    special_time: reboot
    job: /usr/local/bin/test
```
