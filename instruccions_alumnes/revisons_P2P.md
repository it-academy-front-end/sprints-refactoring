# Guía para Code Review y Feedback entre Estudiantes

## Introducción

Esta guía tiene como objetivo proporcionar un proceso estructurado y efectivo para hacer code review y dar feedback  entre compañeros de clase (parejas).

**¿Por qué es importante?**
- Aprendizaje activo: Descubres nuevas soluciones y buenas prácticas.
- Calidad del código: Detectas errores antes y mejoras la mantenibilidad.
- Habilidad profesional: El code review es esencial en entornos laborales. 

## ¿Cómo Realizar una Code Review?

### 1. Preparación

1. **Descarga y Prueba:** Descarga el proyecto del compañero y pruébalo en tu entorno local.
   
2. **Creación de Issue:** Crea una **issue** en el repositorio de la dueña del proyecto con el título:  
- `Code review Sprint [Número] - [Nombre-revisa]`. Esto facilita la organización y seguimiento del feedback.

### 2. Métodos de Revisión

1. **Revisión Asíncrona (GitHub Issues)**
- Sigue los **criterios técnicos de revisión** detallados más abajo.
- Documenta tus hallazgos en la issue usando el **formato de documentación de una code review** detallado mas abajo.
 
2. **Revisión en Parelles (Síncrona/Presencial)**
- La revisión se realiza de manera síncrona, presencialmente y por parejas.
- El **autor** explica: el objetivo de la solución, las decisiones técnicas tomadas, los puntos clave a considerar.
- El **revisor**: lee el código detenidamente, identifica posibles mejoras, plantea dudas y propuestas de cambio y documenta sus hallazgos en la issue usando el **formato de documentación de una code review** detallado mas abajo.

## Criterios Ténicos a Observar en una Code Review
1. **Cumplimiento del Enunciado**
- Verificar que la solución cumple todos los requisitos especificados.
- Asegurar que las funcionalidades obligatorias están implementadas correctamente.
- Comprobar que los casos especiales y posibles errores se gestionan adecuadamente.
- Revisar que el código está escrito en inglés: nombres de clases, métodos, variables y comentarios.

2. **Calidad del código**
    **Formato y Convenciones**
    - Mantener una indentación coherente según los estándares del lenguaje.
    - Usar correctamente espacios y saltos de línea en estructuras de control.
    - Escribir comentarios breves y claros solo cuando sean necesarios.
    - Mantener una organización consistente en todos los archivos del proyecto.

    **Nomenclatura**
    - Usar nombres descriptivos para clases, métodos y variables.
    - Evitar abreviaturas poco claras o nombres genéricos.
    - Seguir las convenciones de nomenclatura establecidas en el proyecto.
    - Emplear nombres que indiquen la función o responsabilidad de cada elemento.

    **Métodos Cortos con Única Responsabilidad**
    - Verificar que los métodos y clases sean concisos y no hagan demasiadas cosas.
    - Aplicar el principio de responsabilidad única para mejorar legibilidad y mantenimiento.
    - Considerar dividir métodos complejos en otros más específicos cuando sea necesario.

    **Control de la Complejidad**
    - Reducir condicionales y bucles anidados innecesarios.
    - Usar estrategias como early returns o fail fast para simplificar la lógica.
    - Evitar el uso excesivo de variables temporales o flags que compliquen el flujo.

    **Estructuras de Datos**
    - Elegir las colecciones adecuadas para cada tipo de dato.
    - Evitar iteraciones o modificaciones ineficientes de listas y conjuntos.
    - Considerar construcciones del lenguaje que puedan simplificar la lógica.

3. **Robustez y Manejo de Errores**
- Garantizar que las excepciones se manejan correctamente.
- Evitar capturas demasiado genéricas, priorizando manejo específico de errores.
- Minimizar el uso de valores nulos, empleando alternativas que mejoren el control.
- Asegurar que no hay errores que queden sin tratamiento o notificación.

4. **Estructura del Proyecto**
- Verificar que las clases están organizadas coherentemente en paquetes.
- Comprobar que los archivos tienen nombres apropiados que reflejen su propósito.
- Asegurar que las dependencias están bien gestionadas sin imports innecesarios.

    **Archivo  .gitignore**
    - Incluir archivos que no deben estar en el repositorio (ej: de compilación).
    - Revisar que no se exponen secretos ni datos sensibles.

    **Archivo README.md** confirmar que incluye:
    - Descripción y propósito del proyecto.
    - Tecnologías utilizadas.
    - Instrucciones claras para configuración y ejecución.
    - Capturas de pantalla o demos cuando sea relevante.

## ¿Cómo Dar Feedback Efectivo?
Una buena revisión no solo señala errores, sino que inspira mejoras y celebra los aciertos.
¿Listos para convertiros en expertos en code review? ¡A practicar! 💻🔍

1. **Buenas Practicas de una Code review**
- Mantén una actitud constructiva: se revisa el código, no a la persona.
- Anota dudas y sugerencias de forma clara y respetuosa.
- El objetivo es que la revisión sea efectiva y promueva una mejora continua.

2. **Estructura tu feedback en 3 partes:**
- **Fortalezas**: "El sistema de rutas está muy bien organizado."
- **Áreas de mejora**: "El componente Button podría reutilizarse en otras vistas."
- **Sugerencias concretas**: "Usa Array.map() para simplificar este loop."

### Formato de documentación de una Code Review
Puedes usar esta estructura para documentar la Code Review realizada:

    ```html
    ## Code Review Sprint 3 - Manuela Grajales Duque

    ### 🔧 **Funcionalidad**  
    - ✅ Todo el CRUD funciona según lo esperado.  
    - ❌ El botón "Guardar" no muestra feedback al usuario cuando falla el API.  

    ### 🧹 **Clean Code**  
    - 👍 Los nombres de variables son muy claros (`userList`, `handleSubmit`).  
    - 👀 Oportunidad: Elimina el código comentado en `utils/helpers.js`.  

    ### 📚 **README**  
    - ✨ Muy completo, pero falta añadir cómo ejecutar los tests.  

    ### 🤝 **Feedback General**  
    ¡Excelente trabajo! El código es limpio y funcional. Sugiero añadir un spinner durante las llamadas al API para mejorar la UX.   
    ```