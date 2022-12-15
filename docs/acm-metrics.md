# Advanced Cluster Management (ACM) Metrics

| Metric Name                                                  | Metric Type | Description                                                  | Status      |
|--------------------------------------------------------------|-------------|--------------------------------------------------------------|-------------|
| acm_managed_cluster_info                                     | gauge       | Managed cluster information                                  | STABLE      |
| acm_managed_cluster_labels                                   | gauge       | Managed cluster labels                                       | STABLE      |
| acm_search_indexer_http_duration_seconds                     | histogram   | Time the search indexer takes to process HTTP requests.      | STABLE      |
| acm_search_indexer_hits_total                                | counter     | The total number of incoming requests to the search indexer. | STABLE      |
| cluster:policy_governance_info:propagated_count              |             |                                                              | STABLE      |
| cluster:policy_governance_info:propagated_noncompliant_count |             |                                                              | STABLE      |
| policy:policy_governance_info:propagated_count               |             |                                                              | STABLE      |
| policy:policy_governance_info:propagated_noncompliant_count  |             |                                                              | STABLE      |
| policyreport_info                                            | gauge       | Open Cluster Management PolicyReport Info.                   | STABLE      |
| search_authn_failed_total                                    | counter     | The total number of authentication requests that has failed. | STABLE      |
| search_authz_failed_total                                    | counter     | The total number of authorization requests that has failed.  | STABLE      |
| search_db_connection_failed_total                            | counter     | The total number of DB connection that has failed.           | STABLE      |
| search_db_connection_success_total                           | counter     | The total number of DB connection that has succeeded.        | STABLE      |
| search_dbquery_duration_seconds                              | histogram   | Latency of DB requests in seconds.                           | STABLE      |
| search_http_duration_seconds                                 | histogram   | Latency of of HTTP requests in seconds.                      | STABLE      |
| search_http_total                                            | counter     | Total number HTTP requests.                                  | STABLE      |
