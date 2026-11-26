# Developer tools — Frappe / ERPNext Apps

> Part of the [Apps Catalog](../apps-catalog.md) — 8 apps in this category. Each app is short: what it does, why it helps, one **How we can use it** line for NexTash work, and the GitHub link + install command. Test on staging first.


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
