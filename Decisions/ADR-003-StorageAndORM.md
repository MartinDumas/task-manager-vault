---
type: decision
title: 'ADR-003: SQLite та SQLAlchemy'
created: '2026-10-25'
updated: '2026-10-25'
tags:
- adr
- persistence
source: https://github.com/MartinDumas/task-manager-app/blob/main/docs/app-requirements.md
status: documented
---

# ADR-003 — SQLite та SQLAlchemy

**Статус:** прийнято, ПР1.

## Контекст

Локальний прототип не потребує окремого серверу СУБД; дані створюються для навчальних цілей.

## Рішення

Використати [[SQLiteStorage|SQLite]] для сховища і SQLAlchemy 2.x як ORM із [[RepositoryLayer|Repository Layer]]. Поля визначаються через [[DataModels|Data Models]].

## Альтернативи

- PostgreSQL: відхилено через зайву інфраструктуру на етапі MVP.
- Зберігання JSON-файлів: відхилено через потребу керованих запитів та атомарних змін.

## Наслідки

Простий локальний запуск, можливість тестувати CRUD та агрегації. Обсяг і одночасність роботи обмежені рамками локального прототипу.

