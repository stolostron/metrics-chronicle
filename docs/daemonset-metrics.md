# Daemonset Metrics

| Metric Name                                    | Metric Type | Description                                                                                                     | Status |
|------------------------------------------------|-------------|-----------------------------------------------------------------------------------------------------------------|--------|
| kube_daemonset_status_desired_number_scheduled | gauge       | The number of nodes that should be running the daemon pod.                                                      | STABLE |
| kube_daemonset_status_number_unavailable       | gauge       | The number of nodes that should be running the daemon pod and have none of the daemon pod running and available | STABLE |
