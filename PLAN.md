# MISSION $100K — План и сверка (v2)

> **Обновлено:** 2026-04-11 (пятница) · **День 10 / 365** · **Фаза 0 — Фундамент**
> **Финиш:** 1 апреля 2027 · **Цель:** $100K/мес
>
> **v2 (11.04.2026):** полная переработка стратегии. Добавлены все продукты (Praxisansatz, Good/Beauty News, Daxi, калькулятор). LinkedIn сдвинут с cold outreach на витрину портфеля. Praxisansatz выведен в Track 1 как единственный продукт с клиентами.

---

## 1. Стратегия — 4 трека к $100K

### Track 1 — Praxisansatz (B2B, DACH)
**Статус:** в проде, работает в нескольких поликлиниках в Германии.
Система информирования пациентов в залах ожидания: Smart TV, голосовые объявления, интерактивные карты маршрутов к кабинетам. Python + sockets + Angular + Google Cloud + Telegram logging.

**Почему Track 1:** единственный продукт с доказанным PMF и платящими клиентами. Масштабирование одного рабочего продукта > запуск нового с нуля.

**Цель Phase 0-1 (апрель-июнь):**
- [ ] Зафиксировать текущий MRR и unit economics
- [ ] Landing на morozco.tech/praxis или отдельный домен
- [ ] 5 outreach-писем в клиники DACH-региона (тёплые через существующих клиентов)
- [ ] Case study из текущих внедрений для LinkedIn и сайта

### Track 2 — Fractional CTO (услуги)
**Статус:** позиционирование готово, LinkedIn обновлён, домен morozco.tech live.

**Сдвиг стратегии (11.04):** убираем cold outreach как основной канал. 120 cold contacts в месяц при 0.15% конверсии = 0.2 клиента. Не работает. Вместо этого:
- Портфель из 7 продуктов = доказательство компетенции
- LinkedIn посты 3/нед = входящий трафик (12 постов готовы)
- Referrals от клиентов Praxisansatz = тёплый канал
- CCA-F бейдж = credibility layer (фон, не блокер)

**Цель:** 1-2 клиента к концу июня через входящие, не исходящие.

### Track 3 — Продукты (SaaS + tools)

**3a. Lingo (Greek App)** — €12/мес, русскоязычные экспаты Кипр
- Статус: 60% ready, 4 урока, 80 заданий, 11 типов упражнений
- Ближайшее: dogfood (Кирилл сам учит греческий каждый день)
- Блокер: мало контента (нужно 15+ уроков), vocabulary не заполнен
- Hard kill: 10 платящих к 30.06 или side-project
- Стратегия: `saas_idea_1.md`

**3b. Cyprus Tax Calculator** — бесплатный лид-магнит для экспатов
- Статус: в работе. Встреча 12.04 — специалист разрешила использовать свои Excel-наработки
- План: веб-калькулятор на основе её Excel
- Монетизация: бесплатный инструмент → лиды на Fractional CTO / консалтинг
- Аудитория: та же что Lingo (русскоязычные IT на Кипре)

**3c. Daxi** — AI-платформа обучения/тестирования
- Статус: готов (FastAPI + React Native + ChromaDB + OpenAI)
- GPT-грейдинг, flashcards, spaced repetition, allowlist
- Монетизация: B2B SaaS для компаний (onboarding, тестирование сотрудников) или white-label для образовательных платформ
- Приоритет: ниже Praxis и Lingo, но готов к демо

### Track 4 — Медиа-автоматизация (Good News / Beauty News)

**Good News** — tech/AI/VR/startups. Live, 4 GitHub Actions, Telegram.
**Beauty News** — beauty/fashion. Live, создан 09.04, 57 RSS + NotebookLM.

**Монетизация:**
- Спонсорские интеграции в Telegram-каналах при росте аудитории
- Продажа автоматизации как SaaS ("запусти свой AI-новостной канал за час")
- Портфолио для Fractional CTO ("я строю AI-автоматизации, вот примеры")
- White-label для ниш (медицина, юридический, крипто)

**Приоритет:** работает автоматически, не требует внимания. Растить органически.

---

## 2. Что уже сделано (дни 1-10)

### Инфраструктура
- [x] LinkedIn профиль полностью обновлён под Fractional CTO (06.04)
- [x] 12 постов написаны, аудит + перевод на EN (08.04)
- [x] Post #1 "Dropped Notion" опубликован (08.04) — 61 impression, 1 реакция
- [x] Post #2 "Cyberpsychosis / Garry Tan" опубликован (09.04)
- [x] 4 warm comments под целевыми постами (10.04)
- [x] Домен morozco.tech куплен + Cloudflare Email Routing (09.04)
- [x] Landing morozco.tech deployed — Three.js + Cloudflare Pages (09.04)
- [x] GitHub private repo + Working Copy iOS для мобильного доступа (08.04)
- [x] Миграция с Notion на file-based систему (08.04)

### CCA-F
- [x] Claude 101 + AI Fluency пройдены (неделя 1)
- [x] Partner Network заявка подана (10.04) → мягкий отказ (16.04), предложили "Powered by Claude"
- [ ] Building Applications with the Claude API (0/8 часов)

### Outreach
- [x] 10 cold connects отправлены, 8 accepted (07.04)
- [x] Pitch + 3 DM-шаблона готовы (outreach_pitch.md)
- [x] 5 warming-комментов (07.04) + 4 содержательных коммента (10.04)

### SaaS
- [x] saas_idea_1.md — стратегия Lingo зафиксирована (08.04)
- [x] decision_log/lingo-wedge — обоснование выбора wedge (08.04)

---

## 3. Где мы прямо сейчас

**Day 10/365. Пятница 11.04. Phase 0 — Фундамент.**

Стратегия пересмотрена. Переключаемся с "протянутой руки" (cold outreach, CCA-F зависимость) на продуктовую стратегию с Praxisansatz как якорем.

---

## 4. Спринт: дни 10-17 (11-18 апреля)

### Пятница 11.04 — Стратегия
- [x] Пересмотр плана, добавление всех продуктов
- [x] Praxisansatz: аудит кода (medoc + flask-medoc), оценка SaaS-readiness

### Суббота 12.04 — Калькулятор + чтение
- [ ] Встреча со специалистом по кипрскому налоговому калькулятору
- [ ] Подготовить Post #3 к публикации в воскресенье

### Воскресенье 13.04 — Публикация + отдых
- [ ] Опубликовать Post #3 "setNativeValue for React forms in Playwright"
- [ ] Финализировать план на неделю

### Понедельник 14.04 — Praxis: landing + демо
- [ ] Landing page для Praxis (глобальный positioning, EN)
- [ ] Записать 30-сек демо-видео (врач жмёт кнопку → экран в зале → маршрут)
- [ ] Pricing: €149-299/мес за клинику

### Вторник 15.04 — Praxis: листинги + visibility
- [ ] ProductHunt launch подготовка
- [ ] Capterra / G2 листинг
- [ ] Post #4 "Keeping context between Claude sessions" (среда по графику)

### Среда 16.04 — Lingo dogfood
- [ ] Добавить 5 уроков контента (артикли, базовые глаголы)
- [ ] Включить lesson locking + seed vocabulary
- [ ] Опубликовать Post #4

### Четверг 17.04 — Lingo dogfood + калькулятор
- [ ] Ещё 5 уроков + тест spaced repetition
- [ ] Калькулятор: начать разработку на основе Excel-наработок

### Пятница 18.04 — Ретро + Post #5
- [ ] Ретро недели
- [ ] Post #5 "Day 16 of 365" (пятница по графику)

---

## 5. Месячные milestones — апрель (Phase 0, обновлено 11.04)

- [x] LinkedIn профиль оформлен
- [ ] 6/12 постов опубликовано (3/нед, мы на 2/12)
- [ ] Praxisansatz: MRR зафиксирован, case study написан, 5 outreach-писем
- [ ] Lingo: 15+ уроков, daily dogfood запущен
- [ ] Cyprus Tax Calculator: Excel-наработки получены (12.04), начать разработку
- [ ] CCA-F: Building with Claude API курс начат (Partner Network ответ ждём)
- [ ] Тиль + начало Далио прочитаны

### Финансовый горизонт (пересмотрен 11.04)

| Месяц | Track 1 (Praxis) | Track 2 (Fractional) | Track 3 (SaaS) | Итого |
|-------|-------------------|---------------------|-----------------|-------|
| Апрель (P0) | текущий MRR | $0 | $0 | текущий |
| Май-Июнь (P1) | +2-3 клиники | 1 клиент $5-15K | Lingo beta | $10-20K |
| Июль-Сен (P2) | 10 клиник | 2-3 клиента | Lingo + Daxi | $30-50K |
| Окт-Дек (P3) | DACH expansion | 3-4 клиента | multi-product | $50-80K |
| Янв-Мар (P4) | — | — | — | $100K |

---

## 6. Портфель продуктов

| Продукт | Роль в стратегии | Приоритет |
|---------|-----------------|-----------|
| Praxisansatz | Revenue engine, B2B anchor | Высший |
| Fractional CTO | Cash flow, credibility | Высокий |
| Lingo | Personal dogfood → SaaS | Средний |
| Cyprus Tax Calc | Lead magnet, local market | Средний |
| Daxi | B2B SaaS, ready to deploy | Низкий (пока) |
| Good/Beauty News | Portfolio, passive growth | Фон |

---

## 7. Decision log

- `decision_log/2026-04-08-notion-drop.md` — отказ от Notion
- `decision_log/2026-04-08-lingo-wedge.md` — Tier 1 wedge = греческий для Кипра
- **2026-04-11 — стратегический pivot.** Сдвиг с cold outreach на продуктовую стратегию. Praxisansatz = Track 1. LinkedIn = витрина, не канал продаж. CCA-F = фон.

---

## 8. Как сверяемся

1. **Каждый день** — Claude отмечает в PLAN.md что сделано
2. **Каждую пятницу** — ретро недели, обновление спринта
3. **В конце месяца** — закрытие milestones
4. **Всё живёт в** `/Users/kirill/MyApps/Plan/` + GitHub private repo

---

## 9. Связанные файлы

- `saas_idea_1.md` — стратегия Lingo
- `cert_cca_f.md` — план CCA-F сертификации
- `LINKEDIN_CONTENT_KIT.md` — 12 постов на 4 недели
- `outreach_pitch.md` — pitch + DM шаблоны
- `reading_plan_365.md` — 28 книг / 365 дней
- `HANDOFF.md` — точка остановки между сессиями
- `decision_log/` — все архитектурные решения
