<!-- markdownlint-disable MD041 -- главная начинается с HTML-блока «герой» -->
<div class="sg-hero" markdown="1">

# Стайлгайд: документация по разработке ПО

Единый стандарт для всей документации организации: голос и тон, терминология,
типографика, шаблоны документов и процессы работы с документацией в репозитории.

[Начать с принципов](principles.md){ .md-button .md-button--primary }
[Шаблоны документов](documents/readme.md){ .md-button }

</div>

<div class="sg-stats" markdown="1">
<span class="sg-stat">20+ страниц правил</span>
<span class="sg-stat">уровни MUST · SHOULD · MAY</span>
<span class="sg-stat">линтеры и CI</span>
<span class="sg-stat">docs-as-code</span>
</div>

## Куда идти дальше

<div class="sg-cards" markdown="1">

<div class="sg-card" markdown="1">
<p class="sg-card__title"><span class="sg-card__icon"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="9"/><path d="M15.5 8.5l-2 5-5 2 2-5z"/></svg></span>Принципы</p>
<p>Восемь принципов, из которых выводятся все правила руководства.</p>
<p><a href="principles.md">Читать раздел</a></p>
</div>

<div class="sg-card" markdown="1">
<p class="sg-card__title"><span class="sg-card__icon"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M4 20l4-1 10-10a2.1 2.1 0 0 0-3-3L5 16z"/><path d="M13.5 6.5l3 3"/></svg></span>Текст</p>
<p>Голос и тон, терминология, числа, даты и единицы измерения.</p>
<p><a href="text/tone.md">Открыть раздел</a></p>
</div>

<div class="sg-card" markdown="1">
<p class="sg-card__title"><span class="sg-card__icon"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><rect x="4" y="4" width="16" height="16" rx="2.5"/><path d="M4 9.5h16M9.5 9.5V20"/></svg></span>Оформление</p>
<p>Заголовки, списки, типографика, код, ссылки и изображения.</p>
<p><a href="formatting/structure.md">Открыть раздел</a></p>
</div>

<div class="sg-card" markdown="1">
<p class="sg-card__title"><span class="sg-card__icon"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M7 3.5h7l4.5 4.5v12.5H7z"/><path d="M13.5 3.5V8H18M9.8 12.5h5M9.8 15.8h5"/></svg></span>Документы</p>
<p>Шаблоны README, инструкций, справочника API и журнала изменений.</p>
<p><a href="documents/readme.md">Открыть раздел</a></p>
</div>

<div class="sg-card" markdown="1">
<p class="sg-card__title"><span class="sg-card__icon"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><circle cx="7" cy="6" r="2.5"/><circle cx="7" cy="18" r="2.5"/><circle cx="17" cy="12" r="2.5"/><path d="M7 8.5v7M9.5 6h3a2.5 2.5 0 0 1 2.5 2.5v1M9.5 18h3a2.5 2.5 0 0 0 2.5-2.5v-1"/></svg></span>Процессы</p>
<p>Коммиты, ветки, Pull Request и ревью документации.</p>
<p><a href="process/commits.md">Открыть раздел</a></p>
</div>

<div class="sg-card" markdown="1">
<p class="sg-card__title"><span class="sg-card__icon"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M12 6.5C10 4.8 7.3 4.4 4.5 5v13c2.8-.6 5.5-.2 7.5 1.5 2-1.7 4.7-2.1 7.5-1.5V5c-2.8-.6-5.5-.2-7.5 1.5z"/><path d="M12 6.5v13"/></svg></span>Глоссарий</p>
<p>Термины, которые во всей документации пишутся единообразно.</p>
<p><a href="glossary.md">Открыть раздел</a></p>
</div>

</div>

## Для кого это руководство

- **Авторы документации** — инженеры, аналитики, техписатели, разработчики:
  руководство отвечает на вопрос «как написать и оформить».
- **Ревьюеры** — на что смотреть в Pull Request с документацией.
- **Новые сотрудники** — быстрый вход в стандарты команды.

## Статусы правил

Каждое правило помечено уровнем обязательности:

| Уровень | Обозначение | Как трактуется на ревью |
| --- | --- | --- |
| Обязательно | **MUST** | Pull Request не может быть одобрен с нарушением |
| Рекомендуется | **SHOULD** | Нарушение допустимо, если автор обосновал его в PR |
| Допустимо | **MAY** | Свободный выбор автора |

Большинство правил проверяется автоматически линтерами в CI
(markdownlint и cspell), остальные — на ревью.

## Как пользоваться

1. Перед написанием документа прочитайте раздел [Принципы](principles.md)
   и раздел о соответствующем типе документа (например,
   [Инструкции](documents/how-to.md)).
2. При сомнениях в формулировке — [Голос и тон](text/tone.md)
   и [Терминология](text/terminology.md).
3. Перед коммитом — [Коммиты](process/commits.md)
   и [Ветки и Pull Request](process/branches-pr.md).
4. Перед публикацией проверьте чек-лист в разделе о вашем типе документа
   и прогоните линтеры (`npm run lint`).

## Разделы руководства

- [О руководстве](about.md) — область применения, роли, версионирование.
- [Принципы](principles.md) — 8 принципов, на которых строится всё остальное.
- [Текст](text/tone.md) — голос, терминология, числа и даты.
- [Оформление](formatting/structure.md) — структура, типографика, код, ссылки.
- [Документы](documents/readme.md) — шаблоны README, инструкций, API, CHANGELOG.
- [Именование](naming.md) — файлы, папки, репозитории.
- [Процессы](process/commits.md) — коммиты, ветки, PR, ревью.
- [Глоссарий](glossary.md) — термины, используемые в руководстве.

Правило меняется только через Pull Request: см.
[CONTRIBUTING.md](https://github.com/Sophie505-bit/style-guide-project/blob/main/CONTRIBUTING.md).
