# Prompts: Contexto y Configuración Maestra

Esta carpeta contiene los **"drivers"** del sistema, organizados por entorno de desarrollo o herramienta de IA.

Aquí es donde la ingeniería de prompts se encuentra con la arquitectura de software. Para usar la IA correctamente, **debes cargar el archivo `prompt.md` correspondiente a la herramienta que estés utilizando**.

## Estructura y Uso

### 1. Entornos Específicos
Si estás trabajando con una herramienta concreta, usa su carpeta dedicada. El archivo `prompt.md` dentro de cada carpeta define el rol, la filosofía y las reglas de trabajo para ese entorno.

| Herramienta | Ruta del Prompt | Descripción |
|-------------|-----------------|-------------|
| **OpenCode** | [opencode/prompt.md](opencode/prompt.md) | Prompt maestro para la CLI de OpenCode. Define el rol de Arquitecto y flujo de trabajo. |
| **Cursor** | [cursor/prompt.md](cursor/prompt.md) | Adaptación para Cursor IDE. Prioriza `.cursorrules` y desarrollo fullstack. |
| **Claude Code** | [claude/prompt.md](claude/prompt.md) | Configuración para Claude. Enfocada en planificación y contexto persistente. |
| **Gemini** | [gemini/prompt.md](gemini/prompt.md) | Adaptación para Google Gemini. Análisis profundo y código robusto. |
| **Windsurf** | [windsurf/prompt.md](windsurf/prompt.md) | Configuración para Windsurf. Flujos ágiles y sesiones limpias. |
| **ChatGPT** | [chatgpt/prompt.md](chatgpt/prompt.md) | Adaptación versátil para tareas de desarrollo y revisión. |

### 2. Universal
Si buscas la referencia base o quieres crear un prompt híbrido, consulta la carpeta universal.

*   **Universal:** [universal/ai-architect.md](universal/ai-architect.md) - El "Manual del Arquitecto". La fuente de verdad para todas las configuraciones anteriores.

## Cómo aplicar un Prompt

1. **En CLI (OpenCode):** Copia el contenido de `prompt.md` y pégalo al inicio de tu sesión.
2. **En IDEs (Cursor, Windsurf):** Copia el contenido a `.cursorrules` o al archivo de reglas de tu proyecto.
3. **En Web (Claude, ChatGPT):** Pégalo en el primer mensaje del "Custom Instructions" o al inicio del chat.

> *"El éxito de una aplicación construida con IA no depende de la capacidad de programar, sino de la calidad de la planificación."*
