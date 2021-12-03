## Introduce
Deploy Thanos in Kubernetes

## All thanos ports

---

| Component      | Interface               | Port  |
| -------------- | ----------------------- | ----- |
| Sidecar        | gRPC                    | 10901 |
| Sidecar        | HTTP                    | 10902 |
| Query          | gRPC                    | 10903 |
| Query          | HTTP                    | 10904 |
| Store          | gRPC                    | 10905 |
| Store          | HTTP                    | 10906 |
| Receive        | gRPC (store API)        | 10907 |
| Receive        | HTTP (remote write API) | 10908 |
| Receive        | HTTP                    | 10909 |
| Rule           | gRPC                    | 10910 |
| Rule           | HTTP                    | 10911 |
| Compact        | HTTP                    | 10912 |
| Query Frontend | HTTP                    | 10913 |



### grafana 添加 thanos-querier 数据源

<img src="doc/pics/grafana_add-thanos-querier.png" alt="grafana_add-thanos-querier" style="zoom:50%;" />



### thanos-querier 截图

<img src="doc/pics/thanos-query_stores.png" alt="thanos-query_stores" style="zoom:50%;" />



### thanos 相关的 k8s 资源

![all-thanos-svc-sts-deploy-pod](doc/pics/all-thanos-svc-sts-deploy-pod.png)
