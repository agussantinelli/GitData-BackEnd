---
name: readme-auto-sync
description: Mandatory rules for updating the README.md automatically in GitData-BackEnd.
---

# 🔄 GitData README Auto-Sync

Guidelines for keeping the BackEnd README synchronized.

## 📏 Rules
1. **Estructura de Capas**:
   - **CUÁNDO**: Cada vez que crees, muevas o elimines un archivo `.ts` o un directorio en `src/`.
   - **QUÉ HACER**: Actualizar el bloque `<pre>` de "Estructura de Capas" en el `README.md`.
2. **Tests Status**:
   - **CUÁNDO**: Al agregar nuevos tests de Jest.
   - **QUÉ HACER**: Actualizar el contador de tests si existe un badge o sección específica.
