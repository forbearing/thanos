## Introduce
Deploy Thanos in Kubernetes

## All thanos components ports

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



### grafana add thanos-querier datasource

<img src="doc/pics/grafana_add-thanos-querier.png" alt="grafana_add-thanos-querier" style="zoom:50%;" />



### thanos-querier web UI

<img src="doc/pics/thanos-querier_webui-1.png" alt="thanos-querier_webui-1" style="zoom:50%;" />

<img src="doc/pics/thanos-querier_webui-2.png" alt="thanos-query_stores" style="zoom:50%;" />

### thanos-ruler web UI

<img src="doc/pics/thanos-ruler_webui-1.png" alt="thanos-ruler_webui-1" style="zoom:50%;" />

<img src="doc/pics/thanos-ruler_webui-2.png" alt="thanos-ruler_webui-2" style="zoom:50%;" />

### thanos-store web UI

<img src="doc/pics/thanos-store_webui-1.png" alt="thanos-store_webui-1" style="zoom:50%;" />

### thanos-compactor web UI

<img src="doc/pics/thanos-compactor_webui-1.png" alt="thanos-compactor_webui-1" style="zoom:50%;" />

### All thanos k8s resources

![all-thanos-svc-sts-deploy-pod](doc/pics/thanos-svc-sts-deploy-pod.png)
