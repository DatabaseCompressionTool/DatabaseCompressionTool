<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/dct-press-dark.gif">
    <source media="(prefers-color-scheme: light)" srcset="assets/dct-press-light.gif">
    <img src="assets/dct-press-light.gif" alt="Database Compression Tool" width="200">
  </picture>
</p>

<h1 align="center">Database Compression Tool</h1>

<p align="center">
  <b>Свёртка и сжатие баз 1С: продукт вместо проекта</b><br>
  На базах от 200 ГБ размер сокращается в 2–3 раза, база до терабайта сворачивается за 5 часов,<br>
  свёртку запускает ваш администратор, данные остаются внутри вашего контура.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/версия-6.8.0-2f81f7?style=flat-square" alt="Версия 6.8.0">
  <img src="https://img.shields.io/badge/реестр_российского_ПО-включён-2ea043?style=flat-square" alt="Реестр российского ПО">
  <img src="https://img.shields.io/badge/свидетельство-Роспатент-2ea043?style=flat-square" alt="Свидетельство Роспатента">
  <img src="https://img.shields.io/badge/Infostart_Awards_2024-победитель-f0883e?style=flat-square" alt="Победитель Infostart Awards 2024">
  <img src="https://img.shields.io/badge/1С-8.3.15…8.3.27_|_8.5.1-c9d1d9?style=flat-square" alt="Платформы 1С">
</p>

<p align="center">
  <a href="https://databasecompressiontool.ru">Сайт продукта</a> ·
  <a href="https://databasecompressiontool.ru/files/DCT_DEMO.zip">Скачать демо</a> ·
  <a href="https://infostart.ru/marketplace/2163140/">Купить на Infostart</a> ·
  <a href="https://databasecompressiontool.ru/roi">Калькулятор экономии</a>
</p>

<p align="center">
  <img src="assets/dct-demo.webp" width="800" alt="DCT в работе: потоковое выполнение этапа свёртки и отчёт «Анализ сжимаемости данных», прогноз до и факт после">
</p>

<p align="center">
  ▶ <a href="https://rutube.ru/video/20fb6644767bda088f521cee8d9bd92c/">Знакомство с DCT за минуту</a> ·
  <a href="https://rutube.ru/video/11ddc86693a293b68e58c65946f790cd/">Подробный обзор, 19 мин</a> ·
  <a href="https://www.youtube.com/@DatabaseCompressionTool/videos">Канал на YouTube</a>
</p>

---

## Что это

Database Compression Tool (DCT) это внешняя обработка для платформы «1С:Предприятие 8». Она выполняет свёртку и сжатие базы данных, сохраняя логическую целостность учётных данных: в рабочей базе остаются актуальные остатки и нужные периоды, движения закрытых периодов сворачиваются во входящие остатки на выбранную дату.

Конфигурацию менять не нужно, БСП не требуется. Инструмент работает внутри вашего контура: свёртку запускает ваш администратор, данные не покидают инфраструктуру компании.

## Цифры

| | |
|---|---|
| **51%** | медиана сжатия по 104 клиентским базам, в половине случаев 34–67% |
| **56%** | среднее сжатие на базах от 200 ГБ |
| **5 часов** | свёртка базы до терабайта, до 300 ГБ примерно за 2 часа |
| **15 минут** | настройка перед запуском |
| **300+** | успешных кейсов: розница, производство, логистика, строительство, госсектор |
| **до 8 потоков** | многопоточная свёртка с балансировщиком |

## Подтверждённые результаты на базах клиентов

| Конфигурация | Было | Стало | Сжатие | Время свёртки |
|---|---|---|---|---|
| 1С:Бухгалтерия 3.0 | 394 ГБ | 96 ГБ | 76% | 1 ч 50 мин |
| 1С:ERP 2 | 1,7 ТБ | 470 ГБ | 73% | 10 ч 35 мин |
| 1С:УПП 1.3 | 1,3 ТБ | 341 ГБ | 73% | 16 часов |
| 1С:КА 2 | 877 ГБ | 254 ГБ | 71% | 5 ч 27 мин |
| 1С:УТ 10.3 | 1,1 ТБ | 402 ГБ | 64% | 21 час |

Это сильные результаты, а не типичные: медиана сжатия по 104 клиентским базам 51%, в половине случаев результат укладывается в 34–67%. Полное распределение и методика замера: [статистика свёртки](https://databasecompressiontool.ru/statistika-svertki-1s).

## Совместимость

**Работает:** типовые, доработанные и самописные конфигурации, управляемые и обычные формы. Платформы 8.3.15…8.3.27 и 8.5.1. MS SQL Server 2008–2025, PostgreSQL 9–18 (включая сборки для 1С), файловые базы. Сервер 1С под Windows, при этом СУБД может стоять на Linux: связка «сервер 1С на Windows + PostgreSQL на Linux» поддерживается полностью.

**Не работает:** сервер 1С:Предприятия под Linux (ограничение касается только сервера приложений, не СУБД), базы в сервисе 1С:Fresh, базы с принудительно включённым разделением данных, СУБД IBM DB2 и Oracle.

Подробная таблица совместимости: [databasecompressiontool.ru/support](https://databasecompressiontool.ru/support)

## Чего продукт не делает

- не исправляет ошибки учёта и не заменяет обслуживание СУБД: если база тормозит из-за дисков, фрагментированных индексов или тяжёлых доработок, объём тут ни при чём;
- не трогает регистры расчёта зарплатных конфигураций: записи прошлых периодов участвуют в текущих расчётах, поэтому их движения сохраняются без изменений. Остальные данные зарплатных конфигураций сворачиваются штатно;
- не уменьшает журнал регистрации: он хранится вне базы и на её размер не влияет.

Разбор ограничений: [Чего свёртка не сделает](https://databasecompressiontool.ru/articles/chto-svertka-ne-ispravit)

## Как попробовать

Бесплатная демо-версия строит отчёт «Анализ сжимаемости» на вашей базе и показывает прогноз результата до покупки: сколько именно освободится гигабайт.

**[Скачать демо](https://databasecompressiontool.ru/files/DCT_DEMO.zip)** · **[Посчитать экономию](https://databasecompressiontool.ru/roi)** · **[Купить на Infostart](https://infostart.ru/marketplace/2163140/)**

Продажи и техническая поддержка идут через маркетплейс Infostart: договор, счёт и закрывающие документы для юрлиц, ответ поддержки в течение 24 рабочих часов.

## Репозитории

| Репозиторий | Назначение |
|---|---|
| [docs](https://github.com/DatabaseCompressionTool/docs) | Публичная документация: совместимость, быстрый старт, FAQ, история версий |
| [DCT-issues](https://github.com/DatabaseCompressionTool/DCT-issues) | Сообщения об ошибках и запросы совместимости |

## Быстрые ссылки

- [Главная](https://databasecompressiontool.ru/)
- [Обзор продукта](https://databasecompressiontool.ru/product)
- [Редакции и цены](https://databasecompressiontool.ru/editions)
- [Калькулятор экономии (ROI)](https://databasecompressiontool.ru/roi)
- [Совместимость, документация, FAQ](https://databasecompressiontool.ru/support)
- [Статьи и руководства](https://databasecompressiontool.ru/articles/)
- [Видео на YouTube](https://www.youtube.com/@DatabaseCompressionTool/videos)
- [История версий](https://databasecompressiontool.ru/changelog)

---

<p align="center">
  <sub>© Команда DCT · Победитель Infostart Awards 2024 · Реестр российского ПО · Свидетельство Роспатента</sub>
</p>

