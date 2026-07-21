# Тест кейсове — boilerplate-mochachai (starter)

Легенда: **P** = Priority · **Статус**: ⬜ Placeholder (`assert.fail()`) / ✅ Имплементиран

## Integration tests with chai-http (`tests/2_functional-tests.js`)

| ID | Тест | Статус | Очакван резултат след довършване | P |
|---|---|---|---|---|
| TC-01 | `GET /hello` без name | ⬜ Placeholder | `200`, текст `hello Guest` | P1 |
| TC-02 | `GET /hello?name=xy_z` | ⬜ Placeholder | `200`, текст `hello xy_z` | P1 |
| TC-03 | `PUT /travellers` `{surname: "Colombo"}` | ⬜ Placeholder (липсва `.send()`) | `200`, JSON `{name: "Cristoforo", surname: "Colombo"}` | P1 |
| TC-04 | `PUT /travellers` `{surname: "da Verrazzano"}` | ⬜ Placeholder (изобщо няма HTTP заявка) | `200`, JSON `{name: "Giovanni", surname: "da Verrazzano"}` | P1 |

## Functional Tests with Zombie.js

| ID | Тест | Статус | Очакван резултат след довършване | P |
|---|---|---|---|---|
| TC-05 | `browser.site` е зададен | ⬜ Placeholder (`browser` не е дефиниран в suite-а) | `Browser.site` е зададен на валиден URL; `browser` инстанция е създадена в `suiteSetup` | P1 |
| TC-06 | Подаване на "Colombo" в HTML формата | ⬜ Placeholder | Показва се `name: Cristoforo`, `surname: Colombo` | P1 |
| TC-07 | Подаване на "Vespucci" в HTML формата | ⬜ Placeholder | Показва се `name: Amerigo`, `surname: Vespucci` | P1 |

## Ръчни/допълнителни кейсове (след довършване на suite-а)

| ID | Стъпки | Очакван резултат | P |
|---|---|---|---|
| TC-08 | Изпрати `PUT /travellers` с несъществуваща фамилия | Определи и документирай очакваното поведение (404/празен обект) | P2 |
| TC-09 | Изпрати `GET /hello?name=<script>` | Стойността се връща escaped (XSS проверка) | P1 |
| TC-10 | Изпълни `npm test` след пълно довършване | Всички тестове минават зелено, без `assert.fail()` | P1 |

## Забележка
За референтна, вече завършена имплементация на същия suite виж
`qa-docs/TEST_CASES.md` в repo [`QA`](https://github.com/dimitarbeograd-QA/QA).
