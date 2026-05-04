# Prompts para IA de Desarrollo

## ¿Qué es un Prompt?

Un **prompt** es una instrucción estructurada que le das a una inteligencia artificial para guiar su comportamiento, definir su rol, establecer reglas de trabajo y lograr resultados consistentes y de alta calidad.

En el contexto de desarrollo de software, un buen prompt transforma una IA genérica en un **asistente especializado** que entiende tu stack, tus convenciones de código, tu filosofía de trabajo y tu proceso de desarrollo.

### ¿Por qué son importantes?

1. **Contexto persistente:** Las IAs no recuerdan conversaciones pasadas entre sesiones. Un buen prompt les da todo el contexto necesario desde el primer mensaje.
2. **Consistencia:** Garantiza que la IA siga las mismas reglas y patrones en cada interacción, evitando código inconsistente o malas prácticas.
3. **Eficiencia:** Reduce drásticamente la cantidad de iteraciones necesarias. La IA entiende lo que necesitas desde el inicio, no después de 10 mensajes de corrección.
4. **Calidad:** Un prompt bien estructurado incluye reglas de seguridad, arquitectura, testing y deploy que la IA aplicará automáticamente.
5. **Escalabilidad:** Puedes reutilizar y adaptar prompts entre proyectos, creando una biblioteca de instrucciones que mejora con el tiempo.

### Anatomía de un buen prompt

| Elemento | Descripción |
|----------|-------------|
| **Rol** | Define quién es la IA (ej: Arquitecto Senior, QA Expert) |
| **Filosofía** | Principios de trabajo que debe seguir siempre |
| **Contexto** | Stack tecnológico, estructura del proyecto, convenciones |
| **Instrucciones** | Pasos específicos a seguir, fase por fase |
| **Reglas** | Lo que la IA NUNCA debe hacer (hardcodear secrets, saltar tests) |
| **Seguridad** | Manejo de credenciales, validación de entradas, protección de datos |

### Cómo usar esta carpeta

1. Elige la IA con la que vas a trabajar en la tabla de abajo
2. Entra a la carpeta correspondiente
3. Copia el `base-manual.md` y adáptalo a tu proyecto
4. Pégalo al inicio de tu sesión con la IA o configúralo como archivo de contexto (`.cursorrules`, `CLAUDE.md`, etc.)

---

## Menú Principal

| IA | Carpeta | Descripción |
|----|---------|-------------|
| **Claude Code** | [claude-code/](claude-code/) | IA de Anthropic, excelente para arquitectura y planificación |
| **Cursor** | [cursor/](cursor/) | IDE con IA integrada, ideal para desarrollo fullstack |
| **Gemini** | [gemini/](gemini/) | IA de Google, fuerte en análisis y generación de código |
| **Windsurf** | [windsurf/](windsurf/) | IDE con IA, optimizado para flujos de trabajo ágiles |
| **OpenCode** | [opencode/](opencode/) | CLI de código abierto para desarrollo asistido por IA |
| **ChatGPT** | [chatgpt/](chatgpt/) | IA de OpenAI, versátil para múltiples tareas de desarrollo |

---

## Filosofía de Trabajo (Aplica a todas las IAs)

Cada carpeta contiene un `base-manual.md` basado en el **Manual del Arquitecto de IA** que establece los principios fundamentales:

- **Planificación antes de programar**
- **Simplicidad Radical**
- **Fases Pequeñas con validación constante**
- **Seguridad por Diseño**
