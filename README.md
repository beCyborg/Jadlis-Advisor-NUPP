# Jadlis Advisor — NUPP

Интерактивный project advisor на основе мета-системы **NUPP** (Nearly Universal Principles of Projects) — 6 почти универсальных принципов, лежащих в основе PRINCE2, PMBOK, P3.express, DSDM, Scrum и XP.

## Что делает

Диагностирует любую проектную ситуацию через 6 NUP-линз одновременно:

- **NUP1 — Affiliations**: Методология как инструмент, а не как идентичность. Method tribalism, Agile vs Waterfall
- **NUP2 — Energy**: Оптимизация энергии и ресурсов. Decision fatigue, 80/20, sustainable pace
- **NUP3 — Proactivity**: Проактивность вместо реактивности. 3 уровня планирования, risk management
- **NUP4 — Weakest Link**: Холистический взгляд на все домены проекта. Cherry picking vs tailoring
- **NUP5 — Purpose**: Ясная цель для каждого действия. Parallel worlds test, elevator mirror
- **NUP6 — Repeatability**: Повторяемые элементы вместо ad hoc. Чеклисты, workflows, циклы

## Как работает

1. Собирает контекст: тип проекта, методология, роль, стадия, проблема
2. Запускает **NUP Scan** — применяет все 6 принципов одновременно как диагностические линзы
3. Оценивает каждый NUP: Green / Yellow / Red
4. Приоритизирует Red-сигналы по влиянию на проект
5. Даёт рекомендации с привязкой к конкретной методологии и контексту

## Установка

```bash
claude plugin install jadlis-advisor-nupp@jadlis-advisors
```

Или локально:

```bash
claude --plugin-dir "/path/to/Jadlis-Advisor-NUPP"
```

## Использование

Advisor доступен **только по явному вызову**:

```
/jadlis-advisor-nupp:advisor
```

Примеры запросов:
- "Проект буксует, не могу понять почему"
- "Какую методологию выбрать для нового проекта?"
- "Мы используем Scrum, но он не работает"
- "Команда выгорает, конфликты, низкая мотивация"
- "Зачем нам этот процесс? Это бюрократия"
- "Как адаптировать PRINCE2 для нашего проекта?"

## Структура

```
├── .claude-plugin/
│   └── plugin.json
├── skills/
│   └── advisor/
│       ├── SKILL.md                       # NUP Scan + навигация
│       └── references/
│           ├── nup1-affiliations.md       # Результаты > аффилиации
│           ├── nup2-energy.md             # Энергия и ресурсы
│           ├── nup3-proactivity.md        # Проактивность
│           ├── nup4-weakest-link.md       # Слабое звено
│           ├── nup5-purpose.md            # Ясная цель
│           └── nup6-repeatability.md      # Повторяемые элементы
└── README.md
```

## Источник

NUPP — Nearly Universal Principles of Projects (nupp.guide), Nader K. Rad, 2025.
Лицензия: Creative Commons Attribution 4.0 International.
