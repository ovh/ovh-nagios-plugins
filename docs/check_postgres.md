# check_postgres

## disabled_databases

Check if databases allow connections. Raise an alert if they are not.

```
command[check_postgres_disabled_databases]=/opt/ovh-nagios-plugins/bin/check_postgres --skip-recovery --user monitoring disabled_databases
```

## invalid_indices

Check the number of invalid indices on all databases.

```
command[check_postgres_invalid_indices]=/opt/ovh-nagios-plugins/bin/check_postgres --skip-recovery --user monitoring invalid_indices
```

The monitoring user should have permissions to list indices.
