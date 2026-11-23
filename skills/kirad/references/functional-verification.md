# Functional Verification

[简体中文](functional-verification.zh.md)

## Prioritize real user workflows over unit test coverage

Do not become so focused on high unit test coverage that you neglect end-to-end functional verification from the user's perspective. Within reasonable cost, test user-facing functionality end to end as thoroughly as practical. Demonstrating that a feature actually works for users is more valuable than achieving 100% unit test coverage.

## Base verification claims on observed results

Report what you actually executed, what you observed, and the scope covered by that evidence. Do not present partial tests, mocked behavior, or static checks as proof that a real user workflow works end to end.

- **Good:** In the target environment, complete "create → save → reopen," confirm that the saved content is present, and report the environment, actions, and observed result.
- **Bad:** Mock the save API to return success, or observe HTTP 200 alone, and declare that creation, saving, and persistence all work.
