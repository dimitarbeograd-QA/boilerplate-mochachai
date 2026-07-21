# Архитектура — boilerplate-mochachai (starter fork)

## Общ преглед
Express приложение „Famous Italian Explorers" — starter версия на същата
curriculum апликация, документирана изцяло в repo [`QA`](https://github.com/dimitarbeograd-QA/QA)
(решена версия). Тук `server.js` съществува на root ниво (за разлика от `QA`,
където той липсва — виж `QA/ARCHITECTURE.md`).

## Файлова структура
| Път | Роля |
|---|---|
| `server.js` | Express app — маршрути `/hello`, `/travellers`, HTML форма |
| `tests/1_unit-tests.js` | Unit тестове (виж статус в `qa-docs/TEST_CASES.md`) |
| `tests/2_functional-tests.js` | Integration + Zombie.js тестове — **все още placeholder-и** (`assert.fail()`) |
| `test-runner.js` | Custom Mocha runner за структуриран отчет |
| `assertion-analyser.js` | Помощна логика за анализ на асъртите |
| `public/` | Статични клиентски файлове |
| `views/` | Pug/HTML изгледи, вкл. формата |

## Статус
Виж [`qa-docs/TEST_CASES.md`](qa-docs/TEST_CASES.md) за точния статус на всеки
тест (placeholder vs. имплементиран). За референтна имплементация виж
[`QA`](https://github.com/dimitarbeograd-QA/QA) repo-то.

## Роли
Няма ролева/auth логика — публичен API за учебни цели.
