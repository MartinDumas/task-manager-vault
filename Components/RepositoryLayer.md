---
type: component
title: Шар доступу до даних
created: '2026-10-25'
updated: '2026-10-25'
tags:
- architecture
- repository
source: https://github.com/MartinDumas/task-manager-app/blob/main/docs/app-requirements.md
status: planned
---

# Repository Layer

**Стан:** запланований компонент.

Інкапсулює операції SQLAlchemy 2.x над [[DataModels|ORM-моделями]] в [[SQLiteStorage|SQLite]]. Не містить HTTP-логіки.

## Операції

- Створити, прочитати, оновити, видалити [[Task|Task]].
- Отримати список із [[TaskSearchAndFiltering|пошуком, фільтрами та пагінацією]].
- Порахувати записи для [[TaskStatistics|статистики]].
- Забезпечити коректне керування транзакціями (NFR-04).

Доступ за договором через [[ServiceLayer|сервісний шар]]. Обґрунтування сховища: [[ADR-003-StorageAndORM|ADR-003]].

