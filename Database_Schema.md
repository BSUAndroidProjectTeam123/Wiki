# Схема базы данных

База данных используется для хранения истории завершенных партий.

## Визуальная схема

```markdown
erDiagram
    game_history {
        INTEGER id PK "Уникальный ID игры (Автоинкремент)"
        INTEGER timestamp "Время завершения партии (в миллисекундах)"
        INTEGER playerScore "Очки, набранные игроком"
        INTEGER dealerScore "Очки, набранные дилером"
        TEXT result "Результат: Win, Loss или Draw"
    }
```

## SQL-файл
Структура таблиц в формате SQL доступна по ссылке:
[database.sql](database.sql)