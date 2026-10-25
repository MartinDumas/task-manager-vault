---
type: component
title: Схеми запитів і відповідей
created: '2026-10-25'
updated: '2026-10-25'
tags:
- architecture
- validation
source: https://github.com/MartinDumas/task-manager-app/blob/main/docs/app-requirements.md
status: planned
---

# Request/Response Schemas

**Стан:** запланований компонент.

Pydantic-схеми валідують HTTP-поля від [[ApiRouter|API Router]] та формують публічні відповіді незалежно від [[DataModels|ORM-моделей]].

Правила: `title` 1–120 символів, `description` до 2000, [[TaskStatus|статус]] та [[TaskPriority|пріоритет]] із дозволених enum, [[DueDate|дата]] ISO 8601, `limit` 1–100 і `offset >= 0`.

Невалідні запити не повинні змінювати дані. Перевірка — [[TestSuite|unit/API тести]].

