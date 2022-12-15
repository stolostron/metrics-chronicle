# ETCD Metrics

| Metric Name                                          | Metric Type | Description                                     | Status |
|------------------------------------------------------|-------------|-------------------------------------------------|--------|
|  etcd_debugging_mvcc_db_total_size_in_bytes          | gauge       | Total size of the underlying database in bytes. | |
|  etcd_debugging_snap_save_total_duration_seconds_sum | histogram   | Latencies while etcd is committing an incremental snapshot of its most recent changes to disk. | |
|  etcd_disk_backend_commit_duration_seconds_bucket    |             | | |
|  etcd_disk_backend_commit_duration_seconds_sum       |             | | |
|  etcd_disk_wal_fsync_duration_seconds_bucket         | histogram   | The latency distributions of fsync called by wal. | |
|  etcd_disk_wal_fsync_duration_seconds_sum            |             | | |
|  etcd_mvcc_db_total_size_in_bytes                    | gauge       | Total size of the underlying database physically allocated in bytes. | |
|  etcd_network_client_grpc_received_bytes_total       | counter     | The total number of bytes received from grpc clients.     | |
|  etcd_network_client_grpc_sent_bytes_total           | counter     | The total number of bytes sent to grpc clients.           | |
|  etcd_network_peer_received_bytes_total              | counter     | The total number of bytes received from peers.            | |
|  etcd_network_peer_sent_bytes_total                  | counter     | The total number of bytes sent to peers.                  | |
|  etcd_object_counts                                  | gauge       | Number of stored objects at the time of last check split by kind. This metric is replaced by apiserver_storage_object_counts. | |
|  etcd_server_client_requests_total                   | counter     | The total number of client requests per client version.   | |
|  etcd_server_has_leader                              | gauge       | Whether or not a leader exists. 1 is existence, 0 is not. | |
|  etcd_server_health_failures                         | counter     | The total number of failed health checks.                 | |
|  etcd_server_leader_changes_seen_total               | counter     | The number of leader changes seen.                        | |
|  etcd_server_proposals_applied_total                 | gauge       | The total number of consensus proposals applied.          | |
|  etcd_server_proposals_committed_total               | gauge       | The total number of consensus proposals committed.        | |
|  etcd_server_proposals_failed_total                  | counter     | The total number of failed proposals seen.                | |
|  etcd_server_proposals_pending                       | gauge       | The current number of pending proposals to commit.        | |
|  etcd_server_quota_backend_bytes                     | gauge       | Current backend storage quota size in bytes.              | |
