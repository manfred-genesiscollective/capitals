# Hands-on observations from the user's signed-in TradeZella account (screenshots)

Compiled 2026-11-09 from screenshots the user supplied of their own logged-in session at app.tradezella.com. These are first-hand observations of the live UI (high confidence for what is visible; anything inferred is marked as such). Screenshots are stored in ./screenshots/.

## Screenshot 01 — Dashboard, Demo account (app.tradezella.com/tracking)

File: screenshots/01-dashboard-demo-account.png

### Global chrome
- Top bar (dark purple): hamburger menu, TradeZella wordmark/logo, a prominent "Zella AI" button (bull icon) at top right, notification bell, account/profile icon.
- Left rail of icons (collapsed sidebar), top to bottom: a purple "+" (add trades / quick add), dashboard (highlighted), calendar, notebook/journal, reports (bar chart), a strategy/playbook-style icon, a prop-firm/wallet-style icon, then a divider, then replay (play icon), a backtesting/chart-line icon, and a folder icon. Exact labels not visible in collapsed state (inference from icon shapes and known route list /tracking, /tracking/notebook, /tracking/reports, /tracking/strategy, /tracking/replay-scenarios, /tracking/progress-tracker).
- Breadcrumb "Tracking" above the page title "Dashboard".
- Page-level controls, right-aligned: "Dollar" dropdown (display unit; presumably Dollar / R / ticks / pips), "Filters" dropdown, "Date range" dropdown, account selector showing "Demo account".
- A cube icon button above the widget grid (inference: dashboard "edit widgets"/customize layout control).

### Demo state / onboarding
- Yellow banner: "DEMO — You are currently viewing Demo Trades. Ready to add your own trades? [Add trades]". New accounts are seeded with a demo dataset so the dashboard is never empty; the primary CTA is to add real trades.

### Widgets visible (top rows)
- Net P&L: $14,742, with a small badge "110" next to the label (inference: number of trades in range). Info tooltip icon on every widget title.
- Trade win %: 31.78%, semicircular gauge with three colored counts: 34 (green, wins), 3 (blue, breakeven), 73 (red, losses).
- Profit factor: 1.82, shown as a green/red donut ring.
- Day win %: 57.58%, semicircular gauge with counts 19 (green days), 3 (blue, breakeven days), 14 (red, losing days).
- Avg win/loss trade: 3.90 (ratio), with a horizontal green/red bar labelled $964 (avg win) and -$247 (avg loss).
- Zella score: radar/spider chart with axes including Win %, Profit factor, Consistency (other axes cut off; known full set is Win %, Profit factor, Avg win/loss, Recovery factor, Max drawdown, Consistency).
- Progress tracker: a GitHub-style heatmap grid (rows Sun..Thu visible, columns by week across Oct/Nov) with an "Explore" button.
- Daily net cumulative P&L: area chart from roughly $6,000 to $16,000 (demo data).

### Design observations
- Light content area on a near-white background, card-based widget grid, generous whitespace, a single accent purple, green/red semantic colors, small info icons for metric definitions, numbers large and left-aligned in each card.
- The demo dataset itself is instructive: a 31.78% trade win rate with a 3.90 avg win/loss ratio and 1.82 profit factor is a deliberately "low win rate, high payoff" example, which reinforces TradeZella's messaging that win rate alone does not define profitability.
