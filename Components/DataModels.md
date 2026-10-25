---
type: component
title: Моделі даних
created: '2026-10-25'
updated: '2026-10-25'
tags:
- architecture
- model
source: https://github.com/MartinDumas/task-manager-app/blob/main/docs/app-requirements.md
status: planned
---

# Data Models

**Стан:** запланований компонент.

SQLAlchemy ORM-модель для [[Task|Task]] із полями `id`, `title`, `description`, `status`, `priority`, `due_date`, `created_at`, `updated_at`.

Інваріанти предметної області: [[TaskStatus|перелік статусів]], [[TaskPriority|перелік пріоритетів]], [[DueDate|тип дати]]. Значення за замовчуванням задані вимогами ПР1.

Моделі описують персистентні записи [[SQLiteStorage|SQLite]]; HTTP-контракти визначає окремо [[RequestResponseSchemas|Request/Response Schemas]].

