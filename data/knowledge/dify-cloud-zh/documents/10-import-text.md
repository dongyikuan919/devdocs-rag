# 上传本地文件

> 来源：[Dify 官方文档](https://github.com/langgenius/dify-docs/blob/9b666acf0a07a4f93e2d14ca9914a1ca227e2f93/zh/cloud/use-dify/knowledge/create-knowledge/import-text-data/readme.mdx)
> 署名：LangGenius / Dify documentation contributors；许可：[CC BY 4.0](../LICENSE-CC-BY-4.0.txt)。
> 下载日期：2026-10-26；上游提交：`9b666acf0a07a4f93e2d14ca9914a1ca227e2f93`。
> 本文为格式整理版本：保留正文、FAQ、表格与警告，移除展示组件和截图引用；原文见 [MDX](../originals/10-import-text.mdx)。

> 本文档由 AI 自动翻译。如有任何不准确之处，请参考 [英文原版](https://docs.dify.ai/en/cloud/use-dify/knowledge/create-knowledge/import-text-data/readme)。

**注意：**
    知识库创建后，其数据源无法更改。

创建即用型知识库时，可上传本地文件作为其数据源：

1. 点击 **知识库** > **创建** > **创建即用型知识库**。

2. 选择 **导入已有文本** 作为数据源，然后上传文件。

上传限制因套餐而异（[了解更多](https://dify.ai/zh/pricing)）：

| | Sandbox | Professional 和 Team |
|:--|:--|:--|
| 单次上传文件数 | 1 | 50 |
| 单个文件大小 | 15 MB | 50 MB |
---

**对于文件中的图片**

    JPG、JPEG、PNG 和 GIF 格式且小于 2 MB 的图片将作为附件，自动提取到对应的分段。这些图片可独立管理，并在检索时与分段一同返回。

    提取的图片 URL 会保留在分段文本中，但你可以放心删除这些 URL 以保持文本整洁，这不会影响已提取的图片。

    若在索引设置中选择多模态嵌入模型（带有 **Vision** 图标），则提取出的图片也将被向量化并索引以供检索。

    每个分段最多支持 10 个图片附件，超出的图片不会被提取。

    以上提取规则适用于如下图片类型：

    - DOCX 和 XLSX 文件中嵌入的图片

        **提示：**
            其他文件类型（如 PDF）中嵌入的图片，可通过在 [知识流水线](https://docs.dify.ai/zh/cloud/use-dify/knowledge/knowledge-pipeline/readme) 中使用合适的文档提取插件进行提取。

    - 在任何文件类型中，通过以下 Markdown 语法引用、URL 可访问的图片：

        - `![alt text](image_url)`
        - `![alt text](image_url "optional title")`
