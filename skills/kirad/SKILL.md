---
name: kirad
license: MIT
description: "Engineering guidance for development, testing, and problem fixing, including solution design, feature iteration, and writing documents or prompts for humans or agents."
---

# Keep It Right, Avoid Dirty Code

[简体中文](SKILL.zh.md)

## Common Sense

### Follow Clean Architecture and maintain a single source of truth

Follow Clean Architecture and the single source of truth principle when designing new features or making incremental changes to existing designs.

### Avoid unnecessary white-box descriptions

In documents and prompts, include implementation details when they help the reader use, understand, troubleshoot, or modify the relevant capability. Avoid white-box descriptions that do not serve the current task; they add unnecessary context load. Documents explaining implementation principles should include the relevant internals.

Focus on information that helps humans or agents use and understand those capabilities: black-box usage, the minimum necessary background and design rationale, troubleshooting, and interpreting outputs. Neither humans nor agents should have to become domain experts in a module just to use it.

- **Good:** A report export guide explains the export entry point, input requirements, output location, and troubleshooting. A prompt to debug a failed export includes the relevant call chain and logs.
- **Bad:** A report export usage guide walks through every internal class and call sequence before explaining how to export a report.

### Keep operational safeguards proportionate

Avoid excessive defensive operations, such as calculating hashes before and after Git or file operations without a concrete need. Match safeguards and verification effort to the actual risk and uncertainty.

### Write useful explanations instead of defensive disclaimers

In comments, documents, and prompts, explain the relevant behavior, purpose, and usage directly. Avoid self-protective disclaimers and irrelevant explanations of what an action does not mean or what was not done, such as "this does not imply..." or "did X but did not do Y." Wording that does not help the reader understand or act adds context load, entropy, and maintenance debt.

### Make explanations easy to understand

When communicating with collaborators, use diagrams when they make an explanation clearer; even a simple ASCII diagram can be more useful than a wall of text. Prefer familiar words, straightforward sentences, and explanations that are easy to follow and hard to misinterpret. Minimize invented jargon. Avoid assembling technical terms and convoluted syntax into prose that reads like an academic paper or patent specification.

When a description may be ambiguous, consider adding positive and negative examples to clarify the intended interpretation.

## Intent Routing

Apply Common Sense throughout the work, including when writing documents or prompts for humans or agents. Read only the references relevant to the current intent; if multiple intents apply, combine the relevant guidance.

| Intent | Guidance |
| --- | --- |
| Development: solution design, new features, or iteration on existing features | [Design and development](references/design-and-development.md); when implementing or iterating on user-facing functionality, also read [Functional verification](references/functional-verification.md). |
| Testing | [Functional verification](references/functional-verification.md) |
| Problem fixing | [Problem fixing](references/problem-fixing.md) and [Functional verification](references/functional-verification.md); also read [Design and development](references/design-and-development.md) if the fix changes the design. |
