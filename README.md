# duplicity-backup

A backup script based around duplicity

## Environment Variables

| Variable         | Default                          |
| ---------------- | -------------------------------- |
| `PASSPHRASE`     | _None_                           |
| `INC_FILE`       | `/etc/duplicity-backup/includes` |
| `DEST`           | `/mnt/backups`                   |
| `DUPLICITY_ARGS` | `--full-if-older-than 1M`        |

**IMPORTANT** - If no `PASSPHRASE` is specified, duplicity will prompt for a GPG
passphrase. Ensure it is set for non-interactive execution to work properly.
