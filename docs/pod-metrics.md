# Pod Metrics

| Metric Name                                       | Metric Type | Description                                                     | Status |
|---------------------------------------------------|-------------|-----------------------------------------------------------------|--------|
| kube_pod_container_resource_limits                | gauge       | The number of requested limit resource by a pod container.      | STABLE |
| kube_pod_container_resource_limits_cpu_cores      | gauge       | The number of CPU cores requested limit resource by a container | STABLE |
| kube_pod_container_resource_limits_memory_bytes   | gauge       | Total memory limits (bytes) of a pod container.                 | STABLE |
| kube_pod_container_resource_requests              | gauge       | The number of requested request resource by a pod container.    | STABLE |
| kube_pod_container_resource_requests_cpu_cores    | gauge       | The number of CPU cores requested by a pod container.           | STABLE |
| kube_pod_container_resource_requests_memory_bytes | gauge       | Total memory requests (bytes) of a pod container.               | STABLE |
| kube_pod_info                                     | gauge       | Information about pod.                                          | STABLE |
| kube_pod_owner                                    | gauge       | Information about the Pod's owner.                              | STABLE |
