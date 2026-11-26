# Integrations — Frappe / ERPNext Apps

> Part of the [Apps Catalog](../apps-catalog.md) — 11 apps in this category. Each app is short: what it does, why it helps, one **How we can use it** line for NexTash work, and the GitHub link + install command. Test on staging first.


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
