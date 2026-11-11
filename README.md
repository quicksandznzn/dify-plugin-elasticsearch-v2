## Elasticsearch （Non-Pre-Auth）

- **Author:** [quicksandzn](https://github.com/quicksandznzn)
- **Github:** https://github.com/quicksandznzn/dify-plugin-elasticsearch-v2
- **Version:** 0.0.2
- **Type:** tool

### Deprecation notice

Use [Elasticsearch](https://marketplace.dify.ai/plugin/quicksandzn/elasticsearch) (`quicksandzn/elasticsearch`) for new workflows. This listing (`quicksandzn/elasticsearch_v2`) is being retired. Dify now lets you save multiple credentials for the maintained Elasticsearch plugin and select a credential for each tool node.

### Migrate an existing workflow

1. Install the maintained Elasticsearch plugin in your Dify workspace.
2. In its credential settings, create a named credential for each Elasticsearch connection. Copy the endpoint, certificate verification setting, and authentication details from your existing v2 node settings.
3. Replace each v2 Query or Create node with the corresponding tool from the maintained plugin. Copy its query or document settings, select the matching credential, and reconnect any downstream references to the node outputs.
4. Run the workflow and confirm that each node connects to the intended Elasticsearch instance before removing the v2 plugin.

### 迁移说明

`quicksandzn/elasticsearch_v2` 将停止维护。请安装 [Elasticsearch](https://marketplace.dify.ai/plugin/quicksandzn/elasticsearch)，为每个连接分别保存一套凭据。将工作流中的 v2 查询或写入节点替换为对应工具，复制原有参数，为每个节点选择对应凭据，并更新下游节点对这些输出的引用。验证工作流后再卸载 v2。

### Description
- Support version 7.17+
- Support mode create/query , delete and update not in plan
- This plugin is used to search for data in Elasticsearch.

### Usage

- Query Example

![img.png](_assets/img-7.png)

