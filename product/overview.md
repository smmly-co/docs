# SMMly product overview

SMMly is a self-hosted social media marketing panel for creators, agencies, service businesses, and resellers.

It brings a service catalogue, customer accounts, prepaid balances, order workflows, provider connections, and administration into one panel. The product is designed for operators who want to manage their own customer-facing SMM business.

> **Availability note:** This guide describes the target product experience. Individual features may be unavailable or changing while the product is being completed and verified.

## Core workflows

### Discover services

Browse services by platform and category. A useful service listing should show:

- Service name and description
- Service type and supported target format
- Rate and billing unit
- Minimum and maximum quantity
- Estimated start or delivery information, where available
- Refill coverage and duration, where applicable
- Cancellation availability, where applicable
- Service-specific requirements and restrictions

Rates should be clear before a customer confirms an order. Unless a service states otherwise, the target pricing model is a rate per 1,000 units.

### Place an order

Choose a service, provide the requested public profile/post/channel link or username, enter a quantity within the service limits, review the charge, and submit.

SMMly should never ask customers for their social platform password. Customers are responsible for submitting a valid target and keeping it accessible while delivery is in progress.

### Track delivery

The order history provides an order ID, selected service, target, quantity, charge, start count, remaining quantity, and current status where those fields are available.

Delivery speed is service- and provider-dependent. Estimates are not guarantees.

### Manage account balance

Customers add funds through the payment methods enabled for their account and use their panel balance for orders. Order-related credits and refunds are reflected in account transaction history.

Panel balance is order credit. It should not be presented as a cash-withdrawal facility unless a separate policy explicitly says otherwise.

### Get help

Support requests should include the order ID and the target link for order-related questions. Payment requests should include the payment reference and method, but never card secrets, passwords, or API keys.

## Service eligibility

Not every service supports every workflow. Refill, cancellation, drip-feed, custom comments, and other advanced options must be shown only when the selected service supports them.

## Reseller workflows

SMMly is designed to support programmatic reseller workflows through a customer API. The API is currently a draft; see the [API repository](https://github.com/smmly-co/smmpanel-api) for release status.
