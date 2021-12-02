### thanos querier

如果没有部署 thanos store 组件，在 `thanos-querier` 中把 `- --store=dnssrv+_grpc._tcp.thanos-store.monitoring.svc.cluster.local` 注释掉