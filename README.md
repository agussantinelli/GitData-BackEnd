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
</div>

<hr>
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
      <td><b>Framework</b></td>
      <td>NestJS</td>
      <td>Arquitectura modular, mantenible y altamente testeable.</td>
    </tr>
    <tr>
      <td><b>Language</b></td>
      <td>TypeScript</td>
      <td>Contratos de interfaces robustos entre capas (Domain/Infra).</td>
    </tr>
    <tr>
      <td><b>External SDK</b></td>
      <td>Octokit (GitHub)</td>
      <td>Comunicación fluida y tipada con la API oficial de GitHub.</td>
    </tr>
    <tr>
      <td><b>Validation</b></td>
      <td>Zod</td>
      <td>Sanitización de DTOs y garantía de integridad de datos.</td>
    </tr>
    <tr>
      <td><b>Caching</b></td>
      <td>Redis / In-Memory</td>
      <td>Mitigación de Rate-Limits y optimización de latencia.</td>
    </tr>
    <tr>
      <td><b>Testing</b></td>
      <td>Vitest</td>
      <td>Pruebas unitarias de algoritmos y lógica de dominio.</td>
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
```
<hr />

<h2 align="left">⚖️ Licencia</h2>

<p align="left">
  Este proyecto está bajo la <b>Licencia GNU General Public License v3.0 (GPLv3)</b>. Puedes consultar los términos legales completos en el archivo 
  <a href="LICENSE"><code>LICENSE</code></a> incluido en la raíz de este repositorio.
</p>

<p align="left">
  <i>
    🤝 <b>Compromiso Copyleft:</b> La GPLv3 permite el uso, estudio, modificación y distribución de este software. Sin embargo, cualquier obra derivada o modificación distribuida debe ser publicada bajo esta misma licencia, garantizando que el software permanezca libre y accesible para todos.
  </i>
</p>
<hr />

<h2 align="left">🤝 Contribución</h2>

<p align="left">
  ¡Agradecemos enormemente tu interés en contribuir a este proyecto! Dado que este software se distribuye bajo la <b>Licencia GNU General Public License v3.0 (GPLv3)</b>, cualquier contribución que realices debe ser compatible con esta misma licencia.
</p>

<p align="left">
  Para contribuir:
  <ul>
    <li>Haz un <a href="https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/proposing-changes-with-pull-requests/creating-a-pull-request-from-a-fork" target="_blank">fork de este repositorio</a>.</li>
    <li>Crea una nueva rama para tu funcionalidad (<code>git checkout -b feature/nueva-funcionalidad</code>).</li>
    <li>Realiza tus cambios.</li>
    <li>Envía un <a href="https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/proposing-changes-with-pull-requests/creating-a-pull-request" target="_blank">Pull Request</a> detallando tus modificaciones.</li>
  </ul>
</p>

<p align="left">
  ¡Gracias por ser parte! 🙌✨
</p>

<hr>
<p align="center">Desarrollado con ❤️ y mucho 🧉 para la comunidad de GitHub</p>
