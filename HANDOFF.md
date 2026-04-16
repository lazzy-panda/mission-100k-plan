# Handoff — 11.04.2026 вечер → 12.04.2026 утро

## Где остановились

День 10/365. Пятница вечер. Завтра суббота 12.04 — встреча по калькулятору + подготовка Post #3.

### Что сделано сегодня (11.04)

- **Стратегический pivot:** отказ от cold outreach как основного канала. Продуктовая стратегия с 4 треками.
- **PLAN.md v2:** полная переработка. Praxisansatz = Track 1, Fractional CTO через inbound = Track 2, SaaS (Lingo, калькулятор, Daxi) = Track 3, медиа-автоматизация = Track 4.
- **Praxisansatz аудит:** изучен код medoc (Angular 17) + flask-medoc (Flask/SocketIO). Выявлены SaaS-gaps: hardcoded hospitals (Ahlen/Hamm), German-only, no multi-tenant, no persistent DB.
- **Каталогизация всех проектов:** 7 продуктов позиционированы и записаны в PLAN.md.
- **Morozco Mediacenter:** решено удалить. Убран из PLAN.md. GitHub repo deletion pending (нужен `gh auth refresh -s delete_repo`).
- **4 warm comments опубликованы** на LinkedIn (10.04 утром).
- **Partner Network:** статус "review in progress" с 10.04.
- **cert_cca_f.md:** обновлён Step 1 на done.
- **Память:** сохранены project_praxis_absatz.md и project_cyprus_tax_calc.md.

### Решения дня
- Praxis продаём глобально, не только DACH. Лендинг на EN с понедельника.
- LinkedIn = витрина портфеля, не канал продаж. Посты продолжаем 3/нед.
- CCA-F = фон, не блокер. Делаем параллельно, не ждём.
- С текущими клиниками (Ahlen/Hamm) не работаем — ищем новых.

## С чего начать завтра

### Суббота 12.04
1. **Встреча со специалистом по кипрскому налоговому калькулятору** — ключевое решение: адаптируем его Excel или пишем сами.
2. **Подготовить Post #3** "setNativeValue for React forms in Playwright" к публикации в воскресенье.
3. **Удалить morozco-mediacenter repo** после `gh auth refresh -s delete_repo`.

### Воскресенье 13.04
- Опубликовать Post #3.
- Финализировать план на неделю.

### Понедельник 14.04
- Landing page Praxisansatz (глобальный positioning, EN).
- 30-сек демо-видео.
- Pricing: €149-299/мес за клинику.

## Uncommitted изменения
- `M cert_cca_f.md` — Step 1 marked done + naming fixes
- `M outreach_pitch.md` — изменения из прошлых сессий
- `?? morozco-tech-landing/` — лендинг morozco.tech

## Открытые блокеры
- ~~Partner Network:~~ закрыт. Мягкий отказ 16.04 — предложили "Powered by Claude" (для встраивания в продукт, не партнёрка)
- GitHub delete_repo scope не выдан — нужна интерактивная авторизация
- Калькулятор: Excel-наработки получены от специалиста (12.04), нужно начать разработку
