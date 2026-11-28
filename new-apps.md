# New Frappe / ERPNext Apps — Useful Ones Only

Every new app found during daily research, in one place. Only apps that can actually help an ERPNext user or developer are listed here — with what it does, why it helps, **and the GitHub link + install command, so you don’t waste time finding it**.

## 2026-11-28

### mypos — POS for coffee shop chains on Frappe/ERPNext v16
- **What:** A full point-of-sale app for coffee / drinks chains, built on ERPNext v16's own POS Invoice, POS Profile, shifts and accounting/stock — the app adds the counter operation layer: menu by Price List with sizes and paid toppings, takeaway/dine-in, walk-in customers, loyalty points, cash and VietQR/SePay bank transfer, kitchen screen (not started → done → completed, paid orders only), table cards, QR self-ordering from the phone, a customer-facing display, and an order-status TV board. Role-based workspaces (Cashier / Kitchen / Manager / Admin), shifts cannot close with open orders. Brand data lives on the Branch, so one install serves many branches. Tested on ERPNext 16.61.0. MIT licensed, with install and operations docs.
- **Why it helps:** POS is one of the most-requested ERPNext add-ons for retail and food clients, and this one is complete and documented rather than a scaffold — cashier, kitchen and customer screens in one app, on top of native POS Invoices so accounting stays clean. A ready-made offer for cafes, juice bars and small restaurant chains.
- **Note:** Payments are Vietnam-specific (VietQR via SePay) and prices are in VND — the payment methods would need swapping for Pakistani banks / QR payments, but the POS operation layer is generic.
- **GitHub:** https://github.com/bvt1207/mypos
- **Install:** `bench get-app https://github.com/bvt1207/mypos.git --branch version-16` then `bench --site <site> install-app mypos`
- **Source:** https://github.com/bvt1207/mypos

### erpnext-agent-tools — QuickBooks Online to ERPNext migration with full history, plus AI bookkeeping agents
- **What:** Moves a QuickBooks Online company to ERPNext with its full history, proven correct against QuickBooks' own numbers — a CLI (`eat migrate extract` takes a read-only snapshot of every record, monthly trial balances and the journal; `eat migrate plan` dry-runs every document to be created, in order, for review). Then AI agents work the books: read-only by default, writing only through proposals a person approves inside ERPNext, with every call audited. Comes with a 6-minute narrated video demoed on a real Intuit sandbox company. MIT licensed.
- **Why it helps:** QuickBooks-to-ERPNext migration is a classic NexTash service, and this tool does the hard part — verified full-history migration — plus a safe, auditable way to offer "AI bookkeeper" work on top of ERPNext. A strong demo for winning migration clients.
- **Note:** The Frappe app lives in the `frappe_app/` subfolder (app name `agent_tools`) — install from that folder, not the repo root; the migration CLI is the main entry point. Video: https://youtu.be/cfwKiii5rdk
- **GitHub:** https://github.com/nschwermann/erpnext-agent-tools
- **Install:** Frappe app in `frappe_app/` (app `agent_tools`); migration CLI `eat` per the repo README
- **Source:** https://github.com/nschwermann/erpnext-agent-tools

### servepos — open-source restaurant POS for ERPNext (Frappe app + desktop + waiter app)
- **What:** A restaurant POS: the Frappe app (41 doctypes) plus a Windows/macOS desktop POS and an Android waiter app, with guest menu and QR ordering. The project is mature — desktop releases are already at v2.19.3 — and was newly published on GitHub on 26 November 2026. AGPL-3.0.
- **Why it helps:** Restaurants are a natural ERPNext POS vertical, and this covers the whole flow (tables, kitchen, payments, guest menu) with ready-made desktop and mobile apps instead of just a web screen. A credible package to offer restaurant clients.
- **GitHub:** https://github.com/badeeltechnology/servepos
- **Install:** `bench get-app https://github.com/badeeltechnology/servepos --branch version-16` then `bench --site <site> install-app servepos` — desktop POS and waiter APK from the repo README
- **Source:** https://github.com/badeeltechnology/servepos

### washingtonia_attendance — ZKTeco ADMS push-protocol attendance gateway for Frappe/HRMS v16
- **What:** A ZKTeco attendance gateway that serves the ADMS `/iclock` endpoints itself (no nginx rewrite or proxy rule): terminals push punches, roster rows and biometric templates; the app keeps them as an append-only event log and projects punches into HRMS Employee Checkin records. The protocol ("wire") layer is stdlib-only and fixture-driven — every protocol rule is covered by a test fixture — with explicit invariants (persist, then acknowledge). Built for Frappe v16. MIT licensed, with CI and tests.
- **Why it helps:** ZKTeco devices are everywhere in Pakistani offices and factories, and pushing their attendance into HRMS is a constant implementation ask. This is a well-engineered, tested gateway instead of a one-off script — a ready-made piece for HRMS implementations.
- **GitHub:** https://github.com/azharul-islam/washingtonia_attendance
- **Install:** `bench get-app https://github.com/azharul-islam/washingtonia_attendance.git` then `bench --site <site> install-app washingtonia_attendance`
- **Source:** https://github.com/azharul-islam/washingtonia_attendance

### contract_management — Contract Lifecycle Management for ERPNext (evening)
- **What:** A Contract Lifecycle Management app for Frappe/ERPNext: contracts with a counterparty portal API, built with CI (install + unit tests on every push to `develop`) and Frappe Semgrep linting. MIT licensed. The README is short on feature detail, so treat the scope as "contracts + counterparty portal" until a pilot confirms more.
- **Why it helps:** Contracts (supplier agreements, customer contracts, renewals) are usually tracked in spreadsheets even at ERPNext clients — a CLM app inside ERPNext closes that gap, and the counterparty portal is a genuinely useful piece for letting the other side see their contract.
- **GitHub:** https://github.com/susan2610/contract_management
- **Install:** `bench get-app https://github.com/susan2610/contract_management --branch develop` then `bench --site <site> install-app contract_management`
- **Source:** https://github.com/susan2610/contract_management

## 2026-11-27

### Fossible HIS (Biograph) — open-source hospital information system on Frappe/ERPNext
- **What:** Production-grade Hospital Information System built natively on Frappe/ERPNext — EHR, OPD/IPD, ADT, bed management, LIS (LOINC), RIS (DICOM), pharmacy, billing and insurance/RCM, inventory, HR/payroll and accounting on one database and one API. A fork and enhancement of Marley Healthcare, by Tacten / FossibleWorks, launched publicly 24 November 2026. Standards: FHIR R4, HL7, DICOM, LOINC, ICD-10, SNOMED-CT; HIPAA-ready, ABDM/NABH support. Agent-ready via Hydra MCP (typed MCP tools over every doctype). GPL-3.0, $0 per-user fees, self-host anywhere; also a one-click install on Frappe Cloud.
- **Why it helps:** Hospitals and clinics are a strong ERPNext vertical — they need OPD/IPD, pharmacy, lab, billing and HR in one system, and this is exactly that, already built. NexTash can offer hospital implementations without building the clinical side from scratch, and existing ERPNext Healthcare knowledge transfers directly.
- **Note:** the repo was renamed from `biograph` to `HealthCentral`, default branch `biograph-fh`; the Frappe app inside is named `healthcare`. The product site calls it "Fossible HIS", the repo README calls it "Biograph" — same system.
- **GitHub:** https://github.com/Tacten/HealthCentral
- **Install:** `bench get-app https://github.com/Tacten/HealthCentral`
- **Source:** https://www.fossibleworks.com/products/fossible-his/ · launch listing: https://www.nicheloom.com/launches/115993/

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
