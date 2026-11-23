# My Skills

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![skills.sh](https://skills.sh/b/lkv1988/my-skill)](https://www.skills.sh/lkv1988/my-skill/kirad)
[![Security audits](https://img.shields.io/badge/Security_audits-View_reports-blue.svg)](https://www.skills.sh/lkv1988/my-skill/kirad)

[简体中文](README.zh.md)

A personal collection of reusable agent skills, developed and refined through everyday work.

## Skills

| Skill | Name | Purpose |
| --- | --- | --- |
| [kirad](skills/kirad/SKILL.md) | Keep It Right, Avoid Dirty Code | Engineering guidance for design, development, testing, and problem fixing. |

## Structure

Each skill lives in `skills/<skill-name>/`, with `SKILL.md` as its entry point. Supporting files are added only when needed.

```text
skills/
└── <skill-name>/
    ├── SKILL.md
    ├── scripts/       # Optional automation
    ├── references/    # Optional supporting documentation
    └── assets/        # Optional templates and resources
```

Skills are kept in a flat directory structure. This README serves as the index as the collection grows.

## Using the Skills

Install KIRAD in your project with the [Skills CLI](https://github.com/vercel-labs/skills). Requires Node.js 22.20 or later and npm.

```bash
npx skills add lkv1988/my-skill --skill kirad
```

Follow the installer prompts to select your agent. Add `--global` to make the skill available across projects.

Read the skill's `SKILL.md` for its guidance and references.

## License

[MIT](LICENSE)
