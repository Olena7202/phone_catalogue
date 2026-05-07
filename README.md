# Phone Catalogue

A phone, tablet, and accessories catalogue web app built with `React + TypeScript`.
The project includes product listing, filtering and sorting, a product details page, a cart, and favorites.

Live demo: [https://olena7202.github.io/phone_catalogue/](https://olena7202.github.io/phone_catalogue/)

## Features

- Browse catalog categories: phones, tablets, accessories.
- Sort products by `Newest`, `Alphabetically`, or `Cheapest`.
- Pagination and configurable items per page.
- Product details page with selectable options.
- Add items to favorites and cart (stored in `localStorage`).
- Responsive layout with a mobile menu (`BurgerMenu`).

## Tech Stack

- `React 18`
- `TypeScript`
- `React Router`
- `SCSS`
- `Vite` (via `@mate-academy/scripts`)
- `ESLint`, `Prettier`, `Stylelint`

## Run Locally

### 1) Install dependencies

```bash
npm install
```

### 2) Start the app

```bash
npm start
```

After startup, the app will be available at a local URL shown in the terminal.

## NPM Scripts

- `npm start` - run the development server.
- `npm run build` - create a production build.
- `npm run lint` - format and lint JS/TS + SCSS.
- `npm run lint-js` - lint JavaScript/TypeScript.
- `npm run lint-css` - lint styles.
- `npm run format` - format `ts/tsx` with Prettier.
- `npm run deploy` - deploy to GitHub Pages.

## Project Structure

- `src/modules` - pages and larger UI modules.
- `src/shared` - shared reusable components.
- `src/Context` - global application state.
- `src/fetch` - local API layer (`public/api`).
- `public/api` - JSON data source for the catalog.

## Routing

Main routes:

- `/` - home page.
- `/phones`, `/tablets`, `/accessories` - category pages.
- `/product/:productId` - product details page.
- `/favorites` - favorites page.
- `/cart` - cart page.

## Deploy to GitHub Pages

1. Set the correct `homepage` value in `package.json`.
2. Run:

```bash
npm run deploy
```

## Data & API

The project uses a local file-based API from `public/api`.
Requests are made via `fetch` to:

- `api/products.json`
- `api/phones.json`
- `api/tablets.json`
- `api/accessories.json`
