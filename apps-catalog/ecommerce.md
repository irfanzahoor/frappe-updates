# E-commerce — Frappe / ERPNext Apps

> Part of the [Apps Catalog](../apps-catalog.md) — 3 apps in this category. Each app is short: what it does, why it helps, one **How we can use it** line for NexTash work, and the GitHub link + install command. Test on staging first.


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
