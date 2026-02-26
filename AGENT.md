# AGENT.md — 发布规范

## 版本语义

| 变更类型 | 版本位 | 示例 |
|----------|--------|------|
| bug 修复 | patch | 1.2.x |
| 新增功能 | minor | 1.x.0 |
| 破坏性变更 | major | x.0.0 |

## 每次发布必须完成

1. 更新 `SKILL.md` frontmatter 中的 `version` 字段
2. 在 `CHANGELOG.md` 顶部插入新版本记录（Keep a Changelog 格式）
3. commit message 格式：`chore: release vX.X.X`
4. 创建 Git tag：`vX.X.X`

## 文件位置

- 主技能文件：`SKILL.md`（保持 < 500 行）
- 参考文件：`references/*.md`（按需加载，不计入行数限制）
- 需求文档：`docs/requirements-v1.2.md`
- 发布规范：`AGENT.md`（本文件）

## references/ 按需加载规则

| 文件 | 加载时机 |
|------|----------|
| `journal-profiles.md` | 期刊归属判断模糊时 |
| `method-econometrics.md` | 模式 A（计量实证）激活时 |
| `method-engineering-econ.md` | 模式 B（工程经济学）激活时 |
| `transfer-guide.md` | 每篇必加载，生成模块 5 前 |
| `output-template.md` | 每篇必加载，输出前格式校验 |
