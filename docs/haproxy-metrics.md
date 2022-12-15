# Haproxy Metrics

| Metric Name                                                | Metric Type | Description                                                         | Status |
|------------------------------------------------------------|-------------|---------------------------------------------------------------------|--------|
| haproxy_backend_connection_errors_total                    | gauge       | Total of connection errors.                                         |        |
| haproxy_backend_connections_total                          | gauge       | Total number of connections.                                        |        |
| haproxy_backend_current_queue                              | gauge       | Current number of queued requests not assigned to any server.       |        |
| haproxy_backend_http_average_response_latency_milliseconds | gauge       | Average response latency of the last 1024 requests in milliseconds. |        |
| haproxy_backend_max_sessions                               | gauge       | Maximum observed number of active sessions.                         |        |
| haproxy_backend_response_errors_total                      | gauge       | Total of response errors.                                           |        |
| haproxy_backend_up                                         | gauge       | Current health status of the backend (1 = UP, 0 = DOWN).            |        |
