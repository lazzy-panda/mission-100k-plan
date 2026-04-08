# MISSION $100K — План и сверка

> Сверка с планом ведётся прямо в диалоге с Claude. Этот файл — **единственный** источник правды по статусу. Notion отключён 08.04.2026 (был дублирующим слоем, не работал).
>
> **Сегодня:** 2026-04-08 (среда) · **День 7 / 365** · **Фаза 0 — Фундамент**
> **Финиш:** 1 апреля 2027 · **Цель:** $100K/мес (Fractional CTO + SaaS)
>
> **Мобильный доступ:** GitHub private repo → Working Copy на iOS (настройка 08.04.2026).

---

## 1. Что уже сделано

### Структура плана (фазы и цель)

- **Цель:** $100K/мес к 1 апреля 2027 (подтверждено 06.04.2026).
- **Фазы:**
  - 🟡 Phase 0 — Фундамент (дни 1–29, апрель)
  - 🟢 Phase 1 — Первые деньги (дни 30–89, май–июнь)
  - 🔵 Phase 2 — Масштабирование (дни 90–179, июль–сентябрь)
  - 🟣 Phase 3 — Dev Studio (дни 180–269, октябрь–декабрь)
  - 🔴 Phase 4 — Визионер (дни 270–365, январь–март 2027)
- **Notion (отключён 08.04.2026).** Был workspace «План», база `📅 План 365`, дашборд с чекбоксами. За первые 7 дней 0/365 отмечено — система не работала. Workspace оставлен dormant (не удалён). Больше ничего туда не пишется. Единственный источник правды — этот файл.

### LinkedIn
- Профиль: <https://www.linkedin.com/in/kirill-morozov-51003037/> (верифицированный, переключились 06.04.2026 — старый `kirill-morozov-7226a0361` больше не используется)
- ✅ **Профиль полностью обновлён 06.04.2026** через Playwright. Headline, about, и **вся история карьеры переписана под Fractional CTO позиционирование** с архитектурой+автоматизацией в каждой карточке: Founder, AdTech Platform Contract (новая, Aug 2025–Present, anonymized как Dream Platform), UGC Contract, Praxisansatz (title→Senior Developer & Automation Lead, end-date Dec 2025), 4xc.com, Freedom Finance, SAS, Mediascope, PwC. Фото и баннер — добавить вручную.
- Готовый контент-кит (хранится в Notion / памяти): тексты профиля Phase 1 и Phase 2, **12 постов** на 4 недели (TIL · Problem→Solution · Opinion · Case · Build-in-public).
- Playwright MCP настроен глобально — можно автоматизировать публикации.
- ⏳ Постов пока опубликовано: **0 / 12**. Первый (TIL) — запланирован на среду 08.04.

### SaaS Track 2 — Lingo (формализовано 08.04.2026)
- Код живёт в `~/Documents/greek-app` (Next.js 16, Drizzle, Clerk, Stripe scaffolding). Форк `sanidhyy/duolingo-clone`, расширен 11 exercise modes + spaced repetition + vocabulary tracking. Полный feature inventory — `~/Documents/greek-app/APP_REPORT.md`.
- Стратегический документ: `saas_idea_1.md` в корне этого workspace.
- Tier 1 wedge: греческий для русскоязычных экспатов на Кипре, €12/мес. Tier 2 (с июля): мультиязычный движок. Tier 3 (с апреля 2027): Leetcode for skills — любой домен.
- Hard kill criterion: если к концу июня нет 10 платящих, Lingo становится side-project, Fractional CTO = Track 1 фулл.

### Программа обучения (`reading_plan_365.md`)
- 28 книг / 12 000 страниц / 365 дней. Старт — 1 апреля 2026.
- Q2 апрель–июнь: Тиль · Далио · Адамс · Брэнсон · Айзексон (Джобс) · Кларк · Кроули · Тегмарк.
- Параллельно: Goodfellow Deep Learning (с мая), Tedrake Robotics (с июля), Sutton Rocket Propulsion (с октября).

### Сертификация CCA-F — Claude Certified Associate (Foundations)
- Полный план: `cert_cca_f.md` (зафиксирован 08.04.2026).
- Зачем: credibility layer для Fractional CTO — бейдж у считанных сотен людей в мире.
- **Прогресс:** ✅ Claude 101 + AI Fluency пройдены (неделя 1 сделана). Осталось: 26 часов за 6 недель.
- Целевая дата экзамена: ~20.05.2026 (день ~48).
- Стоимость: $99 или $0 если попасть в первые 5000 партнёров Claude Partner Network.

### Decision log
- `decision_log/2026-04-08-notion-drop.md` — отказ от Notion, переход на file-based
- `decision_log/2026-04-08-lingo-wedge.md` — Tier 1 wedge Lingo = греческий для русскоязычных Кипра

---

## 2. Где мы прямо сейчас

**Phase 0 — Фундамент. День 7/29.**
Цель фазы: настроить инфраструктуру, добить LinkedIn-профиль, выпустить первые посты, подготовить outreach-машину к Phase 1.

| День | Дата | Фокус | Статус |
|------|------|-------|--------|
| 1 | Чт 02.04 | SaaS + клиенты | ☐ pre-start (до формального старта системы) |
| 2 | Пт 03.04 | LinkedIn + итоги недели | ☐ pre-start |
| 3 | Сб 04.04 | Обучение + стратегия | ☐ pre-start |
| 4 | Вс 05.04 | Отдых + планирование | ☐ pre-start |
| 5 | Пн 06.04 | LinkedIn + планирование | ✅ профиль полностью обновлён через Playwright (headline, about, experience, skills, services, projects), 12 постов готовы |
| 6 | Вт 07.04 | SaaS + outreach | ✅ 10 cold connects отправлены, 5 warming-комментов (Teo/Akshit/Tal/Cristian/Nate), pitch + 3 DM-шаблона, `feedback_human_writing.md` зафиксирован в памяти |
| **7** | **Ср 08.04 — сегодня** | **LinkedIn + нетворкинг** | ✅ миграция с Notion, GitHub repo + iOS, контент-кит v2 (EN), пост #1 опубликован (URN 7447603321424625664) |

---

## 3. Спринт на эту неделю (дни 5–11, 06–12 апреля)

**Понедельник 06.04 — LinkedIn + планирование** ✅
- [x] Залить в профиль текст Phase 1 (headline + about + experience + skills) — сделано через Playwright
- [x] Поставить фото / баннер, проверить URL — сделано вручную
- [x] Запланировать 3 поста недели из контент-кита (TIL, Problem→Solution, Opinion) — зафиксированы в `LINKEDIN_CONTENT_KIT.md` (#1 Ср 08.04, #2 Пт 10.04, #3 Вс 12.04)
- [x] Список 20 целевых аккаунтов на нетворкинг (`outreach_list.md`)
- [+] Extra: profile post-audit cleanup (удалены Angular из Skills + старый проект Beafcake)

**Вторник 07.04 — SaaS + outreach** ✅
- [x] Сформулировать 1-строчный pitch Fractional CTO — v2 в `outreach_pitch.md` секция 1 (pivot на Solutions Architect/Claude Code, без TS/Node в первой строке)
- [x] Шаблон холодного DM (3 варианта) — T1/T2/T3 в `outreach_pitch.md` секция 2
- [x] Первые 10 connection-запросов (все cold, список в `outreach_sent_2026-04-07.md`)
- [+] Extra: 5 warming-комментов под постами целевых (Teo, Akshit, Tal, Cristian, Nate)
- [+] Extra: зафиксирован `feedback_human_writing.md` в auto-memory — non-native English rules + hard bans на AI-vocab/idioms

**Среда 08.04 — LinkedIn + нетворкинг** ← сегодня
- [x] Опубликовать пост #1 — опубликован в 14:22 (EN, "Today I dropped Notion", Build-in-public вместо изначального TIL). URN `urn:li:activity:7447603321424625664`. Первая версия была случайно на русском, удалена, переписана на английский после полного аудита контент-кита
- [x] ~~Прокомментировать 5 постов в нише~~ — сделано вчера в рамках warming раунда
- [x] ~~+10 connection-запросов~~ — лимит invites на месяц исчерпан вчера (10/10). Окно возобновления 03.05
- [x] Переезд трекинга с Notion на файлы в `/Users/kirill/MyApps/Plan` + GitHub private repo → Working Copy для iOS
- [x] Полный аудит и перевод на английский всех 12 постов в `LINKEDIN_CONTENT_KIT.md` (v2)
- [+] Extra (pull-forward из чт): зафиксирована SaaS идея №1 в `saas_idea_1.md`. Tier 1 wedge = Lingo (греческий для русскоязычных экспатов на Кипре, €12/мес). Код уже есть в `~/Documents/greek-app`, сегодня сформулирована стратегия, ICP, pricing, 5 discovery вопросов, hard kill criterion на 30.06

**Четверг 09.04 — SaaS + клиенты + outreach**
- [x] ~~Зафиксировать SaaS-идею №1~~ — сделано вчера вечером, `saas_idea_1.md`
- [ ] Landing-черновик (одна страница) — hero / problem / solution / CTA / waitlist form, домен-решение (lingo.app vs greek-cy.com)
- [ ] 30 минут ресёрча: Stripe в Кипре для EU VAT vs LemonSqueezy (R3 в `saas_idea_1.md`)
- [ ] Поиск 3 целевых Telegram-чатов для discovery (Лимассол / Пафос / Никосия)
- [ ] **Warm DMs** день-2 после accept — 8 принятых за 24ч из 10 cold connects. Шаблоны из `outreach_pitch.md` секция 4.
- [ ] **CCA-F неделя 2 старт:** Building Applications with the Claude API, 2 часа из 8 (план в `cert_cca_f.md`)

**Пятница 10.04 — LinkedIn + итоги недели**
- [ ] Опубликовать пост #2 (Problem→Solution)
- [ ] Ретро недели в Notion: что пошло, что нет, lessons
- [ ] Обновить чекбоксы «Готово» в `📅 План 365`

**Суббота 11.04 — Обучение + стратегия**
- [ ] Тиль *Zero to One* — гл. 1–4 (~80 стр)
- [ ] 5 заметок-тейкавеев в Notion

**Воскресенье 12.04 — Отдых + планирование**
- [ ] Лёгкий план на след. неделю (10 минут)
- [ ] Полный отдых

---

## 4. Месячные milestones — апрель (Phase 0)

- [x] Профиль LinkedIn полностью оформлен (Phase 1 версия) — 06.04
- [ ] 12 постов опубликовано (3/нед × 4 нед)
- [ ] +200 целевых connections
- [ ] 1 SaaS-гипотеза с landing-черновиком
- [ ] Тиль *Zero to One* + Далио *Принципы* (часть 1) прочитаны
- [ ] Outreach-pipeline: **120 cold contacts** (20 пилот + 30/нед × 3.5 нед = ~120)
- [ ] **Реалистичный target по клиентам в апреле: 0.** Месяц на отладку воронки. Первые $$$ — май.
- [ ] Notion `📅 План 365`: ≥25 дней отмечено выполненными

### Воронка и финансовый горизонт (пересчитано 06.04 после ревизии конверсий)

| Месяц | Connections | Cold contacts | Платящие клиенты | MRR target |
|-------|-------------|---------------|------------------|------------|
| Апрель (P0) | +200 | 120 | **0** (пилот воронки) | $0 |
| Май (P1 нач.) | +400 | 150 | 1–2 | $5–10K |
| Июнь (P1 кон.) | +500 | 200 | 3–5 | $10–20K |

**Базовые конверсии для cold LinkedIn:** accept 25% → DM-ответ 15% → звонок 40% → клиент 10% ≈ **0.15% сквозной**. Поэтому 120 cold/мес = ~0.2 клиента математически. Реальные клиенты в мае–июне приходят в основном через **warm/inbound**: контент (12 постов/мес) + комменты под постами целевых аккаунтов + mutual connections.

---

## 5. Как сверяемся (обновлено 08.04.2026)

1. **Каждый день** — Claude сам отмечает в `PLAN.md` что сделано по ходу разговора. В конце дня (или в момент "закрываем день") — Claude финализирует день: статус в спринт-таблице, галочки на конкретных пунктах, extra-результаты вне плана. Кирилл подтверждает или корректирует.
2. **Каждую пятницу** — короткое ретро прямо здесь. Claude собирает понедельник-пятницу из `PLAN.md` + истории чата, обновляет раздел спринта на следующую неделю.
3. **В конце месяца** — закрываем month-milestones, катимся в Phase 1.
4. **Notion отключён.** Всё живёт в `/Users/kirill/MyApps/Plan/` + диалог с Claude. Мобильный доступ — GitHub private repo → Working Copy на iOS.

---

## 6. Закрытые вопросы (решения от 06.04)

- ✅ **LinkedIn-профиль обновлён полностью** через Playwright 06.04.2026:
  - Headline: Fractional CTO & Senior Frontend Architect · 20 yrs · Angular · Next.js · TypeScript · Building AI-assisted products with Claude Code · Open to advisory & founding-engineer roles
  - About: новый текст Phase 1 (stealth EdTech, Claude Code runtime, 365-day learning program)
  - Experience: добавлены Founder (Oct 2025–Present) и UGC Platform Contract (Oct 2024–Sep 2025), Praxisansatz обрезан до Aug 2023–Sep 2024
  - Skills: +Next.js, TypeScript, Claude Code, Model Context Protocol (MCP), Bun.js, Drizzle ORM, AI Agents, Product Discovery
  - Фото и баннер — поставлены пользователем вручную
- ✅ **Mission = $100K/мес к 1 апреля 2027.** Планка сознательно поднята с $50K (предложено мной, согласовано). Память обновлена.
- ✅ **Программа обучения стартует в субботу 11.04.2026** (день 10 плана, слот «Обучение + стратегия»). `reading_plan_365.md` пересчитан под этот старт: Тиль *Zero to One* → дни 11–18, Далио *Принципы* часть 1 → дни 19–30.
