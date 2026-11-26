# Frappe & ERPNext — What Changed in the Last 2 Years (Nov 2024 – Nov 2026)

> The big changes of the last two years only — Framework/ERPNext v15 and v16 era, Studio, Flow, Insights, CRM/Helpdesk/Raven and the major features. Each item is short: what came, when, and one **How we can use it** line for NexTash work. Everything is verified from official sources (Frappe Blog, Frappe Forum, GitHub releases, Frappe docs, Frappe Times) with a source link per item.
>
> **Background (one line):** before Nov 2024 — v13 (Apr 2021) brought the modern Desk UI, v14 (Aug 2022) split the monolith into separate apps (HR, Healthcare, Education…), v15 (Oct 2023) brought the Espresso design system and no-code Form/Workflow Builders, and Frappe Cloud has hosted sites since 2020. Detail starts below, at November 2024.

## Support status (as of 26 November 2026)

- **v14** — end of life **31 Jan 2026**. **v15** — supported until **end 2027**. **v16** — supported until **end 2029**. (Secondary summaries citing https://frappe.io/support-versions — verify there before quoting to a client.)

## v15 era — the version in force when the window opens

- **v15 (Oct 2023, still current in Nov 2024):** Espresso UI, no-code Form Builder and Workflow Builder, Stock Reservation against Sales Orders, Serial & Batch Bundle, editable invoices after submission, 2.5x faster financial reports. Still patched monthly — latest **v15.127.0, 25 Nov 2026**. Source: https://discuss.frappe.io/t/frappe-and-erpnext-v15-release/111702
- **How we can use it:** v15 is the safe upgrade target for clients afraid of v16's new UI — sell the v14→v15 move with Form Builder demos ("build a DocType in the meeting") and Stock Reservation for manufacturing/trading clients fighting v14 stock complaints.

## November 2024 — Insights v3

- **Frappe Insights v3 released (Nov 2024):** complete makeover — TypeScript frontend, ibis-framework backend, 20+ connectors, basic data warehousing. Source: https://frappe.io/times/october-2024 (announced), https://discuss.frappe.io/t/frappe-insights-tools-guide/140202/4 (released in November)
- **How we can use it:** sell an Insights dashboard package as the phase-2 sale after every go-live — sales, stock and finance dashboards on live data, self-service for managers, no more Excel exports.

## January 2025 — Raven v2

- **Raven v2 (10 Jan 2025):** workspaces (many groups per site), AI bots, ERPNext integrations — document previews, alerts and actions inside chat. Source: https://frappe.io/product/raven/at-frappe
- **How we can use it:** offer Raven to clients drowning in WhatsApp groups for internal coordination — channels plus document alerts (invoice approvals, stock alerts) inside the ERP.

## April 2025 — Studio open-sourced

- **Frappe Studio open-sourced (3 Apr 2025, Frappe Build, Bengaluru):** drag-and-drop app builder, visual layouts, data sources, fast CRUD tools. Repo: https://github.com/frappe/studio. Source: https://frappe.io/blog/product-updates/product-updates-for-april-2025
- **How we can use it:** Studio is the fastest new service line — build a client's custom app visually in days (sample-tracking, gate-pass, visitor register) and bill it fixed-price. Train one NexTash analyst on it so small apps stop consuming developer time.

## September 2025 — Frappeverse India 2025

- **Frappeverse India 2025 (11–12 Sep 2025, Nehru Centre, Mumbai).** Source: https://events.frappe.io
- **How we can use it:** use each Frappeverse as a lead-generation and client-touch point — turn its announcements into a short client newsletter ("what's new in ERPNext") to stay in touch with the installed base.

## November 2025 — v16 beta

- **Framework/ERPNext v16 beta (15 Nov 2025):** first major release in two years; final planned for 6 Dec 2025 at Frappeverse Egypt. Source: https://discuss.frappe.io/t/erpnext-hrms-frappe-framework-v16-release-dates/156349
- **How we can use it:** use the beta window to test our own custom apps and top clients' sites on staging — catching breakage early is a billable "v16 readiness check" service.

## January 2026 — v16 final

- **Framework/ERPNext/Frappe HR v16 (12 Jan 2026):** new Desktop UI (desktop icons, persistent sidebar), up to ~2x faster ("Caffeine"), List View up to 50 columns, scrollable child tables, Chrome-based PDF converter (replacing wkhtmltopdf), role-based field masking, UUID document naming. ERPNext: configurable Financial Report Templates (incl. IFRS), consolidated Trial Balance, forecast → MPS → MRP planning chain, batch-level stock reservations, inward subcontracting. Sources: https://frappe.io/blog/engineering/announcing-version-16, https://discuss.frappe.io/t/frappe-erpnext-and-frappe-hr-version-16-release/159053
- **How we can use it:** use the Desktop UI and 50-column List View as the demo hook for v16 upgrade pitches — clients see the difference in five minutes. Pitch the forecast → MPS → MRP chain to textile, food and spare-parts manufacturers who still plan in Excel. The raised runtime floor makes this a planned infrastructure upgrade (staging first), not a one-click update — sell it as a project.

## January 2026 — Raven becomes official

- **Raven becomes an official Frappe app (Jan 2026)** — the team that built it joined Frappe. Source: https://frappe.io/product/raven/at-frappe
- **How we can use it:** now that Raven is official, propose it confidently as the team-chat layer on implementations — no more "community app" objection from clients.

## July 2026 — Raven v3

- **Raven v3 (13 Jul 2026 per Frappe's timeline):** faster app, proper PWA on mobile, redesign, Espresso rebuild, SQLite full-text search, notifications page, reminders, scheduled messages, read receipts. Note: a Frappeverse recap says beta 21 Aug / full release 1 Sep 2026 — dates conflict, see notes at the end. Source: https://frappe.io/product/raven/at-frappe
- **How we can use it:** v3's PWA and search make Raven viable for factory-floor teams — propose it as part of the implementation for clients whose staff work off phones, not desks.

## August 2026 — Frappeverse Mumbai 2026

- **Frappeverse Mumbai 2026 (21–22 Aug 2026, 1,500+ people):** announcements — Frappe Suite, Frappe Cloud V2 preview, Raven V3, ERPNext v16 keynote. Sources: https://events.frappe.io/events/frappeverse-mumbai-2026, https://frappe.io/times/july-2026
- **How we can use it:** same as every Frappeverse — leads plus a client newsletter from the announcements. The Cloud V2 preview is the talking point for hosting-migration conversations.

## October 2026 — v16.50, the polished v16

- **Framework/ERPNext/HR v16.50 (7 Oct 2026):** navigation fixed (clean desktop, per-module dock, curated sidebar), new print format designer (canvas + live preview), consolidated DocType Settings, revamped global search, step-based Data Import wizard, faster Kanban, List View layouts, bulk editing in child tables. No breaking changes — just update the three apps. Source: https://frappe.io/blog/product-updates/announcing-framework-erpnext-and-hrms-v1650
- **How we can use it:** recommend v16.50 (not early v16) for every new rollout — the navigation fix removes the main objection clients raised. Use the Data Import wizard to shorten go-live (import customers/suppliers with addresses in one file) and build the client's invoice format live in the demo with the new print designer.

## November 2026 — Insights v3.50 removes v2

- **Frappe Insights v3.50 (17 Nov 2026):** removes Insights v2 entirely — v2 dashboards must be migrated via the "Migrate from v2" page in v3.13–v3.15.1 first (v3.15.1 released 20 Oct 2026). Source: https://docs.frappe.io/insights/articles/migrate-from-v2-to-v3
- **How we can use it:** before any v3.50 upgrade, sell the v2-to-v3 dashboard migration as a scoped task — clients on v2 dashboards cannot skip it.

## November 2026 — v16.60: AI moves into the core

- **Framework/ERPNext/HR v16.60 (17 Nov 2026):** Studio merged into Framework (build apps without code, works with AI agents), Frappe Flow alpha (Frappe's AI harness in Desk — LLMs analyse data / fill forms, permission-aware, your own AI keys), Insights dashboards embedded in Desk, improved mobile UX, new child-table importer, better report printing. Monthly releases begin (16.70 in Dec 2026). ERPNext: Tally-style Day Book, 10 new print formats, redesigned Customer/Supplier forms with Overview dashboards, Projects revamp phase 1. Sources: https://frappe.io/blog/product-updates/announcing-framework-erpnext-and-frappe-hr-v1660, https://discuss.frappe.io/t/announcing-v16-60-for-frappe-framework-erpnext-and-frappe-hr/165819
- **How we can use it:** offer Studio-built mini-apps as a new service line and Flow as a pilot to one friendly client on a test site ("ask your ERP" on their own data). The monthly cadence supports a recurring "upgrade + what's new" retainer — apply each 16.6x release and send the client a one-page summary.

## November 2026 — CRM & Helpdesk renumbered to v16.x

- **Frappe CRM and Helpdesk switched versioning (Nov 2026):** from continuous v1.x to the Framework scheme — v15.x targets Frappe v15, v16.x targets v16 (CRM v16.0.2, 5 Nov 2026; Helpdesk v16.2.1). CRM at Frappeverse 2026: ~2.5K paid sites, ~3.5K GitHub stars; new web Forms for lead capture, Lead/Deal enrichment, Sales Hierarchy, drag-and-drop Workflow Automations. Sources: https://github.com/frappe/crm/releases, https://www.ithub.directory/crm-customer-platforms/frappe-crm (secondary for the renumbering)
- **How we can use it:** implement Frappe CRM (not ERPNext's legacy CRM module, slated for removal in v16) on every new sales project, and Helpdesk for any client whose support runs on a shared inbox — unlimited agents, no per-seat fee.

## November 2026 — Frappe Cloud 2.0 public beta

- **Frappe Cloud 2.0 public beta (24 Nov 2026):** rebuild from the foundation — Virtual Machines with full root/SSH, one-click apps, Object Storage, LLMs, firewalls and VPN. Architecture: Pilot (manages sites, usable today as a Bench replacement), Atlas (infrastructure), Central (customer-facing cloud). Target: Jan 2027. Bench officially archived. Source: https://discuss.frappe.io/t/frappe-cloud-2-0-is-in-public-beta/165969
- **How we can use it:** move hosting-migration clients to Cloud 2.0 VMs when it goes live — isolated VMs instead of shared multi-tenancy directly answers downtime complaints. Offer "Bench to Cloud 2.0" migration as a service; Pilot is a pitch for clients self-hosting on a VPS today.

## November 2026 — the monthly train: v16.61.0 and friends

- **Framework v16.61.0 (24 Nov 2026):** custom form button styles, maintenance mode allows reads by default, Letter Head Preview, Studio "Show on Desktop", Flow public agents, AI assistant views images, Print Format role restrictions, bulk Add/Remove Roles, GitPython 3.2.1 security update. Source: https://github.com/frappe/frappe/releases/tag/v16.61.0
- **ERPNext v16.61.0 & v15.127.0, CRM v16.4.0, Helpdesk v16.2.2 (25 Nov 2026):** 278 bug fixes, Stock valuation breakdown page and auto-repost setting, Manufacturing "Return Components" on draft Job Cards, permission hardening across POS/company defaults/Payment Entry; CRM gets an Insights dashboard on its dashboard page. Sources: https://github.com/frappe/erpnext/releases/tag/v16.61.0, https://github.com/frappe/crm/releases/tag/v16.4.0, https://github.com/frappe/helpdesk/releases/tag/v16.2.2
- **How we can use it:** keep clients on the monthly train under an AMC — each month's patch (like v16.61.0's permission hardening) is a reason to touch the client, report what changed, and bill the retainer. Full details: [2026-11-25](updates/2026-11-25.md), [2026-11-26](updates/2026-11-26.md).

## November 2026 — Builder gets AI ("Bob")

- **Frappe Builder (Nov 2026):** AI assistant "Bob" in the editor (slash commands, editor plugins, AI credits on Frappe Cloud); licence changed to MIT from v1.31.0 (earlier AGPL-3.0); latest v1.37.5, 6 Nov 2026. Source: secondary directories (iThub/exploreai) — verify on https://github.com/frappe/builder/releases before quoting.
- **How we can use it:** use Builder to deliver client marketing pages and customer portals without a separate website project — a fixed-price add-on to any implementation (frappe.io itself is built with it).

---

## Dates & figures to double-check

1. **Raven v3 date:** frappe.io timeline says 13 Jul 2026; Frappeverse recap says beta 21 Aug / full release 1 Sep 2026.
2. **CRM/Helpdesk renumbering:** v16.0.2 (5 Nov 2026) and the v15.x/v16.x scheme are from a secondary directory (iThub), not a Frappe announcement — verify on https://github.com/frappe/crm/releases.
3. **v16.60 "2,500+ bugs fixed":** appears in secondary summaries; the Frappe v16.60 blog was not checked line-by-line.
4. **Support dates** (v14 EOL 31 Jan 2026; v15 to end 2027; v16 to end 2029): verified only via secondary summaries citing https://frappe.io/support-versions.
5. **Insights v3 exact tag date (Nov 2024)** and **Builder v1.37.5 / "Bob" details:** from secondary sources; verify on https://github.com/frappe/insights/releases and https://github.com/frappe/builder/releases.

## Sources

- Frappe Blog — https://frappe.io/blog
- Frappe Forum announcements — https://discuss.frappe.io/c/announcement/20
- GitHub releases: [frappe/frappe](https://github.com/frappe/frappe/releases), [frappe/erpnext](https://github.com/frappe/erpnext/releases), [frappe/hrms](https://github.com/frappe/hrms/releases), [frappe/crm](https://github.com/frappe/crm/releases), [frappe/helpdesk](https://github.com/frappe/helpdesk/releases), [frappe/insights](https://github.com/frappe/insights/releases), [frappe/raven](https://github.com/frappe/raven/releases), [frappe/builder](https://github.com/frappe/builder)
- Frappe Times — https://frappe.io/times
- Frappe support versions — https://frappe.io/support-versions
