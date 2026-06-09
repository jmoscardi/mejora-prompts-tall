# 🚀 Mejora Prompts TALL

[![Laravel](https://img.shields.io/badge/Laravel-12-FF2D20?style=for-the-badge&logo=laravel)](https://laravel.com)
[![Livewire](https://img.shields.io/badge/Livewire-3-FB70A9?style=for-the-badge&logo=livewire)](https://livewire.laravel.com)
[![TailwindCSS](https://img.shields.io/badge/Tailwind-CSS-38B2AC?style=for-the-badge&logo=tailwind-css)](https://tailwindcss.com)
[![Alpine.js](https://img.shields.io/badge/Alpine.js-3-8BC0D0?style=for-the-badge&logo=alpine.js)](https://alpinejs.dev)

Este repositorio contiene un sistema de instrucciones de ingeniería de prompts diseñado para optimizar requerimientos de desarrollo en el stack **TALL** (Tailwind CSS, Alpine.js, Laravel 12, Livewire 3).

El objetivo es transformar ideas básicas o requerimientos ambiguos en prompts técnicos de alta precisión, listos para ser procesados por **Claude** o **Claude Code**.

---

## 🛠️ ¿Qué hace este optimizador?

Actúa como un **experto en ingeniería de prompts**, refinando cada requerimiento a través de un proceso de análisis técnico:

1. **Análisis de intención**: Razona sobre el problema real, identifica ambigüedades y decide si necesita más información antes de proceder.
2. **Aplicación de convenciones TALL**:
   - **Laravel 12**: Form Requests, Resource Controllers y patrones de Actions.
   - **Livewire 3**: Selección entre Volt (funcional) u OOP según la complejidad del componente.
   - **Tailwind CSS**: Diseño mobile-first y consistencia semántica.
   - **Alpine.js**: Interactividad ligera exclusiva del cliente.
3. **Gestión de contexto**: Soporte nativo para referencias de archivos estilo Claude Code (`@path/file.php#L10-L20`), conservándolas como texto plano para que sigan siendo funcionales al pegar el prompt en la terminal.
4. **Generación de output estructurado**: Produce un prompt final con contexto, estructura de archivos, comportamiento esperado y criterios de aceptación.
5. **Validación proactiva**: Si detecta dudas bloqueantes (que cambian la arquitectura o el flujo principal), detiene la generación y pide aclaraciones antes de continuar.

## 📦 Estructura del output

Cada prompt generado sigue una estructura consistente:

- **Contexto**: Ubicación del requerimiento en el ecosistema de la app.
- **Requerimiento**: Redacción técnica precisa y sin ambigüedades.
- **Stack y restricciones**: Versiones y decisiones técnicas obligatorias.
- **Estructura de archivos**: Guía de archivos a crear o modificar.
- **Comportamiento esperado**: Flujo lógico detallado paso a paso.
- **Criterios de aceptación**: Lista de verificación para el cumplimiento de la tarea.
- **Consideraciones adicionales**: Edge cases y aspectos que el usuario pudo haber pasado por alto.
- **Instrucciones de ejecución**: Reglas de comportamiento para Claude Code al implementar la solución (leer antes de escribir, preguntar antes de asumir, no sobre-ingenierizar, solo tocar lo necesario, verificar lo escrito).

## 🚀 Cómo utilizarlo

Para obtener los mejores resultados, usá **Claude Projects** (disponible en planes Pro y Team):

1. **Creá un nuevo Proyecto** en [Claude.ai](https://claude.ai).
2. **Configurá las instrucciones**: Copiá el contenido íntegro de [`instrucciones.md`](./instrucciones.md) y pegalo en la sección de **"Project Instructions"** (en la barra lateral derecha).
3. **Describí tu requerimiento**: En el chat del proyecto, escribí tu tarea en borrador. Podés referenciar archivos con `@ruta/archivo.blade.php` o `@ruta/archivo.blade.php#L94-L122` si usás Claude Code.
4. **Iterá si hace falta**:
   - Si el requerimiento es claro, recibís el prompt mejorado de inmediato.
   - Si hay dudas bloqueantes, el optimizador te las lista primero. Respondelas en el mismo chat.
5. **Ejecutá**: Una vez generado el bloque ` ```md ``` `, copialo y usalo en una nueva sesión de Claude Code para obtener la implementación.

---

<p align="center">
  <b>mejora-prompts-tall</b> • Un proyecto para elevar la calidad de tu desarrollo TALL.
</p>