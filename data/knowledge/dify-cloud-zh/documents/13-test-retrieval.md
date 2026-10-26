# 测试检索

> 来源：[Dify 官方文档](https://github.com/langgenius/dify-docs/blob/9b666acf0a07a4f93e2d14ca9914a1ca227e2f93/zh/cloud/use-dify/knowledge/test-retrieval.mdx)
> 署名：LangGenius / Dify documentation contributors；许可：[CC BY 4.0](../LICENSE-CC-BY-4.0.txt)。
> 下载日期：2026-10-26；上游提交：`9b666acf0a07a4f93e2d14ca9914a1ca227e2f93`。
> 本文为格式整理版本：保留正文、FAQ、表格与警告，移除展示组件和截图引用；原文见 [MDX](../originals/13-test-retrieval.mdx)。

> 本文档由 AI 自动翻译。如有任何不准确之处，请参考 [英文原版](https://docs.dify.ai/en/cloud/use-dify/knowledge/test-retrieval)。

在知识库中，点击左侧边栏的 **检索测试** 图标，进入测试页面。在这里，可模拟用户提问以测试知识库的检索效果，并尝试不同的检索设置以获得最佳结果。

**注意：**
    在召回测试中调整的检索设置，仅在当前测试会话中临时生效。

**提示：**
    关于检索参数的更多说明，阅读 [指定检索设置](https://docs.dify.ai/zh/cloud/use-dify/knowledge/create-knowledge/setting-indexing-methods#指定检索设置)。

**记录** 板块记录与该知识库相关的所有检索事件，包括：

- 在 **召回测试** 页面进行的测试检索
- 由任何关联应用发起的常规检索请求（无论是测试还是生产环境）

**说明：**
    召回测试与常规检索共用一个 API 接口。
