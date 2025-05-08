



Front: https://github.com/IT-Academy-BCN/ita-best-practices-guides/blob/main/MANUAL_REVISIONES.md

back: https://aspiring-gaura-1f9.notion.site/Guia-per-a-la-Revisi-en-Parelles-1b4d8c2a63c88050bee3d238c0e9f060



# Guía para Dar Feedback entre Estudiantes

## Introducción

Esta guía tiene como objetivo proporcionar un proceso estructurado y efectivo para hacer code review y dar feedback  entre compañeros de clase. Las code review no sólo permite mantener la calidad del código y detectar errores de manera anticipada, sino que también fomenta el aprendizaje colaborativo y el desarrollo profesional.

---

## ¿Cómo realizar una Code review?

### 1. Preparación

1. **Descarga y Prueba:** Descarga el proyecto del compañero y pruébalo en tu entorno local.
   
2. **Creación de Issue:** Crea una **issue** en el repositorio del compañero con el título:  
   - `Revisión Sprint [Número] - Feedback`. Esto facilita la organización y seguimiento del feedback.

### 2. Revisión del Proyecto

#### Funcionalidad

- Verifica que todas las características descritas en el README funcionen correctamente.
- Identifica errores visibles o casos no manejados.

#### Código y Clean Code

- Evalúa si el código sigue principios de **Clean Code**:
  - ¿Está bien estructurado y es fácil de entender?
  - ¿Se evita la duplicación de código?
  - ¿Los nombres de variables, funciones y clases son significativos?

#### Git y Gitflow

- Revisa el uso de Git:
  - ¿Los commits son descriptivos y pequeños?
  - ¿Se respetó la estructura de ramas (Gitflow)?
  - ¿El archivo `.gitignore` está configurado correctamente?

#### Documentación (README)

- Asegúrate de que el README sea claro y completo:
  - ¿Describe el propósito del proyecto y las tecnologías utilizadas?
  - ¿Incluye instrucciones de instalación y ejecución?

#### Estilo y Usabilidad

- Evalúa el diseño y la usabilidad:
  - ¿El diseño es responsive y atractivo?
  - ¿Se manejan adecuadamente los errores para el usuario?
  - ¿Los estilos están bien organizados y no hay redundancia?

### 3. Dar Feedback

- Usa un lenguaje constructivo y amigable:
  - Elogia lo que está bien hecho.
  - Identifica áreas de mejora específicas.
  - Ofrece sugerencias claras para la mejora continua.

### 4. Formato de la Issue de Feedback

**Revisión de Proyecto**

**1. Funcionalidad:**
- Todas las características descritas en el README funcionan correctamente.
- Se observaron errores al procesar formularios vacíos.

**2. Código y Clean Code:**
- El código es legible y sigue principios de Clean Code.
- Se encontró duplicación de código en las funciones `calculateTotal` y `calculateTax`.

**3. Git y Gitflow:**
- Los commits son descriptivos y claros.
- Falta respetar la estructura de Gitflow para un flujo de trabajo más ordenado.

**4. Documentación (README):**
- El README es informativo y completo.
- Se recomienda añadir capturas de pantalla del proyecto para facilitar la comprensión.

**5. Estilo y Usabilidad:**
- El diseño es atractivo y responsive.
- Algunos estilos CSS podrían optimizarse para evitar redundancias.

### Feedback General

¡Excelente trabajo! El proyecto es funcional y tiene un diseño atractivo. Para mejorar, te sugeriría modularizar el código para facilitar su mantenimiento y asegurar que se respeten las convenciones de Gitflow para un desarrollo más estructurado.

---

Con esta guía, los estudiantes tendrán un marco claro para evaluar y mejorar los proyectos de sus compañeros, fomentando un ambiente colaborativo y de aprendizaje continuo.