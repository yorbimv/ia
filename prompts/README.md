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

## Skills para Todas las IAs (Ecosistema Open)

Además de los prompts manuales, existe un **ecosistema estándar de Skills** compatible con OpenCode, Claude Code, Cursor, Gemini, Windsurf y más.

Un **Skill** es un paquete modular de instrucciones que potencia la IA con conocimientos específicos (ej: guías de diseño, mejores prácticas de seguridad, patrones de arquitectura).

### ¿Cómo instalar y usar Skills?

Usamos la CLI `npx skills` de [vercel-labs/skills](https://github.com/vercel-labs/skills).

#### Instalación
Ejecuta en tu terminal el siguiente comando. Puedes especificar a qué IA quieres aplicarlo usando el flag `-a`.

```bash
npx skills add <repositorio> --skill <nombre-del-skill> -a <agente>
```

#### Ejemplo práctico: "Find Skills"
Para instalar el skill que te ayuda a buscar otros skills directamente desde tu IA:

```bash
npx skills add https://github.com/vercel-labs/skills --skill find-skills -a opencode
```

Una vez instalado, el agente de IA cargará automáticamente las instrucciones definidas en el skill.

#### Comandos útiles
- **Listar skills instalados:** `npx skills list`
- **Buscar nuevos skills:** `npx skills find`
- **Instalar para todos los agentes:** `npx skills add <repo> --skill <nombre>` (omite el flag `-a`)

---

## Filosofía de Trabajo (Aplica a todas las IAs)

Cada carpeta contiene un `base-manual.md` basado en el **Manual del Arquitecto de IA** que establece los principios fundamentales:

- **Planificación antes de programar**
- **Simplicidad Radical**
- **Fases Pequeñas con validación constante**
- **Seguridad por Diseño**
