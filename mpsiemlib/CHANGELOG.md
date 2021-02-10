# v0.3.3
## MP SIEM test: 
- R23.1.3482
## Tables
- Добавлен учет специфики API при построчной работе с табличками (set_table_row).  
Теперь делается автоматическое приведение к int для колонок типа number.  
Колонки типа datetime ожидают строку в формате `%d.%m.%Y %H:%M:%S` или int - timestamp
## Wheel
- Добавлены зависимости для сборки whl

---

# v0.3.2
## MP SIEM test: 
- R22.0.3192
- R23.1.3482
## Tables
- Добавление и удаление записей в таблицах построчно
## Helpers
- Загрузка данных в табличные списки через массив JSON

---
# v0.3.1
## MP SIEM test: 
- R22.0.3192
- R23.1.3482
## Incidents
- Учтены изменения в API

---
# v0.2.0
## MP SIEM test: 
- R22.0.3192
## Common
- Зафиксированы имена функций

## Filters
- выгрузка списка папок с фильтрами
- выгрузка списка фильтров
- выгрузка деталей по фильтру

## Health Monitor
- получить общий статус
- получить список ошибок (если есть)
- получить статус лицензии
- получить статус агентов
- получить статус VM контента в MP Core

## Source Monitor
- выгрузка источников и их статуса в мониторинге
- выгрузка форвардеров и их статуса в мониторинге
- получить все источники выбранного форвардера

## Tasks
- остановить, запустить, получить статус задачи
- получить список агентов, модулей, профилей, танспортов, учеток
- получить список задач
- получить список подзадач для активной задачи (история не поддерживается)

---
# v0.1.0
## MP SIEM test: R22.0.3192
## Common
- Аутентификация в IAM, Core
- Аутентификация в PT KB
- Централизованное логирование в каждом модуле (conf/logging.yml)
- Доступ к централизованным настройкам из каждого модуля
- Unit-тесты

## PT KB
- выгрузка списка групп, папок и паков
- выгрузка контента, кроме макросов
- инсталляция и удаление контента из SIEM Server

## Events
- выгрузка событий
- выгрузка с группировкой

## Incidents
- выгрузка инцидентов
- детальная информация по инциденту

## Users and Roles
- выгрузка пользователей, ролей, привилегий, приложений
- детальная информация по пользователю, роле

## Tables
- выгрузка списков из SIEM Server
- выгрузка содержимого
- загрузка содержимого