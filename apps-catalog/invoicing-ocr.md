# Invoicing & OCR — Frappe / ERPNext Apps

> Part of the [Apps Catalog](../apps-catalog.md) — 2 apps in this category. Each app is short: what it does, why it helps, one **How we can use it** line for NexTash work, and the GitHub link + install command. Test on staging first.


### ERPNext OCR — Tesseract OCR inside Frappe (Monogramm)
- **What/why:** free, self-hosted OCR building block — no AI vendor, no per-page fee.
- **How we can use it:** use it as the free OCR layer inside custom builds (scanned delivery notes, CNIC copies) for price-sensitive Pakistani clients.
- **GitHub:** https://github.com/Monogramm/erpnext_ocr — `bench get-app https://github.com/Monogramm/erpnext_ocr`

### ERP OCR Integration — AI invoice import via Drive / email / upload
- **What/why:** supplier invoices (PDF/photo) read by AI — supplier, lines, amounts, VAT extracted and matched — arriving via Drive, email or upload, nothing auto-posted.
- **How we can use it:** sell it to accounts teams drowning in supplier bills as a paid AP-automation add-on; the accountant stays in control because nothing posts automatically.
- **GitHub:** https://github.com/wphamman/erpocr_integration — no `bench get-app` stated in source; see the repo README / OCR Quick Start Guide.

---
