<div align="center">

# 🌐 Supa.NET!

### Community WiFi Marketplace.

*Transforming Neighbourhood Networks into a Shared Digital Utility*

---

[![Status](https://img.shields.io/badge/Status-Concept%20%2F%20Early%20Stage-amber?style=flat-square)](.)
[![Location](https://img.shields.io/badge/Origin-Kampala%2C%20Uganda-blue?style=flat-square)](.)
[![Model](https://img.shields.io/badge/Model-Community%20WiFi%20Mesh-green?style=flat-square)](.)
[![License](https://img.shields.io/badge/License-Proprietary-lightgrey?style=flat-square)](.)

</div>

---

## Table of Contents

1. [The Problem](#1-the-problem)
2. [The Vision](#2-the-vision)
3. [How It Works](#3-how-it-works)
4. [The Supernet Explained](#4-the-supernet-explained)
5. [Market Opportunity](#5-market-opportunity)
6. [Business Model](#6-business-model)
7. [Product Architecture](#7-product-architecture)
8. [Go-to-Market Strategy](#8-go-to-market-strategy)
9. [Challenges & Mitigations](#9-challenges--mitigations)
10. [Competitive Landscape](#10-competitive-landscape)
11. [Technology Stack](#11-technology-stack)
12. [Resource Requirements](#12-resource-requirements)
13. [The Bigger Vision](#13-the-bigger-vision)
14. [Next Steps](#14-next-steps)

---

## 1. The Problem

Internet in Uganda is still too expensive — not because the infrastructure doesn't exist, and not because the providers aren't there. MTN, Airtel, and Liquid Telecom are all present. Unlimited packages exist. The issue is a fundamental mismatch between the **unit of purchase** and the **unit of need**.

Every household buys their own subscription. Individually. Every month. Even though:

- A neighbour's WiFi signal already reaches your home
- Unlimited packages are routinely underutilised (often below 40% capacity)
- The subscription one household pays for could comfortably serve several
- Mobile data as a fallback is expensive and inconsistent

### The Coordination Problem

Informal WiFi sharing already happens everywhere in Kampala. Neighbours already exchange passwords. Relatives already share subscriptions. But informal sharing has critical limitations:

| Limitation | Why It Matters |
|---|---|
| **No fairness** | One household pays; others ride for free |
| **No limits** | The paying subscriber's speeds suffer with no usage controls |
| **No trust layer** | Sharing a home password exposes personal devices on the network |
| **No scale** | The arrangement stays small, personal, and fragile |

> **The Gap:** There is no platform that makes informal WiFi sharing formal, fair, safe, and scalable. That gap is the Supa.NET! opportunity.

---

## 2. The Vision

> *"The infrastructure for affordable internet already exists physically in Kampala's neighbourhoods. The signals are already in the air. The subscriptions are already being paid for. Supa.NET! is the coordination layer that transforms overlapping private networks into one shared public utility."*

**Supa.NET!** is a community-powered WiFi marketplace. It enables households with active unlimited internet subscriptions to share their connectivity with verified neighbours and city residents — earning passive income in return. Roaming users pay a single affordable Supa.NET! subscription and gain seamless access to any host network in the city — no passwords, no friction.

---

## 3. How It Works

Supa.NET! is built on a simple three-sided model:

```
┌─────────────────────────────────────────────────────────────────┐
│                        SUPA.NET! PLATFORM                       │
│         Authentication · Billing · Trust · Management          │
└──────────────────┬───────────────────────────┬──────────────────┘
                   │                           │
         ┌─────────▼────────┐       ┌──────────▼─────────┐
         │      HOSTS        │       │      ROAMERS        │
         │                  │       │                     │
         │  Share existing  │       │  Pay one affordable │
         │  unlimited WiFi  │       │  subscription and   │
         │  subscriptions   │       │  connect anywhere   │
         │                  │       │                     │
         │  → Earn passive  │       │  → No passwords     │
         │    income        │       │  → No friction      │
         └──────────────────┘       └─────────────────────┘
```

| Participant | Role | Value Received |
|---|---|---|
| **Host** | Shares existing unlimited subscription via a Supa.NET!-managed access point | Passive monthly income; effective internet cost drops to zero — or profit |
| **Roamer** | Pays a single Supa.NET! subscription | Affordable internet access on any host network in range |
| **Supa.NET!** | Manages authentication, billing, isolation, and quality | Platform revenue from subscription and commission splits |

---

## 4. The Supernet Explained

The name reflects a genuine technical architecture.

A **supernet**, in the context of Supa.NET!, is a **virtual overlay network** — multiple independent WiFi access points unified under one login, one billing system, and one user identity.

A roamer authenticates once with their Supa.NET! credentials. The underlying physical host network becomes invisible. From the roamer's perspective, there is one network: **Supa.NET!**

This is structurally identical to how international airport WiFi chains, hotel groups, and national hotspot operators work — but built **community-first**, from the neighbourhood up.

### Network Isolation — The Trust Foundation

The feature that makes host participation viable is **mandatory network isolation**. Every Supa.NET! access point separates roamer traffic from the host's personal home network at the router level (VLAN separation).

```
[ ISP Modem / Router ]   ←  provided by MTN / Airtel / Liquid
          │
[ Supa.NET! MikroTik Node ]   ←  installed & managed by Supa.NET!
          │
    ┌─────┴──────┐
    │            │
[ HOME ]    [ SUPA.NET! ]
 Network      Hotspot SSID
    │               │
Host's         Verified
personal       Roamers
devices        only
```

> ⚠️ **Critical Principle:** A host's personal network — their laptop, phone, smart TV, and home devices — is **never** on the same network as a roaming user. This is non-negotiable and enforced at the hardware level.

---

## 5. Market Opportunity

### Why Uganda, Why Now

- Uganda's internet penetration is growing at one of the fastest rates in Sub-Saharan Africa
- Unlimited WiFi packages are now commercially available from multiple providers across Kampala
- Smartphone ownership is accelerating, creating natural roamer demand
- MTN MoMo and Airtel Money provide frictionless payment infrastructure already embedded in daily life
- Urban density in Kampala means WiFi signals from neighbouring homes genuinely overlap — the physical mesh **already exists**

### Addressable Market Segments

| Segment | Profile | Supa.NET! Role |
|---|---|---|
| **Urban Households** | Kampala residents with limited internet budgets | Roamers — pay less for reliable access |
| **Unlimited Subscribers** | MTN/Airtel/Liquid subscribers with underutilised packages | Hosts — earn from idle bandwidth |
| **Students** | University and secondary school students needing data | Roamers — affordable access near campuses |
| **Small Businesses** | Boda stages, kiosks, salons, waiting areas | Hosts with foot traffic earn; customers benefit |
| **Corporates** | Companies with staff who travel the city | Business accounts — city-wide staff connectivity |

---

## 6. Business Model

### Revenue Streams

| Stream | Description |
|---|---|
| **Roamer Subscriptions** | Daily, weekly, and monthly passes sold to end users |
| **Host Commission Split** | Platform retains 30–40% of all roamer revenue attributed to a host node |
| **Business Accounts** | Flat monthly corporate plans for employee city-wide roaming |
| **ISP Partnership Revenue** | Revenue share with ISPs for driving subscriber retention and data volume |
| **Premium Host Tiers** | Hosts with better uptime or hardware earn more — incentivising quality |

### Unit Economics — Illustrative Model

> *For a single active host node:*

| Item | Illustrative Figure |
|---|---|
| Host's monthly ISP subscription cost | UGX 150,000 |
| Active roamers on this node (monthly) | 15 unique users |
| Average roamer spend per month | UGX 25,000 |
| **Gross revenue from node** | **UGX 375,000** |
| Host's share (65%) | UGX 243,750 |
| Supa.NET! platform share (35%) | UGX 131,250 |
| **Host's net gain after ISP cost** | **UGX 93,750 profit per month** |
| **Host's effective internet cost** | **Free — plus income** |

At scale, a host earns passive income while their own internet subscription becomes economically self-sustaining. This is the primary host acquisition argument.

---

## 7. Product Architecture

### Core Components

| Component | Description |
|---|---|
| **Supa.NET! Router Node** | MikroTik-based access point at each host location. Manages dual SSID, VLAN isolation, bandwidth throttling, and captive portal auth. Sits behind the existing ISP router — no ISP equipment changes needed. |
| **Captive Portal / Auth Layer** | When a roamer connects to any Supa.NET! SSID, the system silently verifies their subscription status before granting access. No passwords exchanged between host and roamer. |
| **Host Dashboard** | Web and mobile portal for hosts to monitor earnings, active users, bandwidth usage, and payout history. |
| **Roamer App** | Mobile app showing nearby Supa.NET! hotspots, subscription management, and seamless auto-connect. |
| **Central Management Platform** | Backend system for firmware updates, node health monitoring, billing management, and automated MoMo payouts to hosts. |
| **Payments Integration** | MTN Mobile Money and Airtel Money for both subscription collection and host payout disbursement. |

---

## 8. Go-to-Market Strategy

### Phase 1 — Neighbourhood Proof of Concept *(Months 1–3)*

> Validate the model. Manual everything. One neighbourhood.

- Recruit **3–5 willing hosts** within one neighbourhood
- Deploy MikroTik nodes; set up manual voucher-based access
- Collect payments via MoMo manually; pay host cuts manually
- ✅ **Success metric:** 15+ paying roamers within 60 days

### Phase 2 — Platform Build *(Months 4–9)*

> Build the product on proven demand.

- Develop Host Dashboard, Roamer App, and Central Auth Platform
- Automate MoMo billing and host payouts
- Implement captive portal authentication at hardware level
- Expand to **3 neighbourhoods** in Kampala
- ✅ **Success metric:** 10+ active host nodes, 200+ roamer subscribers

### Phase 3 — ISP Engagement & City Scale *(Months 10–18)*

> Formalise the model. Expand aggressively.

- Approach MTN, Airtel, and Liquid with traction data — propose **licensed reseller or partner model**
- Introduce tiered roamer plans (hourly, daily, monthly, corporate)
- Add host quality ratings and service level indicators
- Expand to bodaboda stages, markets, clinics, and schools
- ✅ **Success metric:** 100+ host nodes, 2,000+ active subscribers

### Phase 4 — Regional Expansion *(18+ Months)*

> Export the model.

- Replicate in Entebbe, Jinja, Mbarara, Gulu
- Launch corporate account product for city-wide employee roaming
- **License the Supa.NET! platform** to operators in Nairobi, Dar es Salaam, and Kigali
- Explore partnerships with national broadband expansion programmes

---

## 9. Challenges & Mitigations

| Challenge | Risk Level | Mitigation |
|---|:---:|---|
| **ISP Terms of Service** — most unlimited packages prohibit commercial reselling | 🔴 High | Early ISP engagement; structure as a partnership, not a resale; pursue formal licensed agreements |
| **Host trust & privacy** — hosts fear strangers accessing their home network | 🔴 High | Mandatory VLAN isolation at hardware level; market this as the core safety feature |
| **Network quality variance** — different hosts offer very different speeds | 🟡 Medium | Host quality ratings; bandwidth guarantees enforced by platform; tiered pricing by quality |
| **Chicken-and-egg problem** — need hosts before roamers; need roamers before hosts see value | 🟡 Medium | Hyper-local launch — seed each neighbourhood densely before moving to the next |
| **Technical complexity for hosts** — non-technical users need to install equipment | 🟡 Medium | Supa.NET! owns, installs, and remotely manages all hardware; host involvement is near-zero |
| **Regulatory uncertainty** — telecoms regulation in Uganda may evolve | 🟢 Low–Med | Proactive engagement with Uganda Communications Commission (UCC) from early stage |
| **Payment reliability** — MoMo transactions can fail or delay | 🟢 Low | Multi-provider MoMo integration; automatic retry logic; clear payout schedules |

---

## 10. Competitive Landscape

No operator in Uganda currently offers a **community-owned, income-generating WiFi sharing network** with automatic authentication, MoMo payments, and network isolation. This is Supa.NET!'s white space.

| Operator | Model | Geography | Why Supa.NET! Is Different |
|---|---|---|---|
| **Fon** | Home router sharing cooperative | Europe, global | ISP-partnered from inception; Supa.NET! is community-first with ISP partnership as a later stage |
| **Karma WiFi** | Pay-per-use shared hotspot network | United States | US market; no MoMo-native payments; not built for African urban density |
| **MTN WiFi Zones** | ISP-operated public hotspots | Uganda | Fixed locations only; not community-distributed; no income for participants |
| **Airtel Public WiFi** | ISP-operated hotspots | Uganda | Same limitation — centrally owned, not community-distributed or income-generating |

---

## 11. Technology Stack

### Why MikroTik for Host Hardware

Consumer-grade routers provided by ISPs are designed for simplicity, not programmability. They cannot:

- Run a captive portal
- Enforce VLAN isolation programmatically
- Be remotely managed via API
- Throttle bandwidth per user class

**MikroTik RouterOS** provides all of these natively, at a cost of approximately **UGX 150,000–300,000** per unit — well within the unit economics of the model.

| Capability Required | MikroTik Support |
|---|:---:|
| Captive portal / subscriber authentication | ✅ Native (HotSpot Manager built-in) |
| VLAN isolation (home vs. roamer network) | ✅ Hardware-enforced |
| Remote API management | ✅ Full REST and Winbox API |
| Per-user bandwidth throttling | ✅ Queue Trees — granular control |
| Multiple SSID broadcast | ✅ Full support |
| Deployment behind existing ISP router | ✅ No ISP equipment changes required |

MikroTik devices are widely used across Uganda and East Africa, with a strong local technician ecosystem and parts availability on **Kampala's Nasser Road**.

---

## 12. Resource Requirements

> *Phase 1 & 2 seed estimates — conceptual range pending Phase 1 validation*

| Resource | Estimated Cost (UGX) |
|---|---|
| MikroTik nodes — Phase 1 pilot (10 hosts) | 2,000,000 – 3,000,000 |
| Software development (Platform, Apps, Auth) | 15,000,000 – 40,000,000 |
| MoMo integration & payment setup | 1,000,000 – 2,000,000 |
| Operations & field installation (Phase 1) | 1,000,000 – 2,000,000 |
| Legal & regulatory consultation (UCC) | 2,000,000 – 5,000,000 |
| Marketing & host acquisition (Phase 1) | 1,000,000 – 3,000,000 |
| **Total estimated Phase 1–2 seed requirement** | **22,000,000 – 55,000,000** |

---

## 13. The Bigger Vision

Supa.NET! is designed from the outset to be **replicable**. Every neighbourhood in every Ugandan city has the same structural conditions: overlapping WiFi signals, underutilised unlimited subscriptions, and a community of people paying more collectively than they need to.

The Kampala proof of concept is not the product — it is the **template**.

```
Kampala Neighbourhood Pilot
         ↓
Other Kampala Neighbourhoods (Ntinda, Bukoto, Kansanga, Naalya)
         ↓
Secondary Ugandan Cities (Jinja, Mbarara, Gulu, Masaka, Mbale)
         ↓
East African Markets (Nairobi, Dar es Salaam, Kigali, Lusaka)
         ↓
Platform Licensing — Supa.NET! as an OS for community WiFi operators globally
```

> **The Long-Term Opportunity:** If even 1% of households in Kampala become Supa.NET! hosts, and each host serves 10 roamers, Supa.NET! becomes the largest distributed WiFi network in Uganda — built not by a telecom company, but by **the community itself**.

---

## 14. Next Steps

The single most important thing Supa.NET! can do right now is **validate the economics in the real world** before building anything complex.

- [ ] Identify **5 founding host households** in one Kampala neighbourhood
- [ ] Install MikroTik nodes and configure manual voucher-based access
- [ ] Onboard first paying roamers via word of mouth
- [ ] Run manual MoMo billing and host payouts for 60 days
- [ ] Document what works, what breaks, and what people actually pay
- [ ] Build the platform on proven demand

---

<div align="center">

---

*Supa.NET! — Kampala, Uganda — 2025*

*This is a community utility, built by the community, for the community.*

---

</div>

