# OpenCode

## ¿Qué es OpenCode?

OpenCode es una herramienta de desarrollo asistida por IA diseñada para ejecutarse en la terminal. Su potencia radica en la capacidad de integrar **Skills** (habilidades) y **Manuales** que definen comportamientos complejos, permitiendo que la IA actúe como un miembro más del equipo con conocimientos específicos y persistentes.

## Estructura Recomendada del Proyecto

Para aprovechar al máximo OpenCode y mantener el contexto ordenado, se recomienda la siguiente estructura de archivos en tu proyecto:

```text
tu-proyecto/
├── .opencode/              # Configuración específica de OpenCode
│   └── config.yaml
├── skills/                 # Carpeta centralizada para tus Skills
│   ├── architect.md        # Rol de Arquitecto (basado en base-manual.md)
│   ├── frontend-expert.md  # Skill especializado en UI
│   └── testing.md          # Skill para QA y Tests
├── docs/                   # Documentación del proyecto
│   └── context.md          # Contexto global del negocio/reglas
└── src/                    # Código fuente
```

## ¿Qué es un Skill?

Un **Skill** es un archivo Markdown (`.md`) que encapsula un conjunto de instrucciones, reglas y conocimientos específicos para que la IA domine un área particular. A diferencia de un prompt de un solo uso, un Skill es **reutilizable y modular**.

### Requisitos para ser considerado un Skill

Para que un archivo sea considerado un Skill válido y útil dentro de OpenCode, debe cumplir con los siguientes puntos críticos:

1. **Definición de Rol Clara:** Debe establecer explícitamente qué "persona" o expertise está adoptando la IA (ej: *"Eres un Arquitecto de Software Senior especializado en Microservicios"*).
2. **Objetivo Específico:** Definir la meta principal del skill (ej: *"Generar endpoints REST seguros y validados"*).
3. **Flujo de Trabajo (Workflow):** Pasos lógicos y secuenciales que la IA debe seguir obligatoriamente al activar el skill.
4. **Reglas y Restricciones:** Límites claros. Lo que la IA **debe** hacer y lo que **nunca** debe hacer (ej: *"Nunca hardcodear credenciales"*).
5. **Contexto y Recursos:** Referencias a documentación oficial, versiones de librerías o convenciones específicas del proyecto.

### Anatomía de un Skill (`.md`)

Todo skill debe seguir una estructura estándar para ser legible y ejecutable correctamente:

```markdown
# Nombre del Skill

## Rol
[Descripción del rol experto]

## Objetivo
[Meta principal a cumplir]

## Workflow
1. Analizar requerimientos
2. [Paso específico]
3. Validar con tests

## Reglas de Oro
- Regla 1 (Ej: Planificación antes de código)
- Regla 2 (Ej: Seguridad por diseño)
- Regla 3 (Ej: Commits atómicos)

## Referencias
- [Enlace a docs oficiales]
```

## Catálogo Global de Skills: skills.sh

No necesitas crear cada skill desde cero. Existe una plataforma centralizada donde puedes descubrir y descargar skills creados por la comunidad, compatibles con OpenCode y otras IAs:

👉 **[https://skills.sh/](https://skills.sh/)**

En este sitio encontrarás skills para:
- **Frameworks:** React, Vue, Next.js, Svelte, etc.
- **Arquitectura:** Clean Architecture, DDD, Hexagonal.
- **DevOps:** Docker, Kubernetes, CI/CD pipelines.
- **Testing:** TDD, BDD, E2E testing.

**¿Cómo usarlos?**
1. Busca el skill que necesitas en `skills.sh`.
2. Copia el contenido o descarga el archivo `.md`.
3. Guárdalo en tu carpeta `skills/` del proyecto.
4. Carga el skill en tu sesión de OpenCode.

---

## Filosofía Base

Recuerda que independientemente del skill específico que uses, todos los proyectos en este repositorio se rigen por el **[Manual del Arquitecto de IA](./base-manual.md)**. Este manual define nuestros principios de planificación, simplicidad y seguridad.
