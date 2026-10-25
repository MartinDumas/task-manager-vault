---
type: concept
title: Статистика завдань
created: '2026-10-25'
updated: '2026-10-25'
tags:
- domain
- analytics
source: https://github.com/MartinDumas/task-manager-app/blob/main/docs/app-requirements.md
status: documented
---

# Статистика завдань

Статистика відображає кількість усіх [[Task|завдань]] і кількість за кожним [[TaskStatus|статусом]] на запит `GET /api/v1/tasks/stats`.

Інваріант: `total = todo + in_progress + done`. Враховуються актуальні записи бази даних; видалені записи не враховуються.

План виконання: [[RepositoryLayer|агрегаційний запит у репозиторії]], [[ServiceLayer|сервісна логіка]], [[ApiRouter|endpoint]], [[TestSuite|тести граничних сценаріїв]].

