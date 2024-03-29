# Observability Metrics

Nomenclature:

- `Not exposed` implies not in ACM Observability [default allow-list](https://github.com/stolostron/multicluster-observability-operator/blob/main/operators/multiclusterobservability/manifests/base/config/metrics_allowlist.yaml)
- `New` implies just added as a part of ACM 2.6 / ACM 2.7
- `From Managed Cluster` implies these are not emitted from the ACM hub Server but from Managed Cluster

| Metric Name | Metric Type | Description                      | Status |
|---------------------------------------------------------|-------------|----------------------------------|--------|
| acm_configmap_reload_watcher_errors_total               | counter     | Total filesystem watcher errors. | STABLE |
| acm_cortex_cache_background_queue_length                | gauge       | Length of the cache background write queue. | STABLE |
| acm_cortex_cache_dropped_background_writes_total        | counter     | Total count of dropped write backs to cache. | STABLE |
| acm_cortex_cache_fetched_keys                           | counter     | Total count of keys requested from cache. | STABLE |
| acm_cortex_cache_hits                                   | counter     | Total count of keys found in cache. | STABLE |
| acm_cortex_cache_request_duration_seconds_bucket        | histogram   | Total time spent in seconds doing cache requests. | STABLE |
| acm_cortex_cache_request_duration_seconds_count         | counter     | | STABLE |
| acm_cortex_cache_request_duration_seconds_sum           | summary     | | STABLE |
| acm_cortex_cache_value_size_bytes_bucket                | histogram   | Size of values in the cache. | STABLE |
| acm_cortex_cache_value_size_bytes_count                 | counter     | | STABLE |
| acm_cortex_cache_value_size_bytes_sum                   | summary     | | STABLE |
| acm_cortex_dns_failures_total                           | counter     | The number of DNS lookup failures. | STABLE |
| acm_cortex_dns_lookups_total                            | counter     | The number of DNS lookups resolutions attempts. | STABLE |
| acm_cortex_dns_provider_results                         | gauge       | The number of resolved endpoints for each configured address. | STABLE |
| acm_cortex_frontend_query_range_duration_seconds_bucket | histogram   | Total time spent in seconds doing query range requests. | STABLE |
| acm_cortex_frontend_query_range_duration_seconds_count  | counter     | | STABLE |
| acm_cortex_frontend_query_range_duration_seconds_sum    | summary     | | STABLE |
| acm_cortex_memcache_client_servers                      | gauge       | The number of memcache servers discovered. | STABLE |
| acm_cortex_memcache_client_set_skip_total               | counter     | Total number of skipped set operations because of the value is larger than the max-item-size. | STABLE |
| acm_cortex_memcache_request_duration_seconds_bucket     | histogram   | Total time spent in seconds doing memcache requests. | STABLE |
| acm_cortex_memcache_request_duration_seconds_count      | counter     | | STABLE |
| acm_cortex_memcache_request_duration_seconds_sum        | summary     | | STABLE |
| acm_grpc_client_handled_total                           | counter     | Total number of RPCs completed by the client, regardless of success or failure. | STABLE |
| acm_grpc_client_handling_seconds_bucket                 | histogram   | Histogram of response latency (seconds) of the gRPC until it is finished by the application. | STABLE |
| acm_grpc_client_handling_seconds_count                  | counter     | | STABLE |
| acm_grpc_client_handling_seconds_sum                    | summary     | | STABLE |
| acm_grpc_client_msg_received_total                      | counter     | Total number of RPC stream messages received by the client. | STABLE |
| acm_grpc_client_msg_sent_total                          | counter     | Total number of gRPC stream messages sent by the client. | STABLE |
| acm_grpc_client_started_total                           | counter     | Total number of RPCs started on the client. | STABLE |
| acm_grpc_req_panics_recovered_total                     | counter     | Total number of gRPC requests recovered from internal panic. | STABLE |
| acm_grpc_server_handled_total                           | counter     | Total number of RPCs completed on the server, regardless of success or failure. | STABLE |
| acm_grpc_server_handling_seconds_bucket                 | histogram   | Histogram of response latency (seconds) of gRPC that had been application-level handled by the server. | STABLE |
| acm_grpc_server_handling_seconds_count                  | counter     | | STABLE |
| acm_grpc_server_handling_seconds_sum                    | summary     | | STABLE |
| acm_grpc_server_msg_received_total                      | counter     | Total number of RPC stream messages received on the server. | STABLE |
| acm_grpc_server_msg_sent_total                          | counter     | Total number of gRPC stream messages sent by the server. | STABLE |
| acm_grpc_server_started_total                           | counter     | Total number of RPCs started on the server. | STABLE |
| acm_healthcheck                                         | gauge       | Indicates if check is healthy (1 is healthy, 0 is unhealthy). | STABLE |
| acm_http_client_dns_duration_seconds_bucket             | histogram   | Trace dns latency histogram. | STABLE |
| acm_http_client_dns_duration_seconds_count              | counter     | | STABLE |
| acm_http_client_dns_duration_seconds_sum                | summary     | | STABLE |
| acm_http_client_in_flight_requests                      | gauge       | A gauge of in-flight requests. | STABLE |
| acm_http_client_request_duration_seconds_bucket         | histogram   | A histogram of request latencies. | STABLE |
| acm_http_client_request_duration_seconds_count          | counter     | | STABLE |
| acm_http_client_request_duration_seconds_sum            | summary     | | STABLE |
| acm_http_client_request_total                           | counter     | Total http client request by code and method. | STABLE |
| acm_http_client_tls_duration_seconds_bucket             | histogram   | Trace tls latency histogram. | STABLE |
| acm_http_client_tls_duration_seconds_count              | counter     | | STABLE |
| acm_http_client_tls_duration_seconds_sum                | summary     | | STABLE |
| acm_http_proxy_requests_total                           | counter     | Counter of proxy HTTP requests. | STABLE |
| acm_http_request_duration_seconds_bucket                | histogram   | Histogram of latencies for HTTP requests. | STABLE |
| acm_http_request_duration_seconds_count                 | counter     | | STABLE |
| acm_http_request_duration_seconds_sum                   | summary     | Tracks the latencies for HTTP requests. | STABLE |
| acm_http_request_size_bytes_count                       | counter     | | STABLE |
| acm_http_request_size_bytes_sum                         | summary     | Size of HTTP requests. | STABLE |
| acm_http_requests_total                                 | counter     | Counter of HTTP requests. | STABLE |
| acm_http_response_size_bytes_bucket                     | histogram   | Histogram of response size for HTTP requests.     | STABLE |
| acm_http_response_size_bytes_count                      | counter     | | STABLE |
| acm_http_response_size_bytes_sum                        | summary     | Tracks the size of HTTP responses. | STABLE |
| acm_manifestwork_count                                  | gauge       | ManifestWork count. | STABLE |
| acm_manifestwork_status_condition                       | gauge       | Managed cluster status condition. | STABLE |
| acm_memcached_commands_total                            | counter     | Total number of all requests broken down by command (get, set, etc.) and status. | STABLE |
| acm_memcached_connections_listener_disabled_total       | counter     | Number of times that memcached has hit its connections limit and disabled its listener. | STABLE |
| acm_memcached_connections_total                         | counter     | Total number of connections opened since the server started running. | STABLE |
| acm_memcached_connections_yielded_total                 | counter     | Total number of connections yielded running due to hitting the memcached's -R limit. | STABLE |
| acm_memcached_current_bytes                             | gauge       | Current number of bytes used to store items. | STABLE |
| acm_memcached_current_connections                       | gauge       | Current number of open connections. | STABLE |
| acm_memcached_current_items                             | gauge       | Current number of items stored by this instance. | STABLE |
| acm_memcached_exporter_build_info                       | gauge       | A metric with a constant '1' value labeled by version, revision, branch, and goversion from which memcached_exporter was built. | STABLE |
| acm_memcached_items_evicted_total                       | counter     | Total number of valid items removed from cache to free memory for new items. | STABLE |
| acm_memcached_items_reclaimed_total                     | counter     | Total number of times an entry was stored using memory from an expired entry. | STABLE |
| acm_memcached_items_total                               | counter     | Total number of items stored during the life of this instance. | STABLE |
| acm_memcached_limit_bytes                               | gauge       | Number of bytes this server is allowed to use for storage. | STABLE |
| acm_memcached_lru_crawler_enabled                       | gauge       | Whether the LRU crawler is enabled. | STABLE |
| acm_memcached_lru_crawler_hot_max_factor                | gauge       | Set idle age of HOT LRU to COLD age * this. | STABLE |
| acm_memcached_lru_crawler_hot_percent                   | gauge       | Percent of slab memory reserved for HOT LRU. | STABLE |
| acm_memcached_lru_crawler_items_checked_total           | counter     | Total items examined by LRU Crawler. | STABLE |
| acm_memcached_lru_crawler_maintainer_thread             | gauge       | Split LRU mode and background threads. | STABLE |
| acm_memcached_lru_crawler_moves_to_cold_total           | counter     | Total number of items moved from HOT/WARM to COLD LRU's. | STABLE |
| acm_memcached_lru_crawler_moves_to_warm_total           | counter     | Total number of items moved from COLD to WARM LRU. | STABLE |
| acm_memcached_lru_crawler_moves_within_lru_total        | counter     | Total number of items reshuffled within HOT or WARM LRU's. | STABLE |
| acm_memcached_lru_crawler_reclaimed_total               | counter     | Total items freed by LRU Crawler. | STABLE |
| acm_memcached_lru_crawler_sleep                         | gauge       | Microseconds to sleep between LRU crawls. | STABLE |
| acm_memcached_lru_crawler_starts_total                  | counter     | Times an LRU crawler was started. | STABLE |
| acm_memcached_lru_crawler_to_crawl                      | gauge       | Max items to crawl per slab per run. | STABLE |
| acm_memcached_lru_crawler_warm_max_factor               | gauge       | Set idle age of WARM LRU to COLD age * this. | STABLE |
| acm_memcached_lru_crawler_warm_percent                  | gauge       | Percent of slab memory reserved for WARM LRU. | STABLE |
| acm_memcached_malloced_bytes                            | gauge       | Number of bytes of memory allocated to slab pages. | STABLE |
| acm_memcached_max_connections                           | gauge       | Maximum number of clients allowed. | STABLE |
| acm_memcached_read_bytes_total                          | counter     | Total number of bytes read by this server from network. | STABLE |
| acm_memcached_slab_chunk_size_bytes                     | gauge       | Number of bytes allocated to each chunk within this slab class. | STABLE |
| acm_memcached_slab_chunks_free                          | gauge       | Number of chunks not yet allocated items. | STABLE |
| acm_memcached_slab_chunks_free_end                      | gauge       | Number of free chunks at the end of the last allocated page. | STABLE |
| acm_memcached_slab_chunks_per_page                      | gauge       | Number of chunks within a single page for this slab class. | STABLE |
| acm_memcached_slab_chunks_used                          | gauge       | Number of chunks allocated to an item. | STABLE |
| acm_memcached_slab_cold_items                           | gauge       | Number of items presently stored in the COLD LRU. | STABLE |
| acm_memcached_slab_commands_total                       | counter     | Total number of all requests broken down by command (get, set, etc.) and status per slab. | STABLE |
| acm_memcached_slab_current_chunks                       | gauge       | Number of chunks allocated to this slab class. | STABLE |
| acm_memcached_slab_current_items                        | gauge       | Number of items currently stored in this slab class. | STABLE |
| acm_memcached_slab_current_pages                        | gauge       | Number of pages allocated to this slab class. | STABLE |
| acm_memcached_slab_hot_age_seconds                      | gauge       | Age of the oldest item in HOT LRU. | STABLE |
| acm_memcached_slab_hot_items                            | gauge       | Number of items presently stored in the HOT LRU. | STABLE |
| acm_memcached_slab_items_age_seconds                    | gauge       | Number of seconds the oldest item has been in the slab class. | STABLE |
| acm_memcached_slab_items_crawler_reclaimed_total        | counter     | Number of items freed by the LRU Crawler. | STABLE |
| acm_memcached_slab_items_evicted_nonzero_total          | counter     | Total number of times an item which had an explicit expire time set had to be evicted from the LRU before it expired. | STABLE |
| acm_memcached_slab_items_evicted_time_seconds           | counter     | Seconds since the last access for the most recent item evicted from this class. | STABLE |
| acm_memcached_slab_items_evicted_total                  | counter     | Total number of times an item had to be evicted from the LRU before it expired. | STABLE |
| acm_memcached_slab_items_evicted_unfetched_total        | counter     | Total nmber of items evicted and never fetched. | STABLE |
| acm_memcached_slab_items_expired_unfetched_total        | counter     | Total number of valid items evicted from the LRU which were never touched after being set. | STABLE |
| acm_memcached_slab_items_moves_to_cold                  | counter     | Number of items moved from HOT or WARM into COLD. | STABLE |
| acm_memcached_slab_items_moves_to_warm                  | counter     | Number of items moves from COLD into WARM. | STABLE |
| acm_memcached_slab_items_moves_within_lru               | counter     | Number of times active items were bumped within HOT or WARM. | STABLE |
| acm_memcached_slab_items_outofmemory_total              | counter     | Total number of items for this slab class that have triggered an out of memory error. | STABLE |
| acm_memcached_slab_items_reclaimed_total                | counter     | Total number of items reclaimed. | STABLE |
| acm_memcached_slab_items_tailrepairs_total              | counter     | Total number of times the entries for a particular ID need repairing. | STABLE |
| acm_memcached_slab_lru_hits_total                       | counter     | Number of get_hits to the LRU. | STABLE |
| acm_memcached_slab_mem_requested_bytes                  | counter     | Number of bytes of memory actual items take up within a slab. | STABLE |
| acm_memcached_slab_warm_age_seconds                     | gauge       | Age of the oldest item in HOT LRU. | STABLE |
| acm_memcached_slab_warm_items                           | gauge       | Number of items presently stored in the WARM LRU. | STABLE |
| acm_memcached_time_seconds                              | gauge       | Current UNIX time according to the server. | STABLE |
| acm_memcached_up                                        | gauge       | Could the memcached server be reached. | STABLE |
| acm_memcached_uptime_seconds                            | counter     | Number of seconds since the server started. | STABLE |
| acm_memcached_version                                   | gauge       | The version of this memcached server. | STABLE |
| acm_memcached_written_bytes_total                       | counter     | Total number of bytes sent by this server to network. | STABLE |
| acm_observatorium_build_info                            | gauge       | A metric with a constant '1' value labeled by version, revision, branch, and goversion from which observatorium was built. | STABLE |
| acm_process_cpu_seconds_total                           | counter     | Total user and system CPU time spent in seconds. | STABLE |
| acm_process_max_fds                                     | gauge       | Maximum number of open file descriptors. | STABLE |
| acm_process_open_fds                                    | gauge       | Number of open file descriptors. | STABLE |
| acm_process_resident_memory_bytes                       | gauge       | Resident memory size in bytes. | STABLE |
| acm_process_start_time_seconds                          | gauge       | Start time of the process since unix epoch in seconds. | STABLE |
| acm_process_virtual_memory_bytes                        | gauge       | Virtual memory size in bytes. | STABLE |
| acm_process_virtual_memory_max_bytes                    | gauge       | Maximum amount of virtual memory available in bytes. | STABLE |
| acm_prometheus_engine_queries                           | gauge       | The current number of queries being executed or waiting. | STABLE |
| acm_prometheus_engine_queries_concurrent_max            | gauge       | The max number of concurrent queries. | STABLE |
| acm_prometheus_engine_query_duration_seconds            | gauge       | | STABLE |
| acm_prometheus_engine_query_duration_seconds_count      | counter     | | STABLE |
| acm_prometheus_engine_query_duration_seconds_sum        | summary     | Query timings. | STABLE |
| acm_prometheus_engine_query_log_enabled                 | gauge       | State of the query log. | STABLE |
| acm_prometheus_engine_query_log_failures_total          | counter     | The number of query log failures. | STABLE |
| acm_prometheus_rule_evaluation_duration_seconds         | gauge       | | STABLE |
| acm_prometheus_rule_evaluation_duration_seconds_count   | counter     | | STABLE |
| acm_prometheus_rule_evaluation_duration_seconds_sum     | summary     | The duration for a rule to execute. | STABLE |
| acm_prometheus_rule_evaluation_failures_total           | counter     | The total number of rule evaluation failures. | STABLE |
| acm_prometheus_rule_evaluations_total                   | counter     | The total number of rule evaluations. | STABLE |
| acm_prometheus_rule_group_duration_seconds              | gauge       | | STABLE |
| acm_prometheus_rule_group_duration_seconds_count        | counter     | | STABLE |
| acm_prometheus_rule_group_duration_seconds_sum          | summary     | The duration of rule group evaluations. | STABLE |
| acm_prometheus_rule_group_interval_seconds              | gauge       | The interval of a rule group. | STABLE |
| acm_prometheus_rule_group_iterations_missed_total       | counter     | The total number of rule group evaluations missed due to slow rule group evaluation. | STABLE |
| acm_prometheus_rule_group_iterations_total              | counter     | The total number of scheduled rule group evaluations, whether executed or missed. | STABLE |
| acm_prometheus_rule_group_last_duration_seconds         | gauge       | The duration of the last rule group evaluation.  | STABLE |
| acm_prometheus_rule_group_last_evaluation_samples       | gauge       | The number of samples returned during the last rule group evaluation. | STABLE |
| acm_prometheus_rule_group_last_evaluation_timestamp_seconds | gauge       | The timestamp of the last rule group evaluation in seconds. | STABLE |
| acm_prometheus_rule_group_rules                             | gauge       | The number of rules. | STABLE |
| acm_prometheus_tsdb_blocks_loaded                           | gauge       | Number of currently loaded data blocks | STABLE |
| acm_prometheus_tsdb_checkpoint_creations_failed_total       | counter     | Total number of checkpoint creations that failed. | STABLE |
| acm_prometheus_tsdb_checkpoint_deletions_failed_total       | counter     | Total number of checkpoint deletions that failed. | STABLE |
| acm_prometheus_tsdb_checkpoint_creations_total              | counter     | Total number of checkpoint creations attempted. | STABLE |
| acm_prometheus_tsdb_checkpoint_deletions_total              | counter     | Total number of checkpoint deletions attempted. | STABLE |
| acm_prometheus_tsdb_clean_start                             | gauge       | -1: lockfile is disabled. 0: a lockfile from a previous execution was replaced. 1: lockfile creation was clean. | STABLE |
| acm_prometheus_tsdb_compaction_chunk_range_seconds_bucket   | histogram   | Final time range of chunks on their first compaction. | STABLE |
| acm_prometheus_tsdb_compaction_chunk_range_seconds_count    | counter     | | STABLE |
| acm_prometheus_tsdb_compaction_chunk_range_seconds_sum      | summary     | | STABLE |
| acm_prometheus_tsdb_compaction_chunk_samples_bucket         | histogram   | Final number of samples on their first compaction. | STABLE |
| acm_prometheus_tsdb_compaction_chunk_samples_count          | counter     | | STABLE |
| acm_prometheus_tsdb_compaction_chunk_samples_sum            | summary     | | STABLE |
| acm_prometheus_tsdb_compaction_chunk_size_bytes_bucket      | histogram   | Final size of chunks on their first compaction. | STABLE |
| acm_prometheus_tsdb_compaction_chunk_size_bytes_count       | counter     | | STABLE |
| acm_prometheus_tsdb_compaction_chunk_size_bytes_sum         | summary     | | STABLE |
| acm_prometheus_tsdb_compaction_duration_seconds_bucket      | histogram   | Duration of compaction runs. | STABLE |
| acm_prometheus_tsdb_compaction_duration_seconds_count       | counter     | | STABLE |
| acm_prometheus_tsdb_compaction_duration_seconds_sum         | summary     | | STABLE |
| acm_prometheus_tsdb_compaction_populating_block             | gauge       | Set to 1 when a block is currently being written to the disk. | STABLE |
| acm_prometheus_tsdb_compactions_failed_total                | counter     | Total number of compactions that failed for the partition. | STABLE |
| acm_prometheus_tsdb_compactions_skipped_total               | counter     | Total number of skipped compactions due to disabled auto compaction. | STABLE |
| acm_prometheus_tsdb_compactions_total                       | counter     | Total number of compactions that were executed for the partition. | STABLE |
| acm_prometheus_tsdb_compactions_triggered_total             | counter     | Total number of triggered compactions for the partition. | STABLE |
| acm_prometheus_tsdb_data_replay_duration_seconds            | gauge       | Time taken to replay the data on disk. | STABLE |
| acm_prometheus_tsdb_exemplar_exemplars_appended_total       | counter     | Total number of appended exemplars. | STABLE |
| acm_prometheus_tsdb_exemplar_exemplars_in_storage           | gauge       | Number of exemplars currently in circular storage. | STABLE |
| acm_prometheus_tsdb_exemplar_last_exemplars_timestamp_seconds | gauge       | The timestamp of the oldest exemplar stored in circular storage. Useful to check for what timerange the current exemplar buffer limit allows. This usually means the last timestampfor all exemplars for a typical setup. This is not true though if one of the series timestamp is in future compared to rest series. | STABLE |
| acm_prometheus_tsdb_exemplar_max_exemplars                    | gauge       | Total number of exemplars the exemplar storage can store, resizeable. | STABLE |
| acm_prometheus_tsdb_exemplar_out_of_order_exemplars_total     | counter     | Total number of out of order exemplar ingestion failed attempts. | STABLE |
| acm_prometheus_tsdb_exemplar_series_with_exemplars_in_storage | gauge       | Number of series with exemplars currently in circular storage. | STABLE |
| acm_prometheus_tsdb_head_active_appenders                     | gauge       | Number of currently active appender transactions. | STABLE |
| acm_prometheus_tsdb_head_chunks                               | gauge       | Total number of chunks in the head block.   | STABLE |
| acm_prometheus_tsdb_head_chunks_created_total                 | counter     | Total number of chunks created in the head. | STABLE |
| acm_prometheus_tsdb_head_chunks_removed_total                 | counter     | Total number of chunks removed in the head. | STABLE |
| acm_prometheus_tsdb_head_gc_duration_seconds_count            | counter     | | STABLE |
| acm_prometheus_tsdb_head_gc_duration_seconds_sum              | summary     | Runtime of garbage collection in the head block. | STABLE |
| acm_prometheus_tsdb_head_max_time                             | gauge       | Maximum timestamp of the head block. | STABLE |
| acm_prometheus_tsdb_head_min_time                             | gauge       | Minimum time bound of the head block. | STABLE |
| acm_prometheus_tsdb_head_samples_appended_total               | counter     | Total number of appended samples. | STABLE |
| acm_prometheus_tsdb_head_series                               | gauge       | Total number of series in the head block. | STABLE |
| acm_prometheus_tsdb_head_series_created_total                 | counter     | Total number of series created in the head. | STABLE |
| acm_prometheus_tsdb_head_series_not_found_total               | counter     | Total number of requests for series that were not found. | STABLE |
| acm_prometheus_tsdb_head_series_removed_total                 | counter     | Total number of series removed in the head. | STABLE |
| acm_prometheus_tsdb_head_truncations_failed_total             | counter     | Total number of head truncations that failed. | STABLE |
| acm_prometheus_tsdb_head_truncations_total                    | counter     | Total number of head truncations attempted. | STABLE |
| acm_prometheus_tsdb_isolation_high_watermark                  | gauge       | The highest TSDB append ID that has been given out. | STABLE |
| acm_prometheus_tsdb_isolation_low_watermark                   | gauge       | The lowest TSDB append ID that is still referenced. | STABLE |
| acm_prometheus_tsdb_lowest_timestamp                          | gauge       | Lowest timestamp value stored in the database. | STABLE |
| acm_prometheus_tsdb_mmap_chunk_corruptions_total              | counter     | Total number of memory-mapped chunk corruptions. | STABLE |
| acm_prometheus_tsdb_out_of_bound_samples_total                | counter     | Total number of out of bound samples ingestion failed attempts. | STABLE |
| acm_prometheus_tsdb_out_of_order_samples_total                | counter     | Total number of out of order samples ingestion failed attempts. | STABLE |
| acm_prometheus_tsdb_reloads_failures_total                    | counter     | Number of times the database failed to reloadBlocks block data from disk. | STABLE |
| acm_prometheus_tsdb_reloads_total                             | counter     | Number of times the database reloaded block data from disk. | STABLE |
| acm_prometheus_tsdb_retention_limit_bytes                     | gauge       | Max number of bytes to be retained in the tsdb blocks, configured 0 means disabled. | STABLE |
| acm_prometheus_tsdb_size_retentions_total                     | counter     | The number of times that blocks were deleted because the maximum number of bytes was exceeded. | STABLE |
| acm_prometheus_tsdb_snapshot_replay_error_total               | counter     | Total number snapshot replays that failed. | STABLE |
| acm_prometheus_tsdb_storage_blocks_bytes                      | gauge       | The number of bytes that are currently used for local storage by all blocks. | STABLE |
| acm_prometheus_tsdb_symbol_table_size_bytes                   | gauge       | Size of symbol table in memory for loaded blocks. | STABLE |
| acm_prometheus_tsdb_time_retentions_total                     | counter     | The number of times that blocks were deleted because the maximum time limit was exceeded. | STABLE |
| acm_prometheus_tsdb_tombstone_cleanup_seconds_bucket          | histogram   | The time taken to recompact blocks to remove tombstones. | STABLE |
| acm_prometheus_tsdb_tombstone_cleanup_seconds_count           | counter     | | STABLE |
| acm_prometheus_tsdb_tombstone_cleanup_seconds_sum             | summary     | | STABLE |
| acm_prometheus_tsdb_vertical_compactions_total                | counter     | Total number of compactions done on overlapping blocks. | STABLE |
| acm_prometheus_tsdb_wal_completed_pages_total                 | counter     | Total number of completed pages. | STABLE |
| acm_prometheus_tsdb_wal_corruptions_total                     | counter     | Total number of WAL corruptions. | STABLE |
| acm_prometheus_tsdb_wal_fsync_duration_seconds                | gauge       | | STABLE |
| acm_prometheus_tsdb_wal_fsync_duration_seconds_count          | counter     | | STABLE |
| acm_prometheus_tsdb_wal_fsync_duration_seconds_sum            | summary     | Duration of WAL fsync. | STABLE |
| acm_prometheus_tsdb_wal_page_flushes_total                    | counter     | Total number of page flushes. | STABLE |
| acm_prometheus_tsdb_wal_segment_current                       | gauge       | WAL segment index that TSDB is currently writing to. | STABLE |
| acm_prometheus_tsdb_wal_truncate_duration_seconds_count       | counter     | | STABLE |
| acm_prometheus_tsdb_wal_truncate_duration_seconds_sum         | summary     | Duration of WAL truncation. | STABLE |
| acm_prometheus_tsdb_wal_truncations_failed_total              | counter     | Total number of WAL truncations that failed. | STABLE |
| acm_prometheus_tsdb_wal_truncations_total                     | counter     | Total number of WAL truncations attempted. | STABLE |
| acm_prometheus_tsdb_wal_writes_failed_total                   | counter     | Total number of WAL writes that failed. | STABLE |
| acm_promhttp_metric_handler_requests_in_flight                | gauge       | Current number of scrapes being served. | STABLE |
| acm_promhttp_metric_handler_requests_total                    | counter     | Total number of scrapes by HTTP status code. | STABLE |
| acm_remote_write_requests_total                               | counter     | Counter of remote write requests. | STABLE |
| acm_thanos_alert_queue_alerts_dropped_total                   | counter     | Total number of alerts that were dropped from the queue. | STABLE |
| acm_thanos_alert_queue_alerts_popped_total                    | counter     | Total number of alerts popped from the queue. | STABLE |
| acm_thanos_alert_queue_alerts_pushed_total                    | counter     | Total number of alerts pushed to the queue. | STABLE |
| acm_thanos_alert_queue_capacity                               | gauge       | Capacity of the alert queue. | STABLE |
| acm_thanos_alert_queue_length                                 | gauge       | Length of the alert queue. | STABLE |
| acm_thanos_alert_sender_alerts_dropped_total                  | counter     | Total number of alerts dropped in case of all sends to alertmanagers failed. | STABLE |
| acm_thanos_alert_sender_alerts_sent_total                     | counter     | Total number of alerts sent by alertmanager. | STABLE |
| acm_thanos_alert_sender_latency_seconds_bucket                | histogram   | Latency for sending alert notifications (not including dropped notifications). | STABLE |
| acm_thanos_alert_sender_latency_seconds_count                 | counter     | | STABLE |
| acm_thanos_alert_sender_latency_seconds_sum                   | summary     | | STABLE |
| acm_thanos_blocks_meta_base_syncs_total                       | counter     | Total blocks metadata synchronization attempts by base Fetcher. | STABLE |
| acm_thanos_blocks_meta_modified                               | gauge       | Number of blocks whose metadata changed. | STABLE |
| acm_thanos_blocks_meta_sync_duration_seconds_bucket           | histogram   | Duration of the blocks metadata synchronization in seconds. | STABLE |
| acm_thanos_blocks_meta_sync_duration_seconds_count            | counter     | | STABLE |
| acm_thanos_blocks_meta_sync_duration_seconds_sum              | summary     | | STABLE |
| acm_thanos_blocks_meta_sync_failures_total                    | counter     | Total blocks metadata synchronization failures.| STABLE |
| acm_thanos_blocks_meta_synced                                 | gauge       | Number of block metadata synced. | STABLE |
| acm_thanos_blocks_meta_syncs_total                            | counter     | Total blocks metadata synchronization attempts | STABLE |
| acm_thanos_bucket_store_block_drop_failures_total             | counter     | Total number of local blocks that failed to be dropped. | STABLE |
| acm_thanos_bucket_store_block_drops_total                     | counter     | Total number of local blocks that were dropped. | STABLE |
| acm_thanos_bucket_store_block_load_failures_total             | counter     | Total number of failed remote block loading attempts. | STABLE |
| acm_thanos_bucket_store_block_loads_total                     | counter     | Total number of remote block loading attempts. | STABLE |
| acm_thanos_bucket_store_blocks_last_loaded_timestamp_seconds  | gauge       | Timestamp when last block got loaded. | STABLE |
| acm_thanos_bucket_store_blocks_loaded                         | gauge       | Number of currently loaded blocks. | STABLE |
| acm_thanos_bucket_store_cached_postings_compressed_size_bytes_total    | counter     | Compressed size of postings stored into cache. | STABLE |
| acm_thanos_bucket_store_cached_postings_compression_errors_total       | counter     | Number of postings compression errors. | STABLE |
| acm_thanos_bucket_store_cached_postings_compression_time_seconds_total | counter     | Time spent compressing postings before storing them into postings cache. | STABLE |
| acm_thanos_bucket_store_cached_postings_compressions_total             | counter     | Number of postings compressions before storing to index cache. | STABLE |
| acm_thanos_bucket_store_cached_postings_fetch_duration_seconds_bucket  | histogram   | The time it takes to fetch postings to respond to a request sent to a store gateway. It includes both the time to fetch it from the cache and from storage in case of cache misses. | STABLE |
| acm_thanos_bucket_store_cached_postings_fetch_duration_seconds_count   | counter     | | STABLE |
| acm_thanos_bucket_store_cached_postings_fetch_duration_seconds_sum     | summary     | | STABLE |
| acm_thanos_bucket_store_cached_postings_original_size_bytes_total      | counter     | Original size of postings stored into cache. | STABLE |
| acm_thanos_bucket_store_cached_series_fetch_duration_seconds_bucket    | histogram   | The time it takes to fetch series to respond to a request sent to a store gateway. It includes both the time to fetch it from the cache and from storage in case of cache misses. | STABLE |
| acm_thanos_bucket_store_cached_series_fetch_duration_seconds_count     | counter     | | STABLE |
| acm_thanos_bucket_store_cached_series_fetch_duration_seconds_sum       | summary     | | STABLE |
| acm_thanos_bucket_store_indexheader_lazy_load_duration_seconds_bucket  | histogram   | Duration of the index-header lazy loading in seconds. | STABLE |
| acm_thanos_bucket_store_indexheader_lazy_load_duration_seconds_count   | counter     | | STABLE |
| acm_thanos_bucket_store_indexheader_lazy_load_duration_seconds_sum     | summary     | | STABLE |
| acm_thanos_bucket_store_indexheader_lazy_load_failed_total             | counter     | Total number of failed index-header lazy load operations. | STABLE |
| acm_thanos_bucket_store_indexheader_lazy_load_total                    | counter     | Total number of index-header lazy load operations. | STABLE |
| acm_thanos_bucket_store_indexheader_lazy_unload_failed_total           | counter     | Total number of failed index-header lazy unload operations. | STABLE |
| acm_thanos_bucket_store_indexheader_lazy_unload_total                  | counter     | Total number of index-header lazy unload operations. | STABLE |
| acm_thanos_bucket_store_queries_dropped_total                          | counter     | Number of queries that were dropped due to the limit. | STABLE |
| acm_thanos_bucket_store_sent_chunk_size_bytes_bucket                   | histogram   | Size in bytes of the chunks for the single series, which is adequate to the gRPC message size sent to querier. | STABLE |
| acm_thanos_bucket_store_sent_chunk_size_bytes_count                    | counter     | | STABLE |
| acm_thanos_bucket_store_sent_chunk_size_bytes_sum                      | summary     | | STABLE |
| acm_thanos_bucket_store_series_blocks_queried_count                    | counter     | | STABLE |
| acm_thanos_bucket_store_series_blocks_queried_sum                      | summary     | Number of blocks in a bucket store that were touched to satisfy a query. | STABLE |
| acm_thanos_bucket_store_series_data_fetched_count                      | counter     | | STABLE |
| acm_thanos_bucket_store_series_data_fetched_sum                        | summary     | How many items of a data type in a block were fetched for a single series request. | STABLE |
| acm_thanos_bucket_store_series_data_size_fetched_bytes_count           | counter     | | STABLE |
| acm_thanos_bucket_store_series_data_size_fetched_bytes_sum             | summary     | Size of all items of a data type in a block were fetched for a single series request. | STABLE |
| acm_thanos_bucket_store_series_data_size_touched_bytes_count           | counter     | | STABLE |
| acm_thanos_bucket_store_series_data_size_touched_bytes_sum             | summary     | Size of all items of a data type in a block were touched for a single series request. | STABLE |
| acm_thanos_bucket_store_series_data_touched_count                      | counter     | | STABLE |
| acm_thanos_bucket_store_series_data_touched_sum                        | summary     | How many items of a data type in a block were touched for a single series request. | STABLE |
| acm_thanos_bucket_store_series_gate_duration_seconds_bucket            | historgram  | How many seconds it took for queries to wait at the gate. | STABLE |
| acm_thanos_bucket_store_series_gate_duration_seconds_count             | counter     | | STABLE |
| acm_thanos_bucket_store_series_gate_duration_seconds_sum               | summary     | | STABLE |
| acm_thanos_bucket_store_series_gate_queries_in_flight                  | gauge       | Number of queries that are currently in flight. | STABLE |
| acm_thanos_bucket_store_series_gate_queries_max                        | gauge       | Maximum number of concurrent queries. | STABLE |
| acm_thanos_bucket_store_series_get_all_duration_seconds_bucket         | histogram   | Time it takes until all per-block prepares and loads for a query are finished. | STABLE |
| acm_thanos_bucket_store_series_get_all_duration_seconds_count          | counter     | | STABLE |
| acm_thanos_bucket_store_series_get_all_duration_seconds_sum            | summary     | | STABLE |
| acm_thanos_bucket_store_series_merge_duration_seconds_bucket           | histogram   | Time it takes to merge sub-results from all queried blocks into a single result. | STABLE |
| acm_thanos_bucket_store_series_merge_duration_seconds_count            | counter     | | STABLE |
| acm_thanos_bucket_store_series_merge_duration_seconds_sum              | summary     | | STABLE |
| acm_thanos_bucket_store_series_refetches_total                         | counter     | Total number of cases where 65536 bytes was not enough was to fetch series from index, resulting in refetch. | STABLE |
| acm_thanos_bucket_store_series_result_series_count                     | counter     | | STABLE |
| acm_thanos_bucket_store_series_result_series_sum                       | summary     | | STABLE |
| acm_thanos_bucket_uiblocks_meta_modified                               | gauge       | Number of blocks whose metadata changed. | STABLE |
| acm_thanos_bucket_uiblocks_meta_sync_duration_seconds_bucket           | histgram    | Duration of the blocks metadata synchronization in seconds. | STABLE |
| acm_thanos_bucket_uiblocks_meta_sync_duration_seconds_count            | counter     | | STABLE |
| acm_thanos_bucket_uiblocks_meta_sync_duration_seconds_sum              | summary     | Number of series observed in the final result of a query. | STABLE |
| acm_thanos_bucket_uiblocks_meta_sync_failures_total                    | counter     | Total blocks metadata synchronization failures. | STABLE |
| acm_thanos_bucket_uiblocks_meta_synced                                 | gauge       | Number of block metadata synced. | STABLE |
| acm_thanos_bucket_uiblocks_meta_syncs_total                            | counter     | Total blocks metadata synchronization attempts. | STABLE |
| acm_thanos_build_info   | gauge       | A metric with a constant '1' value labeled by version, revision, branch, and goversion from which thanos was built. | STABLE |
| acm_thanos_cache_memcached_hits_total                                  | counter     | Total number of items requests to the cache that were a hit. | STABLE |
| acm_thanos_cache_memcached_requests_total                              | counter     | Total number of items requests to memcached. | STABLE |
| acm_thanos_compact_aborted_partial_uploads_deletion_attempts_total     | counter     | Total number of started deletions of blocks that are assumed aborted and only partially uploaded. | STABLE |
| acm_thanos_compact_block_cleanup_failures_total                        | counter     | Failures encountered while deleting blocks in compactor. | STABLE |
| acm_thanos_compact_block_cleanup_loops_total                           | counter     | Total number of concurrent cleanup loops of partially uploaded blocks and marked blocks that were executed successfully. | STABLE |
| acm_thanos_compact_blocks_cleaned_total                                | counter     | Total number of blocks deleted in compactor. | STABLE |
| acm_thanos_compact_blocks_marked_total                                 | counter     | Total number of blocks marked in compactor. | STABLE |
| acm_thanos_compact_downsample_failures_total                           | counter     | Total number of failed downsampling attempts. | STABLE |
| acm_thanos_compact_downsample_total                                    | counter     | Total number of downsampling attempts. | STABLE |
| acm_thanos_compact_garbage_collected_blocks_total                      | counter     | Total number of blocks marked for deletion by compactor. | STABLE |
| acm_thanos_compact_garbage_collection_duration_seconds_bucket          | histogram   | Time it took to perform garbage collection iteration. | STABLE |
| acm_thanos_compact_garbage_collection_duration_seconds_count           | counter     | | STABLE |
| acm_thanos_compact_garbage_collection_duration_seconds_sum             | summary     | | STABLE |
| acm_thanos_compact_garbage_collection_failures_total                   | counter     | Total number of failed garbage collection operations. | STABLE |
| acm_thanos_compact_garbage_collection_total                            | counter     | Total number of garbage collection operations. | STABLE |
| acm_thanos_compact_group_compaction_runs_completed_total               | counter     | Total number of group completed compaction runs. This also includes compactor group runs that resulted with no compaction. | STABLE |
| acm_thanos_compact_group_compaction_runs_started_total                 | counter     | Total number of group compaction attempts. | STABLE |
| acm_thanos_compact_group_compactions_failures_total                    | counter     | Total number of failed group compactions. | STABLE |
| acm_thanos_compact_group_compactions_total                             | counter     | Total number of group compaction attempts that resulted in a new block. | STABLE |
| acm_thanos_compact_group_vertical_compactions_total                    | counter     | Total number of group compaction attempts that resulted in a new block based on overlapping blocks. | STABLE |
| acm_thanos_compact_halted | gauge       | Set to 1 if the compactor halted due to an unexpected error. | STABLE |
| acm_thanos_compact_iterations_total                                    | counter     | Total number of iterations that were executed successfully. | STABLE |
| acm_thanos_compact_retries_total                                       | counter     | Total number of retries after retriable compactor error. | STABLE |
| acm_thanos_compact_todo_compaction_blocks                              | gauge       | | STABLE |
| acm_thanos_compact_todo_compactions                                    | gauge       | | STABLE |
| acm_thanos_consistency_delay_seconds                                   | gauge       | Configured consistency delay in seconds. | STABLE |
| acm_thanos_delete_delay_seconds                                        | gauge       | Configured delete delay in seconds. | STABLE |
| acm_thanos_frontend_downsampled_extra_queries_total                    | counter     | Total number of additional queries for downsampled data. | STABLE |
| acm_thanos_frontend_split_queries_total                                | counter     | Total number of underlying query requests after the split by interval is applied. | STABLE |
| acm_thanos_memcached_client_info                                       | gauge       | A metric with a constant '1' value labeled by configuration options from which memcached client was configured. | STABLE |
| acm_thanos_memcached_dns_failures_total                                | counter     | The number of DNS lookup failures. | STABLE |
| acm_thanos_memcached_dns_lookups_total                                 | counter     | The number of DNS lookups resolutions attempts. | STABLE |
| acm_thanos_memcached_dns_provider_results                              | gauge       | The number of resolved endpoints for each configured address. | STABLE |
| acm_thanos_memcached_getmulti_gate_duration_seconds_bucket             | histogram   | How many seconds it took for queries to wait at the gate. | STABLE |
| acm_thanos_memcached_getmulti_gate_duration_seconds_count              | counter     | | STABLE |
| acm_thanos_memcached_getmulti_gate_duration_seconds_sum                | summary     | | STABLE |
| acm_thanos_memcached_getmulti_gate_queries_in_flight                   | gauge       | Number of queries that are currently in flight. | STABLE |
| acm_thanos_memcached_getmulti_gate_queries_max                         | gauge       | Maximum number of concurrent queries. | STABLE |
| acm_thanos_memcached_operation_data_size_bytes_bucket                  | histogram   | Tracks the size of the data stored in and fetched from memcached. | STABLE |
| acm_thanos_memcached_operation_data_size_bytes_count                   | counter     | | STABLE |
| acm_thanos_memcached_operation_data_size_bytes_sum                     | summary     | | STABLE |
| acm_thanos_memcached_operation_duration_seconds_bucket                 | histogram   | Duration of operations against memcached. | STABLE |
| acm_thanos_memcached_operation_duration_seconds_count                  | counter     | | STABLE |
| acm_thanos_memcached_operation_duration_seconds_sum                    | summary     | | STABLE |
| acm_thanos_memcached_operation_failures_total                          | counter     | Total number of operations against memcached that failed. | STABLE |
| acm_thanos_memcached_operation_skipped_total                           | counter     | Total number of operations against memcached that have been skipped. | STABLE |
| acm_thanos_memcached_operations_total                                  | counter     | Total number of operations against memcached. | STABLE |
| acm_thanos_objstore_bucket_last_successful_upload_time                 | gauge       | Second timestamp of the last successful upload to the bucket. | STABLE |
| acm_thanos_objstore_bucket_operation_duration_seconds_bucket           | histogram   | Duration of successful operations against the bucket. | STABLE |
| acm_thanos_objstore_bucket_operation_duration_seconds_count            | counter     | | STABLE |
| acm_thanos_objstore_bucket_operation_duration_seconds_sum              | summary     | | STABLE |
| acm_thanos_objstore_bucket_operation_failures_total                    | counter     | Total number of operations against a bucket that failed, but were not expected to fail in certain way from caller perspective. Those errors have to be investigated.      | STABLE |
| acm_thanos_objstore_bucket_operations_total                            | counter     | Total number of all attempted operations against a bucket. | STABLE |
| acm_thanos_proxy_store_empty_stream_responses_total                    | counter     | Total number of empty responses received. | STABLE |
| acm_thanos_query_concurrent_gate_duration_seconds_bucket               | histogram   | How many seconds it took for queries to wait at the gate. | STABLE |
| acm_thanos_query_concurrent_gate_duration_seconds_count                | counter     | | STABLE |
| acm_thanos_query_concurrent_gate_duration_seconds_sum                  | summary     | | STABLE |
| acm_thanos_query_concurrent_gate_queries_in_flight                     | gauge       | Number of queries that are currently in flight. | STABLE |
| acm_thanos_query_concurrent_gate_queries_max                           | gauge       | Maximum number of concurrent queries. | STABLE |
| acm_thanos_query_concurrent_selects_gate_duration_seconds_bucket       | histogram   | How many seconds it took for queries to wait at the gate. | STABLE |
| acm_thanos_query_concurrent_selects_gate_duration_seconds_count        | counter     | | STABLE |
| acm_thanos_query_concurrent_selects_gate_duration_seconds_sum          | summary     | | STABLE |
| acm_thanos_query_duplicated_store_addresses_total                      | counter     | The number of times a duplicated store addresses is detected from the different configs in query. | STABLE |
| acm_thanos_query_endpoints_dns_failures_total                          | counter     | The number of DNS lookup failures. | STABLE |
| acm_thanos_query_endpoints_dns_lookups_total                           | counter     | The number of DNS lookups resolutions attempts. | STABLE |
| acm_thanos_query_exemplar_apis_dns_failures_total                      | counter     | The number of DNS lookup failures. | STABLE |
| acm_thanos_query_exemplar_apis_dns_lookups_total                       | counter     | The number of DNS lookups resolutions attempts. | STABLE |
| acm_thanos_query_frontend_queries_total                                | counter     | Total queries passing through query frontend. | STABLE |
| acm_thanos_query_metadata_apis_dns_failures_total                      | counter     | The number of DNS lookup failures. | STABLE |
| acm_thanos_query_metadata_apis_dns_lookups_total                       | counter     | The number of DNS lookups resolutions attempts. | STABLE |
| acm_thanos_query_range_requested_timespan_duration_seconds_bucket      | historgram  | A histogram of the query range window in seconds. | STABLE |
| acm_thanos_query_range_requested_timespan_duration_seconds_count       | counter     | | STABLE |
| acm_thanos_query_range_requested_timespan_duration_seconds_sum         | summary     | | STABLE |
| acm_thanos_query_rule_apis_dns_failures_total                          | counter     | The number of DNS lookup failures. | STABLE |
| acm_thanos_query_rule_apis_dns_lookups_total                           | counter     | The number of DNS lookups resolutions attempts. | STABLE |
| acm_thanos_query_store_apis_dns_failures_total                         | counter     | The number of DNS lookup failures. | STABLE |
| acm_thanos_query_store_apis_dns_lookups_total                          | counter     | The number of DNS lookups resolutions attempts. | STABLE |
| acm_thanos_query_store_apis_dns_provider_results                       | gauge       | The number of resolved endpoints for each configured address. | STABLE |
| acm_thanos_query_target_apis_dns_failures_total                        | counter     | The number of DNS lookup failures. | STABLE |
| acm_thanos_query_target_apis_dns_lookups_total                         | counter     | The number of DNS lookups resolutions attempts | STABLE |
| acm_thanos_receive_config_hash                                         | gauge       | Hash of the currently loaded hashring configuration file. | STABLE |
| acm_thanos_receive_config_last_reload_success_timestamp_seconds        | gauge       | Timestamp of the last successful hashring configuration file reload. | STABLE |
| acm_thanos_receive_config_last_reload_successful                       | gauge       | Whether the last hashring configuration file reload attempt was successful. | STABLE |
| acm_thanos_receive_controller_client_cache_last_resource_version       | gauge       | Last resource version from the Kubernetes API. | STABLE |
| acm_thanos_receive_controller_client_cache_list_duration_seconds_count | counter     | | STABLE |
| acm_thanos_receive_controller_client_cache_list_duration_seconds_sum   | summary     | Duration of a Kubernetes API call in seconds. | STABLE |
| acm_thanos_receive_controller_client_cache_list_items_count            | counter     | | STABLE |
| acm_thanos_receive_controller_client_cache_list_items_sum              | summary     | Count of items in a list from the Kubernetes API. | STABLE |
| acm_thanos_receive_controller_client_cache_short_watches_total         | counter     | Total number of short watch operations. | STABLE |
| acm_thanos_receive_controller_client_cache_watch_duration_seconds_count | counter     | | STABLE |
| acm_thanos_receive_controller_client_cache_watch_duration_seconds_sum   | summary     | Duration of watches on the Kubernetes API. | STABLE |
| acm_thanos_receive_controller_client_cache_watch_events_count           | counter     | Total number of items in watch on Kubernetes API. | STABLE |
| acm_thanos_receive_controller_client_cache_watch_events_sum             | summary     | Number of items in watches on the Kubernetes API. | STABLE |
| acm_thanos_receive_controller_client_cache_watches_total                | counter     | Total number of watch operations. | STABLE |
| acm_thanos_receive_controller_configmap_change_attempts_total           | counter     | Total number of configmap change attempts. | STABLE |
| acm_thanos_receive_controller_configmap_change_errors_total             | counter     | Total number of configmap change errors. | STABLE |
| acm_thanos_receive_controller_configmap_hash                            | gauge       | Hash of the currently loaded configmap. | STABLE |
| acm_thanos_receive_controller_configmap_last_reload_success_timestamp_seconds | gauge       | Timestamp of the last successful configmap. | STABLE |
| acm_thanos_receive_controller_hashring_nodes                            | gauge       | The number of nodes per hashring. | STABLE |
| acm_thanos_receive_controller_hashring_tenants                          | gauge       | The number of tenants per hashring. | STABLE |
| acm_thanos_receive_controller_reconcile_attempts_total                  | counter     | Total number of reconciles. | STABLE |
| acm_thanos_receive_controller_reconcile_errors_total                    | counter     | Total number of reconciles errors. | STABLE |
| acm_thanos_receive_forward_requests_total                               | counter     | The number of forward requests. | STABLE |
| acm_thanos_receive_hashring_nodes                                       | gauge       | The number of nodes per hashring. | STABLE |
| acm_thanos_receive_hashring_tenants                                     | gauge       | The number of tenants per hashring. | STABLE |
| acm_thanos_receive_hashrings_file_changes_total                         | counter     | The number of times the hashrings configuration file has changed. | STABLE |
| acm_thanos_receive_hashrings_file_errors_total                          | counter     | The number of errors watching the hashrings configuration file. | STABLE |
| acm_thanos_receive_hashrings_file_refreshes_total                       | counter     | The number of refreshes of the hashrings configuration file. | STABLE |
| acm_thanos_receive_multi_db_updates_attempted_total                     | counter     | Number of Multi DB attempted reloads with flush and potential upload due to hashring changes. | STABLE |
| acm_thanos_receive_multi_db_updates_completed_total                     | counter     | Number of Multi DB completed reloads with flush and potential upload due to hashring changes. | STABLE |
| acm_thanos_receive_replication_factor                                   | gauge       | The number of times to replicate incoming write requests. | STABLE |
| acm_thanos_receive_replications_total                                   | counter     | The number of replication operations done by the receiver. The success of replication is fulfilled when a quorum is met. | STABLE |
| acm_thanos_rule_alertmanagers_dns_failures_total                        | counter     | The number of DNS lookup failures. | STABLE |
| acm_thanos_rule_alertmanagers_dns_lookups_total                         | counter     | The number of DNS lookups resolutions attempts. | STABLE |
| acm_thanos_rule_alertmanagers_dns_provider_results                      | gauge       | The number of resolved endpoints for each configured address. | STABLE |
| acm_thanos_rule_config_last_reload_success_timestamp_seconds            | gauge       | Timestamp of the last successful configuration reload. | STABLE |
| acm_thanos_rule_config_last_reload_successful                           | gauge       | Whether the last configuration reload attempt was successful. | STABLE |
| acm_thanos_rule_duplicated_query_addresses_total                        | counter     | The number of times a duplicated query addresses is detected from the different configs in rule. | STABLE |
| acm_thanos_rule_evaluation_with_warnings_total                          | counter     | The total number of rule evaluation that were successful but had warnings which can indicate partial error. | STABLE |
| acm_thanos_rule_loaded_rules                                            | gauge       | Loaded rules partitioned by file and group. | STABLE |
| acm_thanos_rule_query_apis_dns_failures_total                           | counter     | The number of DNS lookup failures. | STABLE |
| acm_thanos_rule_query_apis_dns_lookups_total                            | counter     | The number of DNS lookups resolutions attempts. | STABLE |
| acm_thanos_rule_query_apis_dns_provider_results                         | counter     | The number of resolved endpoints for each configured address. | STABLE |
| acm_thanos_shipper_dir_sync_failures_total                              | counter     | Total number of failed dir syncs. | STABLE |
| acm_thanos_shipper_dir_syncs_total                                      | counter     | Total number of dir syncs. | STABLE |
| acm_thanos_shipper_upload_failures_total                                | counter     | Total number of block upload failures. | STABLE |
| acm_thanos_shipper_uploads_total                                        | counter     | Total number of uploaded blocks. | STABLE |
| acm_thanos_status          | gauge       | Represents status (0 indicates failure, 1 indicates success) of the component. | STABLE |
| acm_thanos_store_bucket_cache_getrange_fetched_bytes_total              | counter     | Total number of bytes fetched because of GetRange operation. Data from bucket is then stored to cache. | STABLE |
| acm_thanos_store_bucket_cache_getrange_refetched_bytes_total            | counter     | Total number of bytes re-fetched from storage because of GetRange operation, despite being in cache already. | STABLE |
| acm_thanos_store_bucket_cache_getrange_requested_bytes_total            | counter     | Total number of bytes requested via GetRange. | STABLE |
| acm_thanos_store_bucket_cache_operation_hits_total                      | counter     | Number of operations served from cache for given config. | STABLE |
| acm_thanos_store_bucket_cache_operation_requests_total                  | counter     | Number of requested operations matching given config. | STABLE |
| acm_thanos_store_index_cache_hits_total                                 | counter     | Total number of items requests to the cache that were a hit. | STABLE |
| acm_thanos_store_index_cache_requests_total                             | counter     | Total number of items requests to the cache. | STABLE |
| acm_thanos_store_nodes_grpc_connections                                 | gauge       | Number of gRPC connection to Store APIs. Opened connection means healthy store APIs available for Querier. | STABLE |
