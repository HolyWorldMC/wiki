---
icon: globe-www
---

# REST API

Публичный REST API для разработчиков.

Доступен по адресу: `https://api.holyworld.me`

## Методы

{% openapi-operation spec="liteapi" path="/v2/prime/coins/trades" method="get" %}
[OpenAPI liteapi](https://api.holyworld.me/openapi/public)
{% endopenapi-operation %}

{% openapi-operation spec="liteapi" path="/v2/prime/events/current" method="get" %}
[OpenAPI liteapi](https://api.holyworld.me/openapi/public)
{% endopenapi-operation %}

{% openapi-operation spec="liteapi" path="/v2/prime/events/timetable" method="get" %}
[OpenAPI liteapi](https://api.holyworld.me/openapi/public)
{% endopenapi-operation %}

## Rate limiting

Публичные методы не имеют прикладных ограничений на частоту запросов.

Открытый API содержит только `GET`-запросы.

Анти-DDoS-защита может временно ограничить аномально интенсивный трафик.

## Правила доступа

Перечисленные методы доступны без авторизации.

Для доступа к другим возможностям сервера нужен **специальный токен**, который в данное время выдаётся в индивидуальном порядке при согласовании необходимых прав доступа.
