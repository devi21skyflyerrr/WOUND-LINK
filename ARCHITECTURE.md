# Architecture: WOUND-LINK

Single-page, serverless, offline web app. No backend, no database, no network calls.

```
Nurse / health worker (phone browser)
        |
        v
  index.html (HTML + CSS + JavaScript)
  +-------------------------------------------+
  | Assessment form (patient code, wound,     |
  |   danger signs, risk factors, photo*)     |
  | assess(): URGENT / REFER / MONITOR or     |
  |   HIGH / MODERATE / LOW risk + review days|
  | Follow-up register (localStorage, device) |
  | Caregiver guide (static page)             |
  +-------------------------------------------+
  *photo preview only; not stored or sent
```

## Design decisions
- Offline and static so it works in low-connectivity settings and hosts free on GitHub Pages.
- Patient codes instead of names; the register stays on the device.
- Any danger sign overrides everything else and gives URGENT.
- Intervals and triggers are defaults pending clinical review.

## Roadmap
Validated risk scale (with permission), validated regional-language wording, facility dashboard, optional sensor-based repositioning aid.
