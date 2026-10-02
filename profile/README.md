<p align="center">
  <img src="https://raw.githubusercontent.com/Factory-Zero/.github/main/assets/org-banner.png" alt="Factory Zero — we build companies that operate and grow themselves." width="100%">
</p>

<p align="center">
  <a href="https://factory0.ventures"><img src="https://img.shields.io/badge/FACTORY0.VENTURES-LIVE-FF5A36?style=for-the-badge&labelColor=0A0A0B" alt="factory0.ventures"></a>
  <img src="https://img.shields.io/badge/VENTURES-18-EDEBE6?style=for-the-badge&labelColor=0A0A0B" alt="Ventures: 18">
  <a href="https://github.com/Cratefield/harness"><img src="https://img.shields.io/badge/HARNESS-RUST-EDEBE6?style=for-the-badge&labelColor=0A0A0B" alt="Harness: Rust"></a>
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
| `FZ-004` | **Cratefield** | Infrastructure | `VALIDATION` | [cratefield.com](https://cratefield.com) |
| `FZ-005` | **VibeCaddie** | Developer tools | `VALIDATION` | [vibecaddie.com](https://vibecaddie.com) |
| `FZ-006` | **Colonizer** | Developer tools | `PROTOTYPE` | [colonizer.dev](https://colonizer.dev) |
| `FZ-007` | **FindsYou.work** | Careers | `VALIDATION` | [findsyou.work](https://findsyou.work) |
| `FZ-008` | **SupportGenius** | Support | `VALIDATION` | [supportgeni.us](https://supportgeni.us) |
| `FZ-009` | **promptdecode** | Security | `VALIDATION` | [promptdeco.de](https://promptdeco.de) |
| `FZ-010` | **Groove Guru** | Music | `VALIDATION` | [groove.guru](https://groove.guru) |
| `FZ-011` | **PosPlugin** | Integrations | `VALIDATION` | [posplug.in](https://posplug.in) |
| `FZ-012` | **Keep Shipping** | Developer tools | `VALIDATION` | [keepshipping.run](https://keepshipping.run) |
| `FZ-013` | **Owlpost** | Email | `VALIDATION` | [owlpost.to](https://owlpost.to) |
| `FZ-014` | **Bloodrank** | Community | `VALIDATION` | [bloodrank.dev](https://bloodrank.dev) |
| `FZ-015` | **ratecla.im** | Travel | `VALIDATION` | [ratecla.im](https://ratecla.im) |
| `FZ-016` | **Sealbin** | Security | `VALIDATION` | [sealb.in](https://sealb.in) |
| `FZ-017` | **release.show** | Video | `VALIDATION` | [release.show](https://release.show) |
| `FZ-018` | **Living Brain** | Developer tools | `VALIDATION` | [livingbrain.wiki](https://livingbrain.wiki) |

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

**Living Brain** — a brain for your team that writes its own company wiki and
keeps improving it, planned for Slack, coding agents over MCP, and the terminal
as one fast Rust binary. Team conversations would become Markdown pages for
people, projects, decisions and customers, every fact linked to its source
message, with nightly passes that merge duplicates, surface contradictions and
refresh stale facts. Open core (Apache-2.0, with a commercial `ee/`), built in
Rust as a Cratefield venture on Cloudflare Workers. Nothing is built yet: the
plan is four epics and 38 issues in
[Livingbrain-wiki/livingbrain](https://github.com/Livingbrain-wiki/livingbrain),
and early access is a waitlist.

Every record's full description, aims and public source links are in the
[registry](https://factory0.ventures/ventures/).

> **None of the eighteen is selling yet.** Every venture site states its own status
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
| [**harness**](https://github.com/Cratefield/harness) | The open-source Rust harness every venture backend compiles from. Moved to the [Cratefield](https://github.com/Cratefield) organisation in September 2026, which is the venture that commercialises it. Still MIT, still `factory0-*` crates |
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
