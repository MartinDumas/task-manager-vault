---
type: glossary
title: Глосарій інженерії застосунку і знань
created: '2026-10-25'
updated: '2026-10-25'
tags:
- glossary
- engineering
source: https://github.com/MartinDumas/task-manager-app/blob/main/docs/harness-requirements.md
status: documented
---

# Глосарій інженерії застосунку і знань

| Термін | Визначення / застосування | Зв'язок |
| --- | --- | --- |
| REST API | HTTP-інтерфейс операцій з ресурсами | [[ApiRouter]] |
| Сервісний шар | Реалізація бізнес-логіки | [[ServiceLayer]] |
| Репозиторій даних | Об'єктний інтерфейс доступу до сховища | [[RepositoryLayer]] |
| ORM | Відображення об'єктів у таблиці БД | [[DataModels]] |
| Vault | Локальний каталог пов'язаних Markdown-нотаток | [[ADR-002-SeparateKnowledgeVault]] |
| Wiki-посилання | Зв'язок Markdown-посилання між нотатками | [[MOC-Застосунок]] |
| MOC | Навігаційний індекс знань | [[MOC-Застосунок]] |
| MCP | Протокол типізованих інструментів між агентом та зовнішнім сервісом | [[ADR-004-HarnessAccessBoundary]] |
| Guardrails | Дозволи, попередження та блокування дій агента | [[ADR-004-HarnessAccessBoundary]] |
| ADR | Нотатка з контекстом, рішенням, альтернативами та наслідками | [[ADR-001-LocalRESTAPI]] |
| pytest | Фреймворк автоматизованих тестів Python | [[TestSuite]] |

Для налаштування конектора у наступній роботі використовується цей словник і структура MOC.

