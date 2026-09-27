# blinkit — quick commerce demo

A mobile-first React/Vite mock that implements the Blinkit shopping journey using local product/category data, a reducer-backed context, Framer Motion transitions, and React Router v6.

## Run locally

```bash
npm install
npm run dev
```

## Folder structure

```text
.
├── index.html
├── package.json
├── postcss.config.js
├── tailwind.config.js
└── src
    ├── components/UI.jsx          # shared header, product cards, navigation and cart bar
    ├── context/AppContext.jsx     # persisted cart, address and order reducer state
    ├── data/categories.js         # category and subcategory mock data
    ├── data/products.js           # product mock data
    ├── pages/MainPages.jsx        # location, home, search, category and product pages
    ├── pages/CheckoutPages.jsx    # cart, address, payment, confirmation, tracking, account
    ├── index.css                  # Tailwind and small application styles
    └── main.jsx                   # router and selected-address route guard
```

The browser stores mock state in `localStorage`, so orders are available from the Account tab after checkout.
