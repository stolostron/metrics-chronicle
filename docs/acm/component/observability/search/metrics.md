# Search Metrics

Nomenclature:

- `Not exposed` implies not in ACM Observability [default allow-list](https://github.com/stolostron/multicluster-observability-operator/blob/main/operators/multiclusterobservability/manifests/base/config/metrics_allowlist.yaml)
- `New` implies just added as a part of ACM 2.6 / ACM 2.7
- `From Managed Cluster` implies these are not emitted from the ACM hub Server but from Managed Cluster

| Metric Name                              | Metric Type | Description | Status |
|------------------------------------------|-------------|-------------|--------|
| acm_search_indexer_http_duration_seconds | histogram   | Time the search indexer takes to process HTTP requests. |  Not exposed, New |
| acm_search_indexer_hits_total            | counter     | The total number of incoming requests to the search indexer. |  Not exposed, New  |
| search_authn_failed_total                | counter     | The total number of authentication requests that has failed. |  Not exposed, New  |
| search_authz_failed_total                | counter     | The total number of authorization requests that has failed.  |  Not exposed, New  |
| search_db_connection_failed_total        | counter     | The total number of DB connection that has failed.   |  Not exposed, New  |
| search_db_connection_success_total       | counter     | The total number of DB connection that has succeeded.  |  Not exposed, New  |
| search_dbquery_duration_seconds          | histogram   | Latency of DB requests in seconds.  |  Not exposed, New   |
| search_http_duration_seconds             | histogram   | Latency of of HTTP requests in seconds.  |  Not exposed, New  |
| search_http_total                        | counter     | Total number HTTP requests. |  Not exposed, New   |

## Insights client

| Metric Name       | Metric Type | Description               | Status |
|-------------------|-------------|---------------------------|--------|
| policyreport_info | gauge       | Failed policy per cluster | STABLE |
