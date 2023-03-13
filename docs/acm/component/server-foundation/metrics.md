# Server Foundation Metrics

Nomenclature:

- `Not exposed` implies not in ACM Observability [default allow-list](https://github.com/stolostron/multicluster-observability-operator/blob/main/operators/multiclusterobservability/manifests/base/config/metrics_allowlist.yaml)
- `New` implies just added as a part of ACM 2.6 / ACM 2.7
- `From Managed Cluster` implies these are not emitted from the ACM hub Server but from Managed Cluster.

| Metric Name                                             | Metric Type | Description | Status |
|---------------------------------------------------------|-------------|-------------|--------|
| acm_managed_cluster_labels  | gauge  | Managed cluster labels | STABLE  |
| acm_managed_cluster_info   | gauge | Managed cluster information | Not exposed, STABLE   |
| acm_managed_cluster_count  | - | Managed cluster count | Not exposed, STABLE |
| acm_managed_cluster_addon_status_condition | gauge | Managed cluster addon status condition | Not exposed, New |
| acm_managed_cluster_status_condition | gauge | Managed cluster status condition | Not exposed, New |
| acm_manifestwork_status_condition | gauge | Manifestwork status condition | Not exposed, New |
| acm_manifestwork_count | - | Manifestwork count | Not exposed, New |
