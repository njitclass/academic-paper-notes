# Changelog

All notable changes to this project will be documented in this file.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
Versioning follows [Semantic Versioning](https://semver.org/).

## [1.2.0] - 2026-02-26

### Added
- `references/` 子目录：按需加载的期刊档案、方法论与输出模板
- `docs/requirements-v1.2.md`：完整需求说明书
- `README.md`：跨平台安装文档
- `LICENSE`：MIT 开源许可证
- `CHANGELOG.md`：版本历史记录
- `AGENT.md`：发布规范与版本语义说明

### Changed
- SKILL.md frontmatter 补充 `compatibility`、`metadata` 字段
- description 精简至触发关键词聚焦版本
- 项目目录结构重组，符合 Agent Skills 规范

### Fixed
- 明确区分 Gemini CLI（`.agents/`）与 Antigravity（`.agent/`）安装路径

## [1.1.0] - 2026-02-01

### Added
- 双模式工作流：工程经济学路线（B）+ 计量实证路线（A）
- 混合型文章 A+B 并行输出支持
- 批量处理模式（每批 1 篇循环）
- 批判性四维追问框架

## [1.0.0] - 2026-01-15

### Added
- 初始发布
- 7 模块标准输出结构
- pdf skill 集成支持
