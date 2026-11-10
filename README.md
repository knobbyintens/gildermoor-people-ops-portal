# Gildermoor People Ops portal

This repository holds the machine-readable intake material used by the People
Ops team of Gildermoor Analytics.

- `intake/` — one JSON manifest per onboarding request. Only manifests whose
  `status` is `APPROVED` may be processed.
- `config/onboarding-rules.json` — how an approved manifest maps onto a
  register record (status, badge numbering, owner attribution).

Do not hand-edit manifests; new requests are committed by the intake bot.
