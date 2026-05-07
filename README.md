# Phone Catalogue

Вебзастосунок каталогу телефонів, планшетів та аксесуарів на `React + TypeScript`.
Проєкт містить список товарів, фільтрацію та сортування, сторінку деталей товару, кошик і обране.

## Можливості

- Перегляд каталогу за категоріями: телефони, планшети, аксесуари.
- Сортування товарів (`Newest`, `Alphabetically`, `Cheapest`).
- Пагінація та вибір кількості елементів на сторінці.
- Сторінка деталей товару з вибором характеристик.
- Додавання товарів в обране та кошик (збереження в `localStorage`).
- Адаптивний інтерфейс з мобільним меню (`BurgerMenu`).

## Технології

- `React 18`
- `TypeScript`
- `React Router`
- `SCSS`
- `Vite` (через `@mate-academy/scripts`)
- `ESLint`, `Prettier`, `Stylelint`

## Запуск локально

### 1) Встановити залежності

```bash
npm install
```

### 2) Запустити застосунок

```bash
npm start
```

Після запуску застосунок буде доступний за локальною адресою (URL виводиться в терміналі).

## NPM-скрипти

- `npm start` - запуск dev-сервера.
- `npm run build` - production-збірка.
- `npm run lint` - форматування і перевірка JS/TS + SCSS.
- `npm run lint-js` - перевірка JavaScript/TypeScript.
- `npm run lint-css` - перевірка стилів.
- `npm run format` - форматування `ts/tsx` через Prettier.
- `npm run deploy` - деплой на GitHub Pages.

## Структура проєкту

- `src/modules` - сторінки та великі UI-модулі.
- `src/shared` - спільні перевикористовувані компоненти.
- `src/Context` - глобальний стан застосунку.
- `src/fetch` - робота з локальним API (`public/api`).
- `public/api` - JSON-дані каталогу.

## Роутинг

Основні маршрути:

- `/` - головна сторінка.
- `/phones`, `/tablets`, `/accessories` - сторінки категорій.
- `/product/:productId` - детальна сторінка товару.
- `/favorites` - обране.
- `/cart` - кошик.

## Деплой на GitHub Pages

1. В `package.json` вкажи коректне значення поля `homepage`.
2. Виконай:

```bash
npm run deploy
```

## Дані та API

У проєкті використовується локальний API з файлів у `public/api`.
Запити виконуються через `fetch` до:

- `api/products.json`
- `api/phones.json`
- `api/tablets.json`
- `api/accessories.json`
