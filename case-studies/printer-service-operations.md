# Printer Service Operations Automation

## Problem

A printer service/distribution operation needed to convert service forms, warranty emails, and point-of-sale collection requests into structured CRM records without manual retyping.

## Solution

Implemented Make scenarios connected to Fireberry CRM to parse inbound requests, normalize customer/product data, search for existing accounts and products, create missing records, and open operational service cases.

## Workflow Capabilities

- Email and webhook intake.
- Hebrew field extraction from form-like messages.
- Customer lookup by phone/contact fields.
- Conditional customer creation.
- Product lookup by serial/model fields.
- Warranty email parsing.
- Service case creation and lab collection routing.
- Branching for missing or ambiguous data.

## Systems

Make, Fireberry CRM, email intake, webhooks, regex/code modules, CRM lookup/update modules.

## Portfolio Value

This case demonstrates practical implementation consulting: messy inbound operations were translated into structured CRM workflows with lookup-before-create logic and exception routing.

