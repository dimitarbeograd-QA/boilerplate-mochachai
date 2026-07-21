# Changelog

Форматът следва приблизително [Keep a Changelog](https://keepachangelog.com/).

## [Unreleased]
### Added
- Пълна QA документация (`qa-docs/TEST_PLAN.md`, `TEST_CASES.md`) и bug report темплейт.
- Технически документи: `ARCHITECTURE.md`, `SECURITY.md`, `CONTRIBUTING.md`, `API.md`.
- `test` script в `package.json` (`mocha tests --reporter spec --exit`).

### Known Issues
- Повечето тестове в `tests/2_functional-tests.js` са все още `assert.fail()` placeholder-и — виж `qa-docs/TEST_CASES.md`.

## Преди този журнал
По-ранните промени не са документирани тук — виж `git log` за пълна история.
