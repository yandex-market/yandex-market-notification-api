# API сервиса уведомлений Яндекс Маркета

Вы читаете спецификацию API сервиса уведомлений Яндекс Маркета, с помощью которого можно автоматизировать и упростить работу с маркетплейсом.

## Как сгенерировать сервер API уведомлений

Спецификация поможет сгенерировать файлы сервера на любом языке или фреймворке, которые поддерживает OpenAPI-генератор. Это может значительно упростить интеграцию с Яндекс Маркетом через API сервиса уведомлений.

### Получение спецификации через git

Есть два способа:
1. Выполнить команду `git clone https://github.com/yandex-market/yandex-market-notification-api.git`.
2. Скачать архив с репозиторием через GitHub web-ui: в правом верхнем углу нажмите зеленую кнопку `Code` и в выпадающем списке выберите `Download ZIP`.

### Установка OpenAPI-генератора через пакетные менеджеры

Документация генератора: <https://openapi-generator.tech/docs/installation>

**Для npm (любая ОС)**
`npm install @openapitools/openapi-generator-cli -g`

**Для Homebrew (macOS)**
`brew install openapi-generator`

**Для Scoop (Windows)**
`scoop install openapi-generator-cli`

### Генерация сервера (контракты/модели)

**Для npm (любая ОС)**
`npx @openapitools/openapi-generator-cli generate -i <path to openapi.yaml> -g <generator> -o <output path>`

**Для остальных пакетных менеджеров**
`openapi-generator generate -i <path to openapi.yaml> -g <generator> -o <output path> `

Значения частей запроса:

* `<generator>` — параметр генератора для выбранного языка или фреймворка.
* `<output path>` — выходная директория, куда будет помещен сгенерированный код сервера.
* `<path to openapi.yaml>` — путь к файлу openapi.yaml данной спецификации.

Примеры генераторов:
* spring
* kotlin-spring
* go-server
* aspnetcore
* python-flask
* nodejs-express-server

Полный список генераторов доступен по ссылке: <https://openapi-generator.tech/docs/generators>
