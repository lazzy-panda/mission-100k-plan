# Interview Prep — Senior/Lead/Solution Architect

> Универсальная карта подготовки к ролям Senior/Lead/Solution Architect в финтехе, SaaS или продуктовой компании.
> Добавлено: 16.04.2026

---

## Блок 1. System Design — главный пробел

Основа всех архитекторских интервью.

### Что учить
- **Building blocks:** load balancer, CDN, cache (Redis), message queue (Kafka/RabbitMQ), БД (SQL vs NoSQL), API Gateway, BFF
- **Trade-offs:** consistency vs availability (CAP), latency vs throughput, monolith vs microservices
- **Паттерны:** rate limiting, circuit breaker, retry с backoff, idempotency, eventual consistency
- **Оценки "на салфетке":** сколько RPS выдержит сервер, сколько места займут 1M пользователей

### Ресурсы
1. **System Design Primer** на GitHub — бесплатно, 300k+ звёзд, есть перевод на русский. Начать отсюда.
2. **ByteByteGo (Alex Xu)** — YouTube + книга "System Design Interview Vol.1 и Vol.2". Золотой стандарт.
3. **Hello Interview** — бесплатные разборы популярных задач (Design Twitter, Design Uber и т.д.) с видео.
4. **DesignGurus "Grokking the System Design Interview"** — платный курс (~$40), системный.

### Как учить
Не читать подряд. Брать одну задачу ("Design URL shortener", "Design Instagram") и проходить по шагам: требования → оценки → high-level design → детали → trade-offs. 2-3 задачи в неделю, всего ~15.

---

## Блок 2. Backend архитектура

### Что учить
- REST vs GraphQL vs gRPC — когда что
- Базы данных глубже: индексы, transactions, ACID, шардинг, репликация, SQL vs NoSQL
- Кеширование: где ставить, стратегии инвалидации (cache-aside, write-through)
- Очереди и event-driven: синхронно vs асинхронно, паттерн saga
- Авторизация: OAuth 2.0, JWT, refresh tokens
- Observability: логи, метрики, трейсинг (Prometheus + Grafana + Jaeger)

### Ресурсы
1. **"Designing Data-Intensive Applications"** Мартина Клеппманна — главная книга по бэкенд-архитектуре. Прочитать = быть сильнее 80% "синьоров".
2. **"Fundamentals of Software Architecture"** Марк Ричардс — архитектурные стили, trade-offs, работа архитектора.
3. **Arjan Codes** и **ByteByteGo** на YouTube — короткие ролики по конкретным темам.

---

## Блок 3. Финтех/платежи (доменная специфика)

### Что учить
- PCI DSS — 4 уровня compliance, что значит для разработчика
- Эквайринг: merchant → acquirer → card scheme → issuer
- 3D Secure, tokenization карт
- Идемпотентность платежей (почему нельзя дважды списать)
- SCA (Strong Customer Authentication), PSD2

### Ресурсы
1. **Stripe Docs** — лучшая документация в индустрии. Разделы Payments: идемпотентность, 3DS, PCI.
2. **PCI Security Standards** — PCI DSS Quick Reference Guide, PDF ~40 страниц.
3. **Блоги Adyen, Checkout.com** — разборы реальных архитектурных кейсов.

> На интервью достаточно показать принципы: "карту не логируем, CVV не храним, ввод через iframe провайдера".

---

## Блок 4. AI / LLM / Agentic systems — сильная сторона

Уже впереди многих кандидатов благодаря CCA-F и опыту с Claude Code. Нужно упаковать в "архитекторский" язык.

### Что подтянуть
- Паттерны интеграции с LLM: structured output (JSON schema), function calling, tool use
- RAG (Retrieval-Augmented Generation) — когда и как
- Надёжность: hallucination detection, validation outputs, fallback стратегии
- MCP — архитектура протокола, когда делать свой MCP-сервер
- Agent orchestration: single agent vs multi-agent (LangGraph, CrewAI)
- Оценка качества LLM-систем: evals, A/B тестирование промптов

### Ресурсы
1. **Anthropic Courses** — бесплатные, "Prompt Engineering Interactive Tutorial" и "Tool Use"
2. **Anthropic Cookbook** — практические паттерны
3. **"Building Effective Agents"** — блог Anthropic, канонический текст про агентные паттерны
4. **MCP спецификация** — официальная документация протокола
5. **Simon Willison's Weblog** — лучший агрегатор по LLM-индустрии

---

## Блок 5. Поведенческие вопросы и коммуникация

40% интервью — про работу с командой, принятие решений, обоснование.

### Что готовить
4-5 историй по формуле STAR (Situation-Task-Action-Result):
- [ ] Сложное техническое решение
- [ ] Конфликт с командой или PM
- [ ] Продакшен-инцидент
- [ ] Менторинг джуна
- [ ] Убеждение стейкхолдеров

> Истории должны быть с цифрами: "ускорили на 40%", "сократили баги на 60%".
> Материал уже есть: UGC-платформа, CreatorFlow, опыт техлида.

### Ресурсы
- **"Cracking the PM Interview"** — раздел про behavioral универсален
- **Exponent** на YouTube — бесплатные моки

---

## Практический план

### Полный (6 недель)

| Неделя | Фокус |
|--------|-------|
| 1-2 | System Design Primer (целиком) + 2 задачи на дизайн с Hello Interview |
| 3-4 | Первые 4 главы "Designing Data-Intensive Applications" + 2 задачи System Design |
| 5 | Stripe Docs + PCI Quick Reference — закрыть финтех за неделю |
| 6 | Anthropic Courses + паттерны агентов (быстро, база есть) |

**Параллельно:** раз в 3-4 дня мок-интервью (Pramp / Exponent бесплатно).
**За неделю до интервью:** STAR-истории, чистка резюме/LinkedIn под роль.

### Минимум (2 недели)

- [ ] System Design Primer (разделы: load balancing, кеши, БД, microservices)
- [ ] ByteByteGo на YouTube — 10 ключевых роликов
- [ ] Anthropic Courses — 2 вечера
- [ ] 5 STAR-историй из своего опыта
- [ ] 3-4 мок-интервью
