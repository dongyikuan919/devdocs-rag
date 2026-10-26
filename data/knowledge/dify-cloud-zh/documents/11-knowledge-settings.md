# 调整知识库设置

> 来源：[Dify 官方文档](https://github.com/langgenius/dify-docs/blob/9b666acf0a07a4f93e2d14ca9914a1ca227e2f93/zh/cloud/use-dify/knowledge/manage-knowledge/introduction.mdx)
> 署名：LangGenius / Dify documentation contributors；许可：[CC BY 4.0](../LICENSE-CC-BY-4.0.txt)。
> 下载日期：2026-10-26；上游提交：`9b666acf0a07a4f93e2d14ca9914a1ca227e2f93`。
> 本文为格式整理版本：保留正文、FAQ、表格与警告，移除展示组件和截图引用；原文见 [MDX](../originals/11-knowledge-settings.mdx)。

> 本文档由 AI 自动翻译。如有任何不准确之处，请参考 [英文原版](https://docs.dify.ai/en/cloud/use-dify/knowledge/manage-knowledge/introduction)。

**说明：**
只有工作空间所有者、管理员和编辑者可修改知识库设置。

在知识库中，点击左侧边栏的 **设置** 图标，进入设置页。

| 设置项                | 说明          |
|:----------------------- |:---------------------|
| 名称和图标             | 用于标识和区分知识库。|
| 描述                  | 简要说明知识库的用途和内容。|
| 权限                  | 定义哪些工作空间成员可访问该知识库。**注意：** 被授予访问权限的成员将拥有 [维护知识库内容](https://docs.dify.ai/zh/cloud/use-dify/knowledge/manage-knowledge/maintain-knowledge-documents) 中列出的全部权限。|
| 索引方式               | 决定文档分段的处理和组织方式。详见 [选择索引方式](https://docs.dify.ai/zh/cloud/use-dify/knowledge/create-knowledge/setting-indexing-methods#选择索引方式)。|
| 嵌入模型               | 选择用于将文档分段转化为向量的嵌入模型。**说明：** 更换嵌入模型将对所有分段重新进行向量化。|
| 摘要自动生成           | 自动为文档分段生成摘要。**说明：** 启用后，仅对新添加的文档和分段生效。对于已有分段，请在文档列表中选择文档，然后点击 **生成摘要**。|
| 检索设置               | 决定知识库如何检索相关内容。详见 [指定检索设置](https://docs.dify.ai/zh/cloud/use-dify/knowledge/create-knowledge/setting-indexing-methods#指定检索设置)。|
