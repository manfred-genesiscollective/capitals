# TradeZella Product Features — Feature-by-Feature Inventory (as of 2026-11-09)

> **Research-condition notice (read first).** This workstream was severely constrained by the session's network policy. Every direct page fetch (WebFetch and curl) to tradezella.com, www.tradezella.com, help.tradezella.com, intercom.help, apps.apple.com, pricingsaas.com and web.archive.org was refused by the session proxy (HTTP 403 on CONNECT / `ENOTFOUND`), two attempts to get those hosts allowed were rejected by the environments service, and the shared WebSearch budget for this turn was exhausted after six queries. Consequently **every finding below comes from search-engine result snippets/summaries of the cited pages, not from reading the full pages.** Attributions marked "(snippet; attribution approximate)" mean the search summary did not unambiguously tie the fact to one URL among the results. Nothing below is fabricated; anything that could not be sourced is in a Gaps section. The single most valuable follow-up is to fetch `https://www.tradezella.com/llms-full.txt` (a full-site text dump that TradeZella publishes) plus the Intercom help center (`https://help.tradezella.com/` — the same content is mirrored at `https://intercom.help/tradezella-4066d388d93c/`), which would answer most gaps in one pass.

## Pricing tiers and feature gating (cross-cutting; needed to answer "which tier is each feature gated to")

### Takeaway
TradeZella moved from a two-plan lineup (Basic $29/mo, Pro $49/mo) to three plans — Essential $35/mo, Pro $59/mo, Ultra $99/mo — on July 14, 2026, with pre-existing subscribers grandfathered at their old price while they stay on their plan; exact per-tier feature gating for the new plans could not be verified from snippets.

### Cited Findings
- TradeZella's help center states that as of July 14, 2026 it "updated our pricing" and "now offer[s] three plans." — [Our pricing (help center article 8911582)](https://help.tradezella.com/en/articles/8911582-our-pricing)
- The three current plans are Essential ($35/mo), Pro ($59/mo) and Ultra ($99/mo); the company blog frames this as a move "from two plans to three." — [TradeZella New Pricing: What Every Plan Includes and How It Compares](https://www.tradezella.com/blog/tradezella-pricing); [TradeZella Pricing: Plans, Features & Which to Choose (2026)](https://www.tradezella.com/blog/tradezella-pricing-guide-2026)
- Previous (pre-July-2026) pricing was Basic $29/mo (or $288/yr) and Pro $49/mo; a third-party review describes the Basic plan as covering "one account, three playbooks, reporting, and backtesting." — [daytradingz TradeZella review](https://daytradingz.com/tradezella-review/); [daytradingz TradeZella vs Tradervue](https://daytradingz.com/tradezella-vs-tradervue/) (snippet; attribution approximate)
- TradeZella's own 2026 pricing guide lists Basic with 3 playbooks and Pro with unlimited playbooks (this appears to describe the pre-July-2026 lineup). — [TradeZella Pricing: Plans, Features & Which to Choose (2026)](https://www.tradezella.com/blog/tradezella-pricing-guide-2026)
- Subscribers who signed up before July 14, 2026 "can keep your old price as long as you stay on your current plan." — [Our pricing (help center article 8911582)](https://help.tradezella.com/en/articles/8911582-our-pricing) (snippet; attribution approximate)
- Backtesting is "included from the Essential plan up." — [How to Backtest with TradeZella (2026 Guide)](https://www.tradezella.com/blog/backtest-with-tradezella) (snippet; attribution approximate — could also be the pricing blog post)
- Marketing copy cites broker auto-sync for "500+ brokers" and AI tools including "Zella AI for questions about your data." — [TradeZella New Pricing](https://www.tradezella.com/blog/tradezella-pricing) (snippet; attribution approximate)
- Third-party reviewers claim there is no free trial and no refunds; one says the product "does not offer a free trial or free plan." — [PurePowerPicks TradeZella review (2026)](https://purepowerpicks.com/tradezella-review/); [daytradingz TradeZella review](https://daytradingz.com/tradezella-review/) (snippet; attribution approximate; third-party claims)
- PricingSaaS tracks a TradeZella pricing-page diff dated ISO week 2026-W30 (the week of July 20–26, 2026), consistent with the mid-July 2026 repricing. — [PricingSaaS TradeZella diff 2026W30](https://pricingsaas.com/companies/tradezella/diffs/2026W30); [PricingSaaS TradeZella pricing history](https://pricingsaas.com/companies/tradezella)
- TradeZella publishes competitor comparison pages for Tradervue, TraderSync, TradesViz, TradingView, Forex Tester and NinjaTrader (the latter three framed as "Backtesting comparison · 2026"). — [vs Tradervue](https://tradezella.com/vs/tradervue); [vs TraderSync](https://tradezella.com/vs/tradersync); [vs TradesViz](https://tradezella.com/vs/tradesviz); [vs TradingView](https://www.tradezella.com/vs/tradingview); [vs Forex Tester](https://www.tradezella.com/vs/forex-tester); [vs NinjaTrader](https://www.tradezella.com/vs/ninjatrader)

### Inferences
- Because Basic (3 playbooks) vs Pro (unlimited) was the main gating lever in the old lineup, the new Essential/Pro/Ultra lineup most likely gates on account count, playbook/strategy count, and the newer AI/replay/automated-backtesting tools — but this is inference; the snippets explicitly said tier membership of trade replay and backtesting "could not be confirmed."
- Annual-billing discounts exist but vary by plan (third-party reporting); exact annual prices for Essential/Pro/Ultra were not captured.

### Gaps
- Exact feature matrix per Essential / Pro / Ultra (number of connected accounts, playbook limits, AI features, replay, automated backtesting, mentor/sharing) — not retrievable; fetch https://www.tradezella.com/pricing and https://help.tradezella.com/en/articles/8911582-our-pricing.
- Annual prices for each of the three plans; whether Ultra bundles education/community; whether any free tier exists in 2026.
- Whether the company's "500+ brokers" figure is auto-sync-only or includes CSV/file import.

## Onboarding and setup flow (account creation, broker connect/import, first-run, timezone/currency/commission settings, multiple accounts)

### Takeaway
Only fragments were recoverable: TradeZella has a dedicated "Getting started with TradeZella" help article, markets auto-sync with 500+ brokers, has added broker/prop-firm integrations over time (DAS Trader Pro, NinjaTrader, FTMO), and supports creating trade notes before import and linking them afterward; the actual first-run screens and settings (timezone, currency, commissions) could not be verified.

### Cited Findings
- A current help-center onboarding article exists titled "Getting started with TradeZella." — [Getting started with TradeZella (article 13863136)](https://help.tradezella.com/en/articles/13863136-getting-started-with-tradezella)
- An older onboarding article, "Welcome to TradeZella," exists in the Intercom help center. — [Welcome to TradeZella (article 5801077)](https://intercom.help/tradezella-4066d388d93c/en/articles/5801077-welcome-to-tradezella)
- TradeZella markets broker auto-sync for "500+ brokers." — [TradeZella New Pricing](https://www.tradezella.com/blog/tradezella-pricing) (snippet; attribution approximate)
- A 2024 release note focused on "the backtesting tool and seamless integration with NinjaTrader and FTMO" (quote: "This month's updates focus on strengthening some core areas within TradeZella — the backtesting tool and seamless integration with NinjaTrader and FTMO!"). — [TradeZella Updates blog category](https://www.tradezella.com/category/tradezella-updates) (snippet; the specific 2024 month's post was not identified — candidates: [March Release Notes](https://tradezella.com/blog/march-release-notes), [April 2024 Updates](https://www.tradezella.com/blog/april-2024-tradezella-updates))
- 2023-era release notes added "new broker support such as DAS Trader Pro." — [TradeZella release notes, July–August](https://www.tradezella.com/blog/tradezella-release-notes-july-august) (snippet; attribution approximate)
- Users can "create a trade note before importing a trade and link it later." — [Create a trade note before importing a trade and link it later (article 11517879)](https://intercom.help/tradezella-4066d388d93c/en/articles/11517879-create-a-trade-note-before-importing-a-trade-and-link-it-later)
- Users can set a default profit target and stop loss that applies to their trades. — [Setting default profit target and stop loss for your trades (article 12053164)](https://intercom.help/tradezella-4066d388d93c/en/articles/12053164-setting-default-profit-target-and-stop-loss-for-your-trades)
- The pre-July-2026 Basic plan covered "one account," implying multi-account support is a paid-tier differentiator. — [daytradingz TradeZella review](https://daytradingz.com/tradezella-review/) (snippet)

### Inferences
- The "default profit target and stop loss" setting implies per-trade planned-R / target fields exist on the trade record and can be pre-filled globally, which is the basis for R-multiple and plan-adherence analytics.
- "Create a note before import, link later" implies the trade record and the journal note are separate objects with a many-to-one link established after broker sync.

### Gaps
- Account-creation flow (email/Google/Apple sign-in), first-run wizard steps, timezone and base-currency settings, commission/fee configuration, how multiple trading accounts are added and switched — none verifiable; fetch article 13863136 and the help-center "Getting Started" / "Integrations" collections.
- The authoritative supported-broker list (auto-sync vs file import), and the sync mechanics (credentials, read-only API, sync frequency).

## Dashboard (widgets, Zella Score composition and weights, metrics, filters, calendar)

### Takeaway
The Zella Score (relaunched as "the all-new Zella Score" / "Zella Score 2.0" in December 2024, replacing the earlier "Zella Scale") is an explicitly documented weighted composite of six 0–100 sub-scores: Profit Factor 25%, Average Win/Loss 20%, Max Drawdown 20%, Trade Win % 15%, Recovery Factor 10%, Consistency Score 10%, where each raw metric is scaled against a "Top Threshold" (default 60) as (value ÷ threshold) × 100.

### Cited Findings
- The Zella Score "is built on six metrics, each scored 0–100, then weighted and combined into one overall score," with weights: Recovery Factor 10%, Trade Win % 15%, Average Win/Loss 20%, Profit Factor 25%, Max Drawdown 20%, Consistency Score 10%. — [Introducing the all-new Zella Score (article 10305642)](https://intercom.help/tradezella-4066d388d93c/en/articles/10305642-introducing-the-all-new-zella-score)
- Per-metric scoring uses a threshold formula; "By default, the Top Threshold is set to 60," and the worked example is a 25% trade win rate → (25/60) × 100 = 41.67. — [Introducing the all-new Zella Score (article 10305642)](https://intercom.help/tradezella-4066d388d93c/en/articles/10305642-introducing-the-all-new-zella-score)
- The December 2024 release ("Zella Score 2.0") added metrics: "in addition to Win Rate, Profit Factor, and Average Win/Loss, you'll also see Max Drawdown, Consistency, and Recovery Factor," and points to a separate article for per-score calculations. — [What's NEW: December 2024](https://www.tradezella.com/blog/whats-new-december-2024)
- The predecessor metric was called the "Zella Scale," documented in help articles "What is the Zella Scale" and "Zella Scale: Maximize your trade insights," and updated in the December 2022 release notes ("Zella Scale Update"). — [What is the Zella Scale (article 5961961)](https://intercom.help/tradezella-4066d388d93c/en/articles/5961961-what-is-the-zella-scale); [Zella Scale: maximize your trade insights (article 7218420)](https://help.tradezella.com/en/articles/7218420-zella-scale-maximize-your-trade-insights); [December 2022 release notes](https://tradezella.com/blog/december-release-notes)
- A dedicated help article, "Understanding dashboard widgets and stats," documents the dashboard widgets and their definitions. — [Understanding dashboard widgets and stats (article 7118437)](https://intercom.help/tradezella-4066d388d93c/en/articles/7118437-understanding-dashboard-widgets-and-stats) (contents not retrievable)
- An "edit widget" flow for customizing the dashboard was added in the April/May 2024 release cycle. — [April 2024 Updates](https://www.tradezella.com/blog/april-2024-tradezella-updates); [What's NEW: May 2024](https://www.tradezella.com/blog/whats-new-may-2024) (snippet; attribution approximate between these two)
- Dark mode for the trade page shipped in January 2024. — [January 2024 Release Notes](https://www.tradezella.com/blog/january-2024-release-notes)
- Third-party descriptions of the score conflict with the official one: one review says it rates "consistency, win/loss ratio, and average trade quality," another says it grades discipline/rule-following — the official six-metric breakdown above should be preferred. — [daytradingz TradeZella review](https://daytradingz.com/tradezella-review/); [tradingjournalcom review of TradeZella](https://tradingjournalcom.netlify.app/review/tradezella) (snippet; attribution approximate)

### Inferences
- Since each sub-score is capped by a configurable "Top Threshold," the Zella Score is a bounded 0–100 radar-style composite; the Dec-2024 blog's mention of "per-score calculation" in a separate article suggests each of the six metrics has its own threshold/normalization (e.g., Max Drawdown is likely inverted so lower drawdown scores higher), but the exact formulas for the other five metrics were not recoverable.
- The dashboard is widget-based and user-editable (edit-widget flow), which in a 2024–2026 product almost certainly includes the standard metrics named in the brief (net P&L, win %, profit factor, day win %, avg win/loss, cumulative P&L, daily P&L calendar) — but none of those specific widget names were verified here.

### Gaps
- Exact per-metric formulas and default thresholds for Profit Factor, Average Win/Loss, Max Drawdown, Recovery Factor and Consistency Score; whether users can change the Top Threshold — fetch article 10305642 in full.
- Complete dashboard widget list and definitions (net P&L, day win %, running/cumulative P&L chart, daily P&L calendar, drawdown, streaks), the available date-range presets, and the filter model (account, symbol, tag, playbook) — fetch article 7118437.
- Whether the Zella Score appears on the dashboard, on the trade page, or both, and whether it is computed per account.

## Trade log and individual trade page (columns, executions, chart markers, notes/tags/setups/mistakes, rating, screenshots, running P&L, asset-class handling)

### Takeaway
Verified fragments: trades carry linked notes and tags with custom tag categories (Feb 2024) and tag management (Jun 2024), can be checked against playbook rules, and can be replayed tick-by-tick with entry/exit/scale markers; the full column set, trade rating, screenshots, and asset-class handling could not be verified.

### Cited Findings
- "Custom tag categories" shipped in February 2024. — [TradeZella Release Notes February 2024](https://www.tradezella.com/blog/tradezella-release-notes-february-2024)
- "Tag management" shipped in June 2024, alongside a planned left-side-panel redesign. — [June 2024 Release Notes](https://tradezella.com/blog/june-2024-release-notes)
- Trades can be checked against a playbook "to see how many rules were followed in the actual trade execution," and "missed trades can also be logged." — [daytradingz TradeZella review](https://daytradingz.com/tradezella-review/); [Getting started with the playbook (article 7020769)](https://help.tradezella.com/en/articles/7020769-getting-started-with-the-playbook) (snippet; attribution approximate)
- Trade Replay "replays trades you've taken using real tick-by-tick data from your journal"; "entries and exits show as markers on the chart, and clicking any entry, exit, or scale jumps you to that moment." — [Trade Replay feature page](https://www.tradezella.com/trade-replay); [New in TradeZella: Replay your trades](https://www.tradezella.com/blog/new-in-tradezella-trade-replay)
- Reviewers describe three replay modes: Trade Replay, Day Replay and Scenario Replay. — [daytradingz TradeZella review](https://daytradingz.com/tradezella-review/) (snippet; attribution approximate)
- Trade replay for futures was added in a 2023 release. — [TradeZella release notes, July–August](https://www.tradezella.com/blog/tradezella-release-notes-july-august) (snippet; attribution approximate)
- Trade notes can be created before a trade is imported and linked to it later. — [Article 11517879](https://intercom.help/tradezella-4066d388d93c/en/articles/11517879-create-a-trade-note-before-importing-a-trade-and-link-it-later)
- A default profit target and stop loss can be set for trades. — [Article 12053164](https://intercom.help/tradezella-4066d388d93c/en/articles/12053164-setting-default-profit-target-and-stop-loss-for-your-trades)
- Dark mode exists on the trade page (Jan 2024). — [January 2024 Release Notes](https://www.tradezella.com/blog/january-2024-release-notes)

### Inferences
- "Scale" markers in replay imply execution-level (per-fill) storage, i.e., the trade page shows individual executions and partial entries/exits rather than only an aggregated round-trip.
- Tag "categories" plus "management" suggest tags are typed (e.g., setup / mistake / custom category) and centrally editable/mergeable.

### Gaps
- Exact trade-log columns and sort/filter options; trade rating (stars/scale); screenshot/attachment upload; running-P&L-on-trade display; candle timeframes available on the trade chart; options (Greeks, multi-leg), futures (tick value/multiplier), forex (pip/lot) and crypto handling — none verifiable here.

## Journaling (daily journal, notebook, templates, routines, attachments, rich text)

### Takeaway
TradeZella's Notebook was redesigned in spring 2024 with note tags, search and templates; the daily-journal structure, pre-/post-market routine templates, attachments and rich-text capabilities were not verifiable.

### Cited Findings
- The April/May 2024 releases "added a redesigned notebook with note tags, search, and templates." — [April 2024 Updates](https://www.tradezella.com/blog/april-2024-tradezella-updates); [What's NEW: May 2024](https://www.tradezella.com/blog/whats-new-may-2024) (snippet; attribution approximate between the two)
- Notes are a distinct object that can be created before a trade exists and linked afterwards. — [Article 11517879](https://intercom.help/tradezella-4066d388d93c/en/articles/11517879-create-a-trade-note-before-importing-a-trade-and-link-it-later)

### Inferences
- A template system in the Notebook is the likely vehicle for pre-market / post-market routine checklists; this is inference only.

### Gaps
- Daily journal page layout, template library contents, attachment types/size limits, rich-text editor features, whether journal entries auto-attach that day's trades and P&L — fetch the help center "Notebook"/"Journal" collection.

## Playbooks / Strategies (rule sets, checklists, adherence tracking, per-playbook stats)

### Takeaway
"Playbooks" (launched 2023) have been renamed "Strategies"; each is built from Rules organized into Groups (with a "show rule only when" conditional on rules), trades are scored against how many rules were followed, missed trades can be logged, free community templates (e.g., from Kane and Jade Cap) can be duplicated into a user's strategies, and the pre-July-2026 Basic plan capped users at 3 playbooks vs unlimited on Pro.

### Cited Findings
- "The first step in creating your Playbook is to set your different trading rules according to your strategy and trading style," organized through "Playbook Rules and Groups"; rules are edited via the playbook's "Rules" tab. — [Getting started with the playbook (article 7020769)](https://help.tradezella.com/en/articles/7020769-getting-started-with-the-playbook)
- Constraint: "if a trade is already linked to a rule, you cannot change its 'show rule only when' setting." — [Getting started with the playbook (article 7020769)](https://help.tradezella.com/en/articles/7020769-getting-started-with-the-playbook) (snippet; may instead be in [article 6986848](https://intercom.help/tradezella-4066d388d93c/en/articles/6986848-what-is-a-group-criteria-and-rules-in-the-playbook))
- The help center notes "Playbooks have been renamed to Strategies"; the same article slug appears both as "getting-started-with-the-playbook" and "getting-started-with-strategies." — [Getting started with strategies (article 7020769)](https://intercom.help/tradezella-4066d388d93c/en/articles/7020769-getting-started-with-strategies)
- A dedicated article defines "group criteria and rules" in the playbook (slug variants: "what is a group in the playbook", "what is groups and rules in the playbook"). — [Article 6986848](https://intercom.help/tradezella-4066d388d93c/en/articles/6986848-what-is-a-group-criteria-and-rules-in-the-playbook)
- Trades can be checked against a playbook to see how many rules were followed; missed trades can be logged. — [daytradingz TradeZella review](https://daytradingz.com/tradezella-review/) (snippet; attribution approximate)
- Pre-July-2026 gating: Basic = 3 playbooks, Pro = unlimited playbooks. — [TradeZella Pricing guide 2026](https://www.tradezella.com/blog/tradezella-pricing-guide-2026)
- Community playbooks: users can browse shared playbooks including templates from "Kane" and "Jade Cap"; flow is click a playbook → "Get Free Playbook" → "Duplicate to My Strategy." — [Getting started with TradeZella (article 13863136)](https://help.tradezella.com/en/articles/13863136-getting-started-with-tradezella) (snippet; attribution approximate — the summary said only "one help article")
- The Playbook feature was introduced in a 2023 release. — [TradeZella software updates, February 2023](https://www.tradezella.com/blog/february-trader-software-release-notes); [February release notes](https://www.tradezella.com/blog/february-release-notes) (snippet; attribution approximate)
- TradeZella ran a "Building your trading playbook" webinar (third-party notes dated 2026-02-21). — [Lilys.ai webinar notes](https://lilys.ai/en/notes/trading-strategy-20260221/profitable-trading-strategy)
- A third-party YouTube summary covers "Master trading with Playbook feature in TradeZella." — [Gist.ly summary](https://gist.ly/youtube-summarizer/master-trading-with-playbook-feature-in-tradezella)

### Inferences
- "Show rule only when" implies conditional rules (shown only when a prior rule/criterion is met), and the lock-after-linking constraint implies adherence percentages are stored per trade and would be invalidated by changing rule visibility.
- "Duplicate to My Strategy" wording confirms the 2026 UI label is "Strategy/Strategies" while help URLs and marketing still say "Playbook."

### Gaps
- Per-strategy statistics shown (P&L, win %, expectancy, adherence %), whether strategies auto-assign via criteria, checklist UI on the trade page, and the exact strategy limit per 2026 tier — fetch articles 7020769 and 6986848 and the pricing page.

## Backtesting and Replay (bar-by-bar replay, markets/timeframes, order simulation, journaling of backtests, data coverage)

### Takeaway
TradeZella launched Backtesting in January 2024, later added multi-symbol backtesting, and by 2026 offers both manual bar-replay backtesting and a no-code "automated" mode where a strategy is described in plain English and tested across years of data; it is distinct from Trade Replay, which replays the user's own executed trades on tick data. Backtesting is included from the Essential plan upward.

### Cited Findings
- "January [2024] was one of our biggest product updates, with the launch of Backtesting." — [January 2024 Release Notes](https://www.tradezella.com/blog/january-2024-release-notes)
- A later 2024 release added "backtesting with multiple symbols." — [TradeZella Updates category](https://www.tradezella.com/category/tradezella-updates) (snippet; specific post not identified)
- TradeZella's docs describe backtesting as "a simulation tool that lets traders test their strategies using historical market data." — [How to create a backtesting session (article 8835814)](https://help.tradezella.com/en/articles/8835814-how-to-create-a-backtesting-session) (snippet; attribution approximate)
- TradeZella "offers both manual bar replay and automated plain English backtesting"; the automated version is "no-code, where you describe your strategy in plain English and test it across years of data in minutes." — [Automated Backtesting Inside TradeZella: From Plain English to Results in Minutes](https://www.tradezella.com/blog/tradezella-automated-backtesting-guide); [How to Backtest with TradeZella (2026 Guide)](https://www.tradezella.com/blog/backtest-with-tradezella)
- Trade Replay vs Backtesting: "Trade Replay works on your past executions, while Backtesting tests a strategy on historical data you haven't traded yet." — [What is the trade replay feature and how does it compare to backtesting (article 11787298)](https://help.tradezella.com/en/articles/11787298-what-is-the-trade-replay-feature-in-tradezella-and-how-does-it-compare-to-backtesting)
- Backtesting is included from the Essential plan up. — [How to Backtest with TradeZella (2026 Guide)](https://www.tradezella.com/blog/backtest-with-tradezella) (snippet; attribution approximate)
- TradeZella positions its backtester against TradingView Bar Replay, Forex Tester, FX Replay and NinjaTrader. — [TradingView Bar Replay vs TradeZella](https://www.tradezella.com/blog/tradingview-bar-replay-vs-tradezella-backtesting); [Best Forex Tester alternative](https://www.tradezella.com/blog/forex-tester-alternative); [FX Replay vs TradeZella](https://www.tradezella.com/blog/fx-replay); [FX Replay alternatives 2026](https://www.tradezella.com/blog/fx-replay-alternatives); [The backtesting platform](https://www.tradezella.com/blog/the-backtesting-platform)

### Inferences
- The "automated plain-English" mode is almost certainly an LLM-driven feature (consistent with the "Zella AI" branding), launched after the Jan-2024 manual backtester; its launch date is unknown (no 2025 release notes surfaced).
- Because backtests are "sessions" (article title), results are probably stored as separate backtesting accounts/sessions rather than mixed into live trade analytics — inference only.

### Gaps
- Supported markets and timeframes, tick vs bar data, order types simulated (market/limit/stop, partials), commission/slippage settings, whether backtest trades flow into the journal/reports as a separate account, data history depth and vendor — fetch articles 8835814 and 11787298 and the two 2026 blog guides.

## Reports and analytics (report types, comparison and filtering)

### Takeaway
No report-level detail was recoverable within this session's constraints beyond the fact that "reporting" is bundled even in the entry plan.

### Cited Findings
- The pre-July-2026 Basic plan included "reporting" (alongside one account, three playbooks and backtesting). — [daytradingz TradeZella review](https://daytradingz.com/tradezella-review/) (snippet)

### Inferences
- None safe to make beyond: reports are tier-independent at entry level.

### Gaps
- Entire reports catalogue (by setup/tag/mistake, time of day, day of week, duration, instrument, price, volume, R-multiple, streaks, drawdown), comparison mode, saved filters — fetch the help-center "Reports" collection and https://www.tradezella.com/llms-full.txt.

## Progress tracking, goals, insights, AI features, sharing/mentor/community

### Takeaway
TradeZella has a "Progress Tracker" with user-defined rules and markets a "Zella AI" assistant for asking questions about one's own data; sharing, mentor mode and community features were not verifiable (other than the community playbook/strategy template library noted above).

### Cited Findings
- A help article documents "understanding and using Progress Tracker rules." — [Understanding and using progress tracker rules (article 10371695)](https://help.tradezella.com/en/articles/10371695-understanding-and-using-progress-tracker-rules)
- TradeZella markets AI tools including "Zella AI for questions about your data." — [TradeZella New Pricing](https://www.tradezella.com/blog/tradezella-pricing) (snippet; attribution approximate)
- Automated, plain-English backtesting is marketed as a no-code AI capability. — [Automated Backtesting Inside TradeZella](https://www.tradezella.com/blog/tradezella-automated-backtesting-guide)
- Community strategy templates from named traders (Kane, Jade Cap) can be fetched via "Get Free Playbook" and "Duplicate to My Strategy." — [Getting started with TradeZella (article 13863136)](https://help.tradezella.com/en/articles/13863136-getting-started-with-tradezella) (snippet; attribution approximate)

### Inferences
- "Progress Tracker rules" are likely behaviour rules (e.g., max trades/day, max loss) evaluated against imported trades to produce a daily adherence/progress view — distinct from Strategy rules, which describe setups.

### Gaps
- Zella AI scope (chat over data? auto-insights? journaling assistant?), launch date and tier; trade sharing / public trade cards; mentor or coach access; community/Discord; goals UI — fetch https://www.tradezella.com/llms-full.txt and the help-center "AI" and "Progress Tracker" articles.

## Mobile apps (iOS / Android) vs web

### Takeaway
Multiple 2026 sources say TradeZella now ships native iOS and Android apps (closing a long-standing gap), but they disagree on parity with the web app, and no App Store or Google Play listing data (ratings, version history) could be retrieved.

### Cited Findings
- "TradeZella now has iOS and Android apps — this was a long-standing gap that has been addressed." — [Traders Second Brain TradeZella review](https://traderssecondbrain.com/guides/tradezella-review) (snippet; attribution approximate)
- An older source states there is no native mobile app (likely pre-dating the launch). — [TradingBrokers TradeZella review](https://tradingbrokers.com/tradezella-review/) (snippet; attribution approximate)
- One review says "the mobile app retains most of the features of the desktop version, though some advanced analytics might be limited to the web version"; another says the mobile experience "is significantly degraded compared to desktop." — [Modest Money TradeZella app review](https://www.modestmoney.com/tradezella-app-review); [Traders Second Brain: TradeZella alternative](https://traderssecondbrain.com/guides/tradezella-alternative) (snippet; attribution approximate)
- A Trustpilot reviewer singled out trade replay as "the best thing about the tradezella app itself." — [Trustpilot TradeZella reviews](https://uk.trustpilot.com/review/tradezella.com?page=5) (snippet; page attribution approximate)
- Trustpilot scores reported between ~4.4 and ~4.8/5 across ~932 reviews; one analysis questions authenticity, noting "eight in ten five-star reviews come from accounts with one or two reviews." — [Trustpilot (UK)](https://uk.trustpilot.com/review/tradezella.com?page=5); [damnpropfirms TradeZella review, updated July 2026](https://damnpropfirms.com/?p=19038) (snippet; attribution approximate)
- "Mobile responsiveness" (of the web app) was a 2023 release item. — [TradeZella release notes, July–August](https://www.tradezella.com/blog/tradezella-release-notes-july-august) (snippet; attribution approximate)

### Inferences
- The sequence (2023 responsive web → 2026 reviews citing native apps) suggests the native apps launched in 2025 or early 2026, but no primary source confirms the date.

### Gaps
- App Store / Google Play URLs, ratings, version history, what the apps can and cannot do (import? replay? journaling only?) — fetch apps.apple.com and play.google.com listings.

## Settings, export, privacy, notifications, dark mode, shortcuts, integrations

### Takeaway
Verified items are limited to dark mode (trade page, Jan 2024), broker/prop-firm integrations (NinjaTrader, FTMO, DAS Trader Pro; "500+ brokers"), and a weekly-updated public changelog; export, privacy, notifications, shortcuts and TradingView integration were not verifiable.

### Cited Findings
- Dark mode for the trade page — January 2024. — [January 2024 Release Notes](https://www.tradezella.com/blog/january-2024-release-notes)
- NinjaTrader and FTMO integrations (2024); DAS Trader Pro (2023). — [TradeZella Updates category](https://www.tradezella.com/category/tradezella-updates) (snippet; specific posts not identified)
- A left-side navigation panel redesign was announced as planned in June 2024. — [June 2024 Release Notes](https://tradezella.com/blog/june-2024-release-notes)
- TradeZella maintains a changelog: "be sure to check our changelog here. This comprehensive resource provides detailed information about every update, including new features, improvements, and bug fixes—updated on the weekly." — [TradeZella blog](https://www.tradezella.com/blog) (snippet; the changelog's own URL was not surfaced)
- TradeZella publishes an LLM-readable full-site text file. — [llms-full.txt](https://www.tradezella.com/llms-full.txt)

### Inferences
- None.

### Gaps
- CSV/PDF export, data deletion/privacy controls, notification settings, keyboard shortcuts, TradingView or other third-party integrations — not verifiable here.

## Feature history, changelog and roadmap

### Takeaway
A dated trail of public release notes exists from November 2022 through December 2024 (Zella Scale → Playbooks → Trade Replay for futures → Backtesting (Jan 2024) → custom tag categories → Notebook redesign → tag management → Zella Score 2.0), and the July 14, 2026 repricing plus 2026 "automated backtesting" and "Zella AI" content show continued 2025–26 development; no 2025 or 2026 release-notes posts and no roadmap page surfaced in search.

### Cited Findings
- Release-note posts located, in chronological order: Nov 2022 — [link](https://www.tradezella.com/blog/november-release-notes); Dec 2022 (Zella Scale Update) — [link](https://tradezella.com/blog/december-release-notes); Feb 2023 — [link](https://www.tradezella.com/blog/february-trader-software-release-notes); "February release notes" (year unclear) — [link](https://www.tradezella.com/blog/february-release-notes); "March release notes" (year unclear) — [link](https://tradezella.com/blog/march-release-notes); "April–May" (year unclear) — [link](https://www.tradezella.com/blog/april-may-release-notes); "July–August" (year unclear) — [link](https://www.tradezella.com/blog/tradezella-release-notes-july-august); Jan 2024 — [link](https://www.tradezella.com/blog/january-2024-release-notes); Feb 2024 — [link](https://www.tradezella.com/blog/tradezella-release-notes-february-2024); Apr 2024 — [link](https://www.tradezella.com/blog/april-2024-tradezella-updates); May 2024 — [link](https://www.tradezella.com/blog/whats-new-may-2024); Jun 2024 — [link](https://tradezella.com/blog/june-2024-release-notes); Jul 2024 — [link](https://www.tradezella.com/blog/new-in-july-2024); Aug 2024 — [link](https://www.tradezella.com/blog/august-2024-updates); Nov 2024 — [link](https://www.tradezella.com/blog/november-2024-release-notes); Dec 2024 — [link](https://www.tradezella.com/blog/whats-new-december-2024). Category index pages: [tradezella-updates](https://www.tradezella.com/category/tradezella-updates), [product-updates](https://www.tradezella.com/category/product-updates).
- Jan 2024: Backtesting launch + trade-page dark mode. — [January 2024 Release Notes](https://www.tradezella.com/blog/january-2024-release-notes)
- Feb 2024: custom tag categories. — [February 2024 Release Notes](https://www.tradezella.com/blog/tradezella-release-notes-february-2024)
- Spring 2024: Notebook redesign (note tags, search, templates); dashboard edit-widget flow. — [April 2024 Updates](https://www.tradezella.com/blog/april-2024-tradezella-updates); [What's NEW: May 2024](https://www.tradezella.com/blog/whats-new-may-2024)
- Jun 2024: tag management; planned left-panel redesign. — [June 2024 Release Notes](https://tradezella.com/blog/june-2024-release-notes)
- Dec 2024: Zella Score 2.0. — [What's NEW: December 2024](https://www.tradezella.com/blog/whats-new-december-2024)
- Jul 14, 2026: repricing to Essential/Pro/Ultra. — [Our pricing (article 8911582)](https://help.tradezella.com/en/articles/8911582-our-pricing); [TradeZella New Pricing](https://www.tradezella.com/blog/tradezella-pricing)
- The search tool explicitly reported finding "nothing from 2025 or 2026" among release-notes posts. — [TradeZella blog index](https://www.tradezella.com/blog)

### Inferences
- The Trade Replay feature page and "New in TradeZella: Replay your trades" post, plus the automated-backtesting guide, are undated in snippets but are 2025–2026 marketing; they are the best candidates for "recently added" features.

### Gaps
- Dedicated changelog URL and its 2025–2026 entries; any public roadmap or "coming soon" items; Wayback snapshots of the pricing/features pages (web.archive.org was blocked for both WebFetch and the proxy).

## Items from model background knowledge that could NOT be verified in this session (treat as hypotheses to confirm, not findings)
- Founder/CEO Umar Ashraf's YouTube walkthroughs are the primary first-party video tutorials; the brand's video channel content was not reviewable here.
- Trade-page features commonly attributed to TradeZella in prior years (trade rating, screenshots on trades, running P&L on the trade chart, "Zella Insights"-style automated observations, trade-sharing cards, mentor/sharing access) — none confirmed by any snippet in this session; do not report as fact without fetching the help center.
