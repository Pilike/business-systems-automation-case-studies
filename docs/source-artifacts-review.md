# Source Artifacts Review

This note summarizes confidential artifacts reviewed for portfolio applicability. The source files themselves should not be committed.

## Production Company Excel Analysis

Source artifact: Word document describing existing Excel functionality for a production-management workflow.

### Public Portfolio Use

Useful as a case study about requirements discovery and operational system modernization. The artifact documents a real business operating model with production budgets, expenses, income, VAT, petty cash, dashboard metrics, and production reporting.

### Safe Public Framing

> Analyzed an Excel-based production management system and translated its existing workbook logic into a structured requirements map for a future operational system.

### Key Capabilities Identified

- Executive dashboard for annual/monthly expected income and expenses.
- Cash-flow tracking by production.
- Paid and future expense/income tracking.
- VAT calculations.
- Petty cash tracking.
- Production setup fields such as episodes, minutes per episode, overhead, contingency, and approved budget.
- Above-the-line and below-the-line budget categories.
- Invoice splitting across productions and budget categories.
- Duplicate invoice detection needs.
- Multi-currency and exchange-rate improvement opportunities.
- Reporting for production status, income/expense, cash flow, petty cash, and budget variance.

## Legacy Production Finance Workbook

Source artifact: Macro-enabled Excel workbook used as a production finance and operations system.

### Public Portfolio Use

Useful as proof of systems analysis depth. The workbook confirms that the production-company case was not a simple estimate tracker; it included real operating logic across budgets, ledgers, dashboards, templates, office overhead, petty cash, VAT, and cash-flow forecasting.

### Safe Public Framing

> Reviewed a macro-enabled production finance workbook and reconstructed its core data model into a public-safe system blueprint for a future Airtable or business-systems implementation.

### Key Capabilities Identified

- 26-sheet workbook with dashboard, income ledger, expense ledger, lookup/configuration tables, office overhead, budget templates, and production-specific sheets.
- Workbook formulas, data validations, tables, chart objects, pivot artifacts, and VBA content.
- Dashboard rollups for budgets, paid income, paid expenses, future income, future expenses, cash-flow balance, profit/loss, and petty cash.
- Expense ledger fields for production, category, budget item, invoice number, invoice name, description, invoice date, payment terms, payment method, payment date, payment status, VAT treatment, amount before VAT, VAT amount, and final paid amount.
- Income ledger fields for production, payer, payment date, status, milestone, VAT treatment, amount before VAT, VAT amount, final received amount, and invoice reference.
- Production templates with metadata, above-the-line budget sections, below-the-line budget sections, planned vs. actual formulas, and remaining budget calculations.
- Lookup/configuration concepts for currencies, budget formats, production types, VAT rules, payment methods, and production lists.

### Public Safety Notes

Do not publish the workbook, screenshots from the workbook, real sheet names, real production names, vendor names, invoice rows, financial values, macros, or formulas. Use the reconstructed data model and synthetic sample data instead.

## Enterprise Retail CRM Solution Design

Source artifact: CRM solution design PDF for a large retail prospect. The deal did not close, so this should be framed as pre-sales/discovery/solution architecture, not implementation.

### Public Portfolio Use

Useful as evidence of enterprise solution design, CRM architecture, API planning, stakeholder discovery, and implementation planning. This should not be presented as a delivered production project.

### Safe Public Framing

> Supported a pre-sales CRM solution design for an enterprise retail prospect, mapping lead management, ERP integration, customer clubs, customer feedback, service interactions, dashboards, roles, permissions, and rollout milestones.

### Key Capabilities Identified

- Fireberry CRM for accounts, opportunities/leads, tasks, orders, dashboards, and roles.
- ERP integration through a custom API layer.
- Batch sync for systems without webhooks.
- Lead intake from landing pages, web forms, QR codes, manual entry, cold lead uploads, and service channels.
- Duplicate detection by phone/email/customer data.
- Warm and cold lead workflows with SLA stages.
- Customer club membership objects.
- Glassix event/ticket intake into CRM opportunities.
- Inforu subscription/unsubscription integration.
- Future survey/feedback integration with sentiment reporting.
- Role-based dashboards for headquarters, regional managers, managers, and agents.
- Implementation plan with ERD setup, API skeleton, data loading, automations, training, go-live, sync, dashboards, and handoff.
