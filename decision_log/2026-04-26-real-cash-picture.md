# 2026-04-26 — Real cash picture & advisor corrections

## Контекст
Сессия с Claude 26.04.2026. Триггер: внешний advisor дал три коррекции к плану (€100K = stretch, не baseline; одна SaaS-ставка; контракты как машина денег). При раскрытии контекста выяснилось, что PLAN v2 системно занижал реальное состояние дел.

## Что выяснилось

### Реальный кэш (был скрыт от плана)
- Активный контракт **Dream Platform** (НТС «Градиент», ИП Морозов, режим АУСН):
  - Приложение №2 (5 марта — 3 апреля 2026): 1 200 000 ₽ за месяц (intensive scope: ОРД + DevOps)
  - Текущий рейт: **800 000 ₽/мес ≈ €8K/мес** до июля-августа 2026
  - Роль: Tech Lead / Architect в команде клиента (10 разработчиков, не Кирилла)
  - Q1 2026: 116 задач выполнено (Epic 1 ORD/MediaScout + Epic 6 CI/CD на Yandex Cloud)
  - Стек: Angular 17 + NestJS + Yandex Cloud + GitLab CI + PostgreSQL + S3
- **Runway: 3-4 месяца до cliff в августе 2026, если не найден следующий контракт**

### Реальное состояние Praxisansatz
- Проект **завершён ~апрель 2025** (год назад)
- Нет активного MRR
- Stack устарел (Angular 17 + Flask gevent + GAE), DACH compliance мог измениться
- Существующие инсталляции: статус неизвестен
- **Решение: похоронить как актив, оставить как portfolio piece**

### Реальное позиционирование (расхождение с CV)
- CV на Plan/docs/CV-Developer.pdf: "Front End Developer with 8+ years"
- Реальность: Tech Lead / Solution Architect — на Dream Platform делает backend (NestJS), DevOps (GitLab CI, Yandex Cloud), архитектуру (status machines, idempotency, integration patterns), руководит командой 10
- **CV драматически недопозиционирует. Требуется переписать.**

## Решения

| # | Решение | Обоснование |
|---|---------|-------------|
| 1 | €100K → stretch, **€30-50K — baseline** | Реалистичная цель к Q1 2027 через 2-3 контракта Tech Lead уровня + Lingo + Fractional CTO |
| 2 | Lingo — **единственный SaaS-bet** | Calc остаётся как лид-магнит, Daxi заморожен |
| 3 | Fractional CTO позиционирование **остаётся** | Не отказываемся от текущего нарратива |
| 4 | Praxisansatz — **не реанимировать** | Bandwidth, год простоя, нет conviction, advisor запретил вторую SaaS-ставку |
| 5 | Toptal/Arc — **не сейчас** | Высокий риск срезаться на algo-test без 2-3 нед LeetCode подготовки. Re-evaluate осенью 2026 |
| 6 | Track 0 (новый) — **активные контракты как cash engine** | Dream Platform + поиск 2-го контракта до августа |
| 7 | Поиск 2-го контракта — **микс каналов** | Warm network + LinkedIn inbound + прямой outreach в RU/CIS IT |

## Что меняется в PLAN

- v2 → v3 (дата 2026-04-26, Day 25/365)
- Добавляется Track 0 (Active contracts)
- Track 1 (Praxis) — переводится в "completed portfolio", не активный трек
- Track 3 (SaaS) — сжимается до Lingo
- Финансовая таблица — две колонки baseline / stretch
- Раздел Known Risks — Dream Platform = single point of failure
- CV/LinkedIn refresh — отдельная задача в спринте

## Известный риск №1
**100% дохода = один клиент.** Если Dream Platform контракт не продлится после августа и нет замены — доход падает в ноль. Это P1 риск всего плана.
