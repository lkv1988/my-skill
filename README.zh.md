# My Skills

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![skills.sh](https://skills.sh/b/lkv1988/my-skill)](https://www.skills.sh/lkv1988/my-skill/kirad)
[![Security audits](https://img.shields.io/badge/Security_audits-View_reports-blue.svg)](https://www.skills.sh/lkv1988/my-skill/kirad)

[English](README.md)

个人可复用 Agent Skill 集合，在日常工作中积累并持续打磨。

## 技能索引

| Skill | 名称 | 用途 |
| --- | --- | --- |
| [kirad](skills/kirad/SKILL.zh.md) | Keep It Right, Avoid Dirty Code | 面向方案设计、开发、测试与问题修复的工程实践指引。 |

## 目录结构

每个 Skill 放在 `skills/<skill-name>/` 中，以 `SKILL.md` 为入口。仅在实际需要时添加辅助文件。

```text
skills/
└── <skill-name>/
    ├── SKILL.md
    ├── scripts/       # 可选的自动化脚本
    ├── references/    # 可选的补充文档
    └── assets/        # 可选的模板和资源
```

技能目录保持平铺，随着集合增长，由本 README 提供索引。

## 使用方式

通过 [Skills CLI](https://github.com/vercel-labs/skills) 将 KIRAD 安装到项目中。需要 Node.js 22.20 或更高版本及 npm。

```bash
npx skills add lkv1988/my-skill --skill kirad
```

按照安装提示选择所用 Agent。添加 `--global` 可在各项目中使用。

阅读技能的 `SKILL.md`，了解具体指引与参考文档。

## 许可证

[MIT](LICENSE)
