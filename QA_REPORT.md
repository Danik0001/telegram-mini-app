# Технический QA / 15.10.2026

Локальный дизайн-прототип проверен в браузере Codex. Это не тест production и не исследование на людях.

| Ширина окна | Экранов | Переполнение / выход основных контролов |
|---|---:|---|
| 320 px | 55 | Не обнаружено |
| 390 px | 55 | Не обнаружено |
| 430 px | 55 | Не обнаружено |
| 1280 px | 55 | Не обнаружено |

## Сценарии

- PASS — MID required
- PASS — Take MID
- PASS — Take BACK
- PASS — Take ADLIBS
- PASS — MID allows processing
- PASS — BYPASS preserves FX choices
- PASS — Full demo mix to WAV state
- PASS — Samples prompt validation
- PASS — Three Samples variants
- PASS — Samples favourites
- PASS — TON demo connection
- PASS — TON demo disconnect
- PASS — Выход во время активной записи открывает предупреждение

Проверены 55 PNG и 65 экранных SVG, отдельный SVG UI Kit; основной макет 390 px, адаптации ключевых экранов 296/390/1200 px. PNG получены из браузера, SVG — векторное представление DOM с редактируемым текстом. Просмотрены основные экраны и контактный лист.

## Ограничения

Нет настоящего аудио, записи, AI, сохранения, WAV, TON Connect и транзакций. Требуется проверить iOS/Android Telegram, клавиатуру, safe areas, back/close events, разрешения микрофона, реальное время обработки и ошибки backend. Пользовательские тесты и нативная сборка v2 в Figma ещё не выполнены. Текст SVG может переноситься иначе, чем браузерный PNG.
