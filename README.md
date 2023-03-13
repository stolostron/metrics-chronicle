# Metrics Chronicle Overview

ACM inventory list for metrics and labels

## Table of Contents

- Exposed Metrics

## Compatibility Matrix

### [Alerts Metrics](docs/alert-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| :node_memory_MemAvailable_bytes:sum                                          |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| ALERTS                                                                       |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |

### [Assisted Installer Metrics](docs/installer-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| assisted_installer_cluster_creation                                          |    ✘    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| assisted_installer_cluster_installation_started                              |    ✘    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| assisted_installer_cluster_installation_second                               |    ✘    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| assisted_installer_cluster_host_installation_count                           |    ✘    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| assisted_installer_host_installation_phase_seconds                           |    ✘    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| assisted_installer_cluster_host_disk_sync_duration_ms                        |    ✘    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| assisted_installer_cluster_host_image_pull_status                            |    ✘    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| assisted_installer_filesystem_usage_percentage                               |    ✘    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |

### [Authenticated Metrics](docs/authentication-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| authenticated_user_requests                                                  |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| authentication_attempts                                                      |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |

### [Cluster Metrics](docs/cluster-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| cluster:capacity_cpu_cores:sum                                               |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| cluster:capacity_memory_bytes:sum                                            |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| cluster:container_cpu_usage:ratio                                            |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| cluster:container_spec_cpu_shares:ratio                                      |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| cluster:cpu_usage_cores:sum                                                  |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| cluster:memory_usage:ratio                                                   |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| cluster:memory_usage_bytes:sum                                               |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| cluster:usage:resources:sum                                                  |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| cluster_infrastructure_provider                                              |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| cluster_monitoring_operator_reconcile_errors_total                           |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| cluster_monitoring_operator_reconcile_attempts_total                         |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| cluster_operator_conditions                                                  |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| cluster_operator_up                                                          |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| cluster_version                                                              |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| cluster_version_payload                                                      |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |

### [Container Metrics](docs/container-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| container_cpu_cfs_periods_total                                              |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| container_cpu_cfs_throttled_periods_total                                    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| container_cpu_usage_seconds_total                                            |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| container_memory_rss                                                         |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| container_memory_usage_bytes                                                 |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| container_network_receive_bytes_total                                        |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| container_network_receive_bytes_total                                        |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| container_network_receive_packets_total                                      |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| container_network_receive_packets_dropped_total                              |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| container_network_transmit_bytes_total                                       |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| container_network_transmit_packets_total                                     |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| container_network_transmit_packets_dropped_total                             |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| container_spec_cpu_quota                                                     |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |

### [Coredns Metrics](docs/coredns-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| coredns_dns_request_count_total                                              |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| coredns_dns_request_duration_seconds_sum                                     |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| coredns_dns_request_type_count_total                                         |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| coredns_dns_response_rcode_count_total                                       |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |

### [Daemonset Metrics](docs/daemonset-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| kube_daemonset_status_desired_number_scheduled                               |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| kube_daemonset_status_number_unavailable                                     |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |

### [ETCD Metrics](docs/etcd-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| etcd_debugging_mvcc_db_total_size_in_bytes                                   |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| etcd_debugging_snap_save_total_duration_seconds_sum                          |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| etcd_mvcc_db_total_size_in_bytes                                             |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| etcd_disk_backend_commit_duration_seconds_bucket                             |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| etcd_disk_backend_commit_duration_seconds_sum                                |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| etcd_disk_wal_fsync_duration_seconds_bucket                                  |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| etcd_disk_wal_fsync_duration_seconds_sum                                     |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| etcd_object_counts                                                           |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| etcd_network_client_grpc_received_bytes_total                                |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| etcd_network_client_grpc_sent_bytes_total                                    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| etcd_network_peer_received_bytes_total                                       |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| etcd_network_peer_sent_bytes_total                                           |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| etcd_server_client_requests_total                                            |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| etcd_server_has_leader                                                       |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| etcd_server_health_failures                                                  |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| etcd_server_leader_changes_seen_total                                        |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| etcd_server_proposals_failed_total                                           |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| etcd_server_proposals_pending                                                |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| etcd_server_proposals_committed_total                                        |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| etcd_server_proposals_applied_total                                          |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| etcd_server_quota_backend_bytes                                              |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |

### [GRPC Metrics](docs/grpc-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| grpc_server_started_total                                                    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |

### [Haproxy Metrics](docs/haproxy-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| haproxy_backend_connection_errors_total                                      |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| haproxy_backend_connections_total                                            |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| haproxy_backend_current_queue                                                |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| haproxy_backend_http_average_response_latency_milliseconds                   |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| haproxy_backend_max_sessions                                                 |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| haproxy_backend_response_errors_total                                        |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| haproxy_backend_up                                                           |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |

### [HTTP Metrics](docs/http-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| http_requests_total                                                          |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |

### [Instance Metrics](docs/instance-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| instance:node_filesystem_usage:sum                                           |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| instance:node_cpu_utilisation:rate1m                                         |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| instance:node_load1_per_cpu:ratio                                            |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| instance:node_memory_utilisation:ratio                                       |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| instance:node_network_receive_bytes_excluding_lo:rate1m                      |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| instance:node_network_receive_drop_excluding_lo:rate1m                       |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| instance:node_network_transmit_bytes_excluding_lo:rate1m                     |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| instance:node_network_transmit_drop_excluding_lo:rate1m                      |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| instance:node_num_cpu:sum                                                    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| instance:node_vmstat_pgmajfault:rate1m                                       |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| instance_device:node_disk_io_time_seconds:rate1m                             |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| instance_device:node_disk_io_time_weighted_seconds:rate1m                    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |

### [Kubelet Metrics](docs/kubelet-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| kubelet_running_container_count                                              |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| kubelet_runtime_operations                                                   |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| kubelet_runtime_operations_latency_microseconds                              |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| kubelet_volume_stats_available_bytes                                         |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| kubelet_volume_stats_capacity_bytes                                          |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| kube_persistentvolume_status_phase                                           |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |

### [Machine Metrics](docs/machine-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| machine_cpu_cores                                                            |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| machine_memory_bytes                                                         |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |

### [Mixin Metrics](docs/mixin-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| mixin_pod_workload                                                           |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |

### [Node Metrics](docs/node-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| kube_node_labels                                                             |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| kube_node_spec_unschedulable                                                 |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| kube_node_status_allocatable                                                 |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| kube_node_status_allocatable_cpu_cores                                       |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| kube_node_status_allocatable_memory_bytes                                    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| kube_node_status_capacity                                                    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| kube_node_status_capacity_pods                                               |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| kube_node_status_capacity_cpu_cores                                          |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| kube_node_status_condition                                                   |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |

### [OpenShift Metrics](docs/openshift-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| openshift_clusterresourcequota_usage                                         |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| openshift_clusterresourcequota_labels                                        |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |

### [Pod Metrics](docs/pod-metrics.md)

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| kube_pod_container_resource_limits                                           |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| kube_pod_container_resource_limits_cpu_cores                                 |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| kube_pod_container_resource_limits_memory_bytes                              |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| kube_pod_container_resource_requests                                         |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| kube_pod_container_resource_requests_cpu_cores                               |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| kube_pod_container_resource_requests_memory_bytes                            |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| kube_pod_container_status_restarts_total                                     |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| kube_pod_info                                                                |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| kube_pod_owner                                                               |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| kube_pod_status_ready                                                        |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| kube_pod_status_phase                                                        |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| kube_resourcequota                                                           |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |

### Namespace Metrics

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| kube_namespace_labels                                                        |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| namespace:kube_pod_container_resource_requests_cpu_cores:sum                 |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| namespace:kube_pod_container_resource_requests_memory_bytes:sum              |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| namespace:container_memory_usage_bytes:sum                                   |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| namespace_cpu:kube_pod_container_resource_requests:sum                       |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| namespace_pod_name_container_name:container_cpu_usage_seconds_total:sum_rate |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| namespace_workload_pod:kube_pod_owner:relabel                                |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| namespace_workload_pod:kube_pod_owner:relabel                                |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |

### Node Metrics

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| node_cpu_seconds_total                                                       |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| node_disk_bytes_read                                                         |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| node_disk_bytes_written                                                      |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| node_filesystem_avail                                                        |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| node_filesystem_avail_bytes                                                  |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| node_filesystem_free_bytes                                                   |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| node_filesystem_size                                                         |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| node_filesystem_size_bytes                                                   |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| node_memory_MemAvailable_bytes                                               |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| node_memory_MemTotal_bytes                                                   |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| node_namespace_pod_container:container_cpu_usage_seconds_total:sum_rate      |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| node_namespace_pod_container:container_cpu_usage_seconds_total:sum_irate     |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✘     |
| node_netstat_Tcp_OutSegs                                                     |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| node_netstat_Tcp_RetransSegs                                                 |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| node_netstat_TcpExt_TCPSynRetrans                                            |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
| node_network_receive_bytes                                                   |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| node_network_transmit_bytes                                                  |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| node:node_cpu_utilisation:avg1m                                              |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| node:node_disk_utilisation:avg_irate                                         |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| node:node_memory_bytes_total:sum                                             |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| node:node_net_utilisation:sum_irate                                          |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |
| 'node_namespace_pod:kube_pod_info:'                                          |    ✘    |    ✘    |    ✘    |    ✘    |    ✘    |    ✓     |

### Service Metrics

| Metric Name                                                                  | ACM 2.3 | ACM 2.4 | ACM 2.5 | ACM 2.6 | ACM 2.7 | OCP 3.11 |
|------------------------------------------------------------------------------|---------|---------|---------|---------|---------|----------|
| up                                                                           |    ✓    |    ✓    |    ✓    |    ✓    |    ✓    |    ✓     |
