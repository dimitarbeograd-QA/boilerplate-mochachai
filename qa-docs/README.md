# QA документация — boilerplate-mochachai (starter fork)

## Съдържание
- [`TEST_PLAN.md`](TEST_PLAN.md) — стратегия и статус на suite-а (placeholder vs. завършен).
- [`TEST_CASES.md`](TEST_CASES.md) — тест по тест статус + ръчни кейсове.
- Bug report шаблон: [`.github/ISSUE_TEMPLATE/bug_report.md`](../.github/ISSUE_TEMPLATE/bug_report.md).

## Статус
Този repo е **starter template** (форк на freeCodeCamp/boilerplate-mochachai) —
тестовете в `tests/` съдържат `assert.fail()` placeholder-и, очакващи
имплементация. Виж repo [`QA`](https://github.com/dimitarbeograd-QA/QA) за
завършена референтна версия на същите тестове.

## Как да докладваш бъг
1. Отвори нов Issue в GitHub.
2. Избери темплейта **Bug report**.
3. Посочи дали проблемът е в placeholder тест или в реализирана логика.

## Приоритети
- **P1** — критичен тест/функционалност (основните API endpoint-и).
- **P2** — важна, но не блокираща.
- **P3** — козметични/edge-case проблеми.
