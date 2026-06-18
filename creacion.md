---
type: fleeting
title: "Creación del vault roblox — registro de inicialización"
aliases: ["creacion", "registro de inicialización bedrock"]
source: "manual"
captured_at: 2026-06-17
status: "raw"
promoted_to: ""
sources: []
updated_at: 2026-06-17
updated_by: "init@agent"
tags: [type/fleeting, status/raw, domain/projects]
---

# Creación del vault `roblox` — registro de inicialización

> Todo está en su sitio. El vault ya era un vault de Obsidian existente (con plugins como Calendar, Excalidraw y semantic-vault-mcp), y se respetó esa configuración — solo se añadió la estructura Bedrock. La inicialización está completa.

## Resumen

- **Idioma:** Español (es)
- **Preset:** Personal second brain
- **Dominios:** learning, career, projects, ideas, health, finance
- **Nombre del vault:** `roblox` **(default)**

## Archivos creados / actualizados

| Tipo | Ruta | Estado |
|---|---|---|
| Config | `.bedrock/config.json` | Creado |
| CLAUDE.md | `CLAUDE.md` | Creado (es) |
| Obsidian | `.obsidian/app.json` | Actualizado (estaba vacío) |
| Obsidian | `.obsidian/appearance.json` | Actualizado (estaba vacío) |
| Obsidian | `.obsidian/graph.json` | Creado (7 colores por tipo) |
| Obsidian | `.obsidian/core-plugins.json` | ⏭️ Omitido — respeta tus plugins (graph ya activo) |
| Plantilla | `actors/_template.md` · `actors/_template_node.md` | Copiadas verbatim |
| Plantilla | `people/_template.md` · `teams/_template.md` | Copiadas verbatim |
| Plantilla | `topics/_template.md` · `discussions/_template.md` | Copiadas verbatim |
| Plantilla | `projects/_template.md` · `fleeting/_template.md` | Copiadas verbatim |
| Ejemplo | `people/me.md` | Creado (es) |
| Ejemplo | `actors/reading-tracker.md` | Creado (es) |
| Ejemplo | `topics/2026-04-feature-learning-rust.md` | Creado (es) |
| Ejemplo | `projects/side-project-alpha.md` | Creado (es) |
| Registro | `…/claude-bedrock/…/vaults.json` | Creado (roblox = default) |

### Dependencias instaladas durante el setup

| Dependencia | Estado | Notas |
|---|---|---|
| graphify | Instalado ✓ | `graphifyy` 0.8.41 + `SKILL.md` creado en `~/.claude/skills/graphify/` |
| docling | Instalado ✓ | docling 2.103.0 (funcional, pero no en PATH) |
| Confluence API | NO configurado | Opcional |
| Google API | NO configurado | Opcional |
| claude-in-chrome MCP | No encontrado | Fallback opcional |
| git CLI | Disponible ✓ | git 2.54.0 |
| gh CLI | No encontrado | Necesario solo para `commit-push-pr` |

## ¿Qué sigue?

1. **Abre el vault en Obsidian** — ya está configurado. Abre la *Graph View* (Ctrl/Cmd+G) para ver las 4 entidades de ejemplo conectadas, codificadas por color según su tipo.
2. **Ingesta tu primera fuente** — ejecuta `/bedrock:learn <url-o-ruta>` para importar contenido desde un repo de GitHub, una URL remota o un archivo local (markdown, CSV, DOCX, PDF, etc. vía docling).
3. **Pregunta a tu vault** — `/bedrock:ask <pregunta>` busca en todas las entidades. Ej.: `/bedrock:ask ¿qué sé sobre reading-tracker?`
4. **Crea entidades manualmente** — `/bedrock:preserve` con texto libre o estructurado para añadir nuevas notas.
5. **Mantén la salud del vault** — periódicamente `/bedrock:compress` para detectar duplicados, entidades huérfanas y contenido obsoleto.
6. **Reemplaza el contenido de ejemplo** — las 4 entidades de ejemplo (reading-tracker, learning-rust, side-project-alpha) son plantillas demostrativas; edítalas o bórralas al empezar con contenido real sobre Roblox/Luau.
7. **Gestiona vaults** — `/bedrock:vaults` para listar, cambiar el default o eliminar. Usa `--vault roblox` desde cualquier directorio para apuntar a este vault.

## ⚠️ Dos acciones recomendadas

- **PATH de Python:** Agrega `C:\Users\Spectrum\AppData\Local\Python\pythoncore-3.14-64\Scripts` a tu PATH de usuario para que `docling` (y `graphify`) se resuelvan por comando y `/bedrock:learn` los encuentre de forma fiable al ingerir archivos no-markdown.
  - Además, el comando `python` no existe (solo el alias roto de Microsoft Store). Usa `py` o desactiva ese alias en *Settings → Apps → Advanced app settings → App execution aliases*. Esto también causa el error del **stop hook** ("Python was not found...").
- **Git (opcional):** Tu estrategia es `commit-push`, pero este vault aún **no es un repo git** y la CLI `gh` no está instalada. Ejecuta `git init` y, si quieres PRs, instala `gh` (https://cli.github.com/). Mientras tanto, los skills harán commit-only/fallback según corresponda.

> 💡 **Tip:** La graph view trae 7 colores preconfigurados (uno por tipo de entidad). Personalízalos en *Graph View → Groups* si prefieres otra paleta.
