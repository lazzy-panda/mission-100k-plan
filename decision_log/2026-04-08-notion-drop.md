# 2026-04-08 · Drop Notion, move tracking to files + GitHub

**Status:** decided and executed same day.
**Phase:** 0 (день 7/365).

## Context

С начала плана (02.04.2026) трекинг 365-дневного плана жил в Notion:
workspace «План», база `📅 План 365` на 365 строк, дашборд, чекбоксы,
API-интеграция, hardcoded token в 12 JS-файлах.

За первые 7 дней отмечено 0 из 365 дней. Не потому что ничего не
сделано (LinkedIn профиль переделан, 10 cold connects отправлены, 5
warming комментов, pitch + DM-шаблоны, контент-кит v2 полностью на
английском, SaaS идея №1 зафиксирована). А потому что Notion —
внешний слой поверх работы. Открыть Notion, найти день, поставить
галочку — это отдельный ритуал, которого я не делаю.

## Options considered

1. **Оставить Notion, попробовать харднее.** Завести напоминания,
   виджеты, интеграции. Отклонено: уже пробовал неделю, поведенческий
   паттерн не меняется. Проблема не в мотивации, а в том, что трекер
   живёт вне инструмента, в котором идёт работа.

2. **Сторонний tracker (Linear, Height, TickTick).** Отклонено: тот
   же архитектурный недостаток — ещё один внешний слой. Плюс платная
   подписка за функции, которые мне не нужны.

3. **Файлы + git в monorepo рабочего проекта.** Отклонено: план не
   принадлежит ни одному конкретному проекту (Lingo, LinkedIn,
   обучение). Это cross-cutting слой. Нужна отдельная директория.

4. **✅ Выбрано: dedicated file-based workspace в
   `/Users/kirill/MyApps/Plan/`, single source of truth = `PLAN.md`,
   синхронизация через диалог с Claude Code.** Мобильный доступ через
   GitHub private repo + Working Copy на iOS.

## Why

1. **Инструмент встроен в работу.** Я и так сижу в Claude Code каждый
   день. `PLAN.md` открыт, Claude читает и пишет статус по ходу
   разговора. Нет отдельного шага «пойти и отметить».
2. **Plain text выживает всех SaaS.** Markdown читается через 10 лет
   без зависимостей. Notion workspace — нет.
3. **Git = бесплатный audit trail.** Каждый коммит = снимок состояния
   плана. История без дополнительных инструментов.
4. **Мобильный доступ решён.** Working Copy на iOS рендерит markdown
   нативно, не хуже Notion-мобайла. Плюс git-diff с телефона.
5. **Zero cost.** GitHub private repo бесплатный, Working Copy один
   раз ~€20.

## Trade-offs accepted

- **Нет визуального дашборда.** Notion-стайл progress-bars и
  database-views недоступны. Компенсация: sprint-таблица в markdown
  и end-of-week retro. Визуал — nice to have, не критично.
- **Collaboration сложнее.** Если появится team member — git-based
  workflow требует onboarding. Компенсация: пока команда = я + агенты,
  это non-issue. Пересмотр при найме первого человека.
- **Mobile edit UX хуже.** Working Copy редактирует markdown, но не
  так удобно как Notion-клиент. Компенсация: 99% edits идут через
  Claude на ноутбуке. Мобайл только read-mostly.

## Consequences and follow-ups

- Notion workspace оставлен dormant, не удалён (safety net на
  первый месяц). Удалить 08.05.2026 если file-based workflow
  подтвердится.
- 12 JS-файлов с hardcoded Notion token добавлены в `.gitignore`
  (паттерны `notion_*.js`, `build_notion.js`, `rebuild.js`, `update_books.js`).
- **TODO manual:** отозвать Notion integration token на
  https://www.notion.so/my-integrations. Токен никогда не попадал в
  git history (первый коммит уже исключает эти файлы), но ротация
  остаётся best practice.
- `PLAN.md` раздел 5 «Как сверяемся» переписан под file-based поток.
- `project_mission50k.md` в auto-memory обновлён.

## Revisit

- **30.04.2026** — конец Phase 0. Проверить: используется ли
  `PLAN.md` ежедневно? Если <20 ежедневных обновлений за месяц —
  значит и этот workflow не сработал, нужна ревизия.
- **08.05.2026** — удалить dormant Notion workspace если нет
  возвратов.
