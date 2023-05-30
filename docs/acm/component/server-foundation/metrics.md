# Server Foundation Metrics

Nomenclature:

- `Not exposed` implies not in ACM Observability [default allow-list](https://github.com/stolostron/multicluster-observability-operator/blob/main/operators/multiclusterobservability/manifests/base/config/metrics_allowlist.yaml)
- `New` implies just added as a part of ACM 2.6 / ACM 2.7
- `From Managed Cluster` implies these are not emitted from the ACM hub Server but from Managed Cluster.

| Metric Name                                             | Metric Type | Description | Labels | Status |
|---------------------------------------------------------|-------------|-------------|-------|--------|
| acm_managed_cluster_labels  | gauge  | Managed cluster labels | <table> <tr> <th>Number</th> <th>Label</th> <th>Description</th></tr> <tr> <td>1</td> <td>`hub_cluster_id`</td> <td>The cluster ID of the hub cluster.</td> </tr> <tr> <td>2</td> <td>`managed_cluster_id`</td> <td>The managed cluster ID is the cluster ID if the managed cluster is an {ocp-short} cluster, otherwise it is the cluster name.</td> </tr> </table> | STABLE  |
| acm_managed_cluster_info   | gauge | Managed cluster information | <table> <tr> <th>Number</th> <th>Label</th> <th>Description</th> </tr> <tr> <td>1</td> <td>`hub_cluster_id`</td> <td>The cluster ID of the hub cluster.</td> </tr> <tr> <td>2</td> <td>`managed_cluster_id`</td> <td>The managed cluster ID is the cluster ID if the managed cluster is an {ocp-short} cluster, otherwise it is the cluster name.</td> </tr> <tr> <td>3</td> <td>`vendor`</td> <td>The label `vendor` of the managed cluster.</td> </tr> <tr> <td>4</td> <td>`cloud`</td> <td>The label `cloud` of the managed cluster.</td> </tr> <tr> <td>5</td> <td>`service_name`</td> <td>The annotation `open-cluster-management/service-name` of the managed cluster. The values are `Compute` and `Other`.</td> </tr> <tr> <td>6</td> <td>`created_via`</td> <td>The annotation `open-cluster-management/created-via` updated by MCE. The supported values are `Discovery`,`AssistedInstaller`,`Hive` and `Other`.</td> </tr> <tr> <td>7</td> <td>`version`</td> <td>The {ocp-short} version if the managed cluster is an {ocp-short} cluster, otherwise is the Kubernetes version.</td> </tr> <tr> <td>8</td> <td>`available`</td> <td>The condition `ManagedClusterConditionAvailable` of the managed cluster. The values are `True` and `False`.</td> </tr> <tr> <td>9</td> <td>`core_worker`</td> <td>The core count of worker nodes on the managed cluster.</td> </tr> <tr> <td>10</td> <td>`socket_worker`</td> <td>The socket count of worker nodes on the {ocp-short} cluster.</td> </tr></table> |  Not exposed, STABLE   |
| acm_managed_cluster_count  | - | Managed cluster count | |  Not exposed, STABLE |
| acm_managed_cluster_addon_status_condition | gauge | Managed cluster addon status condition | | Not exposed, New |
| acm_managed_cluster_status_condition | gauge | Managed cluster status condition | | Not exposed, New |
| acm_manifestwork_status_condition | gauge | Manifestwork status condition | | Not exposed, New |
| acm_manifestwork_count | - | Manifestwork count | | Not exposed, New |
