# devdocs-rag · 企业知识库智能客服

基于 Java 与 Spring AI 的开源智能客服项目：将企业产品资料转为可检索的知识库，提供带来源的问答，并用可复现的评测检查实际效果。

> 当前状态：已准备仓库和 15 篇中文知识资料；应用代码与问答功能尚未实现。以下能力为计划。

## 项目目标

完成一个能运行、能演示、能解释技术取舍的 Java AI 应用。协作按「实现一版 → 运行体验 → 修正问题 → 补充测试和说明」推进，围绕实际项目整理面试讲解材料。

完整范围见 [项目说明](docs/PROJECT_BRIEF.md)，交付顺序见 [开发里程碑](docs/ROADMAP.md)。

## 首版功能

- 导入 Markdown/TXT，保存来源与版本，避免重复导入。
- 文档切块、Embedding 与向量检索。
- 基于资料生成回答，并展示引用片段、来源和资料版本。
- 证据不足与模型故障时给出明确反馈。
- 提供可演示的问答页面、关键流程测试和固定问题集评测。

示例：「如何邀请团队成员，邀请链接多久过期？」→ 检索官方帮助文档 → 回答并展示可核查的出处。

## 技术路线

Java + Spring Boot + Spring AI；向量存储建议采用 PostgreSQL + pgvector。页面随 Java 应用启动，Python 在后续数据处理和评测有需要时使用。具体依赖版本与运行命令随首个可运行版本提供。

## 已准备的知识资料

[Dify Cloud 中文客服知识资料](data/knowledge/dify-cloud-zh/README.md)：15 篇官方文档，覆盖账号、团队权限、订阅、应用与知识库使用。

- `data/knowledge/dify-cloud-zh/documents/`：15 篇可读 Markdown，供后续导入。
- `originals/`、`sources.json` 和许可文件：保留原文、来源、提交版本与哈希。
- 第三方文档采用 CC BY 4.0；产品计费与配额代表固定提交的快照。

## 开源交付

以本仓库交付完整应用、安装说明、演示、测试、架构说明与评测结果。客服业务工具作为后续里程碑；专项微调在数据和效果需求明确后再评估。

仅提交自写或许可允许公开的数据。模型凭据、真实客服对话与非公开企业资料不入库。首版使用公开资料，后续接入私人知识时须实施服务端权限控制。

## 技术参考

- [Spring AI](https://docs.spring.io/spring-ai/reference/)
- [Spring AI RAG](https://docs.spring.io/spring-ai/reference/api/retrieval-augmented-generation.html)
- [Spring AI pgvector](https://docs.spring.io/spring-ai/reference/api/vectordbs/pgvector.html)

## 许可证

自有代码采用 [MIT License](LICENSE)。第三方文档、数据、模型及权重分别遵循原始许可；本仓库的 MIT 许可不替代这些条款。
