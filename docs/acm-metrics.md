# Advanced Cluster Management (ACM) Metrics

| Metric Name                                                                           | Metric Type | Labels/Tags | Status |
|---------------------------------------------------------------------------------------|-------------|-------------|--------|
| [acm_search_indexer_http_duration_seconds](#acm_search_indexer_http_duration_seconds) |             |             |        |
| [acm_search_indexer_hits_total](#acm_search_indexer_hits_total)                       |             |             |        |
| [search_http_duration_seconds](#search_http_duration_seconds)                         |             |             |        |
| [search_http_total](#search_http_total)                                               |             |             |        |
| [search_authn_failed_total](#search_authn_failed_total)                               |             |             |        |
| [search_authz_failed_total](#search_authz_failed_total)                               |             |             |        |
| [search_db_connection_failed_total](#search_db_connection_failed_total)               |             |             |        |
| [search_db_connection_success_total](#search_db_connection_success_total)             |             |             |        |
| [search_dbquery_duration_seconds](#search_dbquery_duration_seconds)                   |             |             |        |

## Metrics Descriptions

### acm_search_indexer_http_duration_seconds

- Time the search indexer takes to process HTTP requests.

### acm_search_indexer_hits_total

- The total number of incoming requests to the search indexer.

### search_http_duration_seconds

- Latency of of HTTP requests in seconds.

### search_http_total

- Total number HTTP requests.

### search_authn_failed_total

- The total number of authentication requests that has failed

### search_authz_failed_total

- The total number of authorization requests that has failed

### search_db_connection_failed_total

- The total number of DB connection that has failed

### search_db_connection_success_total

- The total number of DB connection that has succeeded

### search_dbquery_duration_seconds

- Latency of DB requests in seconds.
