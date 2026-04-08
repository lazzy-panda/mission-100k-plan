# 2026-04-08 · Lingo Tier 1 wedge = Greek for Russian-speaking Cyprus expats

**Status:** decided.
**Phase:** 0 (день 7/365).
**Связанный документ:** `saas_idea_1.md`

## Context

SaaS Track 2 (стелс EdTech продукт) до сегодняшнего дня существовал
как «приложение для греческого, которое потом станет платформой». Код
в `~/Documents/greek-app` — форк sanidhyy/duolingo-clone, расширен
11 exercise modes + spaced repetition + vocabulary tracking. Технически
MVP на 60% готов. Но стратегического документа не было.

Сегодня на вопрос «с чего начинать коммерчески» я мог либо продолжать
строить engine абстрактно, либо зафиксировать wedge и строить под него.

## Options considered

1. **Multi-language с первого дня.** Запустить Lingo сразу на 5
   языках (греческий, испанский, итальянский, немецкий, английский),
   чтобы максимизировать адресуемый рынок. **Отклонено:** нет
   content-team, нет native-reviewers, размазывает усилие solo
   founder'а. Классическая ошибка "платформа без первого юзера".

2. **English-UI Greek product.** Запустить на английском UI, целиться
   в глобальных expats на Кипре + greek diaspora + туристов. **Отклонено:**
   разводит wedge, теряет преимущество плотной русскоязычной тусовки
   в Лимассоле/Пафосе/Никосии. Глобальная аудитория = paid ads с
   первого дня, которого я не хочу.

3. **B2B продажа школам греческого.** Лицензировать engine языковым
   школам как white-label. **Отклонено:** неправильный motion для
   solo founder (длинный sales-цикл, энтерпрайз-закупка, медленная
   обратная связь).

4. **Английский как язык изучения (а не греческий).** Крупнейший
   рынок, проще acquisition. **Отклонено:** переполненный рынок
   (Duolingo, Busuu, Cambly, Preply, Italki, etc.), нет personal
   market access, нет дифференциатора, я не native English.

5. **✅ Выбрано: Lingo для русскоязычных экспатов на Кипре, учащих
   греческий. Tier 1 wedge.** Затем Tier 2 (мультиязычный движок,
   с июля 2026) → Tier 3 ("Leetcode for skills", с апреля 2027).

## Why

1. **Personal market access.** Я сам живу на Кипре. Я сам в
   аудитории. Я знаю боль как юзер, не как аналитик.
2. **Dogfood loop.** Я первый и самый жесткий QA. Не нужно
   организовывать discovery, чтобы понять, что сломано.
3. **Плотная community.** Русскоязычные в Лимассоле знают друг
   друга. Word-of-mouth работает. 100 платящих за 3 месяца =
   реалистично без paid ads.
4. **Код уже есть на 60%.** Engine собран, 11 exercise modes
   работают, spaced repetition реализован, Clerk + Stripe
   scaffolding готов. Time-to-Tier-1-launch = недели, не месяцы.
5. **Тиль-логика «last mover advantage».** Lingo занимает
   маленькую нишу (structured self-paced Greek для adults в
   конкретной гео-языковой связке), где нет прямых конкурентов.
   Duolingo — инфантильный, Busuu — без глубины по греческому,
   Italki — не self-paced, Anki — без структуры. Дыра реальная.

## Trade-offs accepted

- **Потолок по TAM.** Русскоязычных экспатов на Кипре, учащих
  греческий, — тысячи, не сотни тысяч. Это wedge, не endgame.
  Tier 2 и Tier 3 обязательны для >$10K MRR.
- **Content-moat не решён.** Один я не напишу curriculum до B2.
  Нужен либо native tutor на контракте, либо UGC с ревью. Решение
  откладывается до конца апреля после 5 discovery звонков.
- **Риск Tier 3 platform leak.** Если греко-специфика (ударения,
  озвучка, спряжения) протечёт в каждый слой, Tier 2/3 станут
  rewrite. Mitigation: с первого дня Tier 2 проводить refactor
  review.

## Hard kill criterion

**Если к 30.06.2026 не набрано 10 платящих пользователей — Lingo
становится side-project, Fractional CTO выходит на Track 1
полностью.** Эта планка зафиксирована до того, как эмоции смогут
её пересмотреть. Ретро по метрике 30.06.2026 в конце Phase 1.

## Follow-ups

- **Чт 09.04:** landing-черновик на одну страницу.
- **Пт 10.04:** решение по домену (lingo.app vs greek-cy.com vs
  другой).
- **Вс 12.04:** первые 3 discovery звонка забукированы через
  Telegram-чаты Лимассол.
- **Конец апреля:** решение по контент-moat (native tutor contract
  / UGC / hybrid).
- **30.04.2026:** month-end ретро, конец Phase 0. Проверить, что
  waitlist набирает ≥25 записей.

## Revisit

- **30.06.2026** — hard checkpoint по kill criterion.
- **Каждое month-end ретро** — проверять, что wedge не «расползся»
  обратно в multi-language fantasy.
