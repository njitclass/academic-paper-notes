# Changelog

All notable changes to this project will be documented in this file.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
Versioning follows [Semantic Versioning](https://semver.org/).

## [1.6.0] - 2026-03-12

### Added
- 步骤0 新增“学科迁移方向确认”交互：接收输入后立即向用户展示 4 个学科方向选择清单，等待回复后再开始生成笔记

### Changed
- 模块6 方法论迁移地图：仅展开用户所选学科方向，未选方向一律略去，不输出占位符

---

## [1.5.0] - 2026-03-12

### Added
- 模块2 新增“核心对标文献”小节：含第一作者、年份、文献标题、期刊名称、该文局限、本文比较点

### Changed
- 模块1 题录信息：影响因子、数据可得性、代码可得性各自独立成行
- 模块3 格式规范 4：Caption 无法读取时必须标注，严禁推断或编造
- 模块4 公式规范：必须用原文符号/下标，不限路径，无法读取时标注不编造，符号说明仍保留

---

## [1.4.0] - 2026-03-12

### Added
- 新增模块3 🖼️ 图表导读：3–5 张关键图 + 2–3 张关键表，含图解/关键性/批判性观察
- 图格式：Fig. N；表格式：Table N（不缩写为 Tab.）
- 公式编号：\tag{Eq. N} 保留原文编号
- 原模块3–7 顺移为模块4–8

---

## [1.3.0] - 2026-02-26

### Fixed
- 补写平台原生文件写入机制，强制 8 模块写入 .md。禁止仅向对话流输出
- 修复 computer:// 链接格式
- 去除 Claude 专属表述，提升跨平台兼容性
- 强化输出约束：对话流仅允许路径+摘要
- 完善批量模式错误处理

---

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
