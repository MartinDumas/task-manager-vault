---
type: decision
title: 'ADR-004: межа доступу AI-агента'
created: '2026-10-25'
updated: '2026-10-25'
tags:
- adr
- security
source: https://github.com/MartinDumas/task-manager-app/blob/main/docs/harness-requirements.md
status: documented
---

# ADR-004 — Межа доступу агенту до vault

**Статус:** архітектурне рішення прийнято, технічна реалізація запланована (ПР3–ПР4).

## Контекст

AI-агент працює у WebStorm + GitHub Copilot в репозиторії застосунку; знання у [[ADR-002-SeparateKnowledgeVault|окремому репозиторії]]. Потрібно розділити дозволене читання й контрольований запис.

## Рішення

MCP-сервер планується як єдина дозволена агенту точка доступу до vault. Передбачаються операції `kb_search`, `kb_get_note`, `kb_ingest`; запис потребує дозволу. Guardrails: `allow`, `warn/require approval`, `block`.

## Ризики та перевірка

Папки самі по собі не заважають shell-доступу. На ПР4 потрібні технічні права / ізоляція, hooks або обмеження інструментів та негативні тести обходу. ПР2 створює лише файли Markdown; MCP наразі відсутній.

Див. [[EngineeringGlossary|терміни знань і агентів]] та [[MOC-Застосунок|MOC]].

