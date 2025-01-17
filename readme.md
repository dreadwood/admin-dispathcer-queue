# Admin dispathcer queuet

**Опубликованная версия доступна [тут](https://dreadwood-rx2go-admin-dq.netlify.app/)**

## Описание

Сборка верстки осуществляеться с помощью [Gulp](https://gulpjs.com). Разметка страниц находится в  `src/pug/pages`, шаблонизатор [Pug.js](https://pugjs.org), стили написаны с использованием [SCSS](https://sass-lang.com/), все векторные изображения собираются в единый спрайт `dist/img/sprite.svg` и вызываются в разметке:

```html
<svg width="100" height="100">
  <use xlink:href="img/sprite.svg#{icon-filename}"></use>
</svg>
```

## Команды

- `pnpm i` — установить зависимости
- `build` — собрать проект
- `dev` — запустить режим разработки live server и с отслеживанием изменений в папке `src/`
- `stylelint` — проверить стили в соответсвии со стайл-гайдом
- `stylelint:fix` — ручное исправление стилей в соответсвии со стайл-гайдом (где это возможно)

## Директории

- `dist` — папка со сборкой проекта
- `src` — исходники проекта

## Разработка

- установить [Node.js](https://nodejs.org/en)
- выполнить команду `pnpm i`
- запустить режим разработки `pnpm run dev`
