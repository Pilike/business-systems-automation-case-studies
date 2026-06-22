# Interview Questions By Company

Use this as a guided interview sheet. You do not need perfect memory or client names. Rough answers are useful if they clarify the business problem, your role, the systems involved, and the outcome.

## How To Answer

For each company/project, answer in this format:

- **Purpose:** what the business was trying to fix or improve.
- **Users:** who used it day to day.
- **Before:** what was manual, broken, duplicated, slow, or hard to track.
- **System:** what tools were involved.
- **Your work:** what you personally designed, configured, automated, or supported.
- **Outcome:** time saved, fewer mistakes, faster response, better sales, better visibility, fewer missed tasks.
- **Proof:** screenshots, fake-data recreation, diagrams, docs, rough numbers, or a story from rollout.

## Locwise / Noga

### Current Assumption

This is the flagship AI implementation project: an AI tender intelligence platform with scraping, document AI, Supabase/PostgreSQL, n8n, ASP.NET Core, matching, CRM, WhatsApp, email, onboarding, and production support.

### Questions

1. Who was the target user: business owner, sales team, tender writer, operations manager, or someone else?
2. What was the manual process before Noga existed?
3. How many tender sources or source types did the platform handle at peak?
4. Did clients receive daily/weekly reports, real-time alerts, portal dashboards, or all three?
5. What was the biggest technical challenge: scraping, Hebrew documents, matching accuracy, CRM/payment/onboarding, or production reliability?
6. Did Noga ever help a client identify a real tender opportunity they might have missed?
7. What parts did you build mostly yourself versus configure/integrate?
8. What would you improve in v2: matching accuracy, admin tooling, observability, onboarding, source config UI, or workflow reliability?

## Printer Service Operations

### Current Assumption

The business needed to turn service forms, warranty emails, and point-of-sale/lab collection requests into structured Fireberry CRM records. The workflows performed customer/product lookup, conditional record creation, service case creation, and routing.

### Questions

1. What was the main business pain: too many service emails, duplicate tickets, slow warranty intake, missing customer/product data, or poor lab handoff?
2. Who submitted requests: stores, resellers, customers, technicians, or internal staff?
3. Who used Fireberry after the automation created records?
4. What records were created or updated: account, contact, product, service case, collection request, warranty case?
5. Was the serial number the most important identifier?
6. What happened when the automation found an existing customer or product?
7. What happened when it did not find one?
8. Did the workflow reduce manual typing, response time, duplicate cases, or lost service requests?
9. Were Hebrew forms/emails the reason you needed parsing/code modules?
10. What edge cases do you remember: missing phone, bad serial number, multiple matching customers, missing invoice, unclear warranty?
11. Did you configure anything inside Fireberry, such as fields, views, forms, picklists, permissions, automations, or webhooks?
12. Can we safely say this was a "service operations intake automation"?

## German Property / Rental Operations Company

### Current Assumption

This is the strongest Make/Fireberry business-systems case. It looks like a rental/property operations CRM with lead intake, service requests, rental agreements, unit/publication linking, serial number generation, related-record updates, banking refresh, and AI-assisted email extraction.

### Questions

1. What kind of company was this exactly: property management, real estate rental, co-living, apartment leasing, or building purchase/rental operations?
2. What was the main business goal: faster rental lead handling, cleaner CRM data, service request automation, agreement generation, or operational reporting?
3. Who used the system: leasing team, operations team, finance, legal, property managers, or customer support?
4. What were the core CRM entities: property, unit, publication/listing, tenant, opportunity, rental agreement, service request, supplier offer, contract?
5. What was the rental lead inbox doing before automation?
6. Did leads arrive from email portals, website forms, listing platforms, manual forwarding, or all of these?
7. What did the AI extraction do: identify name/phone/email, listing code, desired unit, message intent, budget, move-in date, or language?
8. What happened after a lead was parsed?
9. Why was serial number generation needed?
10. Was serial generation tied to properties, units, agreements, accounting, or legal documents?
11. What did the rental agreement workflow create or update?
12. What did the "related records" updates solve? Was it keeping opportunity/rental agreement names in sync when a unit changed?
13. What was the Qonto/bank transaction refresh used for?
14. Did service requests include attachments/images, and did OCR/AI classify them?
15. What was the hardest part of this project?
16. Did you design the Fireberry object model or mainly automate on top of an existing one?
17. Any measurable result: faster lead response, fewer missed inquiries, cleaner CRM, reduced manual updates, better finance visibility?
18. Can we safely describe this as "rental operations CRM automation platform"?

## Law Firm

### Current Assumption

This project handled website lead intake and two-way synchronization between Fireberry and Outlook Calendar, including manual repair/test variants.

### Questions

1. What was the law firm's main problem: missed appointments, duplicate calendar entries, manual CRM updates, website lead follow-up, or poor visibility?
2. Was the calendar sync truly two-way, or was one direction primary and the other only for fixes?
3. What events were synced: consultations, court dates, internal tasks, client meetings, deadlines?
4. What Fireberry records did calendar events connect to: client, case, opportunity, task, appointment?
5. Did the workflow prevent duplicate Outlook events?
6. Did it handle event updates/cancellations?
7. Were there conflict cases where both Outlook and Fireberry changed?
8. What website lead fields were captured?
9. Did you create CRM contacts/opportunities/cases from website leads?
10. Did you configure Fireberry forms, fields, event types, or webhooks?
11. What was the business outcome: less manual scheduling, fewer missed meetings, better lead capture, cleaner client records?
12. Can we safely describe this as "CRM-calendar synchronization and legal lead intake"?

## Insurance / Tax Return / National Insurance Business

### Current Assumption

This was a lead automation system for a services business using Facebook Lead Ads, OpenAI extraction, Fireberry account/opportunity creation, customer product generation, and picklist utility flows.

### Questions

1. What services did the company sell: tax returns, national insurance claims, refunds, benefits, financial services, or something else?
2. What was the main pain: high lead volume, messy multilingual data, slow follow-up, duplicate records, manual product creation?
3. Which lead sources were used besides Facebook Lead Ads?
4. What languages did leads arrive in: Hebrew, English, Arabic, Russian, other?
5. What did OpenAI normalize: name, phone, email, service interest, eligibility, notes?
6. What made a lead "real" versus spam/test/unusable?
7. What CRM records were created: account, contact, opportunity, customer product, task?
8. What were "customer products" in this business?
9. Why were picklist value utilities needed?
10. Did the automation assign leads to sales reps or queues?
11. Did it trigger WhatsApp, SMS, email, or CRM follow-up?
12. Did it improve response speed or reduce manual entry?
13. Any rough volume: leads per day/week/month?
14. Can we safely describe this as "AI-assisted multilingual lead normalization and CRM opportunity automation"?

## Airtable Estimating And Bookkeeping System

### Current Assumption

This was a custom Airtable operating system for a production company, likely combining estimating, job tracking, expenses/bookkeeping, and management views.

### Questions

1. What kind of production company was it?
2. What was broken before Airtable: spreadsheets, WhatsApp, paper, disconnected accounting, no estimate history, no job costing?
3. Who used Airtable: owner, office admin, estimator, project manager, bookkeeper, field team?
4. What tables existed: customers, jobs, estimates, line items, expenses, invoices, payments, vendors, employees, tasks?
5. Did estimates generate PDFs, quote documents, emails, or approval links?
6. Did it track actual costs against estimated costs?
7. Did bookkeeping include receivables, payables, expenses, cash flow, taxes, or payment status?
8. Were there Airtable Interfaces or only base views?
9. Did you create forms for intake or expense submission?
10. Did you use Airtable automations/scripts?
11. Did it integrate with email, Google Drive, accounting, forms, or Make?
12. What outcome can we claim: faster estimates, cleaner bookkeeping, better job profitability visibility, fewer missed invoices?
13. Can you find any screenshots, design files, table names, or even a rough sketch?
14. Can we recreate the design with fake data for portfolio purposes?

## ADU Concepts

### Current Assumption

This was a Monday.com CRM migration/implementation for a design, engineering, and construction company. It included automated proposal/contract generation, SLA management, and helped improve sales close rates by roughly 30%.

### Questions

1. What system did ADU use before Monday.com?
2. What were the sales stages?
3. What types of deals were tracked: ADU design, permits, engineering, construction, consultations?
4. What was the biggest sales issue before your implementation: slow follow-up, lost leads, manual contracts, unclear ownership, no reporting?
5. How were proposals generated?
6. How were contracts generated?
7. Did you use Monday automations, integrations, templates, docs, formulas, or external tools?
8. What did SLA management mean in practice?
9. What reminders or escalations did sales reps/managers receive?
10. How was the 30% close-rate improvement measured?
11. Did you build dashboards for pipeline, close rate, aging leads, or rep performance?
12. Were there integrations with email, forms, file storage, e-signature, accounting, or phone systems?
13. What did you personally own: design, migration, board setup, automation, training, support?
14. Can we safely describe this as "sales operations CRM implementation for a construction/design firm"?

## Production Company Excel System

### Current Assumption

This was a discovery and systems-analysis project for a production company that had a complex Excel workbook acting as an operating system for productions, budgets, expenses, income, VAT, cash flow, petty cash, invoices, and reporting. It may connect to the Airtable estimating/bookkeeping story, but that needs confirmation.

### Questions

1. What was the company actually called publicly, and should we anonymize it?
2. Was this the same project as the Airtable estimating/bookkeeping system, or a separate production-finance analysis?
3. What was your exact role: analysis only, system design, Airtable build, Excel cleanup, automation, implementation, or handoff?
4. Was the goal to replace Excel with Airtable, improve Excel, or document requirements for another system?
5. Who used the workbook daily: producer, bookkeeper, production manager, owner, accountant, or office admin?
6. What was painful before the project: duplicate invoices, unclear cash flow, budget overruns, manual VAT calculations, petty cash chaos, or slow reports?
7. Did the system manage multiple productions at once?
8. Did each production have above-the-line and below-the-line budgets?
9. Were invoices split across productions or budget categories in real use?
10. Did the workbook track actual vs planned budget?
11. Did it track future expected income and expenses?
12. Did it support production phases such as pre-production, production, and wrap?
13. Were there multiple currencies or exchange-rate issues in the real process?
14. Did you design a new data model from this analysis?
15. Did you later build any part of it in Airtable?
16. Do you have screenshots, an Airtable base, a schema, or even a rough table list?
17. Any measurable result: faster reports, fewer errors, better cash-flow visibility, easier invoice tracking?
18. Can we safely describe this as "production operations and financial workflow system analysis"?

## Enterprise Retail CRM Proposal

### Current Assumption

This was a pre-sales/discovery CRM solution design with your boss. It mapped a potential Fireberry implementation for an enterprise retail prospect, including lead management, customer clubs, ERP integration, service-channel integrations, marketing consent, dashboards, permissions, API endpoints, sync jobs, and rollout milestones. The deal did not close, so it must be framed as solution design, not implementation.

### Questions

1. What was your personal contribution: discovery notes, diagrams, API planning, ERD, workflows, Hebrew doc writing, Fireberry scoping, or technical review?
2. Did you participate in client meetings, internal planning, or both?
3. Was Fireberry leading the sale and Locwise/you supporting implementation architecture?
4. What was the biggest business need: lead management, ERP integration, customer clubs, service-channel visibility, dashboards, or SLA control?
5. What was Comax supposed to provide: customers, orders, clubs, sales history, inventory, pricing, or all of these?
6. What was Glassix supposed to contribute: tickets, chats, calls, customer interactions, or service requests?
7. What was Inforu supposed to handle: subscription approvals, unsubscribe/subscribe events, SMS/email marketing consent?
8. Was Howazit a future phase for surveys and sentiment?
9. Did you design or help design the API endpoints?
10. Did you help estimate work effort, milestones, or implementation plan?
11. Were the warm/cold lead workflows based on client discovery or your proposed best practice?
12. Was role/permission planning part of your contribution?
13. What did you learn from the deal not closing?
14. Can we safely describe the prospect by industry and scale without naming the company?
15. Would you be comfortable discussing this as "pre-sales CRM solution architecture" in interviews?
16. Any artifacts we can safely recreate: anonymized architecture diagram, API endpoint table, process flow, roles matrix?

## LA Creative Design

### Current Assumption

This may be a lighter business systems/web operations case: website operations, Vtiger CRM, marketing, and support for engineering/design-company workflows.

### Questions

1. What did LA Creative Design sell or deliver?
2. What website work did you do: build, maintain, SEO, landing pages, forms, analytics, hosting?
3. What did Vtiger CRM handle?
4. Did you configure CRM fields, users, pipelines, forms, workflows, or reports?
5. Did website forms create CRM leads?
6. Did you support email marketing or campaigns?
7. Any measurable outcome: more leads, better tracking, easier operations, reduced manual admin?
8. Is there enough material for a case study, or should this stay as resume experience only?

## AutoManager

### Current Assumption

This is better as resume/LinkedIn proof than a GitHub project unless you can create a generalized case study about technical support, demos, cloud onboarding, and dealership CRM/DMS implementation.

### Questions

1. What products did you demo/support most often?
2. What did implementation involve for a new dealership?
3. What kinds of workflows did dealerships need configured?
4. What cloud/Azure tasks did you perform?
5. Did you support dealerships in the US/Canada?
6. Did you work with sales or implementation teams during demos?
7. What were common customer problems you solved?
8. Is there a good story showing technical consulting, not just support tickets?

## Final Portfolio Selection Questions

1. Which three projects do you feel most confident discussing in an interview?
2. Which projects have screenshots, diagrams, or artifacts we can safely recreate?
3. Which projects have measurable outcomes?
4. Which projects involved client discovery or stakeholder presentations?
5. Which projects did you build mostly yourself?
6. Which projects should stay anonymous because they are sensitive?
7. Which projects can be described publicly without naming the company?
