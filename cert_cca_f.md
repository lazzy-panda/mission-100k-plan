# CCA-F — Claude Certified Architect (Foundations)

> Зафиксировано 08.04.2026, день 7/365. Fixed 08.04 evening: правильное название — **Architect**, не Associate. Домен — **claude.com**, не claude.ai.
> Цель: получить официальный CCA-F бейдж от Anthropic за ≤6 недель, повесить на LinkedIn.
> **Факты про экзамен** (verified 08.04.2026 из anthropic.com/news/claude-partner-network):
> - 60 scenario-based MCQs, 120 минут
> - Passing score: **720/1000** (на practice целимся 900+)
> - Стоимость: **$99** или **$0** для первых 5000 partner employees
> - Certification exclusive to employees of Anthropic partner companies — Partner Network вступление обязательно
> Зачем: **credibility layer для Fractional CTO позиционирования.** Бейдж сейчас есть у считанных сотен людей в мире — редкий signal для founders при оценке.
> Связь с Mission $100K: Phase 0 → конец Phase 1. Landing ~20.05.2026 (через 6 недель от сегодня).

---

## Стартовый уровень (08.04.2026)

### Что уже есть (пропускаем / ускоряем)
- Claude Code ежедневно через WebStorm ✅
- Technical Architect опыт, системный дизайн ✅
- 7 лет фронтенд → API-интеграции, OAuth, webhooks, rate limits ✅
- Prompt engineering на практике — 6+ месяцев агентных пайплайнов ✅
- **Неделя 1 курсов пройдена:** Claude 101 + AI Fluency ✅

### Что нужно добить
- **MCP (Model Context Protocol)** — серверы, клиенты, три примитива (tools, resources, prompts)
- **Agentic Architecture** — multi-agent orchestration, hub-and-spoke, coordinator-subagent паттерны
- **Claude Code в CI/CD** — флаг `-p`, CLAUDE.md иерархии, skills frontmatter
- **Structured Output** — JSON schema validation, error recovery
- **Anti-patterns** — 7 ключевых ошибок, которые являются ловушками на экзамене

---

## Веса доменов на экзамене

| Домен | Вес | Статус у меня |
|-------|-----|---------------|
| D1 — Agentic Architecture | 27% | ⚠️ добить hub-and-spoke, coordinator-subagent |
| D2 — MCP | 18% | ❌ с нуля — главный пробел |
| D3 — Claude Code | 20% | 🟡 опыт есть, но спец-флаги и frontmatter — добить |
| D4 — Prompt Engineering & Structured Output | 20% | 🟡 structured output + schema validation — добить |
| D5 — Ethics / AI Fluency | 15% | ✅ Claude 101 + AI Fluency пройдены |

---

## 6-недельный план (ускоренный, не 12 — стартую не с нуля)

### ✅ Неделя 1: Фундамент + регистрация — ПРОЙДЕНО

- [x] Claude 101 (~1.5h)
- [x] AI Fluency: Frameworks & Foundations

**Затрачено:** ~4 часа

---

### 🟡 Неделя 2–3 (дни 8–21, Чт 09.04 – Ср 22.04): API и ядро экзамена

**Курс:** Building Applications with the Claude API (~8h)

Флагман. Покрывает 60% экзамена. System prompts, tool use, context windows, architecture patterns, production application design. Фокус для меня: **structured output и tool definitions** (D4 = 20% + D1 = 27%).

**План:**
- Ср 08.04 (сегодня): старт, 1 час вечером
- Чт 09.04 – Пт 10.04: 3 часа
- Выходные 11–12.04: 2 часа
- Пн 13.04 – Ср 15.04: 2 часа финиш

**Deliverable:** сертификат + заметки в `cert_cca_f_notes.md` (создать по ходу).

**Затрачено:** 0/8 часов

---

### ❌ Неделя 3–4 (дни 16–28, Чт 16.04 – Вт 28.04): MCP (D2 = 18%)

**Курсы:**
- Introduction to MCP
- MCP Advanced

С нуля на Python. Три примитива: tools, resources, prompts. Подключение Claude к внешним сервисам.

**Практика:** создать MCP-сервер для Lingo. Два полезных output'а:
1. Реальный практический опыт для экзамена (проверяют production experience)
2. Tool для собственной работы над SaaS Track 2 (например: `lingo-mcp` — exercise generation, vocabulary lookup, content ingestion)

**Затрачено:** 0/6 часов

---

### ❌ Неделя 4–5 (дни 22–35, Ср 22.04 – Вт 05.05): Claude Code + Agentic Architecture

**Курсы:**
- Claude Code in Action (~1 час, 21 урок)
- Sub-agents in Claude Code (новый курс)
- Skills in Claude Code

**Критично запомнить наизусть:**

- `.mcp.json` = **project-level**, коммитится через VCS
- `~/.claude.json` = **user-level**, персональный конфиг
- **Флаг `-p`** = неинтерактивный режим для CI/CD. Без него CI-задачи зависают бесконечно. Прямой exam вопрос.
- **CLAUDE.md иерархии**: project vs user
- **Skills frontmatter**: `context: fork` для изолированных подагентов

**Правило-ловушка:** если новый член команды не получает инструкции — конфиг всегда на user-level вместо project-level. Классическая ошибка.

**Затрачено:** 0/6 часов

---

### ❌ Неделя 5–6 (дни 36–42, Ср 13.05 – Вт 19.05): Practice Exam + Anti-patterns

**Действия:**
1. Скачать Official Exam Guide PDF из Skilljar
2. Пройти Official Practice Exam (60 вопросов, тот же формат)
3. Целиться на **>900/1000** на практике

**6 сценариев экзамена (на экзамене выпадут 4 из 6 случайным образом):**
1. Customer Support Resolution Agent
2. Code Generation with Claude Code
3. Multi-Agent Research System
4. Developer Productivity with Claude
5. Claude Code for CI/CD
6. Structured Data Extraction

**Главное правило**: многие неправильные ответы — не случайные, а архитектурные анти-паттерны. Знание того, что НЕ делать, — половина экзамена.

**Затрачено:** 0/6 часов

---

### 🎯 Неделя 6 (день ~42, ~20.05.2026): САМ ЭКЗАМЕН

- Заблокировать 2.5 часа в календаре без отвлечений
- Экзамен $99 (или $0 если в первых 5000 партнёров)
- После сдачи: обновить LinkedIn headline + добавить в Experience карточку Founder

---

## Total

| Неделя | Фокус | Часов | Статус |
|--------|-------|-------|--------|
| 1 | Claude 101 + AI Fluency | 4 | ✅ done |
| 2–3 | Building with Claude API | 8 | 🟡 старт 08.04 |
| 3–4 | MCP Intro + Advanced | 6 | ❌ |
| 4–5 | Claude Code + Agents + Skills | 6 | ❌ |
| 5–6 | Practice Exam + Anti-patterns | 6 | ❌ |
| **Остаток** | | **26** | |

**Затрачено на сегодня:** 4/30 часов. **Осталось:** 26 часов за 6 недель ≈ 4.3 часа в неделю.

---

## Чеклист перед экзаменом

- [ ] Все 5 ключевых курсов пройдены с сертификатами
- [ ] Practice exam score **900+/1000**
- [ ] 6 сценариев — знаю паттерны решений для каждого
- [ ] 7 анти-паттернов — помню наизусть
- [ ] MCP — могу написать сервер с нуля (не глядя в доки)
- [ ] Claude Code CI/CD — флаги `-p`, конфиги project vs user, CLAUDE.md иерархии
- [ ] 2.5 часа заблокированы в календаре без отвлечений
- [ ] $99 оплачены (или $0 если в первых 5000 партнёров)

---

## Что делает Кирилл вручную (не могу сделать за тебя)

### Срочно — окно $0 экзамена закрывается (первые 5000 партнёров)

**Блокер обнаружен 08.04 вечер:** Partner Network форма не принимает gmail/outlook/yahoo. Нужен business email на custom domain.

**Решение:** купить личный домен `morozco.tech` + настроить Cloudflare Email Routing (free forever).

- [x] **Шаг 0: Купить домен `morozco.tech`.** ✅ 09.04.2026 через Cloudflare Registrar.
- [x] **Шаг 0.5: Настроить Cloudflare Email Routing.** ✅ 09.04.2026, `kirill@morozco.tech` → gmail.
- [x] **Шаг 0.75: Deploy landing на `morozco.tech`.** ✅ 09.04.2026 — Cloudflare Pages (`morozco-tech` project), Three.js scene с tech-логотипами + 3D Morozco mark, CNAME @ / www → `morozco-tech.pages.dev` (proxied), SSL active. Исходник в `morozco-tech-landing/index.html`.
- [x] **Шаг 1: Apply to Claude Partner Network.** ✅ Подана 09.04.2026 через https://partnerportal.anthropic.com/s/partner-registration. Статус на 10.04: "review in progress", ждём email с activation link. Email: `kirill@morozco.tech`.

**Что писать в форме:**
- Company name: `Kirill Morozov — Fractional CTO Services` (или финальный бренд, если решим иначе)
- Business email: `kirill@morozco.tech`
- Website: `https://morozco.tech` (с coming-soon страницей)
- Country: `Cyprus`
- Use case: Fractional CTO для founders building AI-native products on Claude Code. Own stealth EdTech product in development, bringing Claude to customers through architecture consulting + direct product implementation.

- [ ] **Шаг 2: Request exam access** через https://anthropic.skilljar.com/claude-certified-architect-foundations-access-request — сделать сразу после approval партнёрства.

### Позже (неделя 5–6)

- [ ] Скачать Official Exam Guide PDF из Skilljar после получения access
- [ ] Забронировать слот экзамена на ~20.05.2026 (день 48). Заблокировать 2.5 часа в календаре без отвлечений.
- [ ] Оплатить $99 (или $0 если успел в первые 5000 партнёров)

### После сдачи

- [ ] Обновить LinkedIn headline и Experience → добавить "Claude Certified Architect (Foundations)" (могу сделать через Playwright когда скажешь)
- [ ] Добавить бейдж в профиль LinkedIn (image badge от Anthropic)

---

## Параллельные выгоды (не только бейдж)

1. **MCP-сервер для Lingo** — практическое задание недели 3-4 напрямую полезно для SaaS Track 2. Убиваем двух зайцев: экзамен + рабочий tool.
2. **Glossary + anti-patterns заметки** — пригодятся для LinkedIn постов. Можно вытащить 2-3 TIL поста из материала (Post #8 MCP уже есть в контент-ките, но можно углубить).
3. **Claude Code SOP hardening** — неделя 4-5 про CLAUDE.md иерархии и skills frontmatter напрямую улучшает мой текущий agentic runtime.

---

## Revisit

- **Конец каждой недели (воскресенье):** в retro блоке `PLAN.md` сверять progress по этому файлу. Отмечать часы, ставить ✅ на пройденные курсы.
- **20.05.2026:** экзамен. После — добавить бейдж в LinkedIn профиль через Playwright, закрыть этот файл ✅.
- **Если к 15.05 не готов** — отложить экзамен на 27.05, без эмоций. Лучше сдать с первого раза чем плохо.
