# Orders and order tracking

This guide explains the intended customer order lifecycle in SMMly.

> **Availability note:** Exact screens, fields, and status behavior are subject to the current product release and service configuration.

## Before placing an order

1. Select the platform and service.
2. Read the service type and target requirements.
3. Check the minimum and maximum quantity.
4. Review the rate, estimated timing, refill terms, and cancellation availability.
5. Submit the public link or username requested by the service.
6. Confirm the quantity and displayed charge.

Never provide a social platform password. Keep the target public and unchanged when the service requires public access.

## Order statuses

| Status | Meaning |
|---|---|
| Pending | The order is queued and has not started |
| In progress | Delivery is underway |
| Processing | A service-specific processing state |
| Completed | The requested delivery is complete |
| Partial | Delivery ended before the full quantity was delivered |
| Canceled | The order was canceled |
| Error | The order could not be processed |

The final status and remaining quantity are determined by SMMly's order state and provider synchronization. A provider's wording may be normalized for display.

## Order details

Where available, an order record should show:

- SMMly order ID
- Service name and service ID
- Target link or username
- Requested quantity
- Charge and currency
- Start count
- Remaining quantity
- Current status
- Creation time and latest update
- Refill or cancellation actions when eligible

## Partial delivery

When an order ends before the full requested quantity is delivered, the unused portion is reconciled according to the final order charge and the account's transaction ledger. The account history should show any resulting credit.

## Avoid overlapping orders

Do not submit a second order for the same target while the first is still active unless the service explicitly allows it. Overlapping orders can make delivery counts and eligibility difficult to determine.

## Slow or stalled orders

Delivery estimates are averages, not guarantees. If an order appears stalled, contact support with its order ID and exact target link. Do not create a duplicate order just because progress is slow.
