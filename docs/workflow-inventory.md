# Workflow Inventory

This inventory is based on a local review of Make blueprint exports. Raw exports are not included because they contain private webhook URLs, customer-data mappings, credential placeholders, CRM object names, and business-specific implementation details.

## Summary

| Area | Blueprint count | Main systems | Case study signal |
| --- | ---: | --- | --- |
| Printer service operations | 4 | Make, Fireberry, email/webhook intake, regex/code parsing | Service intake and warranty automation for a distributor/service team. |
| Real estate rental operations | 9 | Make, Fireberry, Outlook/email, HTTP APIs, AI extraction, banking refresh | Rental operations CRM automation and multi-source lead/service workflow system. |
| Law firm operations | 5 | Make, Fireberry, Outlook Calendar, website forms | Calendar sync and lead intake for a legal services workflow. |
| Insurance/tax lead automation | 3 | Make, Fireberry, Facebook Lead Ads, OpenAI, picklist utilities | Lead normalization, multilingual extraction, opportunity creation, and product automation. |

## Notable Workflow Patterns

### Printer Service Operations

- Email and webhook intake for service request forms.
- Hebrew field extraction and normalization.
- Customer lookup by phone/customer fields.
- Conditional customer creation.
- Product lookup and case creation.
- Collection workflow between point-of-sale location and lab.
- Warranty email parsing with branch routing.

### Real Estate Rental Operations

- Rental lead inbox parsing from email sources.
- AI-assisted extraction for messy lead content.
- Publication/unit lookup and CRM association.
- Rental agreement creation and related-record updates.
- Serial number generation with multiple branches.
- Service request creation from Outlook messages and attachments.
- Google Vision/OpenAI-assisted classification in service request flows.
- Banking/transaction refresh automation.
- Unit name changes propagated to related opportunity/rental agreement records.

### Law Firm Operations

- Fireberry-to-Outlook calendar sync.
- Outlook-to-Fireberry calendar sync.
- Manual repair/test variants for calendar sync.
- Website lead intake into CRM.
- Event/customer mapping patterns.

### Insurance And Tax Lead Automation

- Facebook Lead Ads intake.
- Multilingual name/phone/email normalization with OpenAI.
- Fireberry account/opportunity creation.
- Customer product generation based on selected services.
- Picklist value lookup utility.

## Portfolio Signal

These workflows are strong portfolio evidence because they show end-to-end systems thinking across intake, CRM data quality, user communication, and operational follow-up.

The public case studies focus on the durable engineering skills behind the work:

- Requirements gathering from messy business processes.
- CRM data modeling and lookup-before-create design.
- Automation reliability, retries, and exception handling.
- AI-assisted extraction where deterministic parsing is not enough.
- Clear handoff between CRM, email/calendar, finance, and operations workflows.
