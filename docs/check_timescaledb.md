# check_timescaledb

## background_workers

Check if there is at least one background worker started for each TimescaleDB
database so they can properly execute scheduled jobs.

```
command[check_timescaledb_background_workers]=/usr/bin/sudo -u root /opt/ovh-nagios-plugins/bin/check_timescaledb --skip-recovery --user monitoring background_workers
```

## job_errors

Check the number of TimescaleDB jobs in error.

```
command[check_timescaledb_job_errors]=/opt/ovh-nagios-plugins/bin/check_timescaledb --skip-recovery --user monitoring job_errors
```

## version

Compare TimescaleDB extensions installed versions on every databases with the
available version.

```
command[check_timescaledb_version]=/opt/ovh-nagios-plugins/bin/check_timescaledb --skip-recovery --user monitoring version --warning
```
