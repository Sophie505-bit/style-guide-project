# Стайлгайд: документация по разработке ПО (style-guide-project)

Единый стандарт документации по разработке ПО в организации: правила текста,
оформления, структур документов и процессов работы с документацией.
Сайт собирается генератором **MkDocs** (тема **Material**) и публикуется
автоматически на GitHub Pages.

[![CI](https://github.com/Sophie505-bit/style-guide-project/actions/workflows/ci.yml/badge.svg)](https://github.com/Sophie505-bit/style-guide-project/actions/workflows/ci.yml)
[![Deploy to GitHub Pages](https://github.com/Sophie505-bit/style-guide-project/actions/workflows/deploy.yml/badge.svg)](https://github.com/Sophie505-bit/style-guide-project/actions/workflows/deploy.yml)
[![Site](https://img.shields.io/badge/%D1%81%D0%B0%D0%B9%D1%82-blue)](https://sophie505-bit.github.io/style-guide-project/)

Опубликованная версия: [sophie505-bit.github.io/style-guide-project](https://sophie505-bit.github.io/style-guide-project/).

## Состав репозитория

| Путь | Назначение |
| --- | --- |
| `docs/` | Исходники руководства в Markdown |
| `mkdocs.yml` | Конфигурация сайта, навигация, расширения Markdown |
| `.markdownlint-cli2.jsonc`, `cspell.json` | Настройки линтеров |
| `.github/workflows/` | CI: линтинг, сборка и деплой |
| `CONTRIBUTING.md` | Как предложить изменение |

## Локальная сборка

Требования: Python 3.12+, Node.js 20+.

```bash
# 1. Python-зависимости и локальный сервер
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt
mkdocs serve                     # сайт: http://127.0.0.1:8000

# 2. Линтеры (во втором терминале)
npm install
npm run lint                     # markdownlint + cspell
```

Сборка «как в CI»:

```bash
mkdocs build --strict
```

## Состав документации

- **Текст** — голос и тон, терминология, числа и даты.
- **Оформление** — структура, типографика, код, ссылки и изображения.
- **Документы** — шаблоны README, инструкций, справочника API, CHANGELOG.
- **Именование** — файлы, папки, репозитории.
- **Процессы** — коммиты, ветки и Pull Request, ревью.

## Как внести вклад

Инструкция для авторов: [CONTRIBUTING.md](CONTRIBUTING.md).

## Лицензия

[MIT](LICENSE).
