---
name: naming-conventions
description: NestJS naming standards for files and classes in GitData.
---

# 🏷️ GitData Naming Conventions

Standardized naming for a professional NestJS codebase.

## 📂 File Suffixes
- **Controllers**: `[name].controller.ts`
- **Services**: `[name].service.ts`
- **Modules**: `[name].module.ts`
- **DTOs**: `[name].dto.ts` (using Zod)
- **Entities**: `[name].entity.ts` (if applicable)

## 🔡 Case Sensitivity
1. **Files**: Always `kebab-case`.
2. **Classes**: Always `PascalCase` (e.g., `ProfileService`).
3. **Methods/Variables**: Always `camelCase`.
4. **Constants**: `UPPER_SNAKE_CASE`.
  - ❌ `src/services/auth.ts`
  - ❌ `src/services/AuthService.ts`

## Database (Drizzle ORM)

- **Rule**: Use `snake_case` for all table and column names in the database schema.
- **TypeScript Variables**: Use `camelCase` for the TypeScript variable that represents the table or column.
- **Example**:
  ```typescript
  // ✅ Correct
  export const lineaCompra = pgTable("linea_compra", {
    id: serial("id").primaryKey(),
    usuarioId: integer("usuario_id").references(() => usuario.id),
    fechaCreacion: timestamp("fecha_creacion"),
  });

  // ❌ Incorrect (Mixed Key Cases)
  export const LineaCompra = pgTable("LineaCompra", { ... });
  export const lineaCompra = pgTable("lineaCompra", { ... });
  ```

## Other Conventions

- **Directories**: Use `kebab-case` for all directory names.
- **Files**: Use `kebab-case` for most files, except for:
  - React/Astro components (PascalCase, e.g., `UserProfile.tsx`)
  - Classes (PascalCase, if the file exports a single class)
