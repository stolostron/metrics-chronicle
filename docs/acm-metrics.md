# Advanced Cluster Management (ACM) Metrics

Nomenclature:
- `Not exposed` implies not in ACM Observability [default allow-list](https://github.com/stolostron/multicluster-observability-operator/blob/main/operators/multiclusterobservability/manifests/base/config/metrics_allowlist.yaml)
- `New` implies just added as a part of ACM 2.6 / ACM 2.7
- `From Managed Cluster` implies these are not emitted from the ACM hub Server but from Managed Cluster

## Server Foundation Metrics

| Metric Name                                             | Metric Type | Description | Status |
|---------------------------------------------------------|-------------|-------------|--------|
| acm_managed_cluster_labels  | gauge  | Managed cluster labels | STABLE  |
| acm_managed_cluster_info   | gauge | Managed cluster information | Not exposed, STABLE   |
| acm_managed_cluster_count  | - | Managed cluster count | Not exposed, STABLE |
| acm_managed_cluster_addon_status_condition | gauge | Managed cluster addon status condition | Not exposed, New |
| acm_managed_cluster_status_condition | gauge | Managed cluster status condition | Not exposed, New |
| acm_manifestwork_status_condition | gauge | Manifestwork status condition | Not exposed, New |
| acm_manifestwork_count | - | Manifestwork count | Not exposed, New |


## Governance Risk and Compliance Framework Metrics

| Metric Name                                             | Metric Type | Description | Status |
|---------------------------------------------------------|-------------|-------------|--------|
| cluster:policy_governance_info:propagated_count         |recording rule |Total policies propagated per cluster| STABLE|
| cluster:policy_governance_info:propagated_noncompliant_count|recording rule |Total non-compliant policies propagated per cluster| STABLE|
| policy:policy_governance_info:propagated_count          |recording rule |Total policies propagated by count| STABLE|
| policy:policy_governance_info:propagated_noncompliant_count|recording rule |Total non-compliant policies propagated by count| STABLE|
| policy_governance_info| gauge | Compliance per cluster per policy | exposed through recording rule, STABLE|
| policy_propagation_failure_total | counter | Number of failed policy propagation per policy | Not exposed, New |
| policy_user_errors_total | counter | Number of user errors encountered while processing policy | Not exposed, New |
| config_policy_evaluation_seconds_total|counter | The total seconds taken while evaluating the configuration policy. Use this alongside config_policy_evaluation_total. This allows you to detect Configuration Policies that are slow and maybe causing excessive load on the Kubernetes API server. | From managed cluster. Not exposed, New |
| config_policy_evaluation_total| counter |The total number of evaluations per policy. If this time series does not have a value in the past N seconds, it means there is an outage. N would be the shortest evaluation interval (defaults to 10s) of all the configured policies.| From managed cluster. Not exposed, New |
| config_policies_evaluation_duration_seconds_bucket | counter |The total count of observations for a bucket in the histogram: The seconds that it takes to evaluate all configuration policies on the cluster| Not exposed, New |
| config_policies_evaluation_duration_seconds_count |counter | The number of observations for: The seconds that it takes to evaluate all configuration policies on the cluster | Not exposed, New |
| config_policies_evaluation_duration_seconds_sum| counter | The seconds that it takes to evaluate all configuration policies that are ready for evaluation on the cluster. A value over 10 seconds starts to indicate some level of saturation.| From managed cluster. Not exposed, New |
| config_policy_templates_process_seconds_total | counter | The total seconds taken while processing configuration policy templates. | Not exposed, New |
| config_policy_templates_process_total | counter | The total number of processes of configuration policy templates.| Not exposed, New |
| ocm_handle_root_policy_duration_seconds_bucket_bucket | counter | The total count of observations for a bucket in the histogram: Time the handleRootPolicy takes to complete. | Not exposed, New |
| ocm_handle_root_policy_duration_seconds_bucket_count | counter | The total number of observations for: Time the handleRootPolicy takes to complete. | Not exposed, New |
| ocm_handle_root_policy_duration_seconds_bucket_sum | counter| The total sum of observations for: Time the handleRootPolicy takes to complete. | Not exposed, New |

## Governance Risk and Compliance Framework Diagnostic using existing Metrics

| Calculation                                             | Description  |
|---------------------------------------------------------|--------------|
| workqueue_depth{name="policy-status-sync"} | The number of events that could be policy status events that are waiting to be processed. If this is high, then the status updates will be slow to show up on the Hub. |
| controller_runtime_reconcile_errors_total{controller="policy-status-sync"} | The total number of errors when processing new statuses from the managed cluster policy controllers. If this is consistently high, this likely indicates that Policy status updates are not being sent back to the Hub. |
| workqueue_depth{name="policy-status-sync"} | The number of events that could be policy status events that are waiting to be processed. If this is high, then the controller is overwhelmed or stuck. Status updates will be slow. |
| workqueue_depth{name="policy-spec-sync"} | The number of policy changes that are waiting to be synced from the Hub. If this is high, then policy changes will be slow to reflect on the managed cluster. Policy updates are rather infrequent so if the queue gets large, that is signaling a larger problem. |
| workqueue_depth{name="policy-template-sync"} | The number of policy templates (e.g. ConfigurationPolicy) that are awaiting to be created/updated on the managed cluster from the synced replicated policies. If this is high, then policy changes will be slow to reflect on the managed cluster. Policy updates are rather infrequent so if the queue gets large, that is signaling a larger problem. |
| controller_runtime_reconcile_errors_total{controller="policy-spec-sync"} | The total number of errors when syncing updates to policies from the Hub to the managed cluster. If this is consistently high, this likely indicates an outage. |
| controller_runtime_reconcile_time_seconds_bucket{controller="policy-propagator",le="10"} | Latency can be determined by reconcile bucket not showing completed reconciles |
| controller_runtime_reconcile_errors_total{controller="policy-encryption-keys"} ||
| controller_runtime_reconcile_errors_total{controller="policy-propagator"} ||
| controller_runtime_reconcile_errors_total{controller="policy-set"} ||
| controller_runtime_reconcile_total{controller="policy-propagator",result="success"} | Should show reconciles complete as opposed to requeue or error results |


## Insights client

| Metric Name       | Metric Type | Description | Status |
|-------------------|-------------|-------------|--------|
| policyreport_info | gauge |Failed policy per cluster |STABLE |

## Search Metrics

| Metric Name                                             | Metric Type | Description | Status |
|---------------------------------------------------------|-------------|-------------|--------|
| search_authn_failed_total| counter  | The total number of authentication requests that has failed. |  Not exposed, New  |
| search_authz_failed_total  | counter | The total number of authorization requests that has failed.  |  Not exposed, New  |
| search_db_connection_failed_total  | counter  | The total number of DB connection that has failed.   |  Not exposed, New  |
| search_db_connection_success_total  | counter | The total number of DB connection that has succeeded.  |  Not exposed, New  |
| search_dbquery_duration_seconds  | histogram  | Latency of DB requests in seconds.  |  Not exposed, New   |
| search_http_duration_seconds  | histogram | Latency of of HTTP requests in seconds.  |  Not exposed, New  |
| search_http_total  | counter | Total number HTTP requests. |  Not exposed, New   |
| acm_search_indexer_http_duration_seconds | histogram | Time the search indexer takes to process HTTP requests. |  Not exposed, New |
| acm_search_indexer_hits_total  | counter  | The total number of incoming requests to the search indexer. |  Not exposed, New  |


## Observability Metrics



