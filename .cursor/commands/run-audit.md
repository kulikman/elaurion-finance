---
description: Run audit for this repository without inventing external template paths
---

Выполни аудит текущего репозитория, а не внешний шаблон.

1. Прочитай `AGENTS.md` и `CLAUDE.md`, если они есть.
2. Если есть `audit/rules.json` и `audit/AUDIT_PROMPT.md`, используй их как source of truth.
3. Если `audit/` отсутствует, проведи lightweight audit по реальным файлам: stack, scripts, routes, env vars, security-sensitive areas, generated files, docs consistency.
4. Проверь, что docs/rules не выдумывают команды, APIs, routes, env vars, database fields, services или integrations.
5. Не создавай и не изменяй `audit/rules.json` без явного согласия пользователя.
6. После изменений запускай только проверки, которые реально есть в этом repo.

В конце покажи: что проверено, что найдено, что исправлено, какие проверки прошли, остаточные риски.
