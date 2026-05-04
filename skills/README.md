# Ecosistema de Skills para IAs

## ¿Qué es un Skill?

Un **Skill** es un paquete modular de instrucciones que potencia a las IAs con conocimientos específicos. A diferencia de un prompt de un solo uso, un Skill es **reutilizable y estructurado**, permitiendo que la IA actúe como un experto en un área concreta.

### Aplicabilidad
Los skills están diseñados para funcionar con **todas las IAs** que soportan archivos de contexto: OpenCode, Claude Code, Cursor, Gemini, Windsurf, etc.

## Ecosistema Estándar: npx skills

Usamos la CLI `npx skills` de [vercel-labs/skills](https://github.com/vercel-labs/skills) para gestionar habilidades de forma centralizada.

### Instalación y Uso

```bash
# Instalar un skill específico para un agente
npx skills add <repositorio> --skill <nombre> -a <agente>

# Ejemplo: Instalar 'find-skills' para OpenCode
npx skills add https://github.com/vercel-labs/skills --skill find-skills -a opencode
```

### Comandos útiles
- **Listar skills:** `npx skills list`
- **Buscar skills:** `npx skills find`
- **Descubrir más:** [https://skills.sh/](https://skills.sh/)

## Skills Recomendados

Herramientas esenciales de la comunidad que mejoran drásticamente el flujo de trabajo:

| Skill | Descripción | Comando de Instalación |
|-------|-------------|------------------------|
| **🦴 Caveman** | Reduce el uso de tokens en ~75%. La IA responde de forma ultra concisa ("habla como cavernícola inteligente") sin perder precisión técnica. Ideal para ahorrar costos y leer más rápido. | `npx skills add juliusbrussee/caveman -a opencode` |
| **🔍 Find Skills** | Permite buscar y descubrir nuevos skills directamente desde la terminal o el chat de la IA. | `npx skills add vercel-labs/skills --skill find-skills -a opencode` |

**Sub-herramientas de Caveman:**
- `/caveman-commit`: Genera mensajes de commit cortos y limpios.
- `/caveman-review`: Revisiones de código de una sola línea (ej: `L42: 🔴 bug: null check`).
- `/caveman:compress`: Comprime archivos de memoria (como `CLAUDE.md`) para ahorrar tokens de entrada.

## Skills por IA

En esta carpeta encontrarás las configuraciones base (manuales) adaptadas para cada herramienta, listas para ser usadas como contexto o como base para crear tus propios skills.

| IA | Archivo | Descripción |
|----|---------|-------------|
| **OpenCode** | [opencode/](opencode/) | Configuración y estructura de skills para OpenCode |
| **Claude Code** | `claude-base.md` | Manual base adaptado para Claude |
| **Cursor** | `cursor-base.md` | Manual base adaptado para Cursor |
| **Gemini** | `gemini-base.md` | Manual base adaptado para Gemini |
| **Windsurf** | `windsurf-base.md` | Manual base adaptado para Windsurf |
| **ChatGPT** | `chatgpt-base.md` | Manual base adaptado para ChatGPT |
