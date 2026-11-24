# SMMly for resellers

SMMly is being built to support operators who manage customer-facing SMM services and want to connect their own applications to a central service panel.

## Intended reseller workflows

- Browse the available service catalogue.
- Read service rates, limits, and capabilities.
- Create customer orders programmatically.
- Check one or many order statuses.
- Read the authenticated account balance.
- Request eligible refills.
- Check refill status.
- Request cancellation for eligible orders.

## API

The target API follows established SMM V2-style conventions and uses a single POST endpoint with an API key, action name, and JSON response.

The API is not currently released. Review the [draft API specification](https://github.com/smmly-co/smmpanel-api/blob/main/API.md), but do not connect a production panel until SMMly publishes an active endpoint and final compatibility contract.

## Integration safety

- Keep API keys on your server; never expose them in frontend JavaScript.
- Use HTTPS.
- Validate service IDs and quantity limits from the live catalogue.
- Do not retry an order creation request blindly after a timeout.
- Check order status before attempting recovery from an uncertain response.
- Respect per-service refill and cancellation eligibility.
- Reconcile customer billing with your own ledger and SMMly's returned order data.

## Planned compatibility

SMMly aims to preserve familiar SMM V2 action names and request shapes where verified. Exact service-type fields, error responses, rate limits, and supported operations will be confirmed in the released API documentation.
