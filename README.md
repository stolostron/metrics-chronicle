# Metrics Chronicle Overview

Metrics are used to monitor the health of your fleet across components. Continue reading to view the version compatibility table for the exposed metrics and labels used in Red Hat Advanced Cluster Management for Kubernetes (RHACM).

## Compatibility Table

- [Alerts Metrics](#alerts-metrics)
- [Assisted Installer Metrics](#assisted-installer-metrics)
- [Authenticated Metrics](#authenticated-metrics)
- [Cluster Metrics](#cluster-metrics)
- [Container Metrics](#container-metrics)
- [Coredns Metrics](#coredns-metrics)
- [Daemonset Metrics](#daemonset-metrics)
- [ETCD Metrics](#etcd-metrics)
- [GRPC Metrics](#grpc-metrics)
- [Haproxy Metrics](#haproxy-metrics)
- [HTTP Metrics](#http-metrics)
- [Instance Metrics](#instance-metrics)
- [Kubelet Metrics](#kubelet-metrics)
- [Machine Metrics](#machine-metrics)
- [Mixin Metrics](#mixin-metrics)
- [Node Metrics](#node-metrics)
- [OpenShift Metrics](#openshift-metrics)
- [Pod Metrics](#pod-metrics)
- [Namespace Metrics](#namespace-metrics)
- [Kubelet Node Metrics](#node-metrics)
- [Service Metrics](#service-metrics)

### Alerts Metrics

| Metric Name                         | ACM 2.5            | ACM 2.6            | ACM 2.7            | ACM 2.8            |
|-------------------------------------|--------------------|--------------------|--------------------|--------------------|
| :node_memory_MemAvailable_bytes:sum | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| ALERTS                              | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |

### Assisted Installer Metrics

| Metric Name                                           | ACM 2.5            | ACM 2.6            | ACM 2.7            | ACM 2.8            |
|-------------------------------------------------------|--------------------|--------------------|--------------------|--------------------|
| assisted_installer_cluster_creation                   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| assisted_installer_cluster_installation_started       | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| assisted_installer_cluster_installation_second        | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| assisted_installer_cluster_host_installation_count    | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| assisted_installer_host_installation_phase_seconds    | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| assisted_installer_cluster_host_disk_sync_duration_ms | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| assisted_installer_cluster_host_image_pull_status     | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| assisted_installer_filesystem_usage_percentage        | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |

### Authenticated Metrics

| Metric Name                 | ACM 2.5            | ACM 2.6            | ACM 2.7            | ACM 2.8            |
|-----------------------------|--------------------|--------------------|--------------------|--------------------|
| authenticated_user_requests | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| authentication_attempts     | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |

### Cluster Metrics

| Metric Name                                          | ACM 2.5            | ACM 2.6            | ACM 2.7            | ACM 2.8            |
|------------------------------------------------------|--------------------|--------------------|--------------------|--------------------|
| cluster:capacity_cpu_cores:sum                       | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| cluster:capacity_memory_bytes:sum                    | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| cluster:container_cpu_usage:ratio                    | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| cluster:container_spec_cpu_shares:ratio              | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| cluster:cpu_usage_cores:sum                          | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| cluster:memory_usage:ratio                           | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| cluster:memory_usage_bytes:sum                       | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| cluster:usage:resources:sum                          | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| cluster_infrastructure_provider                      | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| cluster_monitoring_operator_reconcile_errors_total   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| cluster_monitoring_operator_reconcile_attempts_total | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| cluster_operator_conditions                          | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| cluster_operator_up                                  | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| cluster_version                                      | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| cluster_version_payload                              | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |

### Container Metrics

| Metric Name                                      | ACM 2.5            | ACM 2.6            | ACM 2.7            | ACM 2.8            |
|--------------------------------------------------|--------------------|--------------------|--------------------|--------------------|
| container_cpu_cfs_periods_total                  | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| container_cpu_cfs_throttled_periods_total        | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| container_cpu_usage_seconds_total                |         :x:        |         :x:        |         :x:        |         :x:        |
| container_memory_rss                             |         :x:        |         :x:        |         :x:        |         :x:        |
| container_memory_usage_bytes                     |         :x:        |         :x:        |         :x:        |         :x:        |
| container_network_receive_bytes_total            |         :x:        |         :x:        |         :x:        |         :x:        |
| container_network_receive_bytes_total            |         :x:        |         :x:        |         :x:        |         :x:        |
| container_network_receive_packets_total          |         :x:        |         :x:        |         :x:        |         :x:        |
| container_network_receive_packets_dropped_total  |         :x:        |         :x:        |         :x:        |         :x:        |
| container_network_transmit_bytes_total           |         :x:        |         :x:        |         :x:        |         :x:        |
| container_network_transmit_packets_total         |         :x:        |         :x:        |         :x:        |         :x:        |
| container_network_transmit_packets_dropped_total |         :x:        |         :x:        |         :x:        |         :x:        |
| container_spec_cpu_quota                         | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |

### Coredns Metrics

| Metric Name                              | ACM 2.5            | ACM 2.6            | ACM 2.7            | ACM 2.8            |
|------------------------------------------|--------------------|--------------------|--------------------|--------------------|
| coredns_dns_request_count_total          | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| coredns_dns_request_duration_seconds_sum | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| coredns_dns_request_type_count_total     | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| coredns_dns_response_rcode_count_total   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |

### Daemonset Metrics

| Metric Name                                    | ACM 2.5            | ACM 2.6            | ACM 2.7            | ACM 2.8            |
|------------------------------------------------|--------------------|--------------------|--------------------|--------------------|
| kube_daemonset_status_desired_number_scheduled | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| kube_daemonset_status_number_unavailable       | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |

### ETCD Metrics

| Metric Name                                         | ACM 2.5            | ACM 2.6            | ACM 2.7            | ACM 2.8            |
|-----------------------------------------------------|--------------------|--------------------|--------------------|--------------------|
| etcd_debugging_mvcc_db_total_size_in_bytes          | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| etcd_debugging_snap_save_total_duration_seconds_sum | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| etcd_mvcc_db_total_size_in_bytes                    | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| etcd_disk_backend_commit_duration_seconds_bucket    | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| etcd_disk_backend_commit_duration_seconds_sum       | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| etcd_disk_wal_fsync_duration_seconds_bucket         | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| etcd_disk_wal_fsync_duration_seconds_sum            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| etcd_object_counts                                  | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| etcd_network_client_grpc_received_bytes_total       | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| etcd_network_client_grpc_sent_bytes_total           | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| etcd_network_peer_received_bytes_total              | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| etcd_network_peer_sent_bytes_total                  | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| etcd_server_client_requests_total                   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| etcd_server_has_leader                              | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| etcd_server_health_failures                         | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| etcd_server_leader_changes_seen_total               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| etcd_server_proposals_failed_total                  | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| etcd_server_proposals_pending                       | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| etcd_server_proposals_committed_total               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| etcd_server_proposals_applied_total                 | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| etcd_server_quota_backend_bytes                     | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |

### GRPC Metrics

| Metric Name               | ACM 2.5            | ACM 2.6            | ACM 2.7            | ACM 2.8            |
|---------------------------|--------------------|--------------------|--------------------|--------------------|
| grpc_server_started_total | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |

### Haproxy Metrics

| Metric Name                                                | ACM 2.5            | ACM 2.6            | ACM 2.7            | ACM 2.8            |
|------------------------------------------------------------|--------------------|--------------------|--------------------|--------------------|
| haproxy_backend_connection_errors_total                    | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| haproxy_backend_connections_total                          | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| haproxy_backend_current_queue                              | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| haproxy_backend_http_average_response_latency_milliseconds | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| haproxy_backend_max_sessions                               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| haproxy_backend_response_errors_total                      | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| haproxy_backend_up                                         | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |

### HTTP Metrics

| Metric Name         | ACM 2.5            | ACM 2.6            | ACM 2.7            | ACM 2.8            |
|---------------------|--------------------|--------------------|--------------------|--------------------|
| http_requests_total | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |

### Instance Metrics

| Metric Name                                               | ACM 2.5            | ACM 2.6            | ACM 2.7            | ACM 2.8            |
|-----------------------------------------------------------|--------------------|--------------------|--------------------|--------------------|
| instance:node_filesystem_usage:sum                        | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| instance:node_cpu_utilisation:rate1m                      | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| instance:node_load1_per_cpu:ratio                         | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| instance:node_memory_utilisation:ratio                    | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| instance:node_network_receive_bytes_excluding_lo:rate1m   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| instance:node_network_receive_drop_excluding_lo:rate1m    | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| instance:node_network_transmit_bytes_excluding_lo:rate1m  | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| instance:node_network_transmit_drop_excluding_lo:rate1m   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| instance:node_num_cpu:sum                                 | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| instance:node_vmstat_pgmajfault:rate1m                    | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| instance_device:node_disk_io_time_seconds:rate1m          | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| instance_device:node_disk_io_time_weighted_seconds:rate1m | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |

### Kubelet Metrics

| Metric Name                                     | ACM 2.5            | ACM 2.6            | ACM 2.7            | ACM 2.8            |
|-------------------------------------------------|--------------------|--------------------|--------------------|--------------------|
| kubelet_running_container_count                 | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| kubelet_runtime_operations                      | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| kubelet_runtime_operations_latency_microseconds | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| kubelet_volume_stats_available_bytes            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| kubelet_volume_stats_capacity_bytes             | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| kube_persistentvolume_status_phase              | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |

### Machine Metrics

| Metric Name          | ACM 2.5            | ACM 2.6            | ACM 2.7            | ACM 2.8            |
|----------------------|--------------------|--------------------|--------------------|--------------------|
| machine_cpu_cores    | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| machine_memory_bytes | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |

### Mixin Metrics

| Metric Name        | ACM 2.5            | ACM 2.6            | ACM 2.7            | ACM 2.8            |
|--------------------|--------------------|--------------------|--------------------|--------------------|
| mixin_pod_workload | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |

### Kubelet Node Metrics

| Metric Name                                | ACM 2.5            | ACM 2.6            | ACM 2.7            | ACM 2.8            |
|--------------------------------------------|--------------------|--------------------|--------------------|--------------------|
| kube_node_labels                           |         :x:        |         :x:        |         :x:        |         :x:        |
| kube_node_spec_unschedulable               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| kube_node_status_allocatable               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| kube_node_status_allocatable_cpu_cores     | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| kube_node_status_allocatable_memory_bytes  | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| kube_node_status_capacity                  | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| kube_node_status_capacity_pods             | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| kube_node_status_capacity_cpu_cores        | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| kube_node_status_condition                 | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |

### OpenShift Metrics

| Metric Name                           | ACM 2.5 | ACM 2.6 | ACM 2.7 | ACM 2.8 |
|---------------------------------------|---------|---------|---------|---------|
| openshift_clusterresourcequota_usage  |   :x:   |   :x:   |   :x:   |   :x:   |
| openshift_clusterresourcequota_labels |   :x:   |   :x:   |   :x:   |   :x:   |

### Pod Metrics

| Metric Name                                       | ACM 2.5            | ACM 2.6            | ACM 2.7            | ACM 2.8            |
|---------------------------------------------------|--------------------|--------------------|--------------------|--------------------|
| kube_pod_container_resource_limits                | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| kube_pod_container_resource_limits_cpu_cores      | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| kube_pod_container_resource_limits_memory_bytes   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| kube_pod_container_resource_requests              | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| kube_pod_container_resource_requests_cpu_cores    | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| kube_pod_container_resource_requests_memory_bytes | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| kube_pod_container_status_restarts_total          |         :x:        |         :x:        |         :x:        |         :x:        |
| kube_pod_info                                     | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| kube_pod_owner                                    | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| kube_pod_status_ready                             |         :x:        |         :x:        |         :x:        |         :x:        |
| kube_pod_status_phase                             |         :x:        |         :x:        |         :x:        |         :x:        |
| kube_resourcequota                                | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |

### Namespace Metrics

| Metric Name                                                                  | ACM 2.5            | ACM 2.6            | ACM 2.7            | ACM 2.8            |
|------------------------------------------------------------------------------|--------------------|--------------------|--------------------|--------------------|
| kube_namespace_labels                                                        |         :x:        |         :x:        |         :x:        |         :x:        |
| namespace:kube_pod_container_resource_requests_cpu_cores:sum                 | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| namespace:kube_pod_container_resource_requests_memory_bytes:sum              | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| namespace:container_memory_usage_bytes:sum                                   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| namespace_cpu:kube_pod_container_resource_requests:sum                       | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| namespace_pod_name_container_name:container_cpu_usage_seconds_total:sum_rate | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| namespace_workload_pod:kube_pod_owner:relabel                                | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| namespace_workload_pod:kube_pod_owner:relabel                                | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |

### Node Metrics

| Metric Name                                                              | ACM 2.5            | ACM 2.6            | ACM 2.7            | ACM 2.8            |
|--------------------------------------------------------------------------|--------------------|--------------------|--------------------|--------------------|
| node_cpu_seconds_total                                                   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| node_disk_bytes_read                                                     |         :x:        |         :x:        |         :x:        |         :x:        |
| node_disk_bytes_written                                                  |         :x:        |         :x:        |         :x:        |         :x:        |
| node_filesystem_avail                                                    |         :x:        |         :x:        |         :x:        |         :x:        |
| node_filesystem_avail_bytes                                              | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| node_filesystem_free_bytes                                               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| node_filesystem_size                                                     |         :x:        |         :x:        |         :x:        |         :x:        |
| node_filesystem_size_bytes                                               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| node_memory_MemAvailable_bytes                                           | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| node_memory_MemTotal_bytes                                               |         :x:        |         :x:        |         :x:        |         :x:        |
| node_namespace_pod_container:container_cpu_usage_seconds_total:sum_rate  | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| node_namespace_pod_container:container_cpu_usage_seconds_total:sum_irate | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| node_netstat_Tcp_OutSegs                                                 | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| node_netstat_Tcp_RetransSegs                                             | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| node_netstat_TcpExt_TCPSynRetrans                                        | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| node_network_receive_bytes                                               |         :x:        |         :x:        |         :x:        |         :x:        |
| node_network_transmit_bytes                                              |         :x:        |         :x:        |         :x:        |         :x:        |
| node:node_cpu_utilisation:avg1m                                          |         :x:        |         :x:        |         :x:        |         :x:        |
| node:node_disk_utilisation:avg_irate                                     |         :x:        |         :x:        |         :x:        |         :x:        |
| node:node_memory_bytes_total:sum                                         |         :x:        |         :x:        |         :x:        |         :x:        |
| node:node_net_utilisation:sum_irate                                      |         :x:        |         :x:        |         :x:        |         :x:        |
| 'node_namespace_pod:kube_pod_info:'                                      |         :x:        |         :x:        |         :x:        |         :x:        |

### Service Metrics

| Metric Name | ACM 2.5            | ACM 2.6            | ACM 2.7            | ACM 2.8            |
|-------------|--------------------|--------------------|--------------------|--------------------|
| up          | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |


View a list of metrics for each component in the [`metric-chronicle/docs`](https://github.com/stolostron/metrics-chronicle/blob/main/docs/):

* [Alerts Metrics](docs/alert-metrics.md)
* [Assisted Installer Metrics](docs/installer-metrics.md)
* [Authenticated Metrics](docs/authentication-metrics.md)
* [Cluster Metrics](docs/cluster-metrics.md)
* [Container Metrics](docs/container-metrics.md)
* [Coredns Metrics](docs/coredns-metrics.md)
* [Daemonset Metrics](docs/daemonset-metrics.md)
* [ETCD Metrics](docs/etcd-metrics.md)
* [GRPC Metrics](docs/grpc-metrics.md)
* [Haproxy Metrics](docs/haproxy-metrics.md)
* [HTTP Metrics](docs/http-metrics.md)
* [Instance Metrics](docs/instance-metrics.md)
* [Kubelet Metrics](docs/kubelet-metrics.md)
* [Machine Metrics](docs/machine-metrics.md)
* [Mixin Metrics](docs/mixin-metrics.md)
* [Node Metrics](docs/node-metrics.md)
* [OpenShift Metrics](docs/openshift-metrics.md)
* [Pod Metrics](docs/pod-metrics.md)
