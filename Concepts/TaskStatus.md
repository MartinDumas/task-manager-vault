---
type: concept
title: Статус завдання
created: '2026-10-25'
updated: '2026-10-25'
tags:
- domain
- status
source: https://github.com/MartinDumas/task-manager-app/blob/main/docs/app-requirements.md
status: documented
related_to:
- Task
- TaskWorkflow
---

# Статус завдання

Статус описує поточний етап виконання [[Task|завдання]] і зберігається в полі `status`.

| Значення | Значення в інтерфейсі | Сутність |
| --- | --- | --- |
| `todo` | Заплановано | Роботу ще не почато; значення за замовчуванням |
| `in_progress` | Виконується | Завдання у процесі |
| `done` | Завершено | Роботу завершено |

У специфікації ПР1 немає обмежень для переходів між дозволеними статусами; у прототипі перехід у будь-який інший дозволений статус можливий через `PATCH /api/v1/tasks/{id}/status`.

Див. [[TaskWorkflow|Життєвий цикл]], [[TaskStatistics|Статистика]] та [[ApiRouter|API Router]].

