# Record Schema

Все записи — Markdown с YAML front matter.

## Общие поля

```yaml
id: stable-ascii-id
type: location|resource|enemy|boss|equipment|expedition|regional_task|mechanic|update
name_ru: ""
name_en: ""
aliases: []
status: official|verified|community|uncertain|obsolete
game_version: ""
checked_at: YYYY-MM-DD
region: ""
tags: []
sources:
  - id: source-id
    type: official|wiki|community|video|user_screenshot
    url: ""
    checked_at: YYYY-MM-DD
```

## Обязательное содержимое записи

### Для локации
- доступ / условия открытия;
- уровень опасности;
- требуемая защита;
- обязательные инструменты;
- враги;
- боссы;
- особые механики;
- основной и возможный лут;
- что брать;
- что можно не брать;
- дешёвая подтверждённая тактика;
- варианты ежедневных/сюжетных заданий.

### Для ресурса
- где добывается;
- как добывается;
- можно ли произвести;
- рецепт;
- станок;
- альтернативные источники;
- переработка;
- основные применения;
- что изменилось по версиям.

### Для экспедиции
- название цепочки;
- номер уровня;
- рекомендуемая мощь;
- угроза;
- требуемый тип специалиста;
- эффекты позиций;
- подтверждённые составы;
- важные способности;
- ежедневная награда/milestone.

## Неизвестные поля

Не заполнять `?` догадкой. Использовать:
```yaml
value: null
note: "не подтверждено"
```
