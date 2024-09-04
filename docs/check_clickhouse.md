# check_clickhouse

## cluster_connectivity

Check if the cluster members are reachable via the SQL interface.

```
command[check_clickhouse_cluster_connectivity]=/opt/ovh-nagios-plugins/bin/check_clickhouse --secure cluster_connectivity
```

## connections

Check the percentage of used connections.

```
command[check_clickhouse_connections]=/opt/ovh-nagios-plugins/bin/check_clickhouse --secure connections
```

## delayed_inserts

Check if insertions are being delayed.

```
command[check_clickhouse_delayed_inserts]=/opt/ovh-nagios-plugins/bin/check_clickhouse --secure delayed_inserts
```

## detached_parts

Check if parts are detached.

```
command[check_clickhouse_detached_parts]=/opt/ovh-nagios-plugins/bin/check_clickhouse --secure detached_parts
```

## keeper_health

Check if the Keeper cluster has been configured and is healthy.

```
command[check_clickhouse_keeper_health]=/opt/ovh-nagios-plugins/bin/check_clickhouse --secure keeper_health
```

## max_part_count_for_partition

Check the maximum number of parts per partition across all partitions of all
tables of MergeTree family. Values larger than 300 indicates misconfiguration,
overload, or massive data loading (according to the
[documentation](https://clickhouse.com/docs/en/operations/system-tables/asynchronous_metrics)).

```
command[check_clickhouse_max_part_count_for_partition]=/opt/ovh-nagios-plugins/bin/check_clickhouse --secure max_part_count_for_partition
```


## pending_files_rate

Check if the number of distributed files in the queue is increasing over time.

```
command[check_clickhouse_pending_files_rate]=/opt/ovh-nagios-plugins/bin/check_clickhouse --secure pending_files_rate
```

## queries

Check the number of running queries.

```
command[check_clickhouse_queries]=/opt/ovh-nagios-plugins/bin/check_clickhouse --secure queries
```

## replication_queue

Check if replication tasks are stuck.

```
command[check_clickhouse_replication_queue]=/opt/ovh-nagios-plugins/bin/check_clickhouse --secure replication_queue
```
