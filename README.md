<div align="center">

# ⚡ GIT DATA ⚡
### *The Ultimate GitHub Profile Intelligence Engine*

[![Vue 3](https://img.shields.io/badge/Frontend-Vue%203-42b883?style=for-the-badge&logo=vue.js)](https://vuejs.org/)
[![NestJS](https://img.shields.io/badge/Backend-NestJS-E0234E?style=for-the-badge&logo=nestjs)](https://nestjs.com/)
[![TypeScript](https://img.shields.io/badge/Language-TypeScript-3178C6?style=for-the-badge&logo=typescript)](https://www.typescriptlang.org/)
[![Clean Architecture](https://img.shields.io/badge/Architecture-Clean-white?style=for-the-badge&logo=architecture)](https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html)

**Git Data** es una plataforma de análisis avanzado diseñada para desglosar el "ADN" de cualquier perfil de GitHub. Utilizando algoritmos de curado de datos y una interfaz de estética *hacker* neón, transforma JSONs crudos en inteligencia accionable.

[Explorar Demo](#) • [Reportar Bug](https://github.com/user/git-data/issues) • [Documentación API](#)

</div>

---

## 🚀 Misión y Visión
El proyecto nace de la necesidad de ir más allá de las estadísticas superficiales. **Git Data** implementa el *Radar de ADN* y *The Hidden Gem* para identificar el verdadero impacto de un desarrollador en el ecosistema open source, todo bajo una arquitectura robusta, testeable y escalable.

---

## 🏗️ Arquitectura del Sistema
El repositorio está estructurado como un **NPM Monorepo**, garantizando coherencia técnica entre el cliente y el servidor.

### 🧩 Core Principles
* **Clean Architecture:** Separación estricta de capas (Dominio, Casos de Uso, Infraestructura).
* **Type Safety:** Uso de **Zod** para validación de esquemas y TypeScript estricto en todo el flujo.
* **Hacker Aesthetic:** UI basada en **PrimeVue** con overrides de **SCSS** para un look oscuro y neón.



---

## 🛠️ Stack Tecnológico

| Componente | Tecnología Principal | Librerías Clave |
| :--- | :--- | :--- |
| **Frontend** | Vue 3 (Composition API) | PrimeVue, Pinia, ECharts, SCSS |
| **Backend** | NestJS | Octokit (GitHub SDK), Cache Manager, Zod |
| **Testing** | Vitest / Cypress | Testing Library, Supertest |
| **DevOps** | Docker | GitHub Actions, Husky (Git Hooks) |

---

## 📦 Estructura del Proyecto

```text
git-data/
├── apps/
│   ├── api/                # Backend NestJS (Clean Architecture)
│   │   ├── src/
│   │   │   ├── domain/     # Entidades y lógica pura (Radar de ADN)
│   │   │   ├── use-cases/  # Orquestación de lógica de negocio
│   │   │   └── infra/      # Controladores, API de GitHub, DB
│   └── web/                # Frontend Vue 3
│       ├── src/
│       │   ├── components/ # UI Atoms/Molecules (PrimeVue)
│       │   ├── composables/# Lógica de estado y side-effects
│       │   └── styles/     # Temas Hacker (Neon SCSS)
├── packages/               # Tipos y utilidades compartidas
└── package.json            # Gestión de Workspaces
