---
type: concept
title: Життєвий цикл завдання
created: '2026-10-25'
updated: '2026-10-25'
tags:
- domain
- workflow
source: https://github.com/MartinDumas/task-manager-app/blob/main/docs/app-requirements.md
status: documented
---

# Життєвий цикл завдання

Послідовність операцій з [[Task|завданням]]: створення → отримання → оновлення атрибутів → зміна [[TaskStatus|статусу]] → за потреби видалення.

## API-операції

1. `POST /api/v1/tasks` — створити, `201`.
2. `GET /api/v1/tasks/{id}` — отримати, `200` або `404`.
3. `PATCH /api/v1/tasks/{id}` — оновити атрибути.
4. `PATCH /api/v1/tasks/{id}/status` — змінити стан.
5. `DELETE /api/v1/tasks/{id}` — видалити, `204` або `404`.

Дії контролюються [[ServiceLayer|сервісним шаром]], маршрутизуються [[ApiRouter|API Router]] і перевіряються [[TestSuite|тестами]].

