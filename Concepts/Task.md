---
type: concept
title: Завдання (Task)
created: '2026-10-25'
updated: '2026-10-25'
tags:
- domain
- task
source: https://github.com/MartinDumas/task-manager-app/blob/main/docs/app-requirements.md
status: documented
---

# Завдання (Task)

**Завдання** — базова сутність однокористувацького Task Manager API, що описує дію, яку планує виконати користувач. Доступ до завдань відбувається через [[ApiRouter|HTTP API]].

## Поля сутності

| Поле | Тип | Обмеження |
| --- | --- | --- |
| `id` | додатне ціле | Унікальний первинний ключ |
| `title` | рядок | 1–120 символів; обов'язкове |
| `description` | рядок або null | До 2000 символів |
| `status` | enum | [[TaskStatus|todo, in_progress, done]] |
| `priority` | enum | [[TaskPriority|low, medium, high]] |
| `due_date` | ISO 8601 date або null | [[DueDate|Дата виконання]] |
| `created_at` | UTC datetime | Час створення |
| `updated_at` | UTC datetime | Час останньої зміни |

Новостворене завдання має `status=todo`, `priority=medium`, якщо користувач не задав інше. Поняття змін стану описано у [[TaskWorkflow|життєвому циклі]].

## Пов'язані реалізації

[[DataModels|Модель даних]] · [[RequestResponseSchemas|Схеми валідації]] · [[RepositoryLayer|Репозиторій]] · [[DomainGlossary|Глосарій]].

> Статус реалізації: специфікація ПР1; програмний код буде створено на наступних практичних.

