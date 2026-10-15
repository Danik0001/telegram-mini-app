# Соответствие MVP и ТЗ

Источник наблюдений: `https://app.asiqpai.site/`, `https://app.asiqpai.site/samples/`, осмотр 14 октября 2026. Веб-режим вне Telegram не доказывает работу серверных операций.

| Возможность | Основание | Экран v2 | Решение |
|---|---|---|---|
| Music / player | Видно в MVP | music | Сохранены позиция, предыдущий/следующий, режим, избранное |
| Library Tracks / Instrumentals | Видно в MVP | library, instrumentals | Сохранены обе категории; поиск — UX-добавление |
| Пять вкладок | Видно в MVP | Все | Music / Library / AI Studio / Wallet / Community |
| AI Studio / обзор двух инструментов | Видно в MVP | studio | Vocal AI и AI Samples |
| Анализ BPM/KEY/SCALE/CONFIDENCE | Видно в Vocal AI | beat, analysis, analysis-loading | Отдельный блок с ручным уточнением |
| MID / BACK / ADLIBS | Видно в Vocal AI | record, recording, take | Дорожки независимы в демосостоянии |
| Mute/Solo и Volume/Pan | Видно в Vocal AI | record, track-settings, mix | Не удалены при упрощении потока |
| Текст и телесуфлёр | Видно в Vocal AI | lyrics, teleprompter, clear-lyrics | Крупный текст и явное подтверждение очистки |
| 3 минуты / 25 МБ | Текст ограничения MVP | record, recording, upload, upload-error | Сохранены, ошибка файла не заменяет дорожку |
| MID CLEAN/PREMIUM/DARK, BACK WIDE, ADLIBS SPACE | Список пресетов MVP | process | Сохранены наименования |
| TUNE AUTO/MANUAL и KEY/SCALE | Подсказка и FX MVP | tune | Отдельный экран, не общий slider интенсивности |
| EQ/COMP/REVERB/DELAY и BYPASS | Видно в MVP | process | BYPASS сохраняет выбранные переключатели |
| Громкость бита / WIDTH / offset | Видно в MVP | mix | Отдельная группа продвинутых настроек |
| Сборка полного микса и WAV | Видно в MVP | mix-confirm, processing, result, export | Без неподтверждённых битности/частоты/цены |
| Нет сохранения проекта между запусками | Явное предупреждение MVP | record, result, exit | Удалено ложное обещание Library проектов |
| Экспорт не равен лицензии бита | Явное предупреждение MVP | beat-detail, beat, export | Сохранено |
| Samples 70–180 BPM / KEY / 4–8 bars | Видно в Samples | samples | Не длительность в секундах |
| Minimal/Dense / 1–3 варианта / квота | Видно в Samples | samples, sample-results | Сохранены |
| Samples Library / избранное | Видно в Samples | sample-library | Отделено от медиатеки Music |
| TON Connect / ASIQ / refresh | Видно в Wallet | wallet-* | Удалены кредиты и выдуманные покупки |
| STON.fi | Ссылка в Wallet | swap-info | Описан внешний путь, обмен не имитирует реальную транзакцию |
| Community / официальные ссылки | Видно в MVP | community, external-link | Без неподтверждённых постов и комментариев |
| Vocal Slicer / AI Fit | Требование Excel-ТЗ; в осмотренном UI не подтверждено | slicer, fit | Проектные сценарии с пометкой «по ТЗ» |
| Профиль и RU/KZ/EN | Требование ТЗ; профиль не виден в осмотренном MVP | LOCALIZATION.md / handoff | Не объявлено уже существующей функцией; точку входа согласовать отдельно |

## Приоритеты после аудита

Сохранить существующую функциональность, раскрывать сложные параметры постепенно, объяснять недоступность кнопок, различать загрузку/пустоту/ошибку, не обещать сохранение или оплату без backend-контракта. Просмотр UI не заменяет проверку алгоритмов и реальных пользовательских задач.
