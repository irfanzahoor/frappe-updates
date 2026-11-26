# CRM & Support — Frappe / ERPNext Apps

> Part of the [Apps Catalog](../apps-catalog.md) — 4 apps in this category. Each app is short: what it does, why it helps, one **How we can use it** line for NexTash work, and the GitHub link + install command. Test on staging first.


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
