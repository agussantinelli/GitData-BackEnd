---
name: code-quality
description: SOLID principles, naming, and "No Comments" policy for GitData-BackEnd.
---

# 💎 GitData BackEnd Code Quality

Standardized rules for maintaining a robust NestJS engine.

## 📏 General Rules
1. **No Comments**: Code must be self-explanatory.
2. **SOLID**: Follow SOLID principles strictly.
3. **Single Responsibility**: Each service/method should do one thing well.
4. **Type Safety**: Use TypeScript and Zod to ensure data integrity across all layers.
is doing. If the code is complex, refactor it or use descriptive variable/function names.
   - *Exception*: Only use comments for complex algorithmic "why" or to document public APIs (JSDoc).
2. **Descriptive Names**: Use intention-revealing names for variables, functions, and classes.
3. **Small Functions**: Functions should do one thing and be small.
4. **DRY**: Don't Repeat Yourself. Abstract common logic.
5. **Clean Diff**: Keep your changes focused and remove any commented-out code before committing.
