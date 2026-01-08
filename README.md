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