# New Frappe / ERPNext Apps — Useful Ones Only

Every new app found during daily research, in one place. Only apps that can actually help an ERPNext user or developer are listed here — with what it does, why it helps, **and the GitHub link + install command, so you don’t waste time finding it**.

## 2026-11-26

### frappex-client — typed Python client for the Frappe / ERPNext REST API (sync + async)
- **What:** Open-source Python library for working with a Frappe/ERPNext site from outside code — backend services, scheduled jobs, data pipelines and bots. Typed sync `Client` and `AsyncClient` with identical methods, automatic pagination (`iter_list`), a typed exception per failure (`NotFoundError`, `PermissionDeniedError`, `ValidationError`, `RateLimitError`…), and safe retries — reads and 429s only, writes are never retried so a network error cannot create duplicate documents. Secure defaults: HTTPS only, certificate checks cannot be disabled, secrets never logged. Fully typed (`mypy --strict`), one dependency (`httpx`), Python 3.10+. Tested against Frappe v14, v15 and v16. MIT licensed, early release (0.1).
- **Why it helps:** The official `frappe-client` is archived and was never on PyPI, so integrations usually hand-write `requests` calls and re-solve pagination, error decoding and retry safety every time. This is the maintained replacement — very handy for NexTash integrations, sync jobs and bots talking to client ERPNext sites.
- **GitHub:** https://github.com/Padmapriyan27/frappex-client
- **Install:** Not a Frappe bench app — it is a Python package: `pip install frappex-client` — docs: https://frappex-client.zeal.ninja
- **Source:** https://discuss.frappe.io/t/frappex-client-a-typed-async-ready-python-client-for-the-frappe-erpnext-rest-api/165958

## 2026-11-25

### Vendalto — free Android app for taking ERPNext sales orders on the road (beta)
- **What:** Android app for salespeople: take sales orders on the phone and they land in ERPNext as submitted Sales Orders. It connects straight to your own ERPNext server through the standard REST API (API key/secret) — nothing to install on the server. Tested with ERPNext v16.
- **Why it helps:** Field sales teams taking orders on the road — a very common ask from distribution and trading clients. Free while in beta; Android only for now.
- **GitHub:** No public GitHub repo found — it is an Android app, not a Frappe bench app, so there is no `bench get-app` install.
- **Install:** Google Play: https://play.google.com/store/apps/details?id=com.vendalto.sales — website: https://vendalto.netlify.app/
- **Source:** https://discuss.frappe.io/t/vendalto-a-free-android-app-for-taking-erpnext-sales-orders-on-the-road-beta/165896

## 2026-11-24

### RedLine — offline-first mobile app for ERPNext field sales reps
- **What:** Flutter mobile app (Android/iOS) that connects directly to your ERPNext site: sales orders, invoices, customers, collections, field visits with GPS, warehouse ops and approvals — with offline-first sync.
- **Why it helps:** Field sales and distribution teams — very common among ERPNext clients — can keep working without internet and sync when back online. A direct fit for distributors and trading businesses.
- **Note:** The UI is Arabic (RTL) only for now — English (LTR) is not available yet, so check language needs before promising it to a client.
- **License:** GPL-3.0.
- **GitHub:** https://github.com/abdullla00/Redline-Representative-App-ERPNEXT
- **Install:** Not a Frappe bench app — it’s a Flutter app. Get it on Google Play, or clone and build it: `git clone https://github.com/abdullla00/Redline-Representative-App-ERPNEXT`
- **Source:** https://discuss.frappe.io/t/introducing-redline-an-offline-first-mobile-app-for-erpnext-sales-representatives/165882

### Itemflow Community — friendly item browser for teams new to ERPNext (v2.9.2)
- **What:** A community Frappe app that gives teams a familiar file-explorer-style interface for ERPNext items: search items, manage multi-UOMs, monitor stock thresholds, toggle product photos, and link documents (Sales Orders, Purchase Orders, Quotations, Purchase Receipts). It does not replace core ERPNext — it is an auxiliary front-end to make daily navigation less overwhelming while staff get trained. Latest release v2.9.2 (24 Nov 2026) focused on item search and selection.
- **Why it helps:** Client teams with no ERP experience often struggle with the standard Desk; this is a gentle on-ramp that can be shown to a client during onboarding. Built by a non-developer for their own small electrical-equipment business, so expect rough edges — check the code before promising it.
- **GitHub:** https://github.com/TheManuNext/itemflow-community
- **Install:** `bench get-app https://github.com/TheManuNext/itemflow-community`
- **Source:** https://discuss.frappe.io/t/itemflow-community-a-custom-frappe-erpnext-app-built-for-my-small-business/165365

## 2026-11-23

### Frappe Flow (alpha) — AI harness inside ERPNext
- **What:** Frappe’s own AI harness that runs alongside Frappe apps, inside Desk. Permission-aware.
- **Why it helps:** AI on your own ERP data, without sending data to a random tool. Still alpha — try on staging first.
- **GitHub:** https://github.com/frappe/frappe — Flow ships with Frappe Framework v16.60, no separate app to install.
- **Source:** https://frappe.io/blog/product-updates/announcing-framework-erpnext-and-frappe-hr-v1660

### Frappe Studio (now in Framework, not a separate app)
- **What:** Build complete apps and custom UIs without writing code. Merged into Frappe Framework in v16.60.
- **Why it helps:** Small internal apps (visitor register, checklist, sample tracker) can now be built by a business analyst, on the same database and permissions as ERPNext.
- **GitHub:** https://github.com/frappe/frappe — Studio ships with Framework v16.60. Open `/studio` on your site.
- **Source:** https://frappe.io/blog/product-updates/announcing-framework-erpnext-and-frappe-hr-v1660

### Frappe Assistant Core — MCP server for ERPNext (Claude / ChatGPT → ERPNext)
- **What:** Open-source MCP server that connects Claude and ChatGPT to your ERPNext site.
- **Why it helps:** Ask AI questions about your real ERP data, create records, and automate checks — with permissions.
- **Status:** 1,100+ installs on Frappe Cloud Marketplace, v15/v16, free core.
- **GitHub:** https://github.com/buildswithpaul/Frappe_Assistant_Core
- **Install:** `bench get-app https://github.com/buildswithpaul/Frappe_Assistant_Core`
- **Source:** https://erpnova.co/resources/blog/ai-in-erpnext-real-vs-marketing

### Raven v3 — team chat with AI agents (official Frappe app)
- **What:** Frappe’s official team chat, now with no-code AI agents and native iOS/Android apps.
- **Why it helps:** Agents in chat can create records, read receipts, and alert on documents — useful for support and operations teams.
- **GitHub:** https://github.com/frappe/raven
- **Install:** `bench get-app https://github.com/frappe/raven`
- **Source:** https://frappe.io/times/october-2026

### Orchestra AI for ERPNext
- **What:** AI assistant + scheduled routines inside ERPNext — chat with your ERP, and routines that run by themselves (reports drafted overnight, documents prepared).
- **Why it helps:** Daily reporting and follow-ups without manual work.
- **Requires:** Frappe/ERPNext v15 or v16.
- **GitHub:** No public GitHub repo found — install from the Marketplace only.
- **Marketplace:** https://cloud.frappe.io/marketplace/apps/concerto

### ChangAI — AI chatbot for ERPNext
- **What:** Ask business questions in plain English inside ERPNext, get answers without SQL.
- **Why it helps:** Managers and accounts teams can query stock, sales, and ledgers in plain language.
- **GitHub:** https://github.com/ERPGulf/changAI
- **Install:** `bench get-app https://github.com/ERPGulf/changAI`
- **Marketplace:** https://cloud.frappe.io/marketplace/apps/changai

### Zikpro AI Invoice OCR
- **What:** Extracts data from PDF/image invoices, validates totals and taxes, matches suppliers, creates Purchase Invoices.
- **Why it helps:** Accounts teams processing many supplier bills — less manual data entry.
- **Status:** Paid, v15/v16, 5 installs as of Nov 2026 — early, but real.
- **GitHub:** https://github.com/Zikpro/invoice-ocr-ai
- **Install:** `bench get-app https://github.com/Zikpro/invoice-ocr-ai`
- **Source:** https://erpnova.co/resources/blog/ai-in-erpnext-real-vs-marketing

### Invoice OCR (free, Tesseract-based)
- **What:** Free OCR for invoices, can auto-create Items.
- **Why it helps:** Same invoice-entry problem as above, free to try for simple invoices. Note: it auto-creates Items it can’t find — supervise that path.
- **Status:** Free, v15, 8 installs as of Nov 2026.
- **GitHub:** https://github.com/Mohtashim-1/Invoice-OCR
- **Install:** `bench get-app https://github.com/Mohtashim-1/Invoice-OCR.git`
- **Source:** https://erpnova.co/resources/blog/ai-in-erpnext-real-vs-marketing

### Frappe Email Flow
- **What:** Provider-neutral email queue rules, delays, and delivery-flow control for Frappe.
- **Why it helps:** Control when outgoing emails leave the Email Queue, without replacing SMTP or your provider.
- **Requires:** Frappe Framework v16.
- **GitHub:** https://github.com/Alex-Yablonsky/frappe-email-flow
- **Install:** `bench get-app frappe_email_flow https://github.com/Alex-Yablonsky/frappe-email-flow`

### New on Frappe Cloud Marketplace — October 2026
- **DocStudio, VunaPOS, Lumen Restaurants, Auri PMS, Jarvis, mForm, Sales AI, Zikpro UK VAT, Tabadul, Compendium** — plus ERPNext Sri Lankan Localisation and OHADA ERPNext Localisation.
- **Why it helps:** POS, restaurants, hotels (PMS), sales AI, and country localisations — check the ones matching your clients’ industries.
- **Marketplace:** https://cloud.frappe.io/marketplace
- **Source:** https://frappe.io/times/october-2026
