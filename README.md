# Metrics Chronicle Overview

ACM inventory list for metrics and labels

## Table of Contents

- Exposed Metrics

## Compatibility Matrix

### [Alerts Metrics](docs/alert-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| :node_memory_MemAvailable_bytes:sum                                          | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| ALERTS                                                                       | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |

### [Assisted Installer Metrics](docs/installer-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| assisted_installer_cluster_creation                                          |   :x:   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| assisted_installer_cluster_installation_started                              |   :x:   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| assisted_installer_cluster_installation_second                               |   :x:   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| assisted_installer_cluster_host_installation_count                           |   :x:   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| assisted_installer_host_installation_phase_seconds                           |   :x:   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| assisted_installer_cluster_host_disk_sync_duration_ms                        |   :x:   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| assisted_installer_cluster_host_image_pull_status                            |   :x:   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| assisted_installer_filesystem_usage_percentage                               |   :x:   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |

### [Authenticated Metrics](docs/authentication-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| authenticated_user_requests                                                  | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| authentication_attempts                                                      | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |

### [Cluster Metrics](docs/cluster-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| cluster:capacity_cpu_cores:sum                                               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| cluster:capacity_memory_bytes:sum                                            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| cluster:container_cpu_usage:ratio                                            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| cluster:container_spec_cpu_shares:ratio                                      | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| cluster:cpu_usage_cores:sum                                                  | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| cluster:memory_usage:ratio                                                   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| cluster:memory_usage_bytes:sum                                               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| cluster:usage:resources:sum                                                  | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| cluster_infrastructure_provider                                              | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| cluster_monitoring_operator_reconcile_errors_total                           | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| cluster_monitoring_operator_reconcile_attempts_total                         | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| cluster_operator_conditions                                                  | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| cluster_operator_up                                                          | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| cluster_version                                                              | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| cluster_version_payload                                                      | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |

### [Container Metrics](docs/container-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| container_cpu_cfs_periods_total                                              | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| container_cpu_cfs_throttled_periods_total                                    | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| container_cpu_usage_seconds_total                                            |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| container_memory_rss                                                         |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| container_memory_usage_bytes                                                 |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| container_network_receive_bytes_total                                        |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| container_network_receive_bytes_total                                        |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| container_network_receive_packets_total                                      |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| container_network_receive_packets_dropped_total                              |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| container_network_transmit_bytes_total                                       |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| container_network_transmit_packets_total                                     |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| container_network_transmit_packets_dropped_total                             |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| container_spec_cpu_quota                                                     | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |

### [Coredns Metrics](docs/coredns-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| coredns_dns_request_count_total                                              | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| coredns_dns_request_duration_seconds_sum                                     | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| coredns_dns_request_type_count_total                                         | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| coredns_dns_response_rcode_count_total                                       | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |

### [Daemonset Metrics](docs/daemonset-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| kube_daemonset_status_desired_number_scheduled                               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| kube_daemonset_status_number_unavailable                                     | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |

### [ETCD Metrics](docs/etcd-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| etcd_debugging_mvcc_db_total_size_in_bytes                                   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| etcd_debugging_snap_save_total_duration_seconds_sum                          | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| etcd_mvcc_db_total_size_in_bytes                                             | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| etcd_disk_backend_commit_duration_seconds_bucket                             | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| etcd_disk_backend_commit_duration_seconds_sum                                | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| etcd_disk_wal_fsync_duration_seconds_bucket                                  | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| etcd_disk_wal_fsync_duration_seconds_sum                                     | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| etcd_object_counts                                                           | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| etcd_network_client_grpc_received_bytes_total                                | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| etcd_network_client_grpc_sent_bytes_total                                    | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| etcd_network_peer_received_bytes_total                                       | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| etcd_network_peer_sent_bytes_total                                           | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| etcd_server_client_requests_total                                            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| etcd_server_has_leader                                                       | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| etcd_server_health_failures                                                  | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| etcd_server_leader_changes_seen_total                                        | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| etcd_server_proposals_failed_total                                           | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| etcd_server_proposals_pending                                                | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| etcd_server_proposals_committed_total                                        | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| etcd_server_proposals_applied_total                                          | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| etcd_server_quota_backend_bytes                                              | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |

### [GRPC Metrics](docs/grpc-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| grpc_server_started_total                                                    | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |

### [Haproxy Metrics](docs/haproxy-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| haproxy_backend_connection_errors_total                                      | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| haproxy_backend_connections_total                                            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| haproxy_backend_current_queue                                                | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| haproxy_backend_http_average_response_latency_milliseconds                   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| haproxy_backend_max_sessions                                                 | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| haproxy_backend_response_errors_total                                        | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| haproxy_backend_up                                                           | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |

### [HTTP Metrics](docs/http-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| http_requests_total                                                          | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |

### [Instance Metrics](docs/instance-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| instance:node_filesystem_usage:sum                                           | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| instance:node_cpu_utilisation:rate1m                                         | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| instance:node_load1_per_cpu:ratio                                            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| instance:node_memory_utilisation:ratio                                       | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| instance:node_network_receive_bytes_excluding_lo:rate1m                      | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| instance:node_network_receive_drop_excluding_lo:rate1m                       | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| instance:node_network_transmit_bytes_excluding_lo:rate1m                     | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| instance:node_network_transmit_drop_excluding_lo:rate1m                      | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| instance:node_num_cpu:sum                                                    | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| instance:node_vmstat_pgmajfault:rate1m                                       | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| instance_device:node_disk_io_time_seconds:rate1m                             | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| instance_device:node_disk_io_time_weighted_seconds:rate1m                    | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |

### [Kubelet Metrics](docs/kubelet-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| kubelet_running_container_count                                              | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| kubelet_runtime_operations                                                   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| kubelet_runtime_operations_latency_microseconds                              | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| kubelet_volume_stats_available_bytes                                         | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| kubelet_volume_stats_capacity_bytes                                          | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| kube_persistentvolume_status_phase                                           | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |

### [Machine Metrics](docs/machine-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| machine_cpu_cores                                                            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| machine_memory_bytes                                                         | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |

### [Mixin Metrics](docs/mixin-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| mixin_pod_workload                                                           | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |

### [Node Metrics](docs/node-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| kube_node_labels                                                             |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| kube_node_spec_unschedulable                                                 | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| kube_node_status_allocatable                                                 | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| kube_node_status_allocatable_cpu_cores                                       | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| kube_node_status_allocatable_memory_bytes                                    | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| kube_node_status_capacity                                                    | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| kube_node_status_capacity_pods                                               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| kube_node_status_capacity_cpu_cores                                          | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| kube_node_status_condition                                                   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |

### [OpenShift Metrics](docs/openshift-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| openshift_clusterresourcequota_usage                                         |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| openshift_clusterresourcequota_labels                                        |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |

### [Pod Metrics](docs/pod-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| kube_pod_container_resource_limits                                           | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| kube_pod_container_resource_limits_cpu_cores                                 | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| kube_pod_container_resource_limits_memory_bytes                              | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| kube_pod_container_resource_requests                                         | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| kube_pod_container_resource_requests_cpu_cores                               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| kube_pod_container_resource_requests_memory_bytes                            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| kube_pod_container_status_restarts_total                                     |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| kube_pod_info                                                                | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| kube_pod_owner                                                               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| kube_pod_status_ready                                                        |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| kube_pod_status_phase                                                        |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| kube_resourcequota                                                           | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |

### Namespace Metrics

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| kube_namespace_labels                                                        |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark: |
| namespace:kube_pod_container_resource_requests_cpu_cores:sum                 | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| namespace:kube_pod_container_resource_requests_memory_bytes:sum              | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| namespace:container_memory_usage_bytes:sum                                   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| namespace_cpu:kube_pod_container_resource_requests:sum                       | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| namespace_pod_name_container_name:container_cpu_usage_seconds_total:sum_rate | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| namespace_workload_pod:kube_pod_owner:relabel                                | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| namespace_workload_pod:kube_pod_owner:relabel                                | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |

### Node Metrics

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| node_cpu_seconds_total                                                       | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| node_disk_bytes_read                                                         |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| node_disk_bytes_written                                                      |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| node_filesystem_avail                                                        |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| node_filesystem_avail_bytes                                                  | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| node_filesystem_free_bytes                                                   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| node_filesystem_size                                                         |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| node_filesystem_size_bytes                                                   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| node_memory_MemAvailable_bytes                                               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| node_memory_MemTotal_bytes                                                   |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| node_namespace_pod_container:container_cpu_usage_seconds_total:sum_rate      | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| node_namespace_pod_container:container_cpu_usage_seconds_total:sum_irate     | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |   :x:   |
| node_netstat_Tcp_OutSegs                                                     | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| node_netstat_Tcp_RetransSegs                                                 | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| node_netstat_TcpExt_TCPSynRetrans                                            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| node_network_receive_bytes                                                   |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| node_network_transmit_bytes                                                  |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| node:node_cpu_utilisation:avg1m                                              |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| node:node_disk_utilisation:avg_irate                                         |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| node:node_memory_bytes_total:sum                                             |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| node:node_net_utilisation:sum_irate                                          |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |
| 'node_namespace_pod:kube_pod_info:'                                          |   :x:   |   :x:   |   :x:   |   :x:   |   :x:   | :white_check_mark:  |

### Service Metrics

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| up                                                                           | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
