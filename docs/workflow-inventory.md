# Workflow Inventory

This inventory is based on a local review of Make blueprint exports. Raw exports are not included because they contain private webhook URLs, customer-data mappings, credential placeholders, CRM object names, and business-specific implementation details.

## Summary

| Area | Blueprint count | Main systems | Public framing |
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

## Publishability

These workflows are strong portfolio evidence, but raw exports are not publishable. They reveal:

- Webhook endpoints and zones.
- CRM object/table/field names.
- Credential placeholders and password-type fields.
- Contact data mappings for phone/email/name/address.
- Client-specific business process logic.
- Routing and branching details that are too close to client implementation.

Use high-level diagrams and case-study writeups instead. Do not publish workflow skeletons, importable examples, node graphs, or reusable implementation logic.
