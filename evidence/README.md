# Evidence: Windows authentication investigation

Подтверждающие скриншоты трёх учебных сценариев.

| Файл | Что показывает |
|---|---|
| [s01-bob-failure-then-success.png](screenshots/s01-bob-failure-then-success.png) | 8 октября 2026 года: отказ 4625 для bob в 21:29:20.254 и успешный вход 4624 в 21:29:48.920; одинаковые источник, компьютер назначения и тип входа 3 |
| [s02-alice-lockout-and-success.png](screenshots/s02-alice-lockout-and-success.png) | 9 октября 2026 года: шесть отказов 4625 для alice, событие блокировки 4740 и более поздний успешный вход 4624 |
| [s03-svcbackup-repeated-failures.png](screenshots/s03-svcbackup-repeated-failures.png) | 9 октября 2026 года: шесть отказов 4625 для svcbackup с близкими интервалами между событиями |

Скриншоты alice и svcbackup извлечены без изменения содержимого из рабочего документа **Authentication-log investigation - Personal lab.docx**. Скриншот bob предоставлен отдельно при дополнении проекта. Содержимое изображений сохранено без изменения.

Для bob видны учётная запись bob, источник 192.168.56.1, компьютер назначения DESKTOP-KN3U7PI и тип входа 3. Интервал между отказом и успешным входом составляет 28,7 секунды. Коды status и subStatus на этом изображении не показаны; их значения в отчёте взяты из рабочего документа.

[Подробный разбор](../docs/investigation.md).
