# Node Metrics

| Metric Name                                                              | Metric Type | Description                                                                          | Status |
|--------------------------------------------------------------------------|-------------|--------------------------------------------------------------------------------------|--------|
| kube_node_spec_unschedulable                                             | gauge       | Whether a node can schedule new pods.                                                | STABLE |
| kube_node_status_allocatable                                             | gauge       | The allocatable for different resources of a node that are available for scheduling. | STABLE |
| kube_node_status_allocatable_cpu_cores                                   | gauge       | The CPU resources of a node that are available for scheduling.                       | STABLE |
| kube_node_status_allocatable_memory_bytes                                | gauge       | The memory resources of a node that are available for scheduling.                    | STABLE |
| kube_node_status_capacity                                                | gauge       | The capacity for different resources of a node.                                      | STABLE |
| kube_node_status_capacity_pods                                           | gauge       | The number of pods the node can schedule.                                            | STABLE |
| kube_node_status_capacity_cpu_cores                                      | gauge       | Total CPU capacity of your cluster’s nodes                                           | STABLE |
| kube_node_status_condition                                               | gauge       | The condition of a cluster node.                                                     | STABLE |
| :node_memory_MemAvailable_bytes:sum                                      |             |                                                                                      | STABLE |
| node_cpu_seconds_total                                                   | counter     | Seconds the CPUs spent in each mode.                                                 | STABLE |
| node_filesystem_avail_bytes                                              | gauge       | Filesystem space available to non-root users in bytes.                               | STABLE |
| node_filesystem_free_bytes                                               | gauge       | Filesystem free space in bytes.                                                      | STABLE |
| node_filesystem_size_bytes                                               | gauge       | Filesystem size in bytes.                                                            | STABLE |
| node_memory_MemAvailable_bytes                                           | gauge       | Memory information field MemAvailable_bytes.                                         | STABLE |
| node_namespace_pod_container:container_cpu_usage_seconds_total:sum_rate  |             |                                                                                      | STABLE |
| node_namespace_pod_container:container_cpu_usage_seconds_total:sum_irate |             |                                                                                      | STABLE |
| node_netstat_Tcp_OutSegs                                                 | untyped     | Statistic TcpOutSegs.                                                                | STABLE |
| node_netstat_Tcp_RetransSegs                                             | untyped     | Statistic TcpRetransSegs.                                                            | STABLE |
| node_netstat_TcpExt_TCPSynRetrans                                        | untyped     | Statistic TcpExtTCPSynRetrans.                                                       | STABLE |
