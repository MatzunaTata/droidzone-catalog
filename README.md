# DroidZone vehicle catalog

Public copy of the vehicle catalog used by the DroidZone apps (e.g. the fuel log):
makes, models and engine/battery variants, each with a **permanent id**.

- File: [`vehicles.json`](vehicles.json) – fetched by the apps about once a week.
- **Generated – do not edit here.** The source of truth lives in the (private) DroidZone repository under
  `catalog/`; a CI workflow publishes it here on every merge to `main`.
- Ids are never changed or removed; outdated entries are marked `"deprecated": true`.
