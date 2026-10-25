---
type: component
title: API Router
created: '2026-10-25'
updated: '2026-10-25'
tags:
- architecture
- api
source: https://github.com/MartinDumas/task-manager-app/blob/main/docs/app-requirements.md
status: planned
---

# API Router

**Стан:** запланований компонент, код ще не створено.

Шар HTTP на FastAPI. Оголошує маршрути `/api/v1/tasks`, зіставляє метод і URL з операцією, передає керування [[ServiceLayer|сервісному шару]] та повертає статуси HTTP / JSON.

## Відповідальність

- CRUD і керування [[TaskStatus|статусом]].
- Запити [[TaskSearchAndFiltering|списку]] та [[TaskStatistics|статистики]].
- Схеми введення / виведення з [[RequestResponseSchemas|Pydantic]].
- Автоматична OpenAPI-документація `/docs`.

Не виконує SQL безпосередньо; взаємодіє із [[ServiceLayer|Service Layer]]. Архітектурний контекст: [[ADR-001-LocalRESTAPI|ADR-001]].

