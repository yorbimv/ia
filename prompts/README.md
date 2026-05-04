# Prompts: Contexto y Configuración Maestra

Esta carpeta contiene los **"drivers"** del sistema. Son los archivos de instrucciones detalladas y manuales base que definen cómo debe comportarse la IA antes de escribir una sola línea de código.

Aquí es donde la magia de la ingeniería de prompts se encuentra con la arquitectura de software. Estos archivos no son simples preguntas; son **contratos de trabajo** que establecen roles, restricciones, flujos de validación y estándares de seguridad.

## Contenido

| Archivo | Propósito | Agente Objetivo |
|---------|-----------|-----------------|
| **ai-architect.md** | El manual definitivo. Transforma a la IA en un Arquitecto Senior Fullstack. Define las 8 fases de desarrollo (desde la extracción de la idea hasta el deploy). | Todos / Universal |
| **claude-base.md** | Adaptación del manual base para **Claude Code**. Enfocado en planificación estructurada y contexto persistente. | Anthropic Claude Code |
| **cursor-base.md** | Adaptación para **Cursor IDE**. Prioriza el uso de `.cursorrules` y optimización para desarrollo fullstack en el editor. | Cursor IDE |
| **gemini-base.md** | Adaptación para **Gemini**. Enfocada en análisis profundo y generación de código robusto. | Google Gemini |
| **windsurf-base.md** | Adaptación para **Windsurf**. Optimizado para flujos de trabajo ágiles y sesiones limpias. | Windsurf IDE |
| **chatgpt-base.md** | Adaptación para **ChatGPT**. Versátil para múltiples tareas de desarrollo y revisión de código. | OpenAI ChatGPT |

## Cómo usar estos Prompts

1.  **Carga Inicial:** Al iniciar una nueva sesión o proyecto, carga el contenido del archivo base correspondiente (`claude-base.md`, `ai-architect.md`, etc.).
2.  **Archivos de Contexto:** En herramientas como Cursor o Claude Code, copia el contenido relevante a `.cursorrules` o `CLAUDE.md` en la raíz de tu proyecto. Esto garantiza que la IA "recuerde" las reglas en cada interacción.
3.  **Adaptación:** Estos son los "manuales base". Siéntete libre de crear subcarpetas o nuevos archivos `.md` aquí para prompts más específicos (ej. `prompts/devops-ci-cd.md`).

---

> *"El éxito de una aplicación construida con IA no depende de la capacidad de programar, sino de la calidad de la planificación."*
