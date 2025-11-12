# Экспорты n8n (workflows)

В этой папке хранятся JSON-экспорты сценариев n8n.  
Именование — **пронумеровано и понятно по смыслу**, чтобы поддерживать порядок и версионирование.

## Как экспортировать workflow из n8n
1. Открой нужный workflow в n8n.
2. Клик по названию → **Export** (или **Download**).
3. Сохрани файл в формате JSON.
4. Переименуй по шаблону (см. ниже) и положи в папку `workflows/`.

## Рекомендованные шаблоны имен
- `01_ai_assistant_base.json` — базовый сценарий ассистента
- `02_ai_assistant_with_error_handling.json` — добавлена обработка ошибок
- `03_ai_assistant_with_notion.json` — интеграция с Notion
- `10_experiment_prompt_tuning.json` — эксперименты с промптами

> Нумерация помогает видеть эволюцию сценариев: 01, 02, 03… 10, 11…

## Таблица сценариев
| Файл | Назначение | Примечание |
|------|------------|------------|
| 01_ai_assistant_base.json | Базовая логика: Input → LLM → Output | Начальная версия |
| 02_ai_assistant_with_error_handling.json | Ветвление: успех/ошибка + логирование | Добавлен retry |
| 03_ai_assistant_with_notion.json | Сохранение результата в Notion | Интеграция API |

## Пример минимального JSON (заглушка)
```json
{
  "name": "AI Assistant (placeholder)",
  "nodes": [],
  "connections": {},
  "active": false,
  "settings": {},
  "version": 1
}
