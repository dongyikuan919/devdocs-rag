# devdocs-rag · 开发文档问答库

帮助开发者从项目文档中找到安装、配置和常见问题的答案，每次回答附上可核查的原文来源。

> 状态：仓库已初始化，业务功能尚未实现。以下是目标范围，不能视为已经可用的能力。

## 使用场景

“数据库连接应该怎么配置？” → 检索文档 → 给出配置说明和文件/章节出处；资料不足时明确说明。

## 首版计划

- 导入 Markdown/TXT 文档，保存文件与章节来源。
- 完成文本切块、向量检索和基于证据的问答。
- 提供简单交互页面；无法从资料确认的问题明确反馈。
- 固定至少 30 道评测题，记录答案正确性、引用有效性和失败案例。

## 项目衔接

提供文档检索能力与问题集，供项目二作为工具使用。先约定简单的 HTTP/文件接口，不提前拆公共 SDK。

- [devdocs-rag](https://github.com/dongyikuan919/devdocs-rag)：开发文档问答库。
- [issue-triage-agent](https://github.com/dongyikuan919/issue-triage-agent)：问题分诊助手。
- [issue-triage-lora](https://github.com/dongyikuan919/issue-triage-lora)：故障分诊微调实验。

## 开发路线

项目一 · 第 1～6 周；学习计划每周投入 8 小时：学习 2 小时、实现 4 小时、评测 1 小时、文档与提交 1 小时。

具体周计划见 [阶段路线图](docs/ROADMAP.md)。采用 Python 主线，实际依赖和运行命令在首个可运行版本中补充。

## 当前范围

首版只处理文本资料和一个项目的知识库；不扩展复杂 PDF/OCR、多人权限或通用知识平台。

## 数据与配置

仅提交自写或许可允许公开的样例。API 密钥、真实私人日志和未经授权的数据不入库；配置方案确定后提供 `.env.example`。

## 学习资料

[Hugging Face LLM Course](https://huggingface.co/learn/llm-course/chapter1/1)

## 许可证

自有代码采用 [MIT License](LICENSE)。第三方文档、数据、基础模型及权重分别遵循其原始许可，不能由本仓库的 MIT 许可证替代。
