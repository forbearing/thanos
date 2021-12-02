### 1. `prometheus.yaml` 说明了 prometheus 需要修改的内容

### 2. `thanos-objstore.yaml` 指定对象存储 bucket，没有对象存储也可以部署 thanos



### 3. grafana 添加 thanos-querier 数据源

<img src="doc/pics/grafana_add-thanos-querier.png" alt="grafana_add-thanos-querier" style="zoom:50%;" />



### 4. thanos-querier 截图

<img src="doc/pics/thanos-query_stores.png" alt="thanos-query_stores" style="zoom:50%;" />

### 5. thanos 所有的 pod 和 service

![all-thanos-service](doc/pics/all-thanos-service.png)

![all-thanos-pod](doc/pics/all-thanos-pod.png)