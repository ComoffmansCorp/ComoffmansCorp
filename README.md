<div align="center">

<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&size=26&pause=1000&color=5B4BE0&center=true&vCenter=true&width=560&lines=Backend-разработчик;Go+%C2%B7+PostgreSQL+%C2%B7+Vue+%C2%B7+Kotlin;Modular+monolith+%C2%B7+Ports+%26+Adapters" alt="Typing SVG" />

</div>

<br/>

<div align="center">

![Domains](https://img.shields.io/badge/Domains-7-5B4BE0?style=for-the-badge)
![Tables](https://img.shields.io/badge/DB_tables-13-5B4BE0?style=for-the-badge)
![Endpoints](https://img.shields.io/badge/REST_endpoints-37-5B4BE0?style=for-the-badge)
![Platforms](https://img.shields.io/badge/Platforms-3-5B4BE0?style=for-the-badge)

</div>

## [Маркетплейс бытовых услуг](https://github.com/ComoffmansCorp/consumer-maintenance-system)

Платформа в духе Профи.ру: клиент публикует заявку, свободные мастера
откликаются с ценой, клиент сам выбирает исполнителя.

<table>
<tr>
<td width="50%" valign="top">

**Backend** — Go, модульный монолит по паттерну **ports & adapters**:
7 независимых доменов (`auth`, `catalog`, `master`, `request`, `review`,
`payment`, `chat`), связанных через интерфейсы, а не прямые импорты.

- PostgreSQL, 13 таблиц, атомарные транзакции при конкурентных откликах
  на одну заявку
- Эскроу-расчёты и рейтинги мастеров — через событийную модель
  (in-process pub/sub), а не прямые вызовы между доменами
- Специализация мастера проверяется на сервере, а не только в интерфейсе

</td>
<td width="50%" valign="top">

**Frontend & mobile** — три клиента на одном API:

- Vue 3 + TypeScript — публичный сайт и встроенная админ-панель
- Kotlin/Android — мобильный клиент мастера,
  [android-customer](https://github.com/ComoffmansCorp/android-customer)
- JWT (access + refresh), REST, Docker Compose — весь стек одной командой

</td>
</tr>
</table>

<div align="center">
<img src="https://skillicons.dev/icons?i=go,postgres,vue,ts,kotlin,docker" height="42"/>
</div>

<br/>

<div align="center">

[![Email](https://img.shields.io/badge/comoffmans%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:comoffmans@gmail.com)

</div>
