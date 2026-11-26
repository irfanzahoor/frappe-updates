# POS & Retail — Frappe / ERPNext Apps

> Part of the [Apps Catalog](../apps-catalog.md) — 5 apps in this category. Each app is short: what it does, why it helps, one **How we can use it** line for NexTash work, and the GitHub link + install command. Test on staging first.


### POSNext — modern offline POS for ERPNext (Vue 3)
- **What/why:** fast billing, multiple payments, discounts, offline mode, touchscreen UI, split payments, coupons/gift cards, shift cash reconciliation — the most credible built-in POS replacement.
- **How we can use it:** make it our default POS offer for retail and pharmacy clients — offline mode sells itself where internet is unreliable, and shift reconciliation replaces manual till counting.
- **GitHub:** https://github.com/BrainWise-DEV/POSNext — `bench get-app https://github.com/BrainWise-DEV/POSNext` (ERPNext v15+, free AGPL-3.0)

### POS Prime — modern POS, zero ERPNext modifications (v14/v15/v16)
- **What/why:** modern Vue 3 POS using only standard DocTypes — no custom fields or DocTypes, installs/uninstalls cleanly, so upgrades stay clean.
- **How we can use it:** propose it to risk-averse clients and clients still on v14 — "zero core changes" is the line that gets a yes from owners worried about upgrade breakage.
- **GitHub:** https://github.com/ravindu2012/pos-prime — `bench get-app https://github.com/ravindu2012/pos-prime` (v14/v15/v16, free)

### POS Awesome — open-source POS (Vue.js + Vuetify)
- **What/why:** the established community POS — widely deployed, so client teams already know it.
- **How we can use it:** use it when a client or their staff already knows POS Awesome from a previous site — no retraining. For v15 sites use the V15 fork.
- **GitHub:** https://github.com/yrestom/POS-Awesome — `bench get-app https://github.com/yrestom/POS-Awesome` · V15 fork: https://github.com/defendicon/POS-Awesome-V15

### TailPOS — offline-first POS
- **What/why:** simple offline-first POS for shops with unreliable internet.
- **How we can use it:** keep as a fallback for small shops where POSNext feels too heavy — but verify first: last activity noted Oct 2022, may be unmaintained. Only propose after a staging test.
- **GitHub:** https://github.com/bailabs/tailpos — `bench get-app https://github.com/bailabs/tailpos`

### X POS — offline-first POS, web / PWA / Electron
- **What/why:** fast, keyboard-driven, fully offline POS, also deployable as a desktop (Electron) app.
- **How we can use it:** offer it to retail/restaurant counters that want a real desktop till app rather than a browser tab.
- **GitHub:** https://github.com/kodlyft/xpos — `bench get-app https://github.com/kodlyft/xpos.git`

---
