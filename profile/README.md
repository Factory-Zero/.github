<p align="center">
  <img src="https://raw.githubusercontent.com/Factory-Zero/.github/main/assets/org-banner.png" alt="Factory Zero — we build companies that operate and grow themselves." width="100%">
</p>

<p align="center">
  <a href="https://factory0.ventures"><img src="https://img.shields.io/badge/FACTORY0.VENTURES-LIVE-FF5A36?style=for-the-badge&labelColor=0A0A0B" alt="factory0.ventures"></a>
  <img src="https://img.shields.io/badge/VENTURES-03-EDEBE6?style=for-the-badge&labelColor=0A0A0B" alt="Ventures: 3">
  <a href="https://github.com/Factory-Zero/harness"><img src="https://img.shields.io/badge/HARNESS-RUST-EDEBE6?style=for-the-badge&labelColor=0A0A0B" alt="Harness: Rust"></a>
</p>

<p align="center">
  <sub>
    <a href="https://factory0.ventures">Site</a> &nbsp;·&nbsp;
    <a href="https://factory0.ventures/ventures/">Ventures</a> &nbsp;·&nbsp;
    <a href="https://factory0.ventures/system/">System</a> &nbsp;·&nbsp;
    <a href="https://factory0.ventures/technology/">Technology</a> &nbsp;·&nbsp;
    <a href="https://factory0.ventures/thesis/">Thesis</a> &nbsp;·&nbsp;
    <a href="https://factory0.ventures/enter/">Enter</a> &nbsp;·&nbsp;
    <a href="https://factory0.ventures/llms.txt">llms.txt</a>
  </sub>
</p>

---

## The company is becoming software.

Software automated the worker. Agents automate the organization.

The traditional company coordinates humans. The AI-native company coordinates
intelligence. Factory Zero is a venture studio built on that shift: it creates,
launches and operates companies through a shared network of autonomous agents,
and it owns them rather than advising them.

Not a fund. Not an accelerator. Not an agency.

---

## One operating system, every function an agent

Factory Zero OS runs as five layers. Each function in each layer is an agent.

| Layer | Agents |
| :--- | :--- |
| `DISCOVER` | Research · Strategy · Analytics |
| `BUILD` | Product · Engineering · Design · QA |
| `OPERATE` | Infrastructure · Security · Support · Finance |
| `DISTRIBUTE` | Growth · Content · Sales |
| `LEARN` | Legal · Knowledge · Optimization |

Every venture inherits the same foundation, so nothing is rebuilt: identity,
payments and billing, analytics, deployment, observability, agent
orchestration, support, marketing automation, finance, knowledge, security,
experimentation and internal tooling are all shared.

Each venture still holds its own brand, product, customers, data boundaries,
strategy, economics and P&L.

---

## The ventures

| | Venture | Category | Stage | |
| :--- | :--- | :--- | :--- | :--- |
| `FZ-001` | **Kontinuum** | Music | `PROTOTYPE` | [kontinuum.audio](https://kontinuum.audio) |
| `FZ-002` | **Undercover Rockstars** | Apparel | `LAUNCH` | [undercoverrockstars.com](https://undercoverrockstars.com) |
| `FZ-003` | **Yoginini** | Wellness | `VALIDATION` | [yoginini.us](https://yoginini.us) |

**Kontinuum** — an AI composer performing on a deterministic real-time engine.
Music written and performed continuously, personalised to the listener, and
playable offline. Not a streaming app and not a DAW: a living instrument.

**Undercover Rockstars** — a clothing house built on one idea: every piece comes
as a matched pair. One pattern is cut twice, once for the day and once for the
night, so the fit never changes when the room does. Drop 01 is eight pairs,
sixteen garments, cut in Bali.

**Yoginini** — a yoga teacher who can see you. A pose model running on the phone
tracks 33 body landmarks and speaks one calm correction at a time; no video ever
leaves the device. Real teachers are bookable by the hour alongside it.

> **None of the three is selling yet.** Every venture site states its own status
> plainly and no checkout is open anywhere. `autonomy` is `null` across the
> registry, which renders as an em dash rather than an invented percentage —
> please do not report any of them as shipped.

The registry lists only what exists. A venture with no public surface does not
get a placeholder row.

---

## Ordinary parts. Assembled once.

Every venture needs a backend, and none of them should build one. The parts a
company needs to exist are written once, as an **open-source harness in Rust**.
A venture picks the modules it wants, wires them in one file, and ships as a
single stateless worker with its own database.

```rust
Harness::builder()
    .venture(Venture::new("factory0", "factory0.ventures")
        .cors_origins(["https://factory0.ventures"]))
    .module(EmailSignup::new().double_opt_in(true))
    .module(Waitlist::new()
        .products(["kontinuum", "undercover-rockstars"]))
    .runtime(Cloudflare::new()
        .db("DB")
        .mailer(Resend::from_env())
        .captcha(Turnstile::from_env()))
    .build()?
```

If a module needs something the runtime cannot provide, or two modules claim the
same table, **the build fails before anything is deployed**. A misconfigured
venture cannot reach production.

| | |
| :--- | :--- |
| Language | Rust |
| Compute | Cloudflare Workers, compiled to WebAssembly |
| Database | Cloudflare D1 today, self-hosted Postgres later |
| Router | `axum`, the same router on the edge and on a server |
| Queries | `sea-query`, one query rendered for SQLite or Postgres |
| Isolation | One worker and one database per venture. Never a shared schema |

---

## Repositories

| Repo | What it is |
| :--- | :--- |
| [**harness**](https://github.com/Factory-Zero/harness) | The open-source Rust harness. Modules ship as `factory0-*` crates |
| [**venture-backend-template**](https://github.com/Factory-Zero/venture-backend-template) | Template for a new venture backend on the harness |
| [**website**](https://github.com/Factory-Zero/website) | [factory0.ventures](https://factory0.ventures). Static HTML, no build step, no dependencies |
| **.github** | This page and the mark |

A first TypeScript attempt at the harness was archived in September 2026 and
superseded by the Rust one. Those repositories are kept read-only and named
`*-ts-archived` so nobody builds on them by mistake.

---

## Enter

Build with us, invest, partner, or join. A human reads every request.

<p align="center">
  <br>
  <a href="https://factory0.ventures/enter/"><b>factory0.ventures/enter</b></a>
  &nbsp;·&nbsp;
  <a href="mailto:contact@factory0.ventures">contact@factory0.ventures</a>
</p>
