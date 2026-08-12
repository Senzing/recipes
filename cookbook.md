# The Senzing Cookbook

Build a working Senzing solution - fraud, customer 360, compliance, and more - by handing plain-English prompts to an AI coding assistant. It does the work; **you don't write code, you paste prompts and watch it cook.**

Each recipe stands up a working Senzing solution - linking the records that refer to the same person or organization across your data sources - through a short sequence of prompts. Recipes are starting points, not gospel: swap in your own data sources and adjust as you go.

You're the **chef**; the **sous-chef** is an AI assistant interpreting each prompt in the moment, backed by the **kitchen staff** - the Senzing MCP, a brigade of specialists. Your result won't be identical to the demo, but it'll usually be close.

> **First time?** Do the one-time [setup](getting-started.md) first - an AI coding assistant, the **Senzing MCP**, and a **Senzing license**. Do it once, then every recipe is just paste-and-cook.

**Filter by** use case, difficulty, or kitchen.

## The recipes

### [Combine Data Sources & Explore Hidden Connections in PPP Loan Data](recipes/clair-data-ingestion-starter.md)
*Foundational · Easy · Local · ~30m · Clair Sullivan*

**What you'll make:** ingest two public data snapshots and get a markdown merge report; optionally serve it in a web visualizer; then fold in a third dataset and refresh.

### [Customer 360 from CRM + Orders](recipes/customer-360-crm-online.md)
*Customer 360 · Intermediate · Local · ~45m · Clair Sullivan*

**What you'll make:** resolve a CRM export and an online-orders feed into one unified customer per person, then serve it as a 360 app - unified profile, complete order and account history, possible-duplicate review, and search.

### [Healthcare Exclusion Screening](recipes/nigel-healthcare-aws-entity-browser.md)
*Compliance · Advanced · AWS · a few hours · Nigel DeFreitas*

**What you'll make:** map two provider datasets, deploy an AWS pipeline, run Senzing V4 ER and export; serve it in an Entity Browser; then add OIG LEIE exclusions and flag excluded providers.
