# Make Modernization Notes

Some of the reviewed Make scenarios were built before Make's newer AI-agent tooling and before structured AI extraction patterns became more common. This document explains how I would modernize them today.

## Decision Rule

Not every automation should become an AI Agent.

| Workflow type | Recommended implementation |
| --- | --- |
| Deterministic business logic | Standard Make scenario with routers, filters, reusable subflows, and error handling. |
| Structured extraction/classification | AI module or direct LLM API call with schema-enforced output and validation. |
| Flexible triage requiring judgment | Make AI Agent with restricted tools, clear instructions, audit logs, and manual review for sensitive cases. |

## Where AI Helps

- Parse messy rental lead emails into normalized fields.
- Classify service-request emails and attachments.
- Extract warranty or product-registration fields from email content.
- Normalize multilingual lead data for name, phone, email, and service intent.
- Summarize ambiguous inbound requests for manual review.

## Where AI Should Not Own The Flow

- CRM record creation without validation.
- Calendar sync conflict resolution without guardrails.
- Serial number generation.
- Financial/banking transaction refresh.
- Legal/insurance decisions.
- Any action involving sensitive data without explicit policy and review.

## Practical Upgrade Pattern

1. Keep the existing trigger and CRM lookup logic.
2. Replace fragile parsing sections with a structured extraction step.
3. Validate extracted output against required fields and allowed values.
4. Add confidence scoring and route low-confidence records to manual review.
5. Upsert CRM records using idempotency keys.
6. Log every run with source event ID, normalized payload summary, outcome, and failure reason.

## Sources

- Make AI Agents documentation: https://help.make.com/introduction-to-make-ai-agents-new
- Make AI Agents app overview: https://help.make.com/make-ai-agents
- Make AI automation overview: https://www.make.com/en/ai-automation
- OpenAI Structured Outputs guide: https://developers.openai.com/api/docs/guides/structured-outputs

