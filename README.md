# 🚀 Mejora Prompts TALL

[![Laravel](https://img.shields.io/badge/Laravel-12-FF2D20?style=for-the-badge&logo=laravel)](https://laravel.com)
[![Livewire](https://img.shields.io/badge/Livewire-3-FB70A9?style=for-the-badge&logo=livewire)](https://livewire.laravel.com)
[![TailwindCSS](https://img.shields.io/badge/Tailwind-CSS-38B2AC?style=for-the-badge&logo=tailwind-css)](https://tailwindcss.com)
[![Alpine.js](https://img.shields.io/badge/Alpine.js-3-8BC0D0?style=for-the-badge&logo=alpine.js)](https://alpinejs.dev)

Este repositorio contiene un sistema de instrucciones de ingeniería de prompts diseñado para optimizar requerimientos de desarrollo en el stack **TALL** (Tailwind CSS, Alpine.js, Laravel 12, Livewire 3).

El objetivo es transformar ideas básicas o requerimientos ambiguos en prompts técnicos de alta precisión, listos para ser procesados por **Claude** o **Claude Code**.

---

## 🛠️ ¿Qué hace este optimizador?

Actúa como un **Arquitecto de Software y Experto en IA**, refinando cada requerimiento a través de un proceso de análisis técnico:

1.  **Análisis de Intención**: Razona sobre el problema real, identifica ambigüedades y define la arquitectura necesaria.
2.  **Aplicación de Convenciones TALL**:
    *   **Laravel 12**: Implementación de *Form Requests*, *Resource Controllers* y patrones de *Actions*.
    *   **Livewire 3**: Selección inteligente entre componentes funcionales (*Volt*) u OOP según la complejidad.
    *   **Tailwind CSS**: Diseño *mobile-first* y consistencia semántica.
    *   **Alpine.js**: Interactividad ligera exclusiva del cliente.
3.  **Gestión de Contexto**: Soporte nativo para referencias de archivos estilo Claude Code (`@path/file.php#L10-L20`).
4.  **Generación de Output Estructurado**: Crea un prompt final organizado con contexto, estructura de archivos, comportamiento y criterios de aceptación.

## 📦 Estructura del Output

Cada prompt generado sigue una estructura estricta para garantizar resultados consistentes:

*   **🎯 Contexto**: Ubicación del requerimiento en el ecosistema de la app.
*   **💻 Requerimiento**: Redacción técnica precisa y sin ambigüedades.
*   **⚙️ Stack y Restricciones**: Versiones y decisiones técnicas obligatorias.
*   **📁 Estructura de Archivos**: Guía de archivos a crear o modificar.
*   **🔄 Comportamiento**: Flujo lógico detallado.
*   **✅ Criterios de Aceptación**: Lista de verificación para el cumplimiento de la tarea.

## 🚀 Cómo utilizarlo

Para obtener los mejores resultados, te recomendamos usar **Claude Projects** (disponible en planes Pro y Team):

1.  **Crea un nuevo Proyecto** en [Claude.ai](https://claude.ai).
2.  **Configura las Instrucciones**: Copia el contenido íntegro de [`instrucciones.md`](./instrucciones.md) y pégalo en la sección de **"Project Instructions"** (en la barra lateral derecha).
3.  **Define tu Requerimiento**: En el chat del proyecto, describe tu tarea (puedes referenciar archivos usando `@` si usas Claude Code o simplemente mencionarlos).
4.  **Genera y Copia**: El optimizador procesará tu entrada y te devolverá el **Prompt mejorado** dentro de un bloque Markdown.
5.  **Ejecuta**: Copia ese prompt y úsalo en una nueva sesión o con Claude Code para obtener la implementación técnica perfecta.

---


<p align="center">
  <b>mejora-prompts-tall</b> • Un proyecto para elevar la calidad de tu desarrollo TALL.
</p>
