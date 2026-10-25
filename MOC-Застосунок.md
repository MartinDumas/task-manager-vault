---
type: moc
title: Мапа змісту Task Manager API
created: '2026-10-25'
updated: '2026-10-25'
tags:
- navigation
- moc
source: https://github.com/MartinDumas/task-manager-app/blob/main/docs/app-requirements.md
status: documented
---

# MOC — Застосунок «Менеджер завдань»

## Предметна область

- [[Task|Завдання (Task)]]
- [[TaskStatus|Статуси завдань]]
- [[TaskPriority|Пріоритети]]
- [[DueDate|Строки виконання]]
- [[TaskWorkflow|Життєвий цикл]]
- [[TaskSearchAndFiltering|Пошук і фільтрація]]
- [[TaskStatistics|Статистика]]

## Компоненти застосунку (заплановані)

- [[ApiRouter|HTTP API Router]]
- [[ServiceLayer|Service Layer]]
- [[RepositoryLayer|Repository Layer]]
- [[DataModels|ORM-моделі]]
- [[RequestResponseSchemas|Pydantic-схеми]]
- [[SQLiteStorage|SQLite Storage]]
- [[TestSuite|Тестування]]

## Архітектурні рішення

- [[ADR-001-LocalRESTAPI|ADR-001 — Локальний REST API]]
- [[ADR-002-SeparateKnowledgeVault|ADR-002 — Окремий vault]]
- [[ADR-003-StorageAndORM|ADR-003 — SQLite та ORM]]
- [[ADR-004-HarnessAccessBoundary|ADR-004 — Межа доступу агента]]

## Термінологія

- [[DomainGlossary|Предметний глосарій]]
- [[EngineeringGlossary|Інженерний глосарій]]

## Допоміжні матеріали

- [[README|Як відкрити vault]]
- [[Template-Concept|Шаблон концепції]]
- [[Template-Component|Шаблон компонента]]
- [[Template-Decision|Шаблон рішення]]
- [[Template-Glossary|Шаблон глосарію]]
- [[Template-MOC|Шаблон MOC]]
