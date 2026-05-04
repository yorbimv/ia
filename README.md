# IA Ecosystem: Prompts, Skills & MCPs

Repositorio centralizado para orquestar y escalar el uso de Inteligencia Artificial en el ciclo de desarrollo de software.

El objetivo es simple: **dejar de depender de la suerte y empezar a depender de la arquitectura.** Aquí se unifica lo mejor de los ecosistemas MCPs (Model Context Protocols), prompts de ingeniería avanzada y Skills modulares. La idea es transformar cualquier agente de IA (sea OpenCode, Claude, Cursor o Gemini) en un arquitecto de software senior capaz de lanzar código en producción sin generar deuda técnica ni "código espagueti".

## Estructura del Repositorio

### 📂 [prompts/](prompts/)
Aquí residen los **"drivers" diarios**. La carpeta está organizada por **entorno de desarrollo** (OpenCode, Cursor, Claude, etc.) para que localices rápidamente la configuración adecuada.

*   **Contenido:** Archivos `prompt.md` por herramienta que definen el rol, reglas de arquitectura y flujos de validación.
*   **Uso:** Se cargan al inicio de la sesión para transformar a la IA en un Arquitecto Senior.

### 📂 [skills/](skills/)
El cerebro modular del sistema. Esta carpeta alberga la documentación y estructura para el ecosistema estándar de **Skills** (`npx skills`).

*   **Contenido:** Guías de instalación, adaptación de skills para diferentes agentes, y la base teórica para crear habilidades especializadas (seguridad, testing, optimización).
*   **Uso:** Sirve como referencia para instalar capacidades nuevas y mantener a los agentes actualizados con las mejores prácticas de la industria.

---

## Páginas de Referencia

Herramientas esenciales para mantener el flujo de trabajo moderno y eficiente:

| Página | Descripción |
|--------|-------------|
| [**skills.sh**](https://skills.sh/) | Directorio y leaderboard del ecosistema de Skills. El lugar para descubrir módulos de conocimiento compatibles. |
| [**npmx.dev**](https://npmx.dev/) | Explorador rápido del registro de npm. Para buscar, comparar y auditar paquetes sin fricción. |

---

## Automatización con OpenCode GitHub

Este repositorio está integrado con el **Agente de OpenCode** para automatizar el mantenimiento y la generación de contenido.

### ¿Qué hace?
El comando `opencode github install` transforma este repo en una herramienta viva. Instala un Workflow de GitHub Actions que permite a la IA "escuchar" Issues y Pull Requests para ejecutar tareas sin abrir la terminal.

### Casos de uso en este proyecto:
1. **Generación de Contenido desde Issues:** Abre un Issue con `/opencode crea un nuevo prompt para [tema]` y la IA generará el archivo y abrirá un Pull Request.
2. **Revisión Automática de PRs:** La IA valida que los nuevos prompts o skills cumplan con la estructura y filosofía definida en este repo.
3. **Mantenimiento:** Actualización automática de índices y READMEs cuando se agregan nuevos archivos.

### Instalación
```bash
opencode github install
```
*(Este comando configura el workflow y la App de GitHub automáticamente).*

---

## Filosofía de Trabajo

> *"Si no está en el contexto, no existe para la IA."*

1. **Planificación sobre implementación:** El código es barato; la dirección correcta es lo caro.
2. **Simplicidad Radical:** Menos archivos, menos magia, más control.
3. **Seguridad por Diseño:** Las credenciales y la validación de datos no son opcionales.
