---
type: decision
title: 'ADR-001: локальний REST API'
created: '2026-10-25'
updated: '2026-10-25'
tags:
- adr
- architecture
source: https://github.com/MartinDumas/task-manager-app/blob/main/docs/app-requirements.md
status: documented
---

# ADR-001 — Локальний REST API

**Статус:** прийнято, ПР1.

## Контекст

Курс має сім практичних робіт; необхідний невеликий застосунок з чіткими критеріями успіху для майбутнього agent harness.

## Рішення

Розробляти локальний однокористувацький REST API на FastAPI без окремого графічного frontend. Ресурс — [[Task|Task]], HTTP-вхід — [[ApiRouter|API Router]].

## Альтернативи

- Повноцінний вебінтерфейс: відхилено через додатковий обсяг.
- Багатокористувацький сервіс: відхилено через потребу в автентифікації й операційній безпеці.

## Наслідки

Позитивно: реалізація й API-тестування вимірювані; Swagger UI автоматичний. Обмеження: немає UI, платформи сповіщень і production-деплою.

Див. [[ADR-003-StorageAndORM|ADR-003]], [[DomainGlossary|глосарій]].

