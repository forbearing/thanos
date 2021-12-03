### thanos receive

- 如果没有对象存储，在配置文件 `thanos-receive.yaml` 中把 `--objstore.config-file=/config/bucket.yaml` 选项注释掉
- 如果没有对象存储，可以把 `- --tsdb.retention=15d` 保留天数调大，比如 `15d`，如果有对象存储可以把它调整为 `2d`
