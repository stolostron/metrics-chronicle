# Documentation

## Table of Contents

- [Documentation](#documentation)
  - [Table of Contents](#table-of-contents)
  - [Metrics Stages](#metrics-stages)
  - [Exposed Metrics](#exposed-metrics)
    - [Default Resources](#default-resources)
    - [Optional Resources](#optional-resources)

## Metrics Stages

Stages about metrics are grouped into three categories：

| Stage        | Description                                                                                                                |
|--------------|----------------------------------------------------------------------------------------------------------------------------|
| EXPERIMENTAL | Metrics which normally correspond to the Kubernetes API object alpha status or spec fields and can be changed at any time. |
| STABLE       | Metrics which should have very few backwards-incompatible changes outside of major version updates.                        |
| DEPRECATED   | Metrics which will be removed once the deprecation timeline is met.                                                        |

## Exposed Metrics

### Default Resources

- [ACM Metrics](acm/README.md)
- [Alerts Metrics](alert-metrics.md)
- [Authentication Metrics](authentication-metrics.md)
- [Cluster Metrics](cluster-metrics.md)
- [Container Metrics](container-metrics.md)
- [CoreDNS Metrics](coredns-metrics.md)
- [DaemonSet Metrics](daemonset-metrics.md)
- [ETCD Metrics](etcd-metrics.md)
- [GRPC Metrics](grpc-metrics.md)
- [HaProxy Metrics](haproxy-metrics.md)
- [HTTP Metrics](http-metrics.md)
- [Installer Metrics](installer-metrics.md)
- [Instance Metrics](instance-metrics.md)
- [Kubelet Metrics](kubelet-metrics.md)
- [Machine Metrics](machine-metrics.md)
- [Mixin Metrics](mixin-metrics.md)
- [Namespace Metrics](namespace-metrics.md)
- [Node Metrics](node-metrics.md)
- [OpenShift Metrics](openshift-metrics.md)
- [Pod Metrics](pod-metrics.md)
- [Server Foundation Metrics](acm/component/server-foundation/metrics.md)

### Optional Resources
