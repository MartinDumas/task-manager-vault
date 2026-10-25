---
type: concept
title: Пошук, фільтрація і сортування
created: '2026-10-25'
updated: '2026-10-25'
tags:
- domain
- query
source: https://github.com/MartinDumas/task-manager-app/blob/main/docs/app-requirements.md
status: documented
---

# Пошук, фільтрація і сортування

Для колекції [[Task|завдань]] плануються запити `GET /api/v1/tasks`.

- `q` — пошук підрядка в `title` або `description` без урахування регістру.
- `status` — фільтрація за [[TaskStatus|станом]].
- `priority` — фільтрація за [[TaskPriority|пріоритетом]].
- `sort_by` — сортування за `created_at` або [[DueDate|due_date]] з вибором напряму.
- `limit` (1–100) та `offset` (не від’ємне) — пагінація.

Параметри проходять валідацію у [[RequestResponseSchemas|схемах]], бізнес-обробку в [[ServiceLayer|сервісі]], виконання запиту у [[RepositoryLayer|репозиторії]].

