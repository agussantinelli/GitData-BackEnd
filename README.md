<div align="center">

<h1 align="center">🛡️ Git Data – BackEnd</h1>

<p align="center">
  <a href="https://github.com/agussantinelli/GitData-FrontEnd" target="_blank" style="text-decoration: none;">
    <img src="https://img.shields.io/badge/💻%20Repo%20Frontend-Vue%203-42b883?style=for-the-badge&logo=vue.js&logoColor=white" alt="Repo Frontend"/>
  </a>
  <a href="https://github.com/agussantinelli/GitData-BackEnd" target="_blank" style="text-decoration: none;">
    <img src="https://img.shields.io/badge/⚙️%20Repo%20Backend-GitData-E0234E?style=for-the-badge&logo=github&logoColor=white" alt="Repo Backend"/>
  </a>
</p>

<p align="center">
  <a href="https://github.com/agussantinelli" target="_blank" style="text-decoration: none;">
    <img src="https://img.shields.io/badge/👤%20Agustín%20Santinelli-agussantinelli-000000?style=for-the-badge&logo=github&logoColor=white" alt="Agus"/>
  </a>
  <a href="https://github.com/martin-ratti" target="_blank" style="text-decoration: none;">
    <img src="https://img.shields.io/badge/👤%20Martín%20Ratti-martin--ratti-000000?style=for-the-badge&logo=github&logoColor=white" alt="Martín"/>
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/NestJS-10.0.0-E0234E?style=for-the-badge&logo=nestjs&logoColor=white" alt="NestJS Badge"/>
  <img src="https://img.shields.io/badge/Node.js-20.0.0-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node Badge"/>
  <img src="https://img.shields.io/badge/TypeScript-5.0.0-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TS Badge"/>
  <img src="https://img.shields.io/badge/pnpm-10.0.0-F69220?style=for-the-badge&logo=pnpm&logoColor=white" alt="pnpm Badge">
  <img src="https://img.shields.io/badge/Octokit-SDK-white?style=for-the-badge&logo=github&logoColor=black" alt="Octokit Badge"/>
  <img src="https://img.shields.io/badge/Zod-Validation-3E67B1?style=for-the-badge&logo=zod&logoColor=white" alt="Zod Badge"/>
  <img src="https://img.shields.io/badge/Vitest-Testing-6E9F18?style=for-the-badge&logo=vitest&logoColor=white" alt="Vitest Badge"/>
  <img src="https://img.shields.io/badge/Swagger-API%20Docs-85EA2D?style=for-the-badge&logo=swagger&logoColor=black" alt="Swagger Badge"/>
  <img src="https://img.shields.io/badge/Redis-Caching-DC382D?style=for-the-badge&logo=redis&logoColor=white" alt="Redis Badge"/>
</p>

**GitData-BackEnd** es el motor analítico de Git Data. Construido bajo los principios de **Clean Architecture**, procesa y cura datos masivos de la API de GitHub para generar inteligencia sobre perfiles técnicos.

</div>

---

## 🎯 Objetivo y Propósito

### El "Por Qué" de Git Data
En un ecosistema saturado de métricas vanidosas (como el número de contribuciones o "streaks"), los reclutadores y líderes técnicos a menudo pierden de vista el **impacto real** y la **calidad técnica** de un desarrollador. 

**Git Data** nace para resolver la opacidad en el análisis de perfiles de GitHub, transformando datos crudos en una radiografía técnica precisa.

### Objetivos Estratégicos
* **🔍 Análisis de ADN Técnico:** Desglosar el stack real de un usuario basándose en la complejidad de sus repositorios, no solo en sus lenguajes más usados.
* **💎 The Hidden Gem (La Joya Oculta):** Algoritmo diseñado para identificar repositorios con alto valor técnico o arquitectónico que suelen quedar enterrados por proyectos menores.
* **📊 Visualización de Alto Impacto:** Sustituir tablas aburridas por un **Radar de Competencias** y **Timelines de Evolución** interactivos, permitiendo una toma de decisiones basada en datos (Data-Driven).
* **🚀 Optimización de Reclutamiento:** Reducir el tiempo de revisión de perfiles técnicos mediante un resumen ejecutivo generado por inteligencia analítica.

> **Propósito Final:** Empoderar a la comunidad dev y a los Tech-Recruiters con una herramienta de auditoría técnica que premie la calidad, la consistencia y la arquitectura sobre el simple volumen de código.

---

## 🏗️ Arquitectura y Diseño
El servidor está diseñado para ser agnóstico a la infraestructura, centrando su valor en el **Dominio**.

* **Entidades/Dominio:** Lógica pura para el cálculo del "Radar de ADN" y "The Hidden Gem".
* **Casos de Uso:** Orquestación de servicios (ej. `AnalyzeUserProfile`).
* **Infraestructura:** Adaptadores para Octokit (GitHub API), caché de datos y persistencia.
* **Seguridad:** Implementación de Rate Limiting y validación estricta con Zod.

---

## 🚀 Características Core
* **Procesamiento Big O Optimizado:** Algoritmos de curado de JSON para manejar repositorios extensos sin latencia.
* **Estrategia de Caché:** Mitigación de límites de la API de GitHub mediante capas de caché temporales.
* **Documentación Proactiva:** Swagger UI integrado para pruebas rápidas de los endpoints.

---

## 📦 Estructura de Capas

```text
src/
├── domain/          # Lógica de Negocio Pura (Entities, Value Objects)
├── use-cases/       # Servicios de Aplicación (Lógica de Orquestación)
├── infrastructure/  # Controladores, Módulos Externos, API GitHub
├── shared/          # DTOs, Decoradores, Excepciones Globales
└── main.ts          # Punto de entrada de la aplicación
