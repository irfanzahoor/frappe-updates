# Frappe / ERPNext Apps Catalog

> Every genuinely useful Frappe/ERPNext app found by global research up to 26 November 2026. Each app is short: what it does, why it helps, one **How we can use it** line for NexTash work, and the GitHub link + install command. Test on staging first; never promise a version you have not tested — entries marked "not stated" need a README check before proposing.
>
> **Already in [new-apps.md](new-apps.md) (not repeated here):** frappex-client, Vendalto, RedLine, Itemflow Community, Frappe Flow, Frappe Studio, Frappe Assistant Core, Raven v3, Orchestra AI, ChangAI, Zikpro AI Invoice OCR, Invoice OCR (free, Tesseract), Frappe Email Flow, DocStudio, VunaPOS, Lumen Restaurants, Auri PMS, Jarvis, mForm, Sales AI, Zikpro UK VAT, Tabadul, Compendium, ERPNext Sri Lankan Localisation, OHADA ERPNext Localisation.

---

## AI tools

### ERPSmith — AI dev copilot for ERPNext (MCP)
- **What/why:** lets Claude (or any MCP client) build and debug customizations on your site, with the user approving every change — less hand-written boilerplate.
- **How we can use it:** drive DocType and script work from Claude on client projects, with the approval gate as our review step; offer "AI-assisted customization" as a faster fixed-price service.
- **GitHub:** https://github.com/abhinavprakash1992/erpsmith — `bench get-app https://github.com/abhinavprakash1992/erpsmith` (Frappe v15/v16, free MIT)

### Ask ALYF — in-Desk AI assistant
- **What/why:** users ask questions and get help with documents inside the Desk, instead of raising a support ticket for every "where is…" question.
- **How we can use it:** bundle it into the handover package for first-time ERP users — it cuts our post-go-live support tickets.
- **GitHub:** https://github.com/alyf-de/ask_alyf — `bench get-app https://github.com/alyf-de/ask_alyf`

### ERPNext Copilot — plain-English queries, actions, charts, scheduled reports
- **What/why:** managers query data, get charts and scheduled reports in plain English — no SQL, no developer per report.
- **How we can use it:** sell it to owners and finance heads who ask for "just one more report" every week; a phase-2 add-on right after go-live, when report requests peak.
- **GitHub:** https://github.com/byt3crafter/erpnext-copilot — `bench get-app https://github.com/byt3crafter/erpnext-copilot`

### NextAssist — multi-provider AI chat assistant
- **What/why:** AI chat assistant running on OpenAI, Claude or Gemini (whichever the client already pays for), with a sandboxed code runner.
- **How we can use it:** propose it to clients who already pay for ChatGPT/Claude and ask "can the AI use our ERP data?" — no new vendor to sell.
- **GitHub:** https://github.com/navdeepghai/nextassist — `bench get-app https://github.com/navdeepghai/nextassist`

### Frappe Crema — LLM toolkit for Frappe (OCR + NL list views + scheduled AI tasks)
- **What/why:** one toolkit for OCR/document extraction into records, natural-language list views and edits, and scheduled AI tasks.
- **How we can use it:** make it our standard AI toolkit on client sites — OCR supplier bills in, plain-language list edits, nightly draft reports — one toolkit to learn instead of a different AI app per client.
- **GitHub:** https://github.com/amsys/crema — `bench get-app https://github.com/amsys/crema`

### HUF AI — open-source AI infrastructure for any Frappe app
- **What/why:** reusable multi-agent / AI-workflow layer for building bespoke AI features instead of one-off scripts.
- **How we can use it:** build custom AI workflows (auto-triage support emails, approve routine POs) on HUF instead of one-off scripts — the work becomes repeatable and billable as a productised service.
- **GitHub:** https://github.com/tridz-dev/huf — `bench get-app https://github.com/tridz-dev/huf`

### Frappe MCP — turn Frappe apps into MCP servers (official Frappe)
- **What/why:** the official building block for exposing any Frappe app to AI agents (Claude etc.) in a controlled way.
- **How we can use it:** the standard way to expose a client's custom app to Claude/ChatGPT — official Frappe code, so it is the safe choice to propose.
- **GitHub:** https://github.com/frappe/mcp — `bench get-app https://github.com/frappe/mcp`

### MCP ERPNext — MCP server with 97 tools (Casys-AI)
- **What/why:** the broadest ready-made tool surface (97 tools, 11 categories) for connecting agents to ERPNext, zero-config via npx.
- **How we can use it:** use it for quick AI-agent demos to clients ("ask Claude about your live stock") in a first meeting; move them to the official Frappe MCP route for production.
- **GitHub:** https://github.com/Casys-AI/mcp-erpnext — not a bench app; MCP server via npx.

---

## POS & Retail

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

## Invoicing & OCR

### ERPNext OCR — Tesseract OCR inside Frappe (Monogramm)
- **What/why:** free, self-hosted OCR building block — no AI vendor, no per-page fee.
- **How we can use it:** use it as the free OCR layer inside custom builds (scanned delivery notes, CNIC copies) for price-sensitive Pakistani clients.
- **GitHub:** https://github.com/Monogramm/erpnext_ocr — `bench get-app https://github.com/Monogramm/erpnext_ocr`

### ERP OCR Integration — AI invoice import via Drive / email / upload
- **What/why:** supplier invoices (PDF/photo) read by AI — supplier, lines, amounts, VAT extracted and matched — arriving via Drive, email or upload, nothing auto-posted.
- **How we can use it:** sell it to accounts teams drowning in supplier bills as a paid AP-automation add-on; the accountant stays in control because nothing posts automatically.
- **GitHub:** https://github.com/wphamman/erpocr_integration — no `bench get-app` stated in source; see the repo README / OCR Quick Start Guide.

---

## HR (beyond official Frappe HR)

**Baseline:** **Frappe HR / HRMS** (official) — https://github.com/frappe/hrms, `bench get-app hrms` — employee lifecycle, leave, attendance, expense claims, performance, payroll, recruitment; free GPL-3.0, v14–v16. **How we can use it:** sell HRMS as a standalone add-on to clients running ERPNext without HR; the ESS PWA at `/hrms` is a mobile attendance pitch for factories with shift workers.

### Discipline HR — attendance discipline & automated payroll penalties
- **What/why:** grace periods and automatic payroll deductions for late attendance — the rules every HR client asks for but HRMS does not ship.
- **How we can use it:** offer it to factories with shift workers where late-coming is a daily HR headache — it replaces the manual spreadsheet the HR head maintains today.
- **GitHub:** https://github.com/cre8tivMaxx/discipline_hr — `bench get-app https://github.com/cre8tivMaxx/discipline_hr`

### Biometric Attendance Sync Tool — ZKTeco fingerprint devices → ERPNext (official Frappe)
- **What/why:** polls biometric devices and syncs punches into Employee Checkin records — no manual CSV imports.
- **How we can use it:** include it in every HRMS proposal for factories/offices that already have ZKTeco machines — punches flow into auto-attendance, a quick win that makes the HR sale easier.
- **GitHub:** https://github.com/frappe/biometric-attendance-sync-tool — not a bench app; clone and run the Python sync scripts: `git clone https://github.com/frappe/biometric-attendance-sync-tool.git`

---

## CRM & Support (beyond official CRM / Helpdesk)

**Baselines:** **Frappe CRM** (official) — https://github.com/frappe/crm, `bench get-app https://github.com/frappe/crm` — leads/deals, Kanban pipeline, ERPNext invoicing link. **Frappe Helpdesk** (official) — https://github.com/frappe/helpdesk, `bench get-app https://github.com/frappe/helpdesk` (v14/v15/v16) — email tickets, SLAs, assignment rules, customer portal, knowledge base. **How we can use them:** make CRM the default sales app instead of ERPNext's legacy CRM module, and Helpdesk the default desk for any client whose support runs on a shared inbox (unlimited agents, no per-seat fee).

### WATI Integration — WhatsApp Business API via WATI, for CRM follow-ups
- **What/why:** sends WhatsApp messages on ERPNext events (new/save/submit/change) with templates — the channel clients in Pakistan/India/Gulf actually read.
- **How we can use it:** offer it to sales teams that chase leads on WhatsApp manually — follow-ups go out automatically on lead/order events.
- **GitHub:** https://github.com/bhavesh95863/wati_integration — `bench get-app https://github.com/bhavesh95863/wati_integration` (verify in repo README; also on Frappe Cloud Marketplace)

### IndiaMART Integration — IndiaMART enquiries → ERPNext Leads
- **What/why:** pulls IndiaMART enquiries into ERPNext as Leads automatically — no re-typing from spreadsheets.
- **How we can use it:** offer it to Indian manufacturers/traders (and Pakistani exporters listing on IndiaMART) — enquiries land in the CRM pipeline by themselves.
- **GitHub:** no public repo verified — Marketplace only (search "Indiamart ERPNext Integration" on https://cloud.frappe.io/marketplace)

### Mautic Integration — marketing automation (Dokos)
- **What/why:** contacts/leads sync with Mautic for campaigns, lead scoring and nurture emails — real marketing automation instead of ERPNext's basic email tools.
- **How we can use it:** offer it to B2B clients with a real sales pipeline who run campaigns from a spreadsheet or a separate tool.
- **GitHub:** https://github.com/dokos-io/mautic — `bench get-app https://github.com/dokos-io/mautic`

### GitHub Helpdesk Integration — GitHub issues/PRs ↔ Frappe Helpdesk
- **What/why:** links GitHub issues, PRs, comments and commits with Helpdesk tickets — no copy-pasting between helpdesk and repo.
- **How we can use it:** use it for NexTash's own support flow and offer it to software-company clients who run Helpdesk.
- **GitHub:** no public repo verified — Marketplace only (https://cloud.frappe.io/marketplace)

---

## Manufacturing

Note: ERPNext core already ships multi-level BOMs, work orders, job cards, Production Plan/MRP, subcontracting and quality inspection — these apps add industry or planning depth.

### Apparelo — garment manufacturing workflow
- **What/why:** cutting/stitching/packing stage workflows that generic work orders do not model — the industry layer for garment clients.
- **How we can use it:** pitch it to garment/textile exporters (Lahore, Faisalabad) instead of custom-building stage workflows — it turns a generic manufacturing sale into an industry-specific one.
- **GitHub:** https://github.com/aerele/apparelo — `bench get-app https://github.com/aerele/apparelo`

### AuMMS — gold manufacturing management
- **What/why:** gold/jewellery manufacturing (purity, wastage, making charges) — a real ERPNext niche in Pakistan/India/Gulf.
- **How we can use it:** offer it to gold/jewellery manufacturers in Pakistan and the Gulf — a niche where few ERP vendors compete.
- **GitHub:** https://github.com/efeone/aumms — `bench get-app https://github.com/efeone/aumms`

### ERPNext Frepple Integration — advanced production planning / APS
- **What/why:** pairs ERPNext with Frepple, the open-source advanced planning & scheduling engine, for constraint-based planning beyond built-in MRP.
- **How we can use it:** offer it as a phase-2 sale to larger factories that outgrow ERPNext's own Production Plan.
- **GitHub:** https://github.com/msf4-0/ERPNext-Frepple-Integration — `bench get-app https://github.com/msf4-0/ERPNext-Frepple-Integration`

### Agriculture — agriculture domain for ERPNext (official Frappe)
- **What/why:** crop/livestock management domain for agri-business clients, inside the same ERP.
- **How we can use it:** offer it to sugar mills, dairy farms and seed companies — a large Pakistani segment most ERP vendors ignore.
- **GitHub:** https://github.com/frappe/agriculture — `bench get-app https://github.com/frappe/agriculture`

---

## E-commerce

### Ecommerce Integrations — Shopify / Amazon / Unicommerce (official Frappe)
- **What/why:** official connectors — Shopify orders in as Sales Orders, stock syncs to Shopify, items upload as drafts; ERPNext stays the source of truth.
- **How we can use it:** the standard answer for any client with a Shopify store; offer it to e-commerce sellers reconciling Shopify and ERPNext manually today.
- **GitHub:** https://github.com/frappe/ecommerce_integrations — `bench get-app https://github.com/frappe/ecommerce_integrations`

### CAZ WooSync — real-time two-way WooCommerce ↔ ERPNext sync
- **What/why:** two-way sync of products, orders, customers, inventory, prices, invoices, refunds, coupons — real-time webhooks with polling fallback, multi-store, queue dashboard. Fills the gap (no maintained Frappe WooCommerce connector for v15/v16).
- **How we can use it:** offer it to every client running a WooCommerce store; the sync-health dashboard lets us support it properly.
- **GitHub:** https://github.com/codeatozcom/CAZ_WOOSYNC — `bench get-app https://github.com/codeatozcom/CAZ_WOOSYNC` (v14–v16, free MIT)

### WooCommerce Connector — WooCommerce sync (Libracore)
- **What/why:** the long-running alternative WooCommerce connector — worth comparing against CAZ WooSync before committing a client.
- **How we can use it:** test both connectors on a staging store and pick the one that fits the client's order volume and product count.
- **GitHub:** https://github.com/libracore/WooCommerceConnector — `bench get-app https://github.com/libracore/WooCommerceConnector`

---

## Integrations

### Frappe WhatsApp Suite — WhatsApp Business API + chat UI + chatbot (3 apps)
- **What/why:** three free apps that work together — WhatsApp Business Cloud API (direct via Meta, no middleman), a chat UI inside Desk, and a chatbot with keyword triggers and AI fallback.
- **How we can use it:** make it our standard WhatsApp offer — order updates, invoice alerts and support chats from inside ERPNext, no paid middleman. Demo the in-Desk chat UI to trading/distribution clients; it replaces the shared phone their sales team passes around.
- **GitHub:** https://github.com/shridarpatil/frappe_whatsapp · https://github.com/shridarpatil/whatsapp_chat · https://github.com/shridarpatil/frappe_whatsapp_chatbot — `bench get-app` each repo (all three on Frappe Cloud Marketplace)

### WABA Integration — WhatsApp Business Cloud API (official Frappe)
- **What/why:** the official Frappe WhatsApp route — the conservative choice when a client wants Frappe-maintained code.
- **How we can use it:** propose it when a client insists on official code; use the community suite above when they also want the chat UI and chatbot.
- **GitHub:** https://github.com/frappe/waba_integration — `bench get-app https://github.com/frappe/waba_integration`

### Payment Core — provider-neutral payment layer (Aerele)
- **What/why:** shared foundation for payment integrations — references, transaction lifecycle, settlement, payment pages, idempotency — so checkout/webhook code is not rewritten per gateway.
- **How we can use it:** adopt it as the foundation for every payment integration we build — payment work becomes repeatable instead of custom per client.
- **GitHub:** https://github.com/aerele/payment-core — `bench get-app https://github.com/aerele/payment-core --branch develop` (Frappe/ERPNext v16, free MIT)

### Stripe Payment — Stripe gateway on Payment Core (Aerele)
- **What/why:** hosted checkout, 3D Secure, subscriptions, signed webhooks — the modern Stripe route for Frappe/ERPNext.
- **How we can use it:** offer it to clients taking international payments/subscriptions through Stripe. Note: Stripe is not available locally in Pakistan, so this fits exporters and Gulf/UK/US-facing businesses, not local PKR collection.
- **GitHub:** https://github.com/aerele/stripe-payment — `bench get-app https://github.com/aerele/stripe-payment --branch develop` (requires Payment Core, free MIT)

### Razorpay Integration — Razorpay payments (official Frappe)
- **What/why:** the standard gateway for Indian clients — UPI/cards through Razorpay, wired into ERPNext Payment Requests.
- **How we can use it:** offer it to Indian clients (or Pakistani exporters selling into India) taking online payments.
- **GitHub:** https://github.com/frappe/razorpay_integration — `bench get-app https://github.com/frappe/razorpay_integration`

### Multi Payment Gateway — payment-choice page for the Webshop
- **What/why:** lists every enabled gateway (Razorpay, Stripe, PayPal, Braintree, Paytm, GoCardless, Cashfree, PayU, COD, bank transfer) at Webshop checkout instead of forcing one.
- **How we can use it:** add it to every Webshop build where the client wants to offer more than one payment option — a small add-on that removes a real checkout objection.
- **GitHub:** https://github.com/Kalvyai-erpnext/ki_erp_multi_payment — `bench get-app https://github.com/Kalvyai-erpnext/ki_erp_multi_payment --branch version-16` (ERPNext 16 only, free MIT)

### ERPNext Shipping — Packlink / LetMeShip / SendCloud shipping
- **What/why:** turns delivery notes into booked shipments with labels and rates instead of a separate shipping portal.
- **How we can use it:** offer it to e-commerce/retail clients who book shipments in a separate portal today — it closes the loop between selling and dispatch.
- **GitHub:** https://github.com/frappe/erpnext-shipping — `bench get-app https://github.com/frappe/erpnext-shipping`

### Twilio Integration — SMS/voice/WhatsApp via Twilio (official Frappe)
- **What/why:** the established SMS route for OTPs, order alerts and reminders when WhatsApp alone is not enough.
- **How we can use it:** use it for OTPs and delivery confirmations where SMS is still needed; Twilio charges per message, so price it into the client's running costs.
- **GitHub:** https://github.com/frappe/twilio-integration — `bench get-app https://github.com/frappe/twilio-integration`

### MSG91 Integration — MSG91 SMS gateway
- **What/why:** direct gateway app for MSG91, a widely used SMS provider in India.
- **How we can use it:** offer it to Indian clients already on MSG91 — SMS alerts on their existing provider and rates.
- **GitHub:** https://github.com/dhwani-ris/frappe_msg91_integration — `bench get-app https://github.com/dhwani-ris/frappe_msg91_integration`

### Frappe Microsoft 365 — Outlook / Teams / OneDrive sync
- **What/why:** two-way Outlook calendar sync, Teams meetings from Frappe Events, transcripts/recordings, Outlook mail over OAuth, Microsoft sign-in.
- **How we can use it:** offer it to corporate clients who live in Outlook/Teams — calendar and mail sync removes the "ERP is a separate island" objection.
- **GitHub:** https://github.com/Bizmap-Technologies-Pvt-Ltd/frappe_microsoft365 — `bench get-app https://github.com/Bizmap-Technologies-Pvt-Ltd/frappe_microsoft365` (Frappe v15/v16)

### ALYF Banking — bank integration & reconciliation (EBICS)
- **What/why:** bank feeds via EBICS plus a modern Bank Reconciliation tool — beats manual statement imports.
- **How we can use it:** only after verifying its status — Awesome Frappe flags this repo as "Archived", so test on staging first and do not promise it to a client until confirmed working.
- **GitHub:** https://github.com/alyf-de/banking — `bench get-app https://github.com/alyf-de/banking`

---

## Localisations

### Pakistan Localisation (official, ERPNext 15+)
- **What/why:** the official Pakistan app — tax setup, compliance and reporting for Pakistani businesses.
- **How we can use it:** install it on every Pakistani implementation by default — it is our home-market advantage over generic ERP vendors.
- **GitHub:** https://github.com/frappe/pakistan — `bench get-app https://github.com/frappe/pakistan`

### Saudi ZATCA e-Invoicing — e-invoicing compliance (Beveren)
- **What/why:** e-invoicing for the Saudi ZATCA standard.
- **How we can use it:** offer it to clients selling in Saudi Arabia (or Saudi exporters) — compliance is a hard requirement there, and the app's pricing is a conversation we can use to upsell.
- **GitHub:** https://github.com/Beveren-Software-Inc/ZATCA_Integration — `bench get-app https://github.com/Beveren-Software-Inc/ZATCA_Integration` (repo URL case is inconsistent between sources — verify exact path before installing)

### UAE VAT / ZATCA — Tax Authority e-invoicing for UAE
- **What/why:** e-invoicing compliance for UAE-based businesses (paid, licence per company per year).
- **How we can use it:** offer it to UAE clients — a compliance add-on that lets us serve the Gulf market properly.
- **GitHub:** no public repo verified — Marketplace only (https://frappecloud.com/marketplace/apps/uae-zatca-e-invoicing)

### Bahrain VAT — VAT integration for Bahrain
- **What/why:** VAT handling for Bahrain (paid app).
- **How we can use it:** offer it to Bahraini clients as part of a Gulf-market package alongside the UAE app.
- **GitHub:** no public repo verified — Marketplace only (search "Bahrain VAT" on https://cloud.frappe.io/marketplace)

### Indonesia Localisation — local accounting rules
- **What/why:** local compliance for Indonesian businesses (paid app).
- **How we can use it:** use it for Indonesian clients — an under-served market where localisation wins the sale.
- **GitHub:** no public repo verified — Marketplace only (search "Indonesia Localisation" on https://cloud.frappe.io/marketplace)

### Kenya Compliance (KRA eTIMS) — Kenya Revenue Authority integration
- **What/why:** KRA eTIMS e-invoicing integration for Kenyan businesses (paid).
- **How we can use it:** offer it to Kenyan clients — compliance is the deciding factor in that market.
- **GitHub:** no public repo verified — Marketplace only (search "Kenya Compliance" on https://cloud.frappe.io/marketplace)

### Portugal Localisation (Dokos) — PT tax + SAF-T
- **What/why:** Portuguese tax configuration, SAF-T reporting and related compliance.
- **How we can use it:** offer it to Portuguese clients — a European market with real localisation needs.
- **GitHub:** https://github.com/dokos-io/portugal — `bench get-app https://github.com/dokos-io/portugal`

### EU VAT (OSS) — EU VAT One Stop Shop
- **What/why:** handles EU VAT OSS for cross-border sales.
- **How we can use it:** offer it to clients selling across the EU — a genuine blocker without it.
- **GitHub:** https://github.com/alyf-de/eu_vat — `bench get-app https://github.com/alyf-de/eu_vat` (free, GPL-3.0)

### German Localisation (official Frappe) — German compliance
- **What/why:** official German localisation — DATEV and local tax handling.
- **How we can use it:** offer it to German clients — official Frappe code makes it the safe choice to propose.
- **GitHub:** https://github.com/frappe/german_localization — `bench get-app https://github.com/frappe/german_localization` (verify URL in repo README before installing)

### French Localisation (Dokos) — FEC reporting and French compliance
- **What/why:** FEC accounting files and French compliance (paid, ~€100/month).
- **How we can use it:** offer it to French clients — compliance is a hard requirement, and the monthly price is easy to justify.
- **GitHub:** https://github.com/dokos-io/france — `bench get-app https://github.com/dokos-io/france` (Frappe v15/v16)

### DACH Region / Swiss Localisation (Dokos) — Switzerland / DACH compliance
- **What/why:** Swiss/DACH accounting and compliance.
- **How we can use it:** offer it to Swiss/Austrian/German clients as part of a DACH package with the German app.
- **GitHub:** https://github.com/dokos-io/dach — `bench get-app https://github.com/dokos-io/dach`

---

## Developer tools

### Print Designer — drag-and-drop print format designer (frappe v14/v15 only)
- **What/why:** visual print format builder — no HTML/Jinja coding for invoices and reports.
- **How we can use it:** use it to design invoice/quotation formats quickly on v14/v15 clients. For v16, use the built-in print format designer (v16.50+) instead — Print Designer's v16 compatibility is unconfirmed, verify on staging first.
- **GitHub:** https://github.com/frappe/print_designer — `bench get-app https://github.com/frappe/print_designer`

### Bench Companion — VS Code extension for bench
- **What/why:** manages bench sites and development from VS Code — less terminal work for the team.
- **How we can use it:** install it for every NexTash developer — it standardises how the team works with bench sites.
- **GitHub:** https://github.com/vineetjacob/bench-companion — VS Code extension, not a bench app.

### Frappe VS Code — Frappe extension for VS Code (official Frappe)
- **What/why:** official VS Code tooling for Frappe development.
- **How we can use it:** standardise the team's editor setup on it — every developer works the same way.
- **GitHub:** https://github.com/frappe/vscode — VS Code extension, not a bench app.

### Frappe S3 Attachment — store attachments on S3
- **What/why:** moves attachments to S3, saving local disk and keeping backups clean.
- **How we can use it:** use it for clients with heavy attachments (photos, PDFs) — it keeps their servers lean and is a standard part of our hosting setup.
- **GitHub:** https://github.com/frappe/s3-attachment — `bench get-app https://github.com/frappe/s3-attachment`

### ERPNext Excel — Excel as a low-code layer
- **What/why:** lets users manage and analyse data in Excel while ERPNext stays the source of truth.
- **How we can use it:** offer it to finance teams that live in Excel — they keep their workflow, we keep the data in ERPNext.
- **GitHub:** https://github.com/frankmoney/erpnext_excel — `bench get-app https://github.com/frankmoney/erpnext_excel`

### ERPNext Import Tool — import via Excel + S3 (paid)
- **What/why:** a guided import tool for bulk data migration — for teams that struggle with the built-in Data Import.
- **How we can use it:** use it on migrations where the client's data is messy spreadsheets — it pays for itself in one go-live.
- **GitHub:** no public repo verified — Marketplace only (search "ERPNext Import Tool" on https://cloud.frappe.io/marketplace)

### Frappe Manager — local Docker-based Frappe development
- **What/why:** Docker-based local development without a full bench install — quicker onboarding for new developers.
- **How we can use it:** use it to onboard new NexTash developers fast — a working local site in minutes instead of a bench setup day.
- **GitHub:** https://github.com/rtcamp/Frappe-Manager — not a bench app; local development tool.

### ERPNext Admin Tools — bulk delete + cache controls for admins
- **What/why:** admin utilities (bulk delete, cache clearing) for support work.
- **How we can use it:** use it internally on client support calls — bulk cleanup without custom scripts.
- **GitHub:** https://github.com/brianlam38/erpnext-admin-tools — `bench get-app https://github.com/brianlam38/erpnext-admin-tools`

---

## Productivity

### Frappe Learning — LMS / academy inside Frappe (official Frappe)
- **What/why:** courses, lessons and quizzes inside the ERP — for training staff and clients.
- **How we can use it:** build the client training academy on it — onboarding courses for new users, with progress tracked. Also use it for NexTash's own onboarding.
- **GitHub:** https://github.com/frappe/learning — `bench get-app https://github.com/frappe/learning` (verify exact bench command in the repo README)

### Frappe Insights — BI dashboards (official Frappe)
- **What/why:** the official BI tool for Frappe/ERPNext — dashboards on live data, self-service for managers.
- **How we can use it:** sell an Insights dashboard package as the phase-2 sale after every go-live — sales, stock and finance dashboards, no more Excel exports. Note: v3.50 (Nov 2026) removed v2 — migrate v2 dashboards before upgrading.
- **GitHub:** https://github.com/frappe/insights — `bench get-app https://github.com/frappe/insights` (free MIT)

### Frappe Drive — file management + Google Docs clone (official Frappe)
- **What/why:** file storage and collaborative docs inside Frappe — a Google Drive/Docs replacement in the same system.
- **How we can use it:** offer it to clients paying for Google Workspace/SharePoint just for shared files — it keeps documents inside the ERP.
- **GitHub:** https://github.com/frappe/drive — `bench get-app https://github.com/frappe/drive`

### Frappe Gameplan — project management inside Frappe (official Frappe)
- **What/why:** project planning and tracking inside Frappe — for clients who run projects in a separate tool.
- **How we can use it:** offer it to service/project clients as a replacement for their separate project tool — one system instead of two.
- **GitHub:** https://github.com/frappe/gameplan — `bench get-app https://github.com/frappe/gameplan`

### Frappe Wiki — wiki / knowledge base (official Frappe)
- **What/why:** a wiki inside Frappe — documentation and SOPs where the team already works.
- **How we can use it:** build the client's SOP library on it during implementation — it becomes part of the handover and reduces support calls.
- **GitHub:** https://github.com/frappe/wiki — `bench get-app https://github.com/frappe/wiki`

### Frappe Email Flow — visual email automation builder
- **What/why:** visual builder for email flows — welcome sequences, reminders, follow-ups — without writing server scripts.
- **How we can use it:** offer it to sales/service clients who send the same emails manually every day — it automates the repetitive follow-ups.
- **GitHub:** https://github.com/Alex-Yablonsky/frappe-email-flow — `bench get-app https://github.com/Alex-Yablonsky/frappe-email-flow`

### Frappe Builder — no-code website & page builder (official Frappe)
- **What/why:** build marketing pages and customer portals visually — frappe.io itself is built with it; AI assistant "Bob" in the editor (Nov 2026); MIT licence from v1.31.0.
- **How we can use it:** deliver client marketing pages and portals as a fixed-price add-on to any implementation — no separate website project.
- **GitHub:** https://github.com/frappe/builder — `bench get-app https://github.com/frappe/builder`

### Frappe Cloud 2.0 — hosting rebuild (Pilot / Atlas / Central)
- **What/why:** the new Frappe Cloud — VMs with root/SSH, one-click apps, Object Storage, LLMs; public beta 24 Nov 2026, target Jan 2027; Bench archived.
- **How we can use it:** move hosting-migration clients to Cloud 2.0 VMs when it goes live — isolated VMs answer downtime complaints. Offer "Bench to Cloud 2.0" migration as a service.
- **GitHub:** no repo — Frappe Cloud product, https://discuss.frappe.io/t/frappe-cloud-2-0-is-in-public-beta/165969

---

## Gaps worth knowing

- **Pakistan payments (Easypaisa / JazzCash):** no free public Frappe app exists. ECOSIRE offers a build-to-order integration from ~$999 (https://ecosire.com/frappe-erpnext-payment-integration/). This is the biggest gap for local clients — a Payment Core integration for Easypaisa/JazzCash would be a genuine product opportunity for NexTash.
- **HR beyond official apps is thin:** no verified third-party recruitment/payroll app found; only Discipline HR and the biometric sync tool.
- **CRM beyond official apps is thin:** no verified standalone third-party Frappe CRM app found — the market relies on Frappe CRM itself.
- **Not verified / verify before proposing:** WooCommerce Fusion, Medusa, South African Localisation, Italian e-invoicing, multi-country Peppol, Paymob/SumUp/Paystack — no verified GitHub URL found. Print Designer v16 and Insights v16 compatibility unconfirmed. KSA ZATCA repo URL case mismatch (see entry). Frappe Learning/Builder exact bench commands — verify in repo README.

## Sources

- Frappe Cloud Marketplace — https://cloud.frappe.io/marketplace
- Awesome Frappe — https://github.com/frappe/awesome-frappe (v14/v15/v16, maintained by Frappe)
- Frappe Community Apps (2025) — https://github.com/frappe/frappe/wiki/Frappe-Community-Apps
- Frappe Forum — https://discuss.frappe.io/c/developers/5 and https://discuss.frappe.io/c/show-your-app/27
- GitHub search: `topic:erpnext` and `frappe` — https://github.com/search?q=topic%3Aerpnext&type=repositories
- ERPNext docs — https://docs.erpnext.com/docs/user/manual/en/erpnext
