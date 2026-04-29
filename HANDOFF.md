# Handoff — 28.04.2026 вечер → 29.04.2026 утро

## Где остановились

День 27/365. Вторник вечер. Спринт 26.04—3.05, Phase 0 — Фундамент.

### Что сделано сегодня (28.04)

- **Dream Platform: большой блок** — Teams Management (admin привязка к командам, изоляция данных team-to-team по tasks/videos/brands/companies, in-platform calls и team-level workflow controls). Multi-tenant.
- **Outreach:** написано 3 контактам с бизнес-встречи в Паралимни (24.04). Простой английский, без идиом. Ответов пока нет (норма для +5 дней с момента знакомства, ждём до пятницы).
- **System Design:** прочитана статья Greiner "CAP Theorem Revisited" — переход от классического CAP к PACELC.
- **CV переписан** под Tech Lead / Solution Architect (см. `docs/CV-TechLead.md`). Сгенерированы DOCX и HTML с CSS-стилем, готовы к печати в PDF.
- **CV обновлён вечером:** Dream Platform теперь = "Architect of two end-to-end subsystems" — добавлен блок про team workspace platform с формулировкой "access enforced at the data boundary, not at the UI" (сильный архитекторский сигнал).
- **LinkedIn:** добавлен morozco.tech в Contact Info.
- **Уборка репо:** 57MB → 2.7MB. Удалены Notion-скрипты, Playwright-снапшоты, дубли лендинг-картинок. Архивированы LINKEDIN_UPDATE.md, outreach_list.md, outreach_sent_2026-04-07.md в `decision_log/archive/`. Запушено в origin/main (commit 8ac6c40).
- **Создан README.md** — entry point с индексом ключевых файлов и ссылкой на System Design Primer на GitHub.
- **Память обновлена:** feedback_human_writing.md расширен 11 новыми non-native idiom-replacement правилами после рефакторинга outreach DM.
- **Память обновлена:** project_dream_platform.md — engagement начался лето 2025 (LinkedIn разбит на 2 entry для одного проекта), формальный контракт от 5 марта 2026.
- **Память обновлена:** project_praxis_absatz.md — end date Dec 2025 (не Apr 2025).

### Решения дня
- LinkedIn ≠ CV ≠ memory: разные витрины, разные даты, разные аудитории. CV синхронизирован с LinkedIn-датами.
- Outreach DM-стиль: простой не-носительский английский, никаких идиом. Применяется ко ВСЕМ дальнейшим текстам.

## С чего начать завтра

### Среда 29.04
1. **Dream Platform: текущая нагрузка** (8ч)
2. **Warm network audit** — список 20+ контактов, кто потенциально может вывести на Tech Lead контракт. БЕЗ сообщений сегодня, только список.
3. **LinkedIn drift fix (5 минут):** добавить буллет про team workspace platform в Dream Platform Experience entry на LinkedIn — синхронизировать с CV.
4. **System Design (если будет окно, 30-40 мин):** Consistency patterns + Availability patterns в Primer — естественное продолжение после CAP.

### Четверг 30.04
- LinkedIn пост #4 (Dream Platform case study, без NDA-конкретики) — был перенесён со вторника
- System Design: CAP theorem deep-dive + Consistency patterns (1.5ч)

### Пт 01.05 — ретро недели + план следующего спринта
- **Ключевое решение пятницы:** кому из warm network написать на след. неделе по 2-му контракту (3-5 имён)

## Uncommitted изменения
- `M PLAN.md` — обновлён прогресс 27.04 + 28.04
- `?? decision_log/2026-04-26-real-cash-picture.md` — существует, не добавлен в git
- `?? interview_prep_architect.md` — существует, не добавлен в git
- `docs/CV-TechLead.md`, `CV-TechLead.docx`, `CV-TechLead.html`, `cv-style.css` — все в `docs/`, gitignored по политике (sensitive)

## Открытые блокеры
- **2-й контракт:** канал поиска не активирован. Warm network audit = первый шаг (29.04).
- **Outreach Параlimni-3:** ждём ответа до пятницы 01.05, иначе move on.
- **Dream Platform контракт до июля-августа 2026:** обсуждение продления нужно начать в июне, не в июле.

## Метрики на сейчас
- Cash run-rate: €8K/мес (Dream Platform)
- Runway без замены: 3-4 месяца до cliff
- Цель baseline: €30-50K/мес к апр 2027
- Цель stretch: $100K/мес к апр 2027
