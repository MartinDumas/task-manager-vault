---
type: concept
title: Термін виконання завдання
created: '2026-10-25'
updated: '2026-10-25'
tags:
- domain
- date
source: https://github.com/MartinDumas/task-manager-app/blob/main/docs/app-requirements.md
status: documented
---

# Термін виконання завдання

`due_date` — необов’язкова дата, до якої бажано виконати [[Task|завдання]]. Формат — ISO 8601 date `YYYY-MM-DD`, **без часу і часового поясу**.

Не плутати з `created_at` і `updated_at`, що зберігаються в UTC datetime. У поточній специфікації не передбачено сповіщення чи заборону прострочених дат; це поза межами MVP.

Поле використовується для сортування в [[TaskSearchAndFiltering|пошуку та фільтрації]]. Валідація відбувається у [[RequestResponseSchemas|схемах]].

