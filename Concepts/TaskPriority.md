---
type: concept
title: Пріоритет завдання
created: '2026-10-25'
updated: '2026-10-25'
tags:
- domain
- priority
source: https://github.com/MartinDumas/task-manager-app/blob/main/docs/app-requirements.md
status: documented
---

# Пріоритет завдання

Пріоритет визначає важливість [[Task|завдання]] для користувача. Дозволені значення: `low` (низький), `medium` (середній), `high` (високий). Значення за замовчуванням — `medium`.

Поле використовується для фільтрації у [[TaskSearchAndFiltering|запитах списку завдань]], перевіряється [[RequestResponseSchemas|Pydantic-схемами]] і зберігається у [[DataModels|моделі]]. Інші значення повинні відхилятися валідацією.

