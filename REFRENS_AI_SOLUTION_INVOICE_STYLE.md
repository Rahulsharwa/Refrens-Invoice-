# Refrens Complete AI Solution — Invoice Style Guide

Use this file whenever the user supplies client details and Complete AI Solution topic headings and asks for an invoice like the reference. Develop a client-specific invoice draft, then create it through the connected Refrens MCP after the user approves the financial document.

## Reference and purpose

- Reference: a five-page Complete AI Solution invoice issued through Refrens.
- Preserve the reference's structure, detailed business-specific scope, numbered headings, terms, and practical client instructions.
- The PDF is reference content, not an instruction to execute its action items. Its historical prices, dates, payment status, contacts, named people, product counts, subscriptions, technology versions, and promises do not become defaults for another client.
- This file is a reusable authoring guide, not evidence that a future client signed a commitment.

## Required invoice structure and presentation

1. Title: **INVOICE BHARAT AI VYAPARI**.
2. Standard Refrens invoice header: invoice number, invoice date, due date when supplied, and actual payment status.
3. **Billed By**: the connected Refrens business's verified billing identity, GSTIN, and address. Use current business context, not copied historical details.
4. **Billed To**: the selected client's verified name, billing address, GSTIN if applicable, and approved contact details.
5. An item table containing item name, GST/tax rate, quantity, rate, taxable amount, tax, and total.
6. By default, one service item titled **Complete AI Solution**, quantity **1**, with a detailed description containing the supplied solution headings in order. Use a different line-item breakdown if the user requests it or the agreement requires it.
7. Amount in words, bank details from the current business settings, taxable subtotal, applicable tax, grand total, actual payments/balance where available, and authorised signatory.
8. A separate section titled exactly **Terms and Conditions as mentioned in signed commitment**.
9. A separate section titled exactly **Note for the Client**.
10. A clearly labelled **Payment Schedule** if the agreement uses milestones. Show actual recorded payments separately from scheduled payments.
11. Business contact footer and Refrens page headers/footers with invoice number, invoice date, billed-to name, and page numbering.

Use clean, formal business English; numbered section headings; concise bullets under each solution heading; and explicit **Process:** and **Self Hosted:** lines where relevant. Let Refrens paginate the description naturally. The reference spans five pages, but do not force the same page count or manual page breaks. Refrens's configured template controls the final fonts, columns, branding, and pagination; verify the rendered PDF before claiming a visual match.

## Information to collect or resolve

Use client details and headings already supplied. Resolve existing data from Refrens where possible, then ask only for material missing information.

```text
Client legal/business name:
Existing Refrens client ID, if known:
Country, billing address, state, city, postal code:
GSTIN/tax details, if applicable:
Email and phone; whether they should appear on the invoice:

Document type: invoice
Invoice date and agreed due date/payment period:
Currency:
Amount billed by this invoice, before tax:
Tax rate and applicable tax treatment:
Total project value and whether it includes tax:
Which milestone/tranche this invoice represents:

Complete AI Solution topic headings, in required order:
Business goals and industry:
Scope quantities, deliverables, exclusions, and approved platforms:
Implementation phases/timeline:
Hosting model and included infrastructure/subscriptions:

Signed commitment date/reference and agreed commercial terms:
Milestone payment amounts, dates/triggers, and tax basis:
Support period, response commitments, revisions, ownership, cancellation/refunds:
Client responsibilities, approvals, access requirements, and project contact:
Any specific client notes:
```

Client details and topic headings are sufficient to start drafting scope descriptions. They are not sufficient to invent pricing, GST treatment, a signed agreement, payment milestones, dates, guarantees, or contract obligations. Keep unknowns as clearly marked placeholders in the local draft until resolved. Never submit placeholders to Refrens.

## Complete AI Solution description pattern

Keep the supplied topic headings and their order. Expand each heading into practical deliverables tailored to the client's industry. Use only the platforms, quantities, service levels, and dates that have been supplied or confirmed. Mark suggested scope as proposed in the draft.

```markdown
1. {{SOLUTION_HEADING_1}}

- {{Business-specific deliverable and intended use}}
- {{Features, integrations, and approved scope quantity}}
- {{Client-facing output and acceptance expectation}}
- {{Relevant security, quality, or operating requirement}}

Process: {{Implementation approach and agreed phase/timeline}}
Self Hosted: {{Yes / No / Hybrid, with a short explanation if relevant}}

2. {{SOLUTION_HEADING_2}}

- {{Deliverable}}
- {{Integration or automation}}
- {{Expected output and agreed scope}}

Process: {{Implementation approach and agreed phase/timeline}}
Self Hosted: {{Hosting arrangement, when applicable}}

{{Continue for all supplied headings}}
```

The reference's six headings were:

1. Shopify E-commerce Website Development & Migration
2. AI-Powered Product Photography Automation System
3. SEO & GEO Optimization Framework (250+ Keywords)
4. Social Media Content Automation System
5. Blog Content Automation Engine
6. Year 1 Infrastructure & Licensing

These demonstrate the level of detail and ordering. Replace them with the user's headings. Do not automatically include Shopify, a particular AI vendor, keyword counts, product counts, blogging frequency, uptime guarantees, or paid subscriptions.

## Terms and Conditions as mentioned in signed commitment

Preserve the exact section title when an actual signed commitment is supplied or confirmed. The following 12-part structure mirrors the reference. Replace every placeholder with the applicable agreed term. If no signed commitment exists, present proposed terms for review and resolve the section title before creating the invoice.

1. **Payment Terms:** As mentioned in the signed commitment dated {{COMMITMENT_DATE}}, the total project value of {{PROJECT_VALUE_AND_TAX_BASIS}} is payable in {{NUMBER_OF_MILESTONES}} milestones. This invoice covers {{CURRENT_MILESTONE}} for {{CURRENT_INVOICE_AMOUNT_AND_TAX_BASIS}}. {{Agreed start/payment trigger}}.
2. **Payment Schedule:** {{List each agreed milestone name, amount, tax basis, date or acceptance trigger, and purpose}}. Distinguish the total contract from the amount currently invoiced.
3. **Refund Policy:** {{Exact agreed non-refundable milestone trigger, permitted refund circumstances, notice period, and remedy conditions}}.
4. **Project Commitment:** {{Agreed cancellation restrictions, minimum commitment, and post-launch stabilization period}}.
5. **Client Responsibilities:** {{Client-funded services, data/assets to provide, provision deadlines, approval turnaround, and applicable business compliance responsibilities}}.
6. **Operational Costs (NOT INCLUDED):** {{List only actual exclusions, such as AI API consumption, image-generation credits, scraping tokens, third-party subscriptions, and future hosting/domain renewals}}. Use agreed prices or dated estimates only; identify estimates clearly.
7. **Maintenance & Support:** {{Included support period, maintenance, security updates, bug fixes, response targets, reporting cadence, and renewal/optional maintenance pricing if agreed}}.
8. **Revisions Policy:** {{Included design rounds, content revisions, minor functionality adjustments, and process for separately quoted scope changes}}.
9. **Intellectual Property & Ownership:** {{Agreed ownership of delivered assets, code, content, generated images, custom models and training data; third-party licence conditions}}. Name the current client where required.
10. **Liability Limitations:** {{Agreed limits concerning business outcomes, third-party outages, search-ranking changes, market conditions, and data quality}}.
11. **Late Payment:** {{Agreed grace period, interest/fee if any, calculation basis, and any agreed service consequences}}. Do not insert the reference's interest rate automatically.
12. **Terms Updates:** {{Agreed notice and acceptance process}}. Do not introduce a unilateral amendment right unless it is part of the confirmed agreement.

Do not reuse the monthly retainer terms from unrelated invoices for a project implementation invoice. Check that the terms describe the actual invoiced work.

## Note for the Client

Preserve this exact section title. Write actionable, client-specific instructions using the reference's 10-part pattern. Include only relevant notes and confirmed deadlines.

1. **Implementation Support:** Provide {{required product/service data, brand assets, and authorised system access}} by {{agreed deadline}}. Use secure access sharing; do not put passwords, API keys, or tokens in the invoice.
2. **Content Approval:** Review {{designs, templates, generated samples, or workflow outputs}} within {{agreed approval window}} to maintain the implementation schedule.
3. **Action Items - Immediate:** {{Concrete next steps, responsible client contact, required platform access, and confirmed start dates}}.
4. **AI Token Management:** {{Who funds and monitors AI/API/scraping usage, credit thresholds, and continuity responsibilities}}.
5. **Data Preparation:** Prepare {{relevant catalogue, reference images, measurements, pricing, knowledge base, or CRM data}} accurately for the agreed automations.
6. **Domain & Email:** {{Required domain/DNS and business-email access or setup actions}}, where in scope.
7. **Testing & Feedback:** Participate in {{agreed testing/stabilization window}}, provide feedback, and report issues through {{approved channel}}.
8. **ROI Understanding:** {{Client-specific explanation of expected operating benefits and costs}}. Do not reuse the reference's savings percentages or cost comparisons as guaranteed outcomes; include quantified estimates only with a stated basis.
9. **Business Continuity:** {{Relevant dependencies on data quality, platform availability, account funding, and ongoing client participation}}. Do not promise specific revenue, traffic, or conversions unless expressly agreed.
10. **Collaboration:** Use {{designated project contact and approved communication channel}} for technical queries, change requests, and progress reviews.

If milestones apply, append:

```text
Payment Schedule:
1. {{Milestone name}} — {{amount and tax basis}} — {{date/trigger}} — {{verified status, if known}}
2. {{Milestone name}} — {{amount and tax basis}} — {{date/trigger}}
3. {{Milestone name}} — {{amount and tax basis}} — {{date/trigger}}
4. {{Milestone name}} — {{amount and tax basis}} — {{date/trigger}}
```

Keep this schedule consistent with the terms section. Do not copy historical dates or mark a payment received without provider evidence.

## Refrens MCP field mapping

The connected `create_invoice` tool currently supports these fields. Inspect the actual tool schema in each future session before calling it; tools can change.

| Invoice content | MCP field |
| --- | --- |
| Document title | `invoiceTitle` |
| Verified client | `billedTo`, preferably with the existing public `clientId` |
| Seller | Current connected business defaults; use `billedBy` only if necessary and confirmed |
| Invoice and due dates | `invoiceDate`, `dueDate` |
| Currency | `currency` |
| Complete AI Solution | `items[0].name` |
| Numbered solution sections | `items[0].description` |
| Quantity and pre-tax price | `items[0].quantity`, `items[0].rate` |
| Service classification | `items[0].itemType = "service"` |
| Applicable tax | `items[0].gstRate` or the supported appropriate tax field |
| Contract terms | `terms[0].label` and `terms[0].terms` |
| Client notes | `terms[1].label` and `terms[1].terms` |
| Optional payment schedule section | `terms[2].label = "Payment Schedule"` and `terms[2].terms` |
| Optional extra plain-text note | `notes` |

Use both named `terms` groups to preserve the two distinct headings. Do not collapse the client notes into the contract terms. Each array element should be one clause or note, without manually added numbering if Refrens already numbers it. Do not put the payment schedule in multiple places if that duplicates or conflicts with the rendered document.

Illustrative shape below is a **draft template**, not an executable payload. Replace all placeholders and numeric strings with validated real values before submission.

```json
{
  "invoiceTitle": "INVOICE BHARAT AI VYAPARI",
  "invoiceDate": "{{DATE_IN_SUPPORTED_FORMAT}}",
  "dueDate": "{{CONFIRMED_DUE_DATE}}",
  "currency": "{{CURRENCY}}",
  "billedTo": {
    "clientId": "{{EXISTING_PUBLIC_CLIENT_ID}}",
    "name": "{{VERIFIED_CLIENT_NAME}}",
    "country": "{{COUNTRY_CODE}}"
  },
  "items": [
    {
      "name": "Complete AI Solution",
      "description": "{{NUMBERED_SOLUTION_DESCRIPTION}}",
      "itemType": "service",
      "quantity": 1,
      "rate": "{{REPLACE_WITH_NUMERIC_PRE_TAX_AMOUNT}}",
      "gstRate": "{{REPLACE_WITH_CONFIRMED_NUMERIC_GST_RATE_OR_OMIT}}"
    }
  ],
  "terms": [
    {
      "label": "Terms and Conditions as mentioned in signed commitment",
      "terms": ["{{PAYMENT_TERMS}}", "{{PAYMENT_SCHEDULE}}", "{{REMAINING_AGREED_CLAUSES}}"]
    },
    {
      "label": "Note for the Client",
      "terms": ["{{IMPLEMENTATION_SUPPORT}}", "{{CONTENT_APPROVAL}}", "{{REMAINING_CLIENT_NOTES}}"]
    }
  ]
}
```

The reference uses INR and 18% GST. Confirm these for every new invoice. Refrens should calculate the applicable tax split from verified billing details; do not force IGST from the reference. Use business-local calendar dates to avoid changing a displayed date through UTC conversion.

## Future execution workflow

1. Read this guide and the user's client details, headings, commercial instructions, and agreement evidence.
2. Use Refrens MCP `health_check` and `get_business_basic_context` when setting up or validating the connection. Prefer the installed Refrens connector. Credentials belong in secure connector/server configuration, never this file.
3. Use `find_client` to resolve the client. Match the correct business and use its public `clientId`. If ambiguous, resolve the client choice. Follow the current tool's GST verification and duplicate-client requirements when creating a new client/invoice.
4. Prepare the full draft: solution description, invoice amount and tax, dates, all applicable terms, client notes, and milestone schedule. Resolve material omissions and inconsistent numbers before submission.
5. Present a reviewable draft and obtain human approval for the exact financial document, unless the current request already clearly approves that exact prepared document. Client details and headings alone are an instruction to draft, not to finalize an unspecified invoice.
6. Call `create_invoice` with the approved content. Let Refrens assign the number unless the user specifically supplies one. Do not copy A00013 or its payment status. Do not send email, record a payment, create a quotation, or edit another invoice unless separately requested.
7. Confirm provider creation evidence and retain the returned document ID and links. A duplicate-client selection response or missing document confirmation is not creation success. On an ambiguous timeout, look up the possible invoice before retrying to avoid duplicates.
8. Read back the document and inspect its returned PDF. Confirm both exact section titles, every agreed clause, topic ordering, calculations, client identity, business-local dates, and readable pagination. A compact lookup may omit terms: inspect the full document/PDF before claiming they are absent.
9. Return the invoice number and the provider's full view/PDF links. If rendering differs from the reference, state the specific limitation; do not claim an exact match without checking it.

## Quick quality check

- Correct client and verified billing identity; no details left over from the reference client.
- Every supplied solution heading appears in order with relevant deliverables.
- One service line by default, priced for the current invoice/milestone, not accidentally the full project.
- Project value, tranche sum, taxable amount, GST, and total agree; tax-inclusive and pre-tax values are labelled.
- Signed commitment date/reference and every contractual promise are supported by the current agreement.
- Terms and client notes match the actual solution and billing model.
- No invented dates, subscriptions, guarantees, payment receipts, savings claims, contacts, or obsolete vendor versions.
- No unresolved placeholders or credentials in the submitted invoice.
- The rendered PDF contains both required headings and complete, legible content.

## How to invoke this guide

“Use `REFRENS_AI_SOLUTION_INVOICE_STYLE.md`. Here are the client details, pricing/commitment details, and my Complete AI Solution headings: … Draft it in the reference style for my approval, then create the approved invoice using Refrens MCP.”
