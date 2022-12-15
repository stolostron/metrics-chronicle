# Kubelet Metrics

| Metric Name                                     | Metric Type | Description                                                                             | Status |
|-------------------------------------------------|-------------|-----------------------------------------------------------------------------------------|--------|
| kubelet_running_container_count                 | gauge       | The number of containers that are currently running.                                    |        |
| kubelet_runtime_operations                      | counter     | The cumulative number of runtime operations available by the different operation types. |        |
| kubelet_runtime_operations_latency_microseconds | gauge       | The latency of each operation by type in microseconds.                                  |        |
| kubelet_volume_stats_available_bytes            | gauge       | The per-PVC free space in bytes.                                                        |        |
| kubelet_volume_stats_capacity_bytes             | gauge       | The per-PVC capacity in bytes.                                                          |        |
