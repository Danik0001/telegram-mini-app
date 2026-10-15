# Структура и сценарии

## Навигация

| Вкладка | Содержание | Основное действие |
|---|---|---|
| Music | Выбранный трек, плеер | Слушать / открыть Library |
| Library | Tracks / Instrumentals | Выбрать трек или бит |
| AI Studio | Vocal AI / AI Samples | Начать создание |
| Wallet | TON Connect, ASIQ | Подключить / обновить баланс |
| Community | Официальные каналы | Открыть внешний канал |

Не создавать шестую вкладку Samples: вход через Studio. Library остаётся медиатекой каталога, сохранённые проекты не обещаются.

## Основной путь Vocal AI

studio → beat → analysis → record → permission → recording → take → record → process → mix → mix-confirm → processing → result → export → export-done.

MID обязателен. BACK/ADLIBS добавляются отдельно; настройки Mute/Solo/Volume/Pan не переносятся между дорожками. Из record доступны lyrics → teleprompter, upload, track-settings. Перезапись открывает retake; отмена активной записи — cancel-take; очистка текста — clear-lyrics. Из process доступны tune и предлагаемые по ТЗ slicer/fit. Выход из незавершённой студийной сессии — exit с предупреждением о потере записи.

## Samples

studio → samples → sample-wait → sample-results → sample-detail. Библиотека — sample-library. Перед генерацией нужны описание, BPM 70–180 и 1/3 варианта. Ошибки/ограничения: sample-empty, sample-error, sample-quota, offline. Сохранение в избранное в демо существует только до перезагрузки; постоянство требует реального сервиса.

## Wallet и Community

wallet → wallet-connect → wallet-connected; обновление → wallet-loading → успешный баланс / wallet-error. Отключение — wallet-disconnect. Обмен — swap-info → внешний STON.fi. Community → external-link → подтверждённый официальный канал.

## Исключения

Каталог: catalog-loading/catalog-error. Микрофон: mic-denied. Загрузка: upload-error. MID отсутствует: no-mid. Обработка: process-error. AI CLEAN недоступен: ai-unavailable. Во всех случаях сохранить понятный путь назад и повторить только релевантное действие.

Верхний picker прототипа позволяет просматривать состояния напрямую. Это инструмент ревью, а не дополнительный пользовательский сценарий.
