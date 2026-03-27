---
name: global-context
description: Directriz maestra del proyecto GitData-BackEnd. Provee el contexto arquitectónico global y OBLIGA al cumplimiento estricto del resto de las skills.
---

# 🌍 GitData BackEnd - Contexto Global

Esta es la **regla maestra** del proyecto. Todas las interacciones en el backend de GitData deben someterse a los lineamientos de **NestJS** y la arquitectura limpia.

## 🏛️ Contexto Arquitectónico (NestJS Modular)

El GitData BackEnd emplea una arquitectura modular basada en el framework **NestJS**.
- **Módulos por Dominio**: Cada feature (ej. `profile`, `github-sync`) debe estar encapsulada en un `Module`.
- **Inyección de Dependencias**: Uso estricto de `@Injectable()` y decoradores de NestJS.
- **Validación**: Uso de **Zod** y `nestjs-zod` para la validación de DTOs.

## ⚖️ Ley de Cumplimiento de Skills

Es OBLIGATORIO respetar las skills especializadas:
1. **`nest`**: Sigue el blueprint de Controllers, Services y Modules.
2. **`code-quality`**: Política de "No Comments" y SOLID.
3. **`naming-conventions`**: Uso de sufijos `.controller.ts`, `.service.ts`, `.module.ts`.
4. **`no-browser`**: PROHIBICIÓN TOTAL del subagente del navegador.

## 🛡️ Flujo de Implementación
1. Definir DTOs con Zod.
2. Crear/Actualizar el `Service` (Lógica de negocio/SDK Octokit).
3. Crear/Actualizar el `Controller` (Mapeo HTTP).
4. Registrar todo en el `Module`.
5. **Tests**: El testing es mandatorio para toda lógica de análisis de perfil (algoritmos).
