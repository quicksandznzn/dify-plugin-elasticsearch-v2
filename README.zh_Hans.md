## Elasticsearch (非预授权)

### 迁移说明

`quicksandzn/elasticsearch_v2` 将停止维护。请安装 [Elasticsearch](https://marketplace.dify.ai/plugin/quicksandzn/elasticsearch)，为每个连接分别保存一套凭据。将工作流中的 v2 查询或写入节点替换为对应工具，复制原有参数，为每个节点选择对应凭据，并更新下游节点对这些输出的引用。验证工作流后再卸载 v2。
