# ☕ myCoffee

**Your personal coffee journal**

myCoffee is a personal, web-based application designed for specialty coffee enthusiasts who want to **brew coffee and keep track of their previous coffees, explore new recipes and have an easy time keeping track of the recipes**.

The application focuses on **guided brewing**, **recipe clarity**, and **brew tracking**, allowing users to compare expected vs actual results and iteratively improve their coffee.

---

## 🎯 Goals

- Provide a **guided brewing experience** for pour-over coffee
- Capture detailed brewing parameters (time, grind, temperature, pours)
- Enable reflection through brew notes and history

---

## 🧠 Design Philosophy

- **Mobile-first** UI (optimized for phones during brewing)
- **Domain-driven structure** (coffee concepts first, UI second)
- **Minimal dependencies** (avoid premature complexity)
- **Local-first** (no accounts, no cloud for MVP)

---

## 🧩 MVP Scope

### Included
- One pour-over recipe
- Guided brew screen with step-based timer
- Brew summary after completion
- Local brew history (stored in browser)

### Explicitly Excluded (for MVP)
- Authentication
- Cloud sync
- Multiple brew methods
- Analytics & charts
- Social features

---

## 🛠️ Tech Stack

- **Frontend**: React + TypeScript
- **Framework**: Next.js (App Router)
- **Styling**: Tailwind CSS
- **State Management**: React hooks (`useState`, `useReducer`)
- **Persistence**: Browser `localStorage`

---

## 🚀 Running the Project (Planned)

```bash
npm install
npm run dev

# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) (or [oxc](https://oxc.rs) when used in [rolldown-vite](https://vite.dev/guide/rolldown)) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type-aware lint rules:

```js
export default defineConfig([
  globalIgnores(['dist']),
  {
    files: ['**/*.{ts,tsx}'],
    extends: [
      // Other configs...

      // Remove tseslint.configs.recommended and replace with this
      tseslint.configs.recommendedTypeChecked,
      // Alternatively, use this for stricter rules
      tseslint.configs.strictTypeChecked,
      // Optionally, add this for stylistic rules
      tseslint.configs.stylisticTypeChecked,

      // Other configs...
    ],
    languageOptions: {
      parserOptions: {
        project: ['./tsconfig.node.json', './tsconfig.app.json'],
        tsconfigRootDir: import.meta.dirname,
      },
      // other options...
    },
  },
])
```

You can also install [eslint-plugin-react-x](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-x) and [eslint-plugin-react-dom](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-dom) for React-specific lint rules:

```js
// eslint.config.js
import reactX from 'eslint-plugin-react-x'
import reactDom from 'eslint-plugin-react-dom'

export default defineConfig([
  globalIgnores(['dist']),
  {
    files: ['**/*.{ts,tsx}'],
    extends: [
      // Other configs...
      // Enable lint rules for React
      reactX.configs['recommended-typescript'],
      // Enable lint rules for React DOM
      reactDom.configs.recommended,
    ],
    languageOptions: {
      parserOptions: {
        project: ['./tsconfig.node.json', './tsconfig.app.json'],
        tsconfigRootDir: import.meta.dirname,
      },
      // other options...
    },
  },
])
```
