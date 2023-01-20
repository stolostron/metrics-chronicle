# ACM Search Metrics

| Metric Name                                                                   | Metric Type | Description                                                  | Status |
|-------------------------------------------------------------------------------|-------------|--------------------------------------------------------------|--------|
| acm_search_indexer_http_duration_seconds                                      | histogram   | Time the search indexer takes to process HTTP requests.      | STABLE |
| acm_search_indexer_hits_total                                                 | counter     | The total number of incoming requests to the search indexer. | STABLE |
| search_authz_failed_total                                                     | counter     | The total number of authorization requests that has failed.  | STABLE |
| search_db_connection_failed_total                                             | counter     | The total number of DB connection that has failed.           | STABLE |
| search_db_connection_success_total                                            | counter     | The total number of DB connection that has succeeded.        | STABLE |
| search_dbquery_duration_seconds                                               | histogram   | Latency of DB requests in seconds.                           | STABLE |
| search_http_duration_seconds                                                  | histogram   | Latency of of HTTP requests in seconds.                      | STABLE |
| search_http_total                                                             | counter     | Total number HTTP requests.                                  | STABLE |
