---
type: component
title: Сервісний шар
created: '2026-10-25'
updated: '2026-10-25'
tags:
- architecture
- service
source: https://github.com/MartinDumas/task-manager-app/blob/main/docs/app-requirements.md
status: planned
depends_on:
- RepositoryLayer
implements:
- TaskWorkflow
governed_by:
- ADR-001-LocalRESTAPI
---

# Service Layer

**Стан:** запланований компонент.

Реалізує правила створення, зміни та обробки [[Task|завдань]] незалежно від HTTP і конкретної БД. Викликається з [[ApiRouter|API Router]], використовує [[RepositoryLayer|Repository Layer]] для доступу до записів.

## Відповідальність

- Оркестрація [[TaskWorkflow|операцій життєвого циклу]].
- Виконання бізнес-перевірок разом із [[RequestResponseSchemas|валідацією]].
- Узгоджені відповіді про відсутній запис.
- Реалізація розрахунків для [[TaskStatistics|статистики]].

Модульні перевірки плануються у [[TestSuite|Test Suite]].

