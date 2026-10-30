# Yandex Market 智库｜AI 接入研究交接

这是供 IT 团队研究真实大模型接入的**脱敏源码交接副本**，与原站独立。仓库公开，无需申请访问。

## 获取完整源码

**[下载脱敏源码 ZIP](https://github.com/Lilrain-hub/yandex-market-ai-handoff/raw/refs/heads/main/yandex-market-ai-handoff-sanitized.zip)**

源码包包含 71 个文件：React/Vite 前端、现有知识搜索与路由、46 篇结构化研究文档、安全素材、运行说明、测试及语料导出脚本。请先下载并解压 ZIP；源码在解压后的 `yandex-market-ai-handoff/` 目录中。

本仓库以 ZIP 交付完整源码，GitHub 的 Code / Download ZIP 下载的是本交接仓库，仍需解压其中的源码包。

## 本地运行

准备 Node.js 22/24 和 pnpm 11，在解压后的源码目录运行：

```sh
pnpm install --frozen-lockfile
pnpm dev
```

```sh
pnpm test
pnpm check:public
pnpm export:knowledge
pnpm build
```

交接前已通过 5 项检查及生产构建。详情见源码包内 README。

## IT 同事从哪里开始

- **[AI 接入研究说明](AI-INTEGRATION.md)**：现有入口位置、数据结构、后续前后端职责与待确认问题。
- **[脱敏说明](REDACTION.md)**：本副本删除、替换和保留的内容。
- `src/HeroConsultation.jsx`：当前首页 AI 入口；只有筹备提示，尚未接入大模型。
- `src/knowledge-data.js`：文章、分类、FAQ 和导航的统一阅读模型。
- `data/knowledge-corpus.json`：46 篇研究文档，保留文章 ID、内容块、相对 URL 等来源回溯字段。

当前搜索是本地关键词搜索。尚未实现独立聊天页面、模型 API、后端服务、向量库、会话协议或 RAG。正式供应商与协议由技术团队确认，API 密钥、模型调用及知识检索应由后端处理。

## 使用边界

真实后台截图、原始文档、联系方式、内部分享地址、个人路径、部署配置及原仓库历史未纳入交接包；敏感商业和财务内容已替换为明确的研究占位，示例服务商已统一匿名化。保留公开平台品牌与官方链接。

**语料明确标记 `productionReady=false`，不能作为当前费用、回款政策或实际业务承诺。** 研究完成后，正式知识应经过授权、业务审核及受控导入。原站代码、内容及发布配置保持不动。

依赖及素材许可说明见源码包内 `NOTICE.md`；本仓库公开不表示原项目代码或素材自动获得额外开源授权。

源码包 SHA-256：

```text
e8793391929ed46afc8f876c49b3bc2f1e95008d6b065f9654c9b19fee6fe77f
```

交接日期：2026-10-30
