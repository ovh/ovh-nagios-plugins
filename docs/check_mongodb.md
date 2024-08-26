# check_mongodb

## canary_read

Connect to perform a read operation on the MongoDB instance and measure
execution time.

```
command[check_mongodb_canary_read]=/opt/ovh-nagios-plugins/bin/check_mongodb --cnf /var/lib/nagios/.mongodb.cnf --tls --tls-allow-invalid-certificates --host 127.0.0.1 --auth-source canary_mongodb canary_read --database canary_mongodb --collection canary_check --warning 500 --critical 1000
```

## canary_write

Connect to perform a write operation on the MongoDB instance and measure
execution time.

```
command[check_mongodb_canary_write]=/opt/ovh-nagios-plugins/bin/check_mongodb --cnf /var/lib/nagios/.mongodb.cnf --tls --tls-allow-invalid-certificates --host 127.0.0.1 --auth-source canary_mongodb canary_write --database canary_mongodb --collection canary_check --warning 500 --critical 1000
```

## connections

Check connection pool usage by comparing current connection count with
configured limit.

```
command[check_mongodb_connections]=/opt/ovh-nagios-plugins/bin/check_mongodb --cnf /var/lib/nagios/.mongodb.cnf --tls --tls-allow-invalid-certificates connections
```

## repl_lag

Measure replication lag between the current node and its source in a Replica
Set.

```
command[check_mongodb_replication_lag]=/opt/ovh-nagios-plugins/bin/check_mongodb --cnf /var/lib/nagios/.mongodb.cnf --tls --tls-allow-invalid-certificates repl_lag
```

## repl_state

Check if Replica Set replication is ok.

```
command[check_mongodb_replication_state]=/opt/ovh-nagios-plugins/bin/check_mongodb --cnf /var/lib/nagios/.mongodb.cnf --tls --tls-allow-invalid-certificates repl_state
```
