<div align="center">

# 🌐 Supa.NET!

### community wifi marketplace.

*transforming neighbourhood networks into a shared digital utility*

---

[![Status](https://img.shields.io/badge/status-concept%20%2F%20early%20stage-amber?style=flat-square)](.)
[![Location](https://img.shields.io/badge/origin-kampala%2C%20uganda-blue?style=flat-square)](.)
[![Model](https://img.shields.io/badge/model-community%20wifi%20mesh-green?style=flat-square)](.)
[![License](https://img.shields.io/badge/license-proprietary-lightgrey?style=flat-square)](.)

</div>

---

## table of contents

(i). [the problem](#i-the-problem)

(ii). [the vision](#ii-the-vision)

(iii). [how it works](#iii-how-it-works)

(iv). [the supernet explained](#iv-the-supernet-explained)

(v). [market opportunity](#v-market-opportunity)

(vi). [business model](#vi-business-model)

(vii). [product architecture](#vii-product-architecture)

(viii). [go-to-market strategy](#viii-go-to-market-strategy)

(ix). [challenges & mitigations](#ix-challenges--mitigations)

(x). [competitive landscape](#x-competitive-landscape)

(xi). [technology stack](#xi-technology-stack)

(xii). [resource requirements](#xii-resource-requirements)

(xiii). [the bigger vision](#xiii-the-bigger-vision)

(xiv). [next steps](#xiv-next-steps)

---

## (i). the problem

internet in uganda is still too expensive — not because the infrastructure doesn't exist, and not because the providers aren't there. MTN, Airtel, and Liquid Telecom are all present. unlimited packages exist. the issue is a fundamental mismatch between the **unit of purchase** and the **unit of need**.

every household buys their own subscription. individually. every month. even though:

- a neighbour's wifi signal already reaches your home
- unlimited packages are routinely underutilised (often below 40% capacity)
- the subscription one household pays for could comfortably serve several
- mobile data as a fallback is expensive and inconsistent

### the coordination problem

informal wifi sharing already happens everywhere in Kampala. neighbours already exchange passwords. relatives already share subscriptions. but informal sharing has critical limitations:

| limitation | why it matters |
|---|---|
| **no fairness** | one household pays; others ride for free |
| **no limits** | the paying subscriber's speeds suffer with no usage controls |
| **no trust layer** | sharing a home password exposes personal devices on the network |
| **no scale** | the arrangement stays small, personal, and fragile |

> **the gap:** there is no platform that makes informal wifi sharing formal, fair, safe, and scalable. that gap is the Supa.NET! opportunity.

---

## (ii). the vision

> *"the infrastructure for affordable internet already exists physically in Kampala's neighbourhoods. the signals are already in the air. the subscriptions are already being paid for. Supa.NET! is the coordination layer that transforms overlapping private networks into one shared public utility."*

**Supa.NET!** is a community-powered wifi marketplace. it enables households with active unlimited internet subscriptions to share their connectivity with verified neighbours and city residents — earning passive income in return. roaming users pay a single affordable Supa.NET! subscription and gain seamless access to any host network in the city — no passwords, no friction.

---

## (iii). how it works

Supa.NET! is built on a simple three-sided model:

```
┌─────────────────────────────────────────────────────────────────┐
│                        Supa.NET! platform                       │
│         authentication · billing · trust · management          │
└──────────────────┬───────────────────────────┬──────────────────┘
                   │                           │
         ┌─────────▼────────┐       ┌──────────▼─────────┐
         │      hosts        │       │      roamers        │
         │                  │       │                     │
         │  share existing  │       │  pay one affordable │
         │  unlimited wifi  │       │  subscription and   │
         │  subscriptions   │       │  connect anywhere   │
         │                  │       │                     │
         │  → earn passive  │       │  → no passwords     │
         │    income        │       │  → no friction      │
         └──────────────────┘       └─────────────────────┘
```

| participant | role | value received |
|---|---|---|
| **host** | shares existing unlimited subscription via a Supa.NET!-managed access point | passive monthly income; effective internet cost drops to zero — or profit |
| **roamer** | pays a single Supa.NET! subscription | affordable internet access on any host network in range |
| **Supa.NET!** | manages authentication, billing, isolation, and quality | platform revenue from subscription and commission splits |

---

## (iv). the supernet explained

the name reflects a genuine technical architecture.

a **supernet**, in the context of Supa.NET!, is a **virtual overlay network** — multiple independent wifi access points unified under one login, one billing system, and one user identity.

a roamer authenticates once with their Supa.NET! credentials. the underlying physical host network becomes invisible. from the roamer's perspective, there is one network: **Supa.NET!**

this is structurally identical to how international airport wifi chains, hotel groups, and national hotspot operators work — but built **community-first**, from the neighbourhood up.

### network isolation — the trust foundation

the feature that makes host participation viable is **mandatory network isolation**. every Supa.NET! access point separates roamer traffic from the host's personal home network at the router level (VLAN separation).

```
[ ISP modem / router ]   ←  provided by MTN / Airtel / Liquid
          │
[ Supa.NET! MikroTik node ]   ←  installed & managed by Supa.NET!
          │
    ┌─────┴──────┐
    │            │
[ home ]    [ Supa.NET! ]
 network      hotspot SSID
    │               │
host's         verified
personal       roamers
devices        only
```

> ⚠️ **critical principle:** a host's personal network — their laptop, phone, smart TV, and home devices — is **never** on the same network as a roaming user. this is non-negotiable and enforced at the hardware level.

---

## (v). market opportunity

### why uganda, why now

- uganda's internet penetration is growing at one of the fastest rates in Sub-Saharan Africa
- unlimited wifi packages are now commercially available from multiple providers across Kampala
- smartphone ownership is accelerating, creating natural roamer demand
- MTN MoMo and Airtel Money provide frictionless payment infrastructure already embedded in daily life
- urban density in Kampala means wifi signals from neighbouring homes genuinely overlap — the physical mesh **already exists**

### addressable market segments

| segment | profile | Supa.NET! role |
|---|---|---|
| **urban households** | Kampala residents with limited internet budgets | roamers — pay less for reliable access |
| **unlimited subscribers** | MTN/Airtel/Liquid subscribers with underutilised packages | hosts — earn from idle bandwidth |
| **students** | university and secondary school students needing data | roamers — affordable access near campuses |
| **small businesses** | boda stages, kiosks, salons, waiting areas | hosts with foot traffic earn; customers benefit |
| **corporates** | companies with staff who travel the city | business accounts — city-wide staff connectivity |

---

## (vi). business model

### revenue streams

| stream | description |
|---|---|
| **roamer subscriptions** | daily, weekly, and monthly passes sold to end users |
| **host commission split** | platform retains 30–40% of all roamer revenue attributed to a host node |
| **business accounts** | flat monthly corporate plans for employee city-wide roaming |
| **ISP partnership revenue** | revenue share with ISPs for driving subscriber retention and data volume |
| **premium host tiers** | hosts with better uptime or hardware earn more — incentivising quality |

### unit economics — illustrative model

> *for a single active host node:*

| item | illustrative figure |
|---|---|
| host's monthly ISP subscription cost | UGX 150,000 |
| active roamers on this node (monthly) | 15 unique users |
| average roamer spend per month | UGX 25,000 |
| **gross revenue from node** | **UGX 375,000** |
| host's share (65%) | UGX 243,750 |
| Supa.NET! platform share (35%) | UGX 131,250 |
| **host's net gain after ISP cost** | **UGX 93,750 profit per month** |
| **host's effective internet cost** | **free — plus income** |

at scale, a host earns passive income while their own internet subscription becomes economically self-sustaining. this is the primary host acquisition argument.

---

## (vii). product architecture

### core components

| component | description |
|---|---|
| **Supa.NET! router node** | MikroTik-based access point at each host location. manages dual SSID, VLAN isolation, bandwidth throttling, and captive portal auth. sits behind the existing ISP router — no ISP equipment changes needed. |
| **captive portal / auth layer** | when a roamer connects to any Supa.NET! SSID, the system silently verifies their subscription status before granting access. no passwords exchanged between host and roamer. |
| **host dashboard** | web and mobile portal for hosts to monitor earnings, active users, bandwidth usage, and payout history. |
| **roamer app** | mobile app showing nearby Supa.NET! hotspots, subscription management, and seamless auto-connect. |
| **central management platform** | backend system for firmware updates, node health monitoring, billing management, and automated MoMo payouts to hosts. |
| **payments integration** | MTN Mobile Money and Airtel Money for both subscription collection and host payout disbursement. |

---

## (viii). go-to-market strategy

### phase (i) — neighbourhood proof of concept *(months 1–3)*

> validate the model. manual everything. one neighbourhood.

- recruit **3–5 willing hosts** within one neighbourhood
- deploy MikroTik nodes; set up manual voucher-based access
- collect payments via MoMo manually; pay host cuts manually
- ✅ **success metric:** 15+ paying roamers within 60 days

### phase (ii) — platform build *(months 4–9)*

> build the product on proven demand.

- develop host dashboard, roamer app, and central auth platform
- automate MoMo billing and host payouts
- implement captive portal authentication at hardware level
- expand to **3 neighbourhoods** in Kampala
- ✅ **success metric:** 10+ active host nodes, 200+ roamer subscribers

### phase (iii) — ISP engagement & city scale *(months 10–18)*

> formalise the model. expand aggressively.

- approach MTN, Airtel, and Liquid with traction data — propose **licensed reseller or partner model**
- introduce tiered roamer plans (hourly, daily, monthly, corporate)
- add host quality ratings and service level indicators
- expand to bodaboda stages, markets, clinics, and schools
- ✅ **success metric:** 100+ host nodes, 2,000+ active subscribers

### phase (iv) — regional expansion *(18+ months)*

> export the model.

- replicate in Entebbe, Jinja, Mbarara, Gulu
- launch corporate account product for city-wide employee roaming
- **license the Supa.NET! platform** to operators in Nairobi, Dar es Salaam, and Kigali
- explore partnerships with national broadband expansion programmes

---

## (ix). challenges & mitigations

| challenge | risk level | mitigation |
|---|:---:|---|
| **ISP terms of service** — most unlimited packages prohibit commercial reselling | 🔴 high | early ISP engagement; structure as a partnership, not a resale; pursue formal licensed agreements |
| **host trust & privacy** — hosts fear strangers accessing their home network | 🔴 high | mandatory VLAN isolation at hardware level; market this as the core safety feature |
| **network quality variance** — different hosts offer very different speeds | 🟡 medium | host quality ratings; bandwidth guarantees enforced by platform; tiered pricing by quality |
| **chicken-and-egg problem** — need hosts before roamers; need roamers before hosts see value | 🟡 medium | hyper-local launch — seed each neighbourhood densely before moving to the next |
| **technical complexity for hosts** — non-technical users need to install equipment | 🟡 medium | Supa.NET! owns, installs, and remotely manages all hardware; host involvement is near-zero |
| **regulatory uncertainty** — telecoms regulation in Uganda may evolve | 🟢 low–med | proactive engagement with Uganda Communications Commission (UCC) from early stage |
| **payment reliability** — MoMo transactions can fail or delay | 🟢 low | multi-provider MoMo integration; automatic retry logic; clear payout schedules |

---

## (x). competitive landscape

no operator in Uganda currently offers a **community-owned, income-generating wifi sharing network** with automatic authentication, MoMo payments, and network isolation. this is Supa.NET!'s white space.

| operator | model | geography | why Supa.NET! is different |
|---|---|---|---|
| **Fon** | home router sharing cooperative | Europe, global | ISP-partnered from inception; Supa.NET! is community-first with ISP partnership as a later stage |
| **Karma WiFi** | pay-per-use shared hotspot network | United States | US market; no MoMo-native payments; not built for African urban density |
| **MTN WiFi Zones** | ISP-operated public hotspots | Uganda | fixed locations only; not community-distributed; no income for participants |
| **Airtel Public WiFi** | ISP-operated hotspots | Uganda | same limitation — centrally owned, not community-distributed or income-generating |

---

## (xi). technology stack

### why MikroTik for host hardware

consumer-grade routers provided by ISPs are designed for simplicity, not programmability. they cannot:

- run a captive portal
- enforce VLAN isolation programmatically
- be remotely managed via API
- throttle bandwidth per user class

**MikroTik RouterOS** provides all of these natively, at a cost of approximately **UGX 150,000–300,000** per unit — well within the unit economics of the model.

| capability required | MikroTik support |
|---|:---:|
| captive portal / subscriber authentication | ✅ native (HotSpot Manager built-in) |
| VLAN isolation (home vs. roamer network) | ✅ hardware-enforced |
| remote API management | ✅ full REST and Winbox API |
| per-user bandwidth throttling | ✅ Queue Trees — granular control |
| multiple SSID broadcast | ✅ full support |
| deployment behind existing ISP router | ✅ no ISP equipment changes required |

MikroTik devices are widely used across Uganda and East Africa, with a strong local technician ecosystem and parts availability on **Kampala's Nasser Road**.

---

## (xii). resource requirements

> *phase (i) & (ii) seed estimates — conceptual range pending phase (i) validation*

| resource | estimated cost (UGX) |
|---|---|
| MikroTik nodes — phase (i) pilot (10 hosts) | 2,000,000 – 3,000,000 |
| software development (platform, apps, auth) | 15,000,000 – 40,000,000 |
| MoMo integration & payment setup | 1,000,000 – 2,000,000 |
| operations & field installation (phase (i)) | 1,000,000 – 2,000,000 |
| legal & regulatory consultation (UCC) | 2,000,000 – 5,000,000 |
| marketing & host acquisition (phase (i)) | 1,000,000 – 3,000,000 |
| **total estimated phase (i)–(ii) seed requirement** | **22,000,000 – 55,000,000** |

---

## (xiii). the bigger vision

Supa.NET! is designed from the outset to be **replicable**. every neighbourhood in every Ugandan city has the same structural conditions: overlapping wifi signals, underutilised unlimited subscriptions, and a community of people paying more collectively than they need to.

the Kampala proof of concept is not the product — it is the **template**.

```
Kampala neighbourhood pilot
         ↓
other Kampala neighbourhoods (Ntinda, Bukoto, Kansanga, Naalya)
         ↓
secondary Ugandan cities (Jinja, Mbarara, Gulu, Masaka, Mbale)
         ↓
East African markets (Nairobi, Dar es Salaam, Kigali, Lusaka)
         ↓
platform licensing — Supa.NET! as an OS for community wifi operators globally
```

> **the long-term opportunity:** if even 1% of households in Kampala become Supa.NET! hosts, and each host serves 10 roamers, Supa.NET! becomes the largest distributed wifi network in Uganda — built not by a telecom company, but by **the community itself**.

---

## (xiv). next steps

the single most important thing Supa.NET! can do right now is **validate the economics in the real world** before building anything complex.

- [ ] (i). identify **5 founding host households** in one Kampala neighbourhood
- [ ] (ii). install MikroTik nodes and configure manual voucher-based access
- [ ] (iii). onboard first paying roamers via word of mouth
- [ ] (iv). run manual MoMo billing and host payouts for 60 days
- [ ] (v). document what works, what breaks, and what people actually pay
- [ ] (vi). build the platform on proven demand

---

<div align="center">

---

*Supa.NET! — Kampala, Uganda — 2025*

*this is a community utility, built by the community, for the community.*

---

</div>
