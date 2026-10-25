---
type: decision
title: 'ADR-005: таксономія та типізовані відношення'
created: '2026-10-25'
updated: '2026-10-25'
tags: [adr, knowledge, security]
source: https://github.com/MartinDumas/task-manager-app/blob/main/docs/ontology.md
status: documented
related_to: [ADR-004-HarnessAccessBoundary, ADR-002-SeparateKnowledgeVault]
---

# ADR-005 — Таксономія й типізовані відношення

**Рішення:** використати 7 категорій нотаток (`concept`, `component`, `decision`, `glossary`, `moc`, `template`, `guide`) і 5 типів зв'язків (`depends_on`, `implements`, `governed_by`, `verifies`, `related_to`) як списки stem у frontmatter.

**Мотивація:** [[MOC-Застосунок|MOC]] показує навігацію, а типізовані відношення виражають різні смисли залежностей компонентів, реалізації й перевірки.

**Обмеження:** це легковаге знання, а не формальна OWL/RDF-онтологія. Джерелом істини залишаються вимоги застосунку й прийняті ADR.

**Верифікація:** виклик `scripts/validate_ontology.py` за структурованим словником із `ontology/schema.yaml`.
