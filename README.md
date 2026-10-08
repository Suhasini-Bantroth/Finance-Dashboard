# FinTrack — Finance Dashboard

A clean, interactive, single-file finance dashboard built with vanilla JavaScript, Tailwind CSS, and Chart.js. Track spending, analyze trends, and manage transactions with a polished dark/light themed interface.

![Dark Mode](https://img.shields.io/badge/Theme-Dark%20%2F%20Light-amber)
![No Framework](https://img.shields.io/badge/Framework-Vanilla%20JS-blue)
![Single File](https://img.shields.io/badge/Architecture-Single%20HTML-green)

---

## Live Demo

Open `index.html` directly in any modern browser. No build step, no server, no dependencies to install.

---

## Features

### Dashboard Overview
- **Animated summary cards** — Total Balance, Monthly Income, Monthly Expenses, and Savings Rate with eased counter animations and month-over-month trend indicators
- **Balance trend chart** — 6-month line chart with gradient fill showing running balance over time
- **Spending breakdown** — Interactive doughnut chart that filters transactions on click
- **Recent transactions** — Quick view of the latest 6 transactions

### Transactions
- Full transaction list with category icons, color coding, and formatted amounts
- **Search** by description or category
- **Filter by type** — Income / Expense / All
- **Filter by category** — Dynamic dropdown populated from actual data
- **Filter by date range** — From/To date pickers
- **Filter by amount range** — Min/Max number inputs
- **Sort** — Newest, Oldest, Highest Amount, Lowest Amount
- **Deferred "Apply Filters"** — Adjust multiple filters without losing cursor focus, then apply once
- **Active filter pills** — Visual display of applied filters with individual removal
- **Clear All** — One-click reset to defaults

### Role-Based UI
- **Admin** — Can add, edit, and delete transactions
- **Viewer** — Read-only access; all mutation controls are hidden with a "View Only" badge
- Switch roles instantly via the sidebar toggle (no backend required)

### Insights
- Top spending category with percentage bar
- Monthly income comparison with delta
- Average daily spending vs. previous month
- Savings rate with target assessment
- Largest single expense
- Net monthly position
- Dynamic observations generated from actual data patterns

### Additional Features
- **Dark / Light mode** with smooth CSS variable transitions
- **CSV export** of currently filtered transactions
- **LocalStorage persistence** — transactions, role, and theme survive page reloads
- **Toast notifications** for all actions (add, edit, delete, export, filter changes)
- **Inline delete confirmation** — no browser `confirm()` dialogs
- **Responsive layout** — sidebar collapses to hamburger menu on tablet/mobile
- **Keyboard support** — Escape closes modals and sidebar
- **Reduced motion** — respects `prefers-reduced-motion`

---

## Technical Architecture

### State Management

A single `state` object serves as the source of truth:

# Finance_dashboard
A finance dashboard built with JS, Tailwind, and Chart.js. It features animated summary cards, balance trend and spending charts, a filterable transaction list with date and amount ranges, a deferred “Apply Filters” flow, role-based UI , CSV export, dark mode, local Storage persistence, and data-driven insights all in one self-contained HTML file.
