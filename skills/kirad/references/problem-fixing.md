# Problem Fixing

[简体中文](problem-fixing.zh.md)

## Assess the problem and determine where the fix belongs

Before treating an observed behavior as a repair task, assess it against the actual goal: is it a problem that needs solving, does it affect the goal, who is responsible for it, and is its repair within the current scope? Do not assume every obstacle should be resolved through changes to the current project.

Use the evidence to determine the appropriate response and where a fix belongs. Investigating a root cause does not mean taking over responsibility for repairing the component that contains it. Proceed directly when the action is clear and within scope; discuss necessary changes to the goal, scope, or important tradeoffs with the collaborator.

- **Good:** A CLI invoked by the project crashes internally. The caller reports the failure and preserves the necessary diagnostic information. Attribute the defect to the CLI and address its repair within the appropriate scope.
- **Bad:** The caller matches the CLI's crash stack trace, adds special branches and compensating behavior, and invents an explanation that presents the internal defect as invalid user input.

## Understand and address the root cause

Investigate beyond surface observations and establish the actual root cause before choosing a fix. Choose a solution that addresses the underlying problem rather than merely patching its visible symptoms.

Do not use inappropriate mocks to bypass failing behavior or make tests pass while leaving the underlying problem unresolved.

The underlying goal is to keep the engineering project correct as it evolves, rather than merely make the immediate task appear complete. A superficial fix or a passing test result does not establish that the problem has been resolved.
