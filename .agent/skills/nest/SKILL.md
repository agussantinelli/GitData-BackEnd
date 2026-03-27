---
name: nest
description: Core architectural rules for NestJS, Modules, Controllers, and Services in GitData.
---

# 🦅 NestJS - Core Architecture

Guide for maintaining the modular integrity of the GitData Engine.

## 🏗 Modular Structure
Each domain feature MUST be encapsulated in its own module:
- `FeatureModule`: Root of the feature.
- `FeatureController`: HTTP endpoints and request handling.
- `FeatureService`: Business logic and data access.

## 🛠 Decorators
1. **Controllers**: Use `@Controller('path')`.
2. **Methods**: Use `@Get()`, `@Post()`, `@Put()`, `@Delete()`.
3. **Dependency Injection**: Use `@Injectable()` for services and inject them via `constructor`.

## 🛡 Validation (Zod)
- Use `ZodValidationPipe` or `nestjs-zod` for DTO validation.
- Every incoming request MUST have a corresponding DTO.

## 🧪 Testing
- **Unit Tests**: Mock dependencies using `@nestjs/testing` or `vi.mock`/`jest.mock`.
- **Logic**: All algorithms involving profile analysis MUST have high test coverage.
