# Refills, cancellations and refunds

These are separate workflows. Their availability depends on the service, current order state, provider capability, and applicable account policy.

## Refills

A refill is a request to replace eligible drops after an order has been delivered. It is not a refund for an order that was never fully delivered.

A service may specify:

- Whether refill is included
- The refill coverage period
- When the coverage period begins
- Conditions that make an order eligible
- Whether the customer can request it directly or must contact support

A refill option should appear only when the server confirms that the order is eligible. A service marked as having no refill coverage does not include replacement for later drops.

## Cancellations

Cancellation is available only for services and orders that can still be stopped. Delivery may begin quickly, and some orders cannot be canceled after processing has started.

A cancellation request is not proof that cancellation succeeded. The final order state must be checked after the request.

## Refunds and unused value

A refund in the SMMly panel is an account-balance credit for eligible undelivered value. It is distinct from a cash refund to the original payment method.

For partial or canceled orders, the final unused amount must be calculated from the order's authoritative financial record and recorded in the account ledger. Do not calculate a refund from a displayed remaining quantity alone.

## Contact support

Include the SMMly order ID and the exact target link. For payment-related requests, include the payment reference and method. Never send passwords, API keys, or full payment credentials.
