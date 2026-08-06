---
name: glowbyte-design
description: Use when creating materials (slides, documents, banners, decks) in the GlowByte brand style — colors, fonts, logo, effects.
---

# GlowByte Design — потребительский скилл

**Версия скилла: 1.0**

Публичный, самообслуживаемый скилл. Не требует токена и доступа к приватным
репозиториям — все данные бренда берутся из публичного манифеста.

## Источник данных

```
https://raw.githubusercontent.com/TerryAirwalker/glowbyte-brandbook/main/manifest.json
```

Скачать/прочитать этот `manifest.json` в начале работы. Не собирать материалы по
памяти — все цвета/шрифты/лого/правила брать из манифеста (см. `entrypoint`/`routing`
в самом манифесте — они описывают, какие разделы читать под какую задачу).

## Брендбук целиком (референс)

```
https://raw.githubusercontent.com/TerryAirwalker/glowbyte-brandbook/main/index.html
```

## Ассеты (логотипы, шрифты)

Реальные бинарные файлы — в публичном репозитории
[glowbyte-brand-assets](https://github.com/TerryAirwalker/glowbyte-brand-assets):

```
https://raw.githubusercontent.com/TerryAirwalker/glowbyte-brand-assets/main/logos/glowbyte-logo-red.svg
https://raw.githubusercontent.com/TerryAirwalker/glowbyte-brand-assets/main/logos/glowbyte-logo-white.svg
https://raw.githubusercontent.com/TerryAirwalker/glowbyte-brand-assets/main/logos/glowbyte-mark.svg
https://raw.githubusercontent.com/TerryAirwalker/glowbyte-brand-assets/main/fonts/Montserrat-Regular.ttf
https://raw.githubusercontent.com/TerryAirwalker/glowbyte-brand-assets/main/fonts/Montserrat-Bold.ttf
https://raw.githubusercontent.com/TerryAirwalker/glowbyte-brand-assets/main/fonts/JetBrainsMono-Regular.ttf
https://raw.githubusercontent.com/TerryAirwalker/glowbyte-brand-assets/main/fonts/JetBrainsMono-Bold.ttf
```

Рыжий логотип — по умолчанию (белый/чёрный фон), белый логотип — для цветного/чёрного
фона (см. `manifest.json` → `colors.forbidden`: рыжий логотип на цветном фоне запрещён).
`glowbyte-mark.svg` — отдельный знак (без слова "lowbyte"), для мест где полный
wordmark не влезает (favicon, мелкий бейдж, аватар); `fill="currentColor"`, перекраска
через CSS `color` — только в пределах фирменной палитры (см. `forbidden`).
Шрифты встраивать в готовые файлы (docx/pptx/pdf), не полагаться на системный Montserrat.

## Перед стартом

См. `manifest.json` → `clarify_before_start` — короткий уточняющий вопрос про язык/
тип материала, если не указан явно.

## Самопроверка перед выдачей

См. `manifest.json` → `self_check_before_delivery.checklist` — пройти обязательно.

## Что этот скилл не делает

Не редактирует брендбук/манифест/движок — это задача приватного авторского скилла
`brandbook-glowbyte`. Этот скилл только использует уже опубликованные данные.
