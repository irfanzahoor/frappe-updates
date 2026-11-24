# New Frappe / ERPNext Apps — Useful Ones Only

Every new app found during daily research, in one place. Only apps that can actually help an ERPNext user or developer are listed here — with what it does, why it helps, **and the GitHub link + install command, so you don’t waste time finding it**.

## 2026-11-24

### RedLine — offline-first mobile app for ERPNext field sales reps
- **What:** Flutter mobile app (Android/iOS) that connects directly to your ERPNext site: sales orders, invoices, customers, collections, field visits with GPS, warehouse ops and approvals — with offline-first sync.
- **Why it helps:** Field sales and distribution teams — very common among ERPNext clients — can keep working without internet and sync when back online. A direct fit for distributors and trading businesses.
- **Note:** The UI is Arabic (RTL) only for now — English (LTR) is not available yet, so check language needs before promising it to a client.
- **License:** GPL-3.0.
- **GitHub:** https://github.com/abdullla00/Redline-Representative-App-ERPNEXT
- **Install:** Not a Frappe bench app — it’s a Flutter app. Get it on Google Play, or clone and build it: `git clone https://github.com/abdullla00/Redline-Representative-App-ERPNEXT`
- **Source:** https://discuss.frappe.io/t/introducing-redline-an-offline-first-mobile-app-for-erpnext-sales-representatives/165882

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
