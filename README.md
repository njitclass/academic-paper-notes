# academic-paper-notes

顶刊学术论文深度学习笔记生成器，专为**能源工程经济学 / 管理科学 / 营销学 / MPaCC** 方向的研究者设计。

**核心价值：** 方法论精准提取 × 批判性缺陷识别 × 跨领域迁移建议 × 研究灵感触发

## 双路线支持

| 路线 | 适用期刊 | 核心方法 |
|------|----------|----------|
| **B · 工程经济学** | Nature Energy、Applied Energy | LCOE / 系统优化 / LCA / 博弈 / 鲁棒优化 |
| **A · 计量实证** | Energy Economics、TAR、AER | DID / IV / RDD / 面板数据 |
| **A+B · 混合** | 兼具两类方法的文章 | 并行输出两路分析 |

## Installation

### 安装到当前项目（自动检测已安装平台）

```bash
npx skills add njitclass/academic-paper-notes
```

### 安装到全局（跨项目可用）

```bash
npx skills add -g njitclass/academic-paper-notes
```

### 仅安装到指定平台

```bash
npx skills add njitclass/academic-paper-notes -a claude-code
npx skills add njitclass/academic-paper-notes -a codex
npx skills add njitclass/academic-paper-notes -a gemini-cli
npx skills add njitclass/academic-paper-notes -a antigravity
npx skills add njitclass/academic-paper-notes -a cursor
```

### 安装到所有平台（跳过确认）

```bash
npx skills add njitclass/academic-paper-notes --all
```

### 各平台安装路径

| 平台 | `--agent` 值 | 项目路径 | 全局路径 |
|------|-------------|----------|----------|
| Claude Code | `claude-code` | `.claude/skills/academic-paper-notes/` | `~/.claude/skills/` |
| Codex CLI | `codex` | `.agents/skills/academic-paper-notes/` | `~/.codex/skills/` |
| Gemini CLI | `gemini-cli` | `.agents/skills/academic-paper-notes/` | `~/.gemini/skills/` |
| Antigravity | `antigravity` | `.agent/skills/academic-paper-notes/` | `~/.gemini/antigravity/skills/` |
| Cursor | `cursor` | `.agents/skills/academic-paper-notes/` | `~/.cursor/skills/` |

> **注意：** Gemini CLI 与 Antigravity 是两个独立 agent，路径不同，请勿混淆。
> - Gemini CLI 项目路径：`.agents/skills/`（复数）
> - Antigravity 项目路径：`.agent/skills/`（单数）

## 触发方式（所有平台一致）

安装后直接对话，无需额外参数：

- "帮我读这篇文章"
- "分析这篇论文"
- "生成读书笔记"
- "方法论迁移"
- "研究切入口"
- 上传 PDF 或粘贴论文内容

`references/` 中的参考文件（期刊档案、方法论指南、输出模板等）会在需要时自动按需加载，无需手动指定。

## 输出格式

- 文件命名：`note-{第一作者姓}-{年份}-{标题前5实词}.md`
- 包含带 APA 题录的结构化 Markdown 笔记
- 对话仅输出文件链接 + 400 字结构化摘要

## 依赖

- **pdf skill**：处理 PDF 输入时必需（读取全文）

## License

MIT © Zhentao Zhu
