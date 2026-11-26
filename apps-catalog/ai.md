# AI tools — Frappe / ERPNext Apps

> Part of the [Apps Catalog](../apps-catalog.md) — 8 apps in this category. Each app is short: what it does, why it helps, one **How we can use it** line for NexTash work, and the GitHub link + install command. Test on staging first.


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
