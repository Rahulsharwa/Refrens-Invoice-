---
name: refrens-service-invoices
description: Draft detailed service invoices from client billing details and scope, then create or update approved invoices in Refrens. Includes package and instalment pricing, separate maintenance and tool billing, client notes, and full general, website, AI SDR, and AI social media terms.
---

# Refrens Service Invoices

Prepare client-specific service invoices in the established detailed format. Start with the user's billing name, GSTIN, PAN, address, and service details. Draft in chat first; create or update the exact invoice after approval. DOCX review is optional when requested. This file contains the complete invoice format, workflow, and terms library; no external reference file is required.

## Operating rules

- Use verified details from the selected connected Refrens business for the seller, tax identity, branding, bank details, and authorised signatory. Do not assume that the business default currency matches this invoice.
- Current user instructions govern presentation and authorised actions. Accepted project documents govern contractual obligations. Identify conflicts instead of silently amending commitments.
- Read the full embedded terms library below. Include every applicable general protection and the relevant service-specific clauses; omit unrelated service clauses. Do not reduce the invoice to result disclaimers alone.
- The library supplies proposed wording, not evidence that a client agreed to it. Preserve qualifications, exceptions, and remedies when tailoring clauses. Do not invent revision counts, warranties, liability caps, deemed-approval periods, commitments, or legal jurisdiction.
- Use “Terms and Conditions as mentioned in signed commitment” only when a signed commitment exists and the clauses match it. Otherwise label unagreed wording “Proposed Terms and Conditions — For Approval.” Separate accepted and proposed clauses when both occur.
- Generic examples and past client invoices do not establish default prices, GST rates, page counts, platforms, implementation targets, hosting periods, maintenance fees, or payment schedules.
- Service details authorise drafting, not unspecified external financial documents. Once the user approves an exact prepared invoice, proceed without requesting the same approval again. A material change of recipient, amount, tax treatment, or commitments requires a revised reviewable draft and approval.
- Use the internal browser exclusively for navigation, login, OAuth, OTP, editing, saving, debugging, and verification. External Chrome is permitted only when the current task explicitly authorises it; an internal-browser failure is not permission to switch.
- Never send the invoice, record a payment, sign a document, or activate a recurring invoice schedule without the user's explicit authorisation for that action.

## Intake and resolution

Accept partial input and use facts already supplied. The minimum starting brief is:

```text
Billing name:
GSTIN or GST registration status:
PAN:
Billing address including state, PIN and country:
Services and features:
```

Pricing can be included in service details. Before the draft can be approved for creation, establish:

- Total project value, currency, tax-inclusive or tax-exclusive basis, and amount billed now.
- Full-project, advance, milestone, quarterly instalment, maintenance, usage, or other billing purpose.
- Agreed tax rate and treatment; invoice date, due date or payment trigger, and invoice number when updating.
- Ordered service titles, included features, quantities, exclusions, platforms, integrations, and environments.
- Commencement trigger, delivery timeline, client dependencies, revisions, approvals, acceptance, warranty, support, and handover.
- Hosting and subscription inclusions, usage allowances, service periods, funding ownership, renewal and recurring arrangements.
- Payment schedule, verified receipts and their allocation, and the accepted agreement or proposed terms status.
- Contact person, email and phone only when provided or required; missing optional contact information does not block an otherwise complete invoice. Do not borrow a related person's details without evidence of relevance.

Ask one consolidated set of focused questions for material omissions. Continue useful drafting while awaiting answers. Use `TO CONFIRM` only in review drafts, with unresolved fields listed outside invoice-ready content. Do not substitute “as agreed” to conceal a material undefined scope or commercial term. Do not create or update an external invoice containing unresolved material fields.

### Billing identity

- Normalise GSTIN and PAN to uppercase. Check expected formats, and compare the supplied PAN with GSTIN characters 3–12 (zero-based slice `[2:12]`) where applicable. A format or embedded-PAN match is not registry verification.
- A mismatch requires clarification; never overwrite the user’s identity details silently. Do not assume an omitted GSTIN means an unregistered client.
- Search existing clients by exact GSTIN and/or name. Match the billing entity, address, and public client identifier; project brand and contact person may differ from the billed legal entity.
- For ambiguous matches, show the meaningful candidates and obtain a clear choice. An ambiguous “yes” does not select between “update existing” and “create new.”
- Use the selected saved public `clientId` on document calls. Follow the current tools' registry and duplicate-choice requirements. When a GSTIN is supplied without a selected existing client, offer registry lookup before creating; use returned registry mappings only after required confirmation, and preserve user-typed values until discrepancies are resolved.
- If PAN has no supported field in the current connector schema, do not invent one. Use the internal editor's supported PAN field, or show it in a clearly labelled invoice billing detail/approved note if acceptable and verify its appearance.

## Pricing and billing

### Package and instalment invoices

- For one bundled solution, put the full amount billed by this invoice on Line Item 1. Put zero on subsequent services included in that package.
- Title the first item to reflect package coverage and billing purpose. It may also describe the first service; do not duplicate that service unnecessarily.
- For a full-project invoice, the first amount is the full agreed package amount. For an instalment or milestone invoice, it is only the current instalment. Identify total contract value separately.
- Every zero-priced item must say “Included in the project package billed through Line Item 1.” Explain that zero means included, not independently free or unlimited work.
- Do not describe the instalment amount as the full solution price. Clarify which services span later milestones and whether the payment schedule affects delivery.
- Use quantity 1 for a package/service line unless another billing unit is agreed. Scope quantities such as pages or posts belong in the description when not billing units.
- Independent packages and separately priced extras require explicit allocation; do not automatically zero-price unrelated work.

### Quarterly payments

- Confirm amount per quarter, first due date, number of instalments, total contract value, tax basis, and billing in advance or arrears.
- Quarterly billing does not automatically change the implementation deadline or create a particular minimum term.
- Reconcile instalments to contract value. For example, four payments of INR 5,00,000 equal INR 20,00,000; a previously stated INR 25,00,000 contract needs an agreed price change or a separate collection arrangement. Do not choose either silently.
- Future instalments appear in the schedule; they are not additional current invoice charges. State whether a calendar date or completion trigger controls when they differ.

### Maintenance and tools

- When maintenance is separately chargeable, prepare a separate invoice for the named service period with its agreed fee, scope, volume, support limits, commencement, term, renewal and cancellation rules.
- Do not infer perpetual maintenance or a recurring schedule from package inclusion or a service title.
- If tools are separate, expressly exclude them from the maintenance fee. Identify subscriptions, APIs, AI tokens, messaging, enrichment, verification, licences and other applicable costs.
- Agree direct client payment versus provider-funded reimbursement/usage invoicing. Record approval thresholds, allowances, evidence, currency/FX basis, taxes and any agreed markup; never invent a markup or expense.
- Draft additional maintenance or tool invoices when relevant; create them only if the user approved those specific documents. Do not activate recurring automation merely because a monthly fee is mentioned.

### Taxes and totals

- Never assume 18% GST or copy a previous invoice's IGST/CGST/SGST split. Confirm tax treatment and use verified seller and place-of-supply details with the current Refrens calculation.
- Distinguish taxable amount, tax, total, contract value, scheduled payments, recorded receipts, and balance due. Label tax-inclusive prices and calculate the base correctly.
- Reconcile quantity × rate, discounts, additional approved charges, tax, round-off, total and verified payment allocation. Do not deduct an advance twice or apply an unrelated project payment to this invoice.
- Use business-local calendar dates. Dates from historical reference documents do not become current due dates.

## Invoice format

Use clear formal business English with concise bullet descriptions. Default branding is the connected business's verified branding; for the Bharat AI Vyapari business use the established title “INVOICE BHARAT AI VYAPARI” where appropriate. Do not carry that branding into another seller's invoices without instruction.

Return the review draft in this order:

1. Invoice title, billing purpose, seller, client, tax identifiers, address, currency, dates and draft status.
2. Service line items, preserving the requested order.
3. Current invoice subtotal, taxes, grand total, amount in words where supported, verified payments and balance; total project value separately when relevant.
4. Shared applicable terms, with accepted and proposed wording correctly labelled.
5. **Note for the Client**, containing actionable inputs, owners, approvals, access, account funding, testing and handover steps.
6. **Payment Schedule**, only where applicable, listing each amount, tax basis, due date/trigger and verified status. Avoid duplicating conflicting schedules in several sections.
7. **Items Requiring Confirmation**, only if needed, outside final invoice content.

### Each service item

```text
Title: Clear service name and agreed quantity or limit
Description:
- Scope of work: Specific deliverables, features and outputs; separate bullets for distinct features.
- Scope limits and exclusions: Quantities, environments, boundaries and dependencies.
- Terms and conditions: Applicable service-specific obligations and limits.
- Risk and mitigation: Concrete risk, agreed practical mitigation and responsible party.
- Client notes: Inputs, data, access, permissions, approvals and actions required.
- Timeline: Confirmed duration/dates, start trigger and dependencies.
- Delivery and acceptance: Observable completion, agreed environment, review/UAT and handover criteria.
- UDP points: Use the user-confirmed meaning when requested.
- Pricing coverage: Package/instalment coverage or included-service statement.
Pricing: Currency and amount, with tax basis
```

- Keep the whole description point-to-point, including terms and timelines. Use readable bullets, not paragraphs masquerading as a single bullet.
- “UDP” has not been defined as a universal term. If requested and undefined, clarify it; do not silently replace it with USP. Do not put an unexplained UDP placeholder on an issued invoice.
- Omit genuinely inapplicable categories; missing material information is not “not applicable.” Keep operational notes distinct from legal terms.
- Do not place passwords, API keys or tokens in content. Include only necessary approved business contact information.
- Use specific functional delivery criteria instead of results-based completion. Preserve required human approval and correction responsibilities.

### Tailoring service descriptions

- **Website:** Specify page/template limits; sign-up, sign-in, RFQ, admin, blogs, webhook and other modules only when included. Address responsive/browser coverage, content/migration limits, integrations, SEO/analytics, deployment, hosting/renewal, QA, acceptance, warranty and handover.
- **AI SDR:** Specify channels, sources, contact/activity allowances, scripts, qualification, follow-ups, CRM/calendar integration, opt-outs/suppression, authorised claims, human escalation and reporting. Separate implementation acceptance from ongoing operation.
- **AI social media:** Specify platforms/accounts, formats, content quantity, scheduling/cadence, approval, review, rights, reporting and operating period. Separate content production, publishing, advertising, moderation and crisis handling. A daily workflow trigger does not guarantee a post on every platform daily.
- **SEO/GEO/blogs:** Specify research and content quantities, fact-check owner, technical tasks, publishing approval, reporting and limits. Ranking/indexing/AI citations are not deliverables unless expressly committed.
- **CRM/rental/franchise/event automation and other services:** Describe approved records, rules, integrations, users, approvals, reporting and representative acceptance cases. Quotation drafts, RFQs, availability checks and AI qualification do not imply autonomous commercial authority.
- Read the relevant full service terms below and carry applicable provisions into the invoice without contradictory repetition.

## Refrens workflow

### Draft and authorisation

1. Discover the available Refrens tools and current schemas rather than assuming a cached payload shape. Use connectivity and basic-business-context tools where needed; read the business clock before resolving relative dates.
2. Resolve the client and search existing invoices for this client/project/billing period. If a draft exists, present its number, amount, purpose and material differences before deciding whether to update or create. Obtain a clear selection when ambiguous.
3. Prepare the complete reviewable draft and consolidated confirmation list. Resolve material contradictions and missing information before external mutation.
4. Obtain approval of the exact financial document. Do not request approval again for an already approved update with no material changes. If a DOCX is requested, provide it for review and incorporate approved edits before proceeding; a DOCX is not mandatory otherwise.

### Create or update

- Use the connected Refrens business automatically; do not ask for its internal business ID. Reuse the saved public client ID when selected; let Refrens assign a new invoice number unless the user specifies an approved number.
- Set currency and service item classification explicitly where supported. Use the current schema for dates and taxes.
- Map each service to a separate item with `name`, `description`, `quantity`, `rate`, and supported tax fields. Keep full descriptions intact; do not compress all services back into one item.
- Use separate named `terms` groups for shared terms, “Note for the Client,” and “Payment Schedule” where supported. Use the correct agreed/proposed terms heading. Follow the template's numbering behaviour rather than double-numbering clauses.
- On updates, capture existing client, items, totals, dates, terms, notes, status, payments and handover/support commitments. Change only the authorised fields. Do not silently erase existing agreed scope, hosting, maintenance or timelines merely because a local draft omitted them; reconcile conflicts.
- Some connector versions can patch terms and party details but cannot patch items/rates. Inspect current capabilities. For unsupported edits use the authenticated internal browser editor, edit the existing invoice, save, and verify; do not replace an update with a new invoice or use guessed/private APIs.
- Preserve intended document status, existing signature state and payment records. Do not sign, send for acceptance, record receipts, cancel, or publish an unrelated document as part of an ordinary update. If saving unexpectedly changes status, identify and resolve or report it rather than calling the invoice a draft falsely.
- A duplicate-client selection response with no creation evidence is not success. Follow the tool's exact explicit-choice/token instructions; never invent tokens or infer a choice from ambiguous approval.
- After a timeout or uncertain create result, look up the intended invoice before retrying to prevent duplicates. If safe completion is blocked, preserve the draft and report the concrete blocker instead of repeatedly creating documents.

### Verify and deliver

- Read back the persisted invoice; compare the exact billing identity, GSTIN/PAN/address, dates, service count/order, descriptions, rates, zero-priced inclusions, currency, tax, total, terms, client notes, schedule, status and payments.
- Check the rendered invoice/PDF for complete descriptions and clauses, readable pagination and totals. A compact lookup may omit terms; inspect the full document or rendered view before declaring them missing.
- Fix authorised omissions or formatting defects and recheck the affected output. If PDF export or rendering is unavailable, distinguish persisted-content verification from unverified PDF layout.
- Return invoice number, billed party, total/tax, due date and actual status with the provider-returned complete view and PDF links when present. Preserve the entire authorisation query string; do not invent or shorten URLs.
- Do not claim an invoice is paid, emailed, signed, approved by the client or visually verified without evidence of that state. If no share link is returned, report the saved invoice and link limitation; do not retry creation to obtain one.

## Invoice preparation acceptance checks

Before seeking final approval or saving an approved invoice, confirm:

- Correct billing entity; no previous client's names, tax identifiers, contacts or amounts leaked into content.
- Every requested service has its title, point-to-point scope, applicable terms, risks/mitigation, notes, timeline, delivery criteria and pricing.
- All applicable protections from the complete library have been considered. Record unresolved material choices outside issued content; never introduce unsupported blanket exemptions.
- Current invoice amount appears once for each package, included components are zero, and instalment totals match the confirmed contract value.
- Maintenance and tool funding are separately stated when applicable, with actual service periods and no invented usage charges.
- Calculations, taxes, schedules, verified receipts and balances reconcile.
- Proposed terms are not presented as signed commitments. No unresolved material placeholders appear on a created invoice.
- The exact create/update is authorised and existing invoices have been checked for duplication.

## Offline review scenarios

Use these scenarios when reviewing or updating this skill; do not create live invoices for validation.

| Scenario | Required behaviour |
| --- | --- |
| Full package of INR 2,00,000 before tax with three included services | Put INR 2,00,000 on the first item, zero on two included items; obtain the applicable tax treatment rather than assuming it. |
| INR 25,00,000 contract and four proposed INR 5,00,000 quarterly payments | Flag the INR 5,00,000 shortfall; clarify price or payment arrangement before external creation. |
| INR 50,000 monthly maintenance plus separate tools | Draft period-specific maintenance separately; exclude tool costs and establish direct payment or approved reimbursement. Do not activate a recurring schedule automatically. |
| Client name, GSTIN, PAN and services but no price | Check identifiers, draft useful scope and terms, and ask for the price and tax basis; do not fabricate a final total. |
| PAN does not match GSTIN's embedded PAN | Identify the mismatch and clarify the billing identity without silently substituting either value. |
| Existing draft and request to revise its amount and items | Confirm the target; update that invoice with current supported tools or the internal editor, preserve authorised commitments, save and verify; do not create a duplicate. |
| A create call times out | Search for the intended document and reconcile the result before any retry. |
| A service has no relevance to website, SDR or social management | Use applicable general terms and tailored service conditions; omit unrelated specialist clauses without dropping shared protections. |

# Complete embedded terms and conditions

The following library reproduces the complete general terms, all 24 numbered sections, and the project-specific preparation checklist. All clauses are available here in full. Tailor them under the operating rules above; retaining the complete library in this skill does not mean every clause applies to every invoice.

# General Terms and Conditions of Service

These terms are intended for incorporation into a quotation, proposal, statement of work, or service agreement before work begins. The applicable project documents must identify the service provider, client, scope, fees, payment schedule, timeline, and any service-specific conditions. These terms apply only when accepted as part of that agreement; adding them to a later invoice does not by itself amend an existing commitment.

“Provider” means the service provider identified in the accepted project documents. “Client” means the customer identified in those documents. “Agreed scope” means the deliverables and limits recorded in the accepted project documents and subsequent written change approvals.

## 1. Service Provider Role

- The Provider is engaged to perform the agreed services and deliver the agreed work with reasonable care and skill.
- The Client remains responsible for its business operations, products, pricing, sales, customer relationships, order fulfilment, and commercial decisions.
- Unless expressly included in the agreed scope, the Provider does not undertake sales execution, lead qualification, customer follow-up, business management, or professional legal, tax, or regulatory advice.
- These role limitations do not remove the Provider’s responsibility to perform its agreed obligations.

## 2. No Guarantee of Results, Leads, or Revenue

- Services do not guarantee sales, revenue, profit, business growth, return on investment, enquiries, RFQs, appointments, leads, or customers unless a specific commitment is expressly agreed in writing.
- Lead quantity, quality, authenticity, relevance, purchase intent, and conversion are not guaranteed. Enquiries may include spam, duplicates, irrelevant submissions, or contacts who do not purchase.
- Lead response, qualification, follow-up, negotiation, and conversion are the Client’s responsibility unless expressly included in scope.
- Advertising performance, cost per lead, acquisition cost, and conversion rates depend on factors including budget, competition, offer quality, targeting, market conditions, and the Client’s sales execution.
- SEO rankings, indexing, traffic, impressions, and visibility in search engines or AI-generated answers are not guaranteed. Platform algorithms and publication decisions are outside the Provider’s control.
- Forecasts, examples, demonstrations, and estimates are illustrative unless expressly incorporated as written contractual commitments.
- Failure to achieve a desired commercial result does not, by itself, establish failure to deliver the agreed services.

## 3. Scope, Limits, and Exclusions

- Work is limited to the agreed deliverables, quantities, pages, modules, integrations, platforms, usage allowances, and service periods.
- Unlisted requirements are excluded unless added through a written change approval.
- Demonstrations and reference examples establish obligations only to the extent expressly incorporated into the agreed scope.
- Additional features, redesigns, migrations, integrations, content, or other expanded requirements may require additional fees and revised timelines.
- The Provider will obtain written approval of additional scope and charges before undertaking chargeable changes.

## 4. Package Pricing and Included Line Items

- Where the invoice uses package pricing, the first line item carries the total solution price and subsequent included components may be shown at zero.
- Zero-priced items are included in the package price; they are not independently free services or commitments to unlimited work.
- Separately chargeable recurring services, renewals, usage charges, and third-party expenses must be identified in the applicable project documents.
- Refund and termination calculations will follow the agreed allocation or a documented valuation of work and committed costs; a zero-priced component does not automatically have no value.

## 5. Client Inputs and Responsibilities

- The Client must provide accurate content, business information, product data, brand assets, access, permissions, and approvals needed for the work.
- The Client must ensure that supplied materials and instructions may lawfully be used for the agreed purpose.
- The Client remains responsible for the accuracy of its product claims, specifications, prices, policies, and approved content.
- Access credentials must be shared through an agreed secure method. The Client must maintain required account ownership and authorisations.
- The Client must nominate an authorised approver and provide consolidated feedback through the agreed channel.

## 6. Approvals, Revisions, and Changes

- Included revision rounds and review windows are those stated in the agreed scope. No unlimited revision entitlement is implied.
- One revision round means one consolidated feedback set submitted and actioned as one pass within the agreed direction and scope.
- Refinements within scope are distinguished from new concepts, new features, changed architecture, rebranding, and changes to previously approved work.
- Approved stages form the basis for subsequent work. Reopening an approved stage may require a written change request, additional fees, and rescheduling.
- Conflicting feedback may be held pending clarification from the authorised approver.
- Deemed approval applies only if the agreement expressly states the review period, notice process, and effect of silence. These terms do not introduce automatic approval by silence.

## 7. Timelines, Dependencies, and Client Delays

- Work begins on the commencement trigger agreed in the project documents, subject to required payments, inputs, access, and authorisations.
- Timelines depend on timely Client cooperation, approvals, agreed scope, and availability of required third-party services.
- Client delays, approved changes, or external dependencies may require revised dates. The Provider will communicate material impacts and reasonable mitigation steps.
- Work may be paused after written notice where missing inputs, access, approvals, or payments prevent progress.
- Restart dates depend on resolution of the issue and resource availability. Any restart charge requires prior agreement.
- Client inactivity does not automatically mean that incomplete work has been delivered. Any inactivity closure process must be expressly agreed.

## 8. Third-Party Platforms and Operating Costs

- Hosting providers, APIs, plugins, payment gateways, advertising platforms, and other external services operate under their own terms and policies.
- The Provider cannot guarantee external account approval, verification, advertising approval, uninterrupted availability, or reinstatement following suspension.
- External outages, deprecations, policy changes, pricing changes, and discontinuation may affect functionality or delivery dates.
- The Provider will identify material impacts it becomes aware of. Adaptation work is included only to the extent stated in the agreed scope or support arrangement.
- The project documents must state who owns, funds, renews, and monitors hosting, domains, licences, API usage, AI tokens, messaging, and other external services.
- Included allowances and service periods are limited to those expressly agreed. Additional expenditure requires the agreed authorisation process.
- Depleted credits, expired subscriptions, or unpaid external accounts may interrupt dependent functionality.

## 9. Hosting, Included Periods, and Renewals

- Any included hosting, server management, domain, maintenance, or support period must be expressly stated, including its start trigger and coverage.
- One year of server costs or management is included only where the accepted project documents expressly provide for it.
- Renewal fees, account ownership, renewal responsibilities, and arrangements after the included period must be recorded in the project documents.
- Hosting inclusion does not imply unlimited storage, traffic, processing, backups, or support.

## 10. AI Content and Automation

- AI-generated content may contain inaccuracies, omissions, unsuitable statements, or material requiring further review.
- The agreed scope must identify who reviews and approves content before publication. Automated publication does not imply human review unless included.
- The Client is responsible for approving business claims and specialised content relating to its products or operations.
- Automation depends on source data, configured rules, credentials, usage allowances, and external systems. Exception handling, monitoring, and manual fallback are included only as agreed.
- AI outputs and automated decisions do not carry a guarantee of factual accuracy, uniqueness, suitability, or commercial results.
- The Provider remains responsible for implementing the agreed configuration and performing any expressly included review or monitoring.

## 11. Security, Data, and Backups

- The Provider will perform the security and data-handling measures agreed for the service and comply with applicable obligations.
- Absolute security, zero data loss, and uninterrupted operation are not guaranteed.
- Backup frequency, retention, restoration, monitoring, incident responsibilities, and recovery targets apply only as expressly agreed.
- Each party must protect confidential information, use it only for authorised purposes, and restrict access to people who need it for the engagement, subject to lawful disclosure requirements.
- Client data must not be used for unrelated purposes without appropriate authorisation. Any required data-processing terms must form part of the agreement.
- Client or external vendor changes may affect functionality and support coverage. Investigation or repair of resulting issues may be separately chargeable after approval.

## 12. Delivery, Testing, and Acceptance

- Delivery is measured against the agreed scope and acceptance criteria, including the specified deployment or handover environment.
- Website or software completion requires the agreed modules to be functional in that environment, subject to the agreed acceptance process.
- The Client must conduct review or UAT within the agreed period and report reproducible defects through the agreed channel with sufficient supporting information.
- A defect is a failure to meet an agreed specification. New requirements, changed preferences, and expanded functionality are change requests.
- Material unresolved defects affecting agreed acceptance criteria must be addressed under the acceptance process; submission alone does not establish acceptance.
- Acceptance occurs by the agreed written approval or other expressly agreed acceptance mechanism.
- Commercial performance and later subjective preferences do not independently change the agreed delivery criteria.

## 13. Warranty, Support, and Maintenance

- Any included defect warranty must specify its duration, commencement, coverage, reporting process, and remedies.
- Warranty coverage concerns defects in delivered work against the agreed specification; it does not automatically include new requirements, content changes, redesigns, external platform changes, or issues caused by unauthorised modifications.
- Support hours, channels, response targets, included volume, and exclusions are those expressly agreed.
- A response target is not a guaranteed resolution time unless expressly stated.
- Ongoing maintenance, updates, monitoring, and additional support require an applicable included period or separate service arrangement.

## 14. Handover and Intellectual Property

- The agreed handover must identify source code, files, documentation, administrative access, and other deliverables to be supplied.
- Ownership or licence rights transfer on the conditions stated in the agreement, including full payment where agreed.
- Pre-existing Provider tools, reusable components, and third-party materials remain subject to their respective ownership and licence terms.
- Any retained components, access restrictions, or licence limitations must be disclosed in the agreement.
- Credentials and access must be transferred securely. Post-handover support continues only as agreed.

## 15. Payments and Suspension

- Fees, advances, milestone amounts, taxes, due dates, and reimbursable expenses are governed by the accepted payment schedule.
- Payments are linked to the agreed billing triggers and are not contingent on commercial results unless expressly agreed.
- Late charges apply only where agreed and permitted by law.
- The Provider may suspend affected work or managed services for overdue payments after the agreed written notice and opportunity to resolve the default.
- Suspension, restoration, and any related charges must follow the agreement and applicable law. Suspension does not authorise deletion of Client data or interference beyond agreed rights.

## 16. No Refund After Commencement

- Once the agreed services have commenced, payments made toward those services, including advances and milestone payments, are non-refundable, subject to applicable law and express contractual remedies.
- Commencement means the documented start of substantive project work, including agreed discovery, planning, design, development, configuration, or service execution. Issuing an invoice or receiving payment alone does not establish commencement.
- Client cancellation, abandonment, changes in plans, management or ownership changes, changed preferences after approval, and dissatisfaction with business results do not independently create a refund entitlement after commencement.
- This policy does not remove remedies arising from the Provider’s breach, failure to perform agreed obligations, or rights that cannot lawfully be excluded.
- The agreement must distinguish project fees from recurring fees, unused third-party funds, and prepaid future service periods. Refund or credit treatment of those amounts must be expressly stated; project commencement does not automatically make every future recurring period non-refundable.
- Payments are not transferable to another project, entity, or service without written agreement.
- Cancellation does not automatically make the entire unpaid project balance due. Amounts payable on termination follow the agreed termination provisions, documented work, and applicable law.

## 17. Recurring Services and Termination

- Recurring services must specify their fee, billing cadence, start trigger, included volume, term, renewal process, and cancellation notice.
- Unused allowances expire or carry forward only as expressly agreed.
- Each party may terminate in accordance with the accepted agreement, including any notice and opportunity to remedy a material breach.
- On termination, the parties will reconcile completed work, work in progress, approved external commitments, payments received, and any applicable refund or credit obligations without double recovery.
- Handover, access removal, data retention or deletion, and transition assistance will follow the agreement and applicable obligations.

## 18. Project Closure

- The project closes following acceptance and completion of the agreed closure and handover obligations.
- Post-closure redesign, restructuring, migration, re-platforming, or additional development requires a new written scope unless covered by an existing warranty or support arrangement.
- Closure does not extinguish surviving confidentiality, intellectual property, payment, warranty, data, or other applicable obligations.

## 19. Liability and Third-Party Claims

- Any aggregate liability cap and exclusion of indirect or consequential losses must be expressly stated in the accepted agreement. This document does not invent a monetary cap.
- Limitations must include applicable exceptions and must not exclude liabilities that cannot lawfully be limited.
- Any Client indemnity for third-party claims concerning Client-supplied materials, unlawful instructions, or misuse must define its scope, limits, notice, defence control, and settlement process in the agreement.
- Client responsibility for supplied materials does not excuse the Provider’s own breach or unauthorised conduct.

## 20. Events Beyond Reasonable Control

- A party affected by an event beyond its reasonable control must notify the other party promptly and take reasonable steps to reduce disruption.
- Affected obligations and timelines may be adjusted to the extent caused by the event, in accordance with the agreement.
- Prolonged disruption, termination rights, and financial reconciliation must follow the agreement. This clause does not automatically waive accrued payment or other unaffected obligations.

## 21. Written Agreement, Changes, and Disputes

- The accepted project documents must identify the documents forming the agreement and their order of priority.
- Changes to scope, fees, timelines, or these terms require agreement by authorised representatives in the agreed written form.
- Earlier discussions are superseded only to the extent stated in the accepted agreement; an invoice does not unilaterally override a signed commitment.
- Governing law, dispute escalation, court jurisdiction, or arbitration arrangements must be expressly agreed. No location or dispute forum is assumed by this document.
- Nothing in these terms excludes mandatory legal rights. Protective clauses remain subject to the accepted agreement and applicable law.

## 22. Website Design and Development

These service-specific terms supplement the general terms above, including the no-refund-after-commencement policy, subject to applicable law and contractual remedies.

1. **Defined scope:** Development covers only the agreed number of pages, templates, features, user roles, integrations, and platforms. Additional requirements require a separate quotation or written change approval.
2. **Feature specifications:** Features such as sign-up, sign-in, RFQ, blog automation, admin dashboards, and webhooks will operate according to their agreed specifications. Naming a feature does not include every possible variation or workflow.
3. **Design approval:** Development proceeds from the approved design and structure. Changes to approved layouts, navigation, branding, or functionality may incur additional charges and extend delivery dates.
4. **Content and assets:** The Client must provide approved text, images, product information, policies, and brand assets unless their creation is included. Delayed or incomplete materials may delay delivery.
5. **Content entry and migration:** Product uploads, page population, historical data migration, and content cleanup are limited to the agreed quantities and formats.
6. **Responsive and browser compatibility:** Compatibility covers the devices, browsers, and versions identified in the scope. Identical appearance across every device and browser is not guaranteed.
7. **Integrations and webhooks:** Integration work covers the agreed systems, events, data fields, and workflows. The Client must provide valid access and subscriptions. External API changes or additional integrations may require separately quoted work.
8. **Hosting and server management:** Included hosting must specify its duration, capacity, management coverage, and renewal arrangement. One year of hosting does not imply unlimited traffic, storage, processing, maintenance, or development.
9. **Domains, licences, and external charges:** Domain registration, premium plugins, themes, email services, payment gateway charges, and other subscriptions are included only where expressly stated.
10. **Performance and SEO:** Speed and technical SEO work will follow the agreed scope. Performance depends on hosting, content, external scripts, and integrations. Specific speed scores, rankings, traffic, or indexing dates are not guaranteed unless expressly committed.
11. **Security and backups:** Security, backup, and restoration measures are limited to the agreed arrangement. Absolute protection against hacking, malware, data loss, or downtime is not guaranteed.
12. **Policies and regulatory content:** The Client must supply or approve privacy policies, terms of use, product claims, and other required business disclosures. Drafting or displaying these pages does not constitute legal advice.
13. **Testing and acceptance:** The Client must review the website against the agreed acceptance criteria within the agreed UAT period and report reproducible defects through the designated channel.
14. **Delivery criteria:** The website is considered delivered when the agreed features are functional in the agreed environment, acceptance requirements are satisfied, and the applicable handover obligations are completed. Delivery is not dependent on generating leads or sales.
15. **Warranty and subsequent changes:** Any defect warranty covers failures against the agreed specifications during its stated period. New requirements, redesigns, client edits, and external platform changes are handled under the applicable support or change arrangement.
16. **Handover and ownership:** Source code, credentials, documentation, account access, and ownership or licence rights will be transferred according to the agreed handover and payment conditions. Third-party components remain subject to their licences.

## 23. AI SDR — Sales Development Representative

These service-specific terms supplement the general terms above, including the no-refund-after-commencement policy, subject to applicable law and contractual remedies.

1. **Defined scope:** The service covers only the agreed prospect sources, communication channels, campaigns, workflows, languages, qualification criteria, CRM integrations, and activity limits.
2. **Service provider role:** The Provider configures and operates the agreed AI sales workflows. The Client remains responsible for its offers, pricing, sales decisions, negotiations, contracts, and customer fulfilment.
3. **No guaranteed outcomes:** The service does not guarantee lead volume, response rates, qualified prospects, booked meetings, attendance, conversions, revenue, or return on investment unless expressly agreed.
4. **Prospect data:** Responsibility for sourcing and validating contact data must be agreed. Contact details may be outdated, inaccurate, duplicated, or unavailable. Verification is included only to the agreed extent.
5. **Outreach authorisation and compliance:** The Client must approve the intended audience, channels, messages, and permitted use of prospect data. The parties must follow applicable outreach, privacy, and platform requirements within their respective responsibilities.
6. **Opt-outs and suppression:** The workflow must provide the agreed process for handling opt-outs, objections, and suppression lists. The Client must share relevant existing restrictions and avoid reintroducing suppressed contacts.
7. **Message approval:** The Client must approve product claims, offers, scripts, follow-up sequences, and qualification rules before activation. Material changes require renewed approval.
8. **AI response limitations:** AI may misunderstand messages, classify prospects incorrectly, or generate inaccurate responses. Human review and escalation will follow the agreed operating process.
9. **Authority limits:** The AI SDR may communicate only within its approved instructions. Discounts, guarantees, contractual commitments, refunds, and other commercial promises require authorised approval unless expressly permitted.
10. **Human escalation:** Complaints, sensitive requests, uncertain answers, and negotiations must follow the agreed escalation process. The Client must provide an available contact for matters requiring its decision.
11. **Qualification criteria:** “Qualified lead” and “qualified meeting” must be defined in writing. Qualification reflects available information and does not guarantee purchasing intent, budget accuracy, or a completed sale.
12. **Meeting scheduling:** Booking depends on prospect cooperation and calendar availability. Cancellations, rescheduling, no-shows, and inaccurate information are not guaranteed against.
13. **Deliverability and account restrictions:** Email delivery, inbox placement, call connection, message delivery, and account availability depend on external providers and recipient systems. Spam filtering, blocked numbers, and platform restrictions may affect performance.
14. **Sending infrastructure and usage costs:** Domains, inboxes, calling numbers, telephony, messaging, contact databases, CRM licences, and AI usage must have agreed funding arrangements and limits. Volume increases require approval.
15. **CRM and data handling:** Data fields, syncing, deduplication, retention, access, and reporting are limited to the agreed configuration. The Client must maintain required permissions and review material data discrepancies.
16. **Monitoring and optimisation:** Monitoring frequency, reporting, campaign adjustments, and support hours must be specified. Continuous human supervision is included only if expressly agreed.
17. **Delivery criteria:** Initial implementation is delivered when the agreed workflows, integrations, approved messaging, and escalation paths pass the agreed acceptance checks. Recurring delivery is measured against agreed activities and reports, rather than guaranteed sales outcomes.
18. **Client follow-up:** The Client is responsible for timely handling of escalations, meetings, proposals, and sales opportunities unless these activities are expressly included.

## 24. AI Social Media Management

These service-specific terms supplement the general terms above, including the no-refund-after-commencement policy, subject to applicable law and contractual remedies.

1. **Defined scope:** Services cover only the agreed social accounts, platforms, content formats, languages, posting frequency, approval workflow, and reporting activities.
2. **Content quantities:** Posts, captions, images, videos, stories, reels, and revisions are limited to the agreed quantities. Unused monthly allowances carry forward only if expressly agreed.
3. **Content production boundaries:** Photography, filming, presenters, voiceovers, advanced editing, influencer coordination, and original research are included only where specified.
4. **Client inputs:** The Client must provide accurate business information, brand guidelines, product details, assets, offers, and timely approvals.
5. **AI-generated content:** AI outputs may contain factual, visual, linguistic, or contextual errors. The agreed review process must be followed before publication. Human review is included only to the stated extent.
6. **Claims and publication approval:** The Client must approve business claims, prices, promotions, testimonials, and specialised statements. The Provider remains responsible for any expressly agreed review duties.
7. **Publishing authority:** The agreement must specify whether each post requires approval or whether publication is authorised within an approved content calendar and brand framework. Silence counts as approval only under an expressly agreed process.
8. **Revisions and rescheduling:** Included revision rounds and deadlines must be stated. Late feedback, changed offers, or changes after approval may affect the publishing schedule and incur additional charges.
9. **No guaranteed growth or results:** Services do not guarantee followers, reach, impressions, engagement, virality, enquiries, leads, sales, or revenue.
10. **Platform dependencies:** Algorithms, outages, moderation, account restrictions, feature changes, and content distribution are controlled by the platforms. Reinstatement or restoration cannot be guaranteed.
11. **Account ownership and access:** The Client retains ownership of its accounts and must provide authorised access. The parties must follow the agreed security process, including appropriate access controls.
12. **Community management:** Comment moderation, direct messages, review responses, and customer support are included only if specified, with clear hours, volumes, response targets, and escalation rules.
13. **Complaints and crisis response:** Sensitive complaints, legal threats, public controversies, and urgent incidents require Client escalation. Crisis management and continuous monitoring require a separate agreed scope.
14. **Advertising and external expenses:** Paid campaigns, ad spend, boosting, stock assets, music licences, scheduling tools, and AI credits are included only where expressly stated.
15. **Intellectual property and usage rights:** Client assets must have appropriate permissions. Stock media, music, AI-generated assets, and external tools remain subject to applicable usage conditions; exclusivity or registrability is not promised.
16. **Reporting:** Reports use the metrics available from the relevant platform or agreed tools. Platform reporting differences, attribution limits, and delayed data may affect figures.
17. **Delivery criteria:** Drafting services are delivered through the agreed content submissions. Publishing services are delivered through the agreed approved publications and reports. Client approval delays and platform failures must be documented and handled under an agreed rescheduling or reconciliation process.
18. **Service ending and handover:** On expiry or termination, scheduled content, account access, approved assets, and outstanding work will be handled under the agreed handover process. Future posting and monitoring cease according to the agreed service end date.

## Project-Specific Details to Record Before Issue

- Provider and Client identities; accepted agreement and document priority.
- Service titles, scope, quantities, exclusions, and package pricing.
- Payment milestones, taxes, due dates, and recurring charges.
- Commencement trigger, timeline, dependencies, and authorised approver.
- Revision limits, feedback windows, acceptance criteria, and closure process.
- Hosting period, usage allowances, renewal costs, and third-party funding.
- Security, backup, data-handling, support, and warranty commitments.
- Handover contents, ownership, licences, and payment conditions.
- Cancellation and recurring-service refund treatment; any agreed liability cap and indemnity.
- Governing law and dispute resolution arrangements.

*Apply only the provisions relevant to the engagement. Resolve project-specific details before issue and have the contractual terms reviewed for the applicable jurisdiction before using them as binding terms.*
