# Test Plan — boilerplate-mochachai (freeCodeCamp starter, fork)

## 1. Обхват
Форк на freeCodeCamp „Quality Assurance and Testing with Chai" starter
boilerplate. За разлика от репозиторий [`QA`](https://github.com/dimitarbeograd-QA/QA)
(решена версия), тестовете тук в `tests/1_unit-tests.js` и
`tests/2_functional-tests.js` са **незавършени placeholder-и**
(`assert.fail()`), очакващи да бъдат имплементирани като част от curriculum
упражнението.

## 2. Цели на тестването
- Проследяване кои тестове все още са placeholder (`assert.fail()`) и кои са реално имплементирани.
- Всеки завършен тест да валидира реалното поведение на `/hello` и `/travellers` (виж завършената версия в repo `QA` за референтна имплементация).
- HTML формата „Famous Italian Explorers" да се тества с Zombie.js, след като placeholder тестовете бъдат довършени.

## 3. Тестова среда
| Компонент | Детайли |
|---|---|
| Runtime | Node.js + Express |
| Test framework | Mocha + Chai + chai-http + Zombie.js |
| Стартиране на тестове | `npm test` |
| Статус на suite-а | Частично имплементиран (виж `TEST_CASES.md`) |

## 4. Видове тестове
1. **Unit тестове** — довършване на `tests/1_unit-tests.js`.
2. **Functional/Integration тестове** — довършване на `/hello`, `/travellers` заявки.
3. **Headless browser тестове (Zombie.js)** — довършване на form submit тестовете.
4. **Referencing** — сравнение с решената версия в repo `QA` при доубършване.

## 5. Критерии за приемане
- Нито един тест не остава с `assert.fail()` placeholder преди merge/release.
- `npm test` минава изцяло (зелен suite) след довършване.
- Функционалността съответства на очакваната от freeCodeCamp curriculum спецификация.

## 6. Изходни артефакти
- `TEST_CASES.md` — статус на всеки тест (placeholder vs. имплементиран) + ръчни кейсове.
- Bug report-и през `.github/ISSUE_TEMPLATE/bug_report.md`.
