# API документация — boilerplate-mochachai

Целева спецификация (виж `qa-docs/TEST_CASES.md` за текущия статус на
имплементацията и тестовете — много от тях все още са placeholder).

## `GET /hello`
| Параметър | Задължителен | Описание |
|---|---|---|
| `name` (query) | Не | По подразбиране: `Guest` |

```
GET /hello           → 200 "hello Guest"
GET /hello?name=xy_z → 200 "hello xy_z"
```

## `PUT /travellers`
**Body**: `{ "surname": "<фамилия>" }`

```
PUT /travellers {surname: "Colombo"}       → 200 {name: "Cristoforo", surname: "Colombo"}
PUT /travellers {surname: "da Verrazzano"} → 200 {name: "Giovanni", surname: "da Verrazzano"}
```

## HTML форма — „Famous Italian Explorers"
Текстово поле `surname` + submit. При подаване показва `span#name`,
`span#surname`, `span#dates`.

За пълна референтна имплементация виж
[`QA` repo](https://github.com/dimitarbeograd-QA/QA/blob/main/API.md).
