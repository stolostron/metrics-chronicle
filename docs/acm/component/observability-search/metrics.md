# Search Metrics

Nomenclature:

- `Not exposed` implies not in ACM Observability [default allow-list](https://github.com/stolostron/multicluster-observability-operator/blob/main/operators/multiclusterobservability/manifests/base/config/metrics_allowlist.yaml)
- `New` implies just added as a part of ACM 2.6 / ACM 2.7
- `From Managed Cluster` implies these are not emitted from the ACM hub Server but from Managed Cluster

| Metric Name                         | Metric Type | Description  | Status  |
| ------------------------------------| ----------- | ------------ | --------|
| search_api_request_duration         | histogram   | Time (seconds) the search api took to process the request | Not exposed, New |
| search_api_db_connection_failed     | counter     | The number of failed database connection attempts.        | Not exposed, New |
| search_api_db_query_duration        | histogram   | Latency (seconds) for database queries.                   | Not exposed, New |
| search_indexer_request_count        | counter     | Total requests received by the search indexer (from managed clusters).| Not exposed, New |
| search_indexer_request_duration     | histogram   | Time (seconds) the search indexer takes to process a request (from managed cluster).| Not exposed, New |
| search_indexer_requests_in_flight   | gauge       | Total requests the search indexer is processing at a given time.| Not exposed, New |
| search_indexer_request_size         | histogram   | Total changes (add, update, delete) in the search indexer request (from managed cluster). Not exposed, New |


## Insights Client

| Metric Name       | Metric Type | Description               | Status |
|-------------------|-------------|---------------------------|--------|
| policyreport_info | gauge       | Failed policy per cluster | STABLE |
