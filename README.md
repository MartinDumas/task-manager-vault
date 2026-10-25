---
type: guide
title: Інструкція до Obsidian vault
created: 2026-10-25
updated: 2026-10-25
tags:
  - guide
  - knowledge
source: https://github.com/MartinDumas/task-manager-app/blob/main/docs/app-requirements.md
status: documented
---

# Task Manager — Knowledge Base

Локальна база знань для агентного розроблення Task Manager API. Це **окремий** Git-репозиторій `MartinDumas/task-manager-vault`; код застосунку зберігається в `MartinDumas/task-manager-app`.

**Початок навігації:** [[MOC-Застосунок]].

## Як відкрити в Obsidian

1. Встановіть Obsidian і запустіть його.
2. Виберіть **Open folder as vault** («Відкрити папку як сховище»).
3. Укажіть кореневу директорію `task-manager-vault` (саме її, а не `Concepts/`).
4. Відкрийте [[MOC-Застосунок]] і перевірте wiki-посилання.
5. Відкрийте **Graph view** (піктограма графа, або Command palette → Open graph view). Натисніть на вузол MOC і перевірте зв’язки.

У `Templates/` — приклади frontmatter для додавання нових нотаток. Усі змістовні нотатки пов'язані посиланнями з MOC.

## Безпека й подальші роботи

ПР2 — це підготовка Markdown-vault. MCP-сервер і технічне обмеження доступу ще **не** реалізовані; їх передбачено у ПР3–ПР4. Не відкривайте одночасно сховище всередині робочої папки агента: локальні клони мають залишатися окремими.
