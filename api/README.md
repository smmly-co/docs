# SMMly API

**Current status: Not released.** The SMMly customer API is currently unavailable. This page is a release-status notice, not an integration guide.

The private application contains a legacy SMM V2-style handler, but its public entry point currently returns HTTP 503 before that handler executes. The action names visible in the older code are not a supported contract.

## Planned API surface

The remediation roadmap identifies the following compatibility direction:

- Preserve existing request and response shapes when restoring legacy actions.
- Restore the existing balance, services, add-order, and order-status actions only after the financial-integrity and order-submission prerequisites are complete.
- Add refill and cancellation only after their behavior, provider capability, and authorization rules are verified.
- Keep pricing and discount behavior consistent between web and API order channels.
- Publish authentication, validation, rate-limit, error, retry, and timeout behavior with the actual implementation.

## Do not integrate yet

Do not build production integrations against guessed URLs, parameters, response fields, or the unreachable legacy handler. Do not assume an endpoint is available because its action name appears in source code.

## Release tracking

The canonical gate checklist is maintained in the [SMMly API repository](https://github.com/smmly-co/smmpanel-api). API documentation and examples will be promoted from draft to supported only after staging verification and owner release approval.
