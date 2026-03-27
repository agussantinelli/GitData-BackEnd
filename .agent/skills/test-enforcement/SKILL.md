---
name: test-enforcement
description: Mandatory rule requiring a corresponding test file for every business logic file in GitData.
---

# 🚔 GitData Test Enforcement

To ensure reliability, every logic file must have a corresponding test file.

## 📏 Rules
1. **Rule of One**: Every `.ts` file in `src/domain`, `src/use-cases`, or `src/infrastructure` MUST have a matching `.spec.ts` or `.test.ts` file.
2. **Naming**: `[filename].spec.ts`.
3. **Tools**: Use Jest (Standard NestJS configuration).
4. **Simultaneous Creation**: If a logic file is created, its test MUST be created in the same step.
