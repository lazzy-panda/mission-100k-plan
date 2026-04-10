# Handoff — 09.04.2026 вечер → 10.04.2026 утро

## Где остановились

День 8/365. Вечер четверга. Завтра пятница 10.04 — по плану Post #2.

### Что сделано сегодня (09.04)
- Купили домен `morozco.tech` через Cloudflare Registrar
- Настроили Cloudflare Email Routing: `kirill@morozco.tech` → gmail
- Задеплоили landing на `morozco.tech` через Cloudflare Pages + кастомный домен, SSL активен
- Убрали matrix-эффект из `morozco-tech-landing/index.html`, увеличили логотип до 90px, подтянули brand name
- Удалили `index-v1.html` и `index-v2.html`, оставили только `index.html`
- Переписали Post #2 с общего киберпанка на конкретный Garry Tan / SXSW / cyberpsychosis хук
- Уменьшили количество "I" в посте с 10 до 2
- Прикрепили картинку `assets/freepik_cinematic-cyberpunk-scene_2752149138.png`
- **Опубликовали Post #2** сегодня (на день раньше графика — было на пт 10.04)
- Проверили engagement Post #1 "Dropped Notion" за сутки: **61 impression, 1 реакция, 0 комментов, 0 репостов**

### Вывод по engagement
Узкое место — охват, не контент. 61 impression = LinkedIn показал только ближайшей сети (~50 connections). Посты #3-12 **не перекраиваем**. Рычаг роста на этой неделе — комменты под чужими постами + warm DMs, не свои посты.

## С чего начать завтра утром

Выбор из трёх треков, в порядке приоритета:

### 1. Warm comments (рычаг охвата, 30-45 мин)
Открыть feed, найти 5-10 целевых постов от founders / CTO / Claude Code community, оставить содержательные комменты (не "great post", а конкретика по теме). Правила из `feedback_human_writing.md` — без AI-лексики, без em-dashes, non-native voice.

### 2. CCA-F Week 2 (2 часа)
Старт курса *Building Applications with the Claude API* (8 часов всего, покрывает 60% экзамена). Фокус: structured output + tool definitions. См. `cert_cca_f.md` строки 56-72. Делать заметки в новый файл `cert_cca_f_notes.md`.

### 3. Anthropic Partner Network (retry)
Вчера портал выдал "technical difficulties". Проверить https://partnerportal.anthropic.com/s/partner-registration снова. Форма:
- Company: `Morozco — Fractional CTO Services`
- Email: `kirill@morozco.tech`
- Website: `https://morozco.tech`
- Country: Cyprus
- Use case: уже написан в `cert_cca_f.md` строки 186
После approval → request exam access на Skilljar.

## Неcommitted изменения в git
- `M cert_cca_f.md` — обновлены Шаги 0, 0.5, 0.75 на done
- `M LINKEDIN_CONTENT_KIT.md` — Post #2 переписан
- `?? morozco-tech-landing/` — весь лендинг новый
- `M outreach_pitch.md` — не трогали сегодня, не знаю статус
- Хорошо бы закоммитить всё утром одним чистым коммитом перед началом работы.

## Открытые блокеры
- Partner Network портал лежит (technical difficulties на вчерашний вечер)
- HF image generation заблокирован `gradio=none` в сессии — если понадобятся картинки, брать из `assets/` или Freepik вручную

## Что НЕ делать
- Не переписывать Posts #3-12 на основе слабого engagement Post #1. Сэмпл слишком маленький.
- Не публиковать Post #3 раньше воскресенья 12.04 — график разреженный специально.
