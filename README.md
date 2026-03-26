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

<br>
<h2>🎯 Objetivo y Propósito</h2>

<p align="justify">
  En un ecosistema saturado de métricas vanidosas, los reclutadores y líderes técnicos a menudo pierden de vista el <b>impacto real</b> y la <b>calidad técnica</b> de un desarrollador. <b>Git Data</b> nace para resolver la opacidad en el análisis de perfiles de GitHub, transformando datos crudos en una radiografía técnica precisa.
</p>

<ul>
  <li><b>🔍 Análisis de ADN Técnico:</b> Desglosar el stack real basándose en la complejidad de los repositorios.</li>
  <li><b>💎 The Hidden Gem:</b> Algoritmo para identificar proyectos con alto valor arquitectónico oculto.</li>
  <li><b>📊 Visualización de Alto Impacto:</b> Radar de competencias y timelines interactivos para decisiones <i>Data-Driven</i>.</li>
  <li><b>🚀 Optimización de Reclutamiento:</b> Reducción drástica en los tiempos de revisión de perfiles técnicos.</li>
</ul>

<blockquote>
  <p>
    <i>"Empoderar a la comunidad dev con una herramienta de auditoría que premie la calidad y la arquitectura sobre el simple volumen de código."</i>
  </p>
</blockquote>

<hr>
<h2>🛠️ Stack Tecnológico</h2>

<table>
  <thead>
    <tr style="background-color: #1a1a1a;">
      <th>Categoría</th>
      <th>Tecnología</th>
      <th>Propósito</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><b>Core Framework</b></td>
      <td>Vue 3 (Composition API)</td>
      <td>Reactividad eficiente y componentes desacoplados.</td>
    </tr>
    <tr>
      <td><b>Build Tool</b></td>
      <td>Vite</td>
      <td>HMR instantáneo para desarrollo ágil.</td>
    </tr>
    <tr>
      <td><b>UI Library</b></td>
      <td>PrimeVue</td>
      <td>Componentes de alta gama con personalización profunda.</td>
    </tr>
    <tr>
      <td><b>State Management</b></td>
      <td>Pinia</td>
      <td>Almacenamiento centralizado y modular del estado.</td>
    </tr>
    <tr>
      <td><b>Data Viz</b></td>
      <td>Apache ECharts</td>
      <td>Renderizado de radares de ADN y mapas de calor.</td>
    </tr>
    <tr>
      <td><b>Styles</b></td>
      <td>SCSS + Neon Theme</td>
      <td>Arquitectura de estilos para la estética Hacker-Dark.</td>
    </tr>
  </tbody>
</table>
<hr>

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
