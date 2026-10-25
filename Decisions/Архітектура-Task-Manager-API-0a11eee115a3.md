---
type: decision
title: Архітектура Task Manager API
created: '2026-10-25'
updated: '2026-10-25'
tags:
- architecture
- github
- fastapi
source: https://github.com/MartinDumas/task-manager-app/blob/main/docs/app-requirements.md
source_id: github:file:docs/app-requirements.md:architecture
source_hash: 16e3f542d99049a95f960004b44808e9c24d2aba86e877d1dc303f8f33694b34
status: documented
---

# Архітектура Task Manager API

Task Manager API задокументовано як локальний однокористувацький REST API на Python 3.12+ і FastAPI, з інтерактивною OpenAPI/Swagger UI документацією на `/docs`; маршрути мають префікс `/api/v1/`. Архітектура шарова: HTTP API → services (бізнес-правила) → repositories (доступ до даних) → SQLite. Для валідації використовується Pydantic, для ORM — SQLAlchemy 2.x; схеми запитів і відповідей відокремлені від ORM-моделей. Автоматизовані перевірки передбачені через pytest/pytest-cov, статичний аналіз — Ruff. Agent harness не є частиною коду застосунку, а vault зберігається фізично окремо. Це задокументовані вимоги та план, не твердження про вже реалізовану архітектуру.

## Пов'язані нотатки

- [[MOC-Застосунок]]
