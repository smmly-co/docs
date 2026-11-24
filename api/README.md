# SMMly API

**Current status: Not released.** The SMMly customer API is currently unavailable. This page is a release-status notice, not an integration guide.

The private application's `apiconnect/index.php` currently returns HTTP 503 before its legacy handler executes. The action names visible behind that containment are not a supported contract.

## Restoration sequence

The private remediation roadmap requires these tasks before the public SMM V2 API is restored:

1. R1-1 — financial-integrity primitives.
2. R1-3 — attributable, capped refunds.
3. R1-4 — safe provider response classification.
4. R2-1 — provider HTTP outside money transactions, a shared submission writer, and protection against resubmitting unknown outcomes.
5. R2-2 — restore the API using the shared submission/refund path and preserve existing request/response shapes.

The API include path must not be repaired and the HTTP 503 containment must not be removed ahead of those prerequisites.

## Compatibility direction

- Preserve existing request and response shapes for the existing SMM V2 actions when restored.
- Keep API and web order pricing/discount behavior aligned under the required owner decision.
- Add new actions only additively and only after their server-side rules and provider capabilities are verified.
- Do not infer support from legacy code, field names, or a roadmap item.

## Refill, cancellation, and provider evidence

Refill/cancel behavior depends on the order-state work in R2-4 and provider-specific capability evidence in R2-6. Provider status synchronization is separately gated by R2-5. Provider evidence must come from current provider documentation and authorized read-only probes; never use live `add`, `refill`, or `cancel` calls as capability tests.

## Do not integrate yet

Do not build production integrations against guessed URLs, parameters, response fields, or the unreachable legacy handler. Do not assume an endpoint is available because its action name appears in source code.

## Release tracking

- [API contract and release status](https://github.com/smmly-co/smmpanel-api/blob/main/CONTRACT-STATUS.md)
- [Evidence-based API release checklist](https://github.com/smmly-co/smmpanel-api/blob/main/RELEASE-CHECKLIST.md)

API documentation and examples will be promoted from draft to supported only after implementation verification, staging tests, and explicit owner release approval.
