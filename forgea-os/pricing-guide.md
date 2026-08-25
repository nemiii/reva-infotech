# Forgea OS module pricing guide

## Purpose

Define an aggressive global launch-pricing model for selective module onboarding. Customers may either buy a bundled plan or activate a single module. The price is identical for customers in India and outside India.

This is a launch pricing proposal, not an irrevocable public price list. It must be reviewed against actual infrastructure, support, payment-processing, and edge-connectivity costs after the first 90 days of paid usage.

## Pricing principles

- Charge per organisation, not per employee, at entry level.
- Include a practical number of users and sites so small teams can adopt without licensing friction.
- Let a customer start with one useful module; do not force a full ERP purchase.
- Bundle multiple modules at a clear discount to encourage connected workflows.
- Keep the advertised list price identical worldwide and use USD as the published currency.
- Charge local taxes, including GST/VAT where applicable, in addition to listed prices.
- Keep self-service onboarding free. Price hands-on implementation separately only when it is offered.
- Do not promise advanced support, custom integrations, high-volume document storage, or hardware as part of these launch prices.

## User licence definitions

Use access-specific user categories. A person may belong to only one paid category at a time; assign the least-privileged category that supports their work.

| User category | Definition | Commercial treatment |
| --- | --- | --- |
| Full-access named user | A specific person with a Forgea login and broad operational or administrative access, such as an administrator, manager, buyer, salesperson, finance user, planner, or inventory controller | Counts against the plan's included full-access users or is charged as a full-access add-on |
| Employee self-service user | A specific employee login limited to ESS profile, shifts, attendance, leave, schedule, notifications, and assigned-team views | Does not consume a full-access seat; use the included Workforce/Connected Operations allowance or a low-cost ESS add-on |
| Named mobile-driver user | A specific driver login for the driver mobile application, assigned delivery runs, proof of delivery, GPS location updates, and delivery-task status | Paid separately from full-access seats because mobile GPS telemetry, sync, storage, and support create ongoing cost |
| Employee/driver record without login | A person record with no Forgea sign-in credential | Free; does not consume any user allowance |
| Technical identity | Edge node, API integration, service account, or connector credential | Not a human user; governed by edge-node/integration policy instead |

Do not price drivers as full-access users. They should be billed as named mobile-driver users at a lower rate, but must not be free when GPS tracking is active.

The low entry price is deliberately positioned against conventional per-user suites. Odoo currently lists its Standard plan at a per-user monthly price, while Zoho One also uses per-user licensing models. Forgea's launch proposition should be: **start with one operational workflow at a predictable organisation price.** [Odoo pricing](https://www.odoo.com/pricing), [Zoho One pricing](https://www.zoho.com/one/pricing/)

## Currency and billing policy

| Policy | Launch decision |
| --- | --- |
| Public price currency | USD |
| India and non-India list price | Same USD amount |
| Monthly billing | Available for every plan and standalone module |
| Annual billing | Pay for 10 months and receive 12 months of access |
| Trial | 14-day self-service trial for eligible modules; no credit card required initially |
| Taxes | Excluded from list price; collected where legally required |
| Price protection | Keep launch prices for the first 12 months of a customer's paid subscription |

At checkout, Indian customers may pay the INR equivalent of the same published USD amount; this is a payment conversion, not a separate India price list.

## Included platform foundation

Every paid plan or standalone module includes the Platform Foundation. It is not sold separately.

- Organisation and initial site
- Up to the included named-user limit
- Role-based access control, user invitations, and audit trail
- Documents/attachments and in-app notifications
- Core master-data framework
- Required module-specific number sequences and approval workflows
- Standard cloud hosting, backups, and product updates

The module onboarding service must create only the defaults required by the purchased modules. It must not provision full-app data or reveal unrelated navigation.

### Document storage allowance policy

Document storage is measured as the total active object-storage footprint for one organisation: attachments, generated documents, exported files, proof-of-delivery files, and uploaded business documents. It is pooled across that organisation's active modules and sites.

It does not include database records, audit logs, product backups, operational telemetry, or edge-node spool data. Those are governed by platform retention and fair-use policies rather than the document-storage add-on.

| Offer type | Included pooled document storage |
| --- | ---: |
| Standalone module | 10 GB per organisation |
| Essential Operations | 10 GB per organisation |
| Business Operations | 50 GB per organisation |
| Connected Operations | 150 GB per organisation |

Usage notifications should be sent at 80%, 90%, and 100% of the allowance. At the limit, retain existing files and block only new uploads until the customer removes files or purchases additional storage; never delete business documents automatically for exceeding a quota.

## Bundled plans

### 1. Essential Operations — **US$79/month** or **US$790/year**

For small teams digitising purchasing and customer billing without a full operations stack.

Included allowance:

- 1 organisation
- 1 site
- 5 full-access named users
- 10 GB pooled document storage
- Platform Foundation

Included modules:

- Procurement
- Invoicing & Receivables

Included onboarding scope:

- Suppliers, items/UOM, PR/PO numbering, and purchasing approval flow
- Customers, tax rules, payment terms, invoice/credit-note/receipt numbering
- Minimum finance configuration required for manual invoices, credit notes, and receipts

Not included:

- Warehouse stock receiving, inventory valuation, dispatch orders, production, maintenance, edge connectivity, or multi-site transfers

This plan remains functional as a purchase-request/PO and manual-invoicing solution. Inventory and Sales connections are presented only as upgrade paths.

### 2. Business Operations — **US$229/month** or **US$2,290/year**

For a growing business that needs an integrated commercial, purchasing, inventory, and financial-control workflow.

Included allowance:

- 1 organisation
- Up to 2 sites
- 15 full-access named users
- 50 GB pooled document storage
- Platform Foundation

Included modules:

- Procurement
- Inventory Operations
- Sales & Order Management
- Invoicing & Receivables
- Accounting & Financial Control
- Maintenance Management

Included onboarding scope:

- Suppliers, customers, items/UOM, warehouses, opening stock, tax rules, payment terms, fiscal periods, chart of accounts, and bank/cash accounts
- PR/PO, sales-order, invoice, payment, stock-movement, and maintenance workflow defaults
- Goods receipt, supplier return, dispatch, customer return, payables, receivables, inventory valuation, and reconciliation connections

Not included:

- Manufacturing execution, edge-based machine monitoring, workforce attendance/leave, delivery-fleet operations, or inter-site transfers

### 3. Connected Operations — **US$479/month** or **US$4,790/year**

For a factory or multi-location operator that wants Forgea OS as its connected operating system.

Included allowance:

- 1 organisation
- Up to 3 sites
- 30 full-access named users
- 100 employee self-service users
- 25 named mobile-driver users
- 1 registered edge node
- 150 GB pooled document storage
- Platform Foundation

Included modules:

- Every Business Operations module
- Manufacturing
- Machine Visibility
- Workforce & ESS
- Mobility & Delivery Operations
- Multi-Site Operations

Included onboarding scope:

- BOMs, routings, production/work-order settings, and inventory material flows
- Machines, edge-node credentials, signal mapping, alarm thresholds, and downtime monitoring
- Employee profiles, departments, shifts, schedules, attendance, and leave setup
- Fleets, vehicles, drivers, delivery-run rules, and proof-of-delivery setup
- At least two sites, site warehouses, transfer-order workflows, and in-transit setup

This plan includes product access, not physical edge hardware, custom PLC/connector development, or implementation consulting.

## Standalone module pricing

Each standalone module includes Platform Foundation, 1 site, and 5 full-access named users unless noted otherwise. Annual price equals ten times the monthly price. Standalone prices intentionally preserve a meaningful bundle discount: customers should choose a bundle whenever they need more than one or two connected operational modules.

| Module | Monthly | Annual | Included core capability | Required onboarding prerequisites |
| --- | ---: | ---: | --- | --- |
| Procurement | US$49 | US$490 | Suppliers, PRs, POs, approvals | Purchasing users, suppliers, items/UOM, PR/PO sequences, approval flow |
| Invoicing & Receivables | US$49 | US$490 | Manual invoices, customer credit notes, receipts, receivables | Customers, tax rules, payment terms, financial posting basics, invoice sequences |
| Machine Visibility | US$199 | US$1,990 | Machines, live signals, alarms, downtime, control plane | Machine users, machines, one edge node, signal mapping, thresholds, notification recipients |
| Inventory Operations | US$79 | US$790 | Warehouses, stock, ledger, movements, reservations | Items/UOM, warehouses, inventory users, opening stock/starting balances |
| Sales & Order Management | US$59 | US$590 | Customers, opportunities, quotations, sales orders, customer returns | Sales users, customers, items/UOM, quotation/order sequences |
| Accounting & Financial Control | US$99 | US$990 | Accounts, periods, tax, journals, payables, payments, reconciliation, reports | Finance users, chart of accounts, account groups, periods, tax rules, bank/cash accounts |
| Manufacturing | US$129 | US$1,290 | BOMs, routings, production orders, work orders | Inventory Operations, items/UOM, warehouses, BOMs, routings, manufacturing users |
| Maintenance Management | US$49 | US$490 | Assets, plans, incidents, repairs, repair logs | Maintenance users, assets/equipment, categories, assignees, workflow defaults |
| Workforce & ESS | US$49 | US$490 | Employees, hierarchy, shifts, attendance, leave, self-service; includes 50 employee self-service users | Employees, departments, shifts, attendance rules, leave policy, approvers |
| Mobility & Delivery Operations | US$89 | US$890 | Fleets, vehicles, drivers, manual delivery runs, inbound shipments, POD; includes 10 named mobile-driver users | Mobility users, fleet, vehicles, drivers, delivery-run sequence, proof rules |
| Multi-Site Operations | US$99 | US$990 | Material requests, transfer orders, in-transit tracking, cross-site dashboard | Inventory Operations, at least two sites, site warehouses, transfer users and workflow |

### Bundle value proposition

The bundle must be visibly cheaper than purchasing the same module set independently. The calculations below use monthly standalone list prices and exclude add-ons.

| Bundle | Equivalent standalone modules | Standalone total | Bundle price | Customer saving |
| --- | --- | ---: | ---: | ---: |
| Essential Operations | Procurement + Invoicing & Receivables | US$98/month | US$79/month | US$19/month (19%) |
| Business Operations | Procurement + Inventory + Sales + Invoicing + Accounting + Maintenance | US$384/month | US$229/month | US$155/month (40%) |
| Connected Operations | All eleven listed modules | US$949/month | US$479/month | US$470/month (50%) |

## Connection rules

Standalone purchase must not expose broken features. Enable these capabilities only when all modules in the left column are active.

| Active modules | Connected capability |
| --- | --- |
| Procurement + Inventory Operations | PO goods receipt and supplier-return stock handling |
| Procurement + Accounting | Supplier invoices, supplier credit notes, payables/payment context |
| Sales + Invoicing & Receivables | Order/customer commercial context for invoicing |
| Sales + Inventory Operations | Dispatch orders, stock reservation/availability, stock-aware customer returns |
| Sales + Inventory Operations + Invoicing | Dispatch/order-based invoicing and financially linked customer returns |
| Inventory Operations + Accounting | Inventory valuation, cost events, financial posting context |
| Manufacturing + Inventory Operations | Material reservation/issue and finished-goods receipt |
| Manufacturing + Accounting | WIP and production-cost reporting |
| Machine Visibility + Maintenance | Alarm/downtime-linked maintenance incidents |
| Machine Visibility + Manufacturing | Machine signal and downtime context in production work |
| Mobility + Sales | Dispatch-order-linked delivery runs |
| Mobility + Procurement or Inventory Operations | Inbound-shipment and receiving transport flows |
| Multi-Site Operations + Inventory Operations | Inter-site stock transfers and in-transit inventory |
| Multi-Site Operations + Mobility | Delivery-run management for transfers |

## Add-ons and overage pricing

Keep add-ons simple and proportionate to the operational cost they introduce at launch.

| Add-on | Monthly | Annual | Notes |
| --- | ---: | ---: | --- |
| Additional full-access named user | US$9 | US$90 | Applies above the plan/module included allowance |
| Additional employee self-service user | US$1 | US$10 | Applies above Workforce/Connected Operations allowance; ESS-only permissions required |
| Additional named mobile-driver user | US$5 | US$50 | Includes driver-app access and normal GPS/task sync; subject to fair-use telemetry limits |
| Additional site | US$25 | US$250 | Requires applicable site setup and administrator access |
| Additional edge node | US$59 | US$590 | Does not include hardware, SIM/data, or custom connector work |
| Additional document storage, 25 GB | US$15 | US$150 | Pooled at organisation level; applies above the included plan/module allowance |
| Guided remote onboarding | US$249 one-time | — | Up to two remote sessions for one selected module |

Do not introduce transaction fees, API-call fees, or user-minimum commitments in the launch period. Reassess only when verified usage costs require them.

## Availability policy

Do not list a module as purchasable merely because a navigation page exists. A module is public only after it meets every requirement below:

1. Selective activation and API module-entitlement guard are implemented.
2. Its onboarding checklist and idempotent default provisioning are implemented.
3. Module-specific navigation and direct-route protection are implemented.
4. Required dependencies are enforced and connected features are gated.
5. The module's browser/API onboarding fixture passes.

Until then, display the module as **Join the early-access list** rather than **Coming Soon** with a checkout action.

Initial public sequence:

1. Procurement
2. Invoicing & Receivables, after current end-to-end readiness gaps are closed
3. Machine Visibility, after selective setup, edge validation, and access protection are complete
4. Business Operations bundle after Inventory, Sales, and Accounting selective onboarding are complete
5. Connected Operations after Manufacturing, Workforce, Mobility, and Multi-Site selective onboarding are complete

## Unit-economics guardrails

The purpose of aggressive pricing is adoption, not subsidising unlimited infrastructure indefinitely.

Before public launch and every 90 days thereafter, calculate per-paid-organisation cost:

```text
monthly COGS =
  compute + database + backup + object storage + observability + email/SMS
  + payment processing + support tooling + allocated edge connectivity cost

gross margin = (monthly revenue - monthly COGS) / monthly revenue
```

Launch guardrails:

- Target at least 60% gross margin for standalone software modules.
- Target at least 50% gross margin for Machine Visibility and named mobile-driver users, because telemetry, location sync, and edge volume can be higher.
- If a customer exceeds normal shared-tenant limits, offer a fair-use or dedicated deployment quote rather than silently degrading service.
- Review module price, included users/sites, storage allowance, and edge-node allowance before raising list price.

## Sales positioning

Use one clear message:

> Start with the workflow you need today. Add connected operations only when your business is ready.

Examples:

- “Run PR and PO approvals from US$49/month—no per-employee licence minimum.”
- “Start invoicing from US$49/month; choose Essential Operations for both workflows at US$79/month.”
- “Monitor machines, alarms, and downtime from US$199/month including one edge node.”
- “Add tracked driver access for US$5 per named driver/month; driver GPS access is separate from manager seats.”

Avoid promising that every integration is included in a standalone module. State the upgrade path positively: “Connect Inventory to receive goods against purchase orders.”

## Pricing change governance

- Record every public price, discount, tax rule, and entitlement in the future billing catalogue rather than hard-coding it in the web application.
- Apply any price change only to new subscriptions unless the customer contract permits renewal changes.
- Require product, finance, and engineering review for changes that alter included users/sites/edge nodes because they affect provisioning and cost.
- Keep subscription entitlement separate from organisation activation and user permissions.

## Decision summary

| Offer | Launch price | Best for |
| --- | ---: | --- |
| Essential Operations | US$79/month | PR/PO plus manual invoicing for a small team |
| Business Operations | US$229/month | Integrated purchasing, stock, sales, billing, accounting, and maintenance |
| Connected Operations | US$479/month | Factory or multi-location operations with manufacturing, telemetry, people, delivery, and transfer workflows |
| Standalone module | US$49–199/month | Customers adopting one workflow at a time |

This model should remain intentionally simple until Forgea has enough paid usage data to distinguish low-cost business modules from higher-cost telemetry, storage, support, and edge workloads.
