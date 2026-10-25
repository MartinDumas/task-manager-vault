---
type: component
title: Сховище SQLite
created: '2026-10-25'
updated: '2026-10-25'
tags:
- architecture
- storage
source: https://github.com/MartinDumas/task-manager-app/blob/main/docs/app-requirements.md
status: planned
---

# SQLite Storage

**Стан:** запланований компонент.

Локальна файлова база SQLite для демонстраційних [[Task|завдань]], доступ через [[RepositoryLayer|Repository Layer]] і SQLAlchemy 2.x. Схема описується в [[DataModels|ORM]].

Обмеження: навчальне локальне використання, без віддаленого production-доступу та зовнішніх користувачів. Секрети не повинні зберігатися в git. Архітектурне рішення: [[ADR-003-StorageAndORM|ADR-003]].

