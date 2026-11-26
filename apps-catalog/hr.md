# HR — Frappe / ERPNext Apps

> Part of the [Apps Catalog](../apps-catalog.md) — 2 apps in this category. Each app is short: what it does, why it helps, one **How we can use it** line for NexTash work, and the GitHub link + install command. Test on staging first.


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
