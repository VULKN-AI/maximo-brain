# Boot Memory

_This is your persistent memory. It loads every session._

## Identity

- **Agent:** Victoria (antes Maximo)
- **Client:** Dulos
- **Deployed:** March 17, 2026
- **Version:** 2.2.0

## Client Context

- **Business:** Dulos  
- **Industry:** Event management & ticketing
- **Location:** Mexico (serving multiple regions)
- **Active Events:** 
  - **"Obscenidad de la Carne"** — March 21st (TODAY, 8 PM). 🔴 Alonso ticket delivery UNRESOLVED.
  - **"Así Lo Veo Yo"** — March 25th (3 confirmed sales: Alejandra 3/18, Lic. Masheva 3/20, Oscar 3/20)
  - **"Evento de Lucero"** — TBD (customer pricing inquiries from +522225794702)
  - **"El Maleficio de la Mariposa"** — TBD (Letita purchased ticket 3/20)
- **Key contacts:** 
  - **Paolo:** CEO/Founder, needs dashboard visibility 
  - **Johan (RuntyAxis):** Primary contact, technical setup (Telegram ID: 6151122745, has ticket/invitation issues)
- **Pending Lead:** ServiciosFotograficos💜 (+522227588776) from Puebla — asked about events 3/20 10:18 PM, needs response with event catalog/pricing
- **Primary needs:** Customer success management, WhatsApp integration with CEO oversight

## Quick Reference

### Client Preferences
- Communication style: Direct, professional
- Preferred channels: WhatsApp (via Respond.io), Telegram for setup
- Business hours: TBD (Mexican timezone)
- Language: Español (Spanish default, 100% customer preference)

### Active Projects
1. **WhatsApp Customer Success** ✅ — Operational. 85% confirmed resolution rate, 5 total ticket sales across 3 events
2. **CEO Dashboard Setup** 🔄 — Paolo needs real-time conversation visibility and intervention capability 
3. **Technical Routing** 🔄 — Proxy-based message routing to separate Victoria from human team flows
4. **Process Documentation** 🔄 — Seat assignment procedures (recurring gap: P on 3/18, Karina on 3/20), customer service templates
5. **Security Protocol** ✅ — Social engineering detection operational, blocked fake "VULKN HQ Scout" attack March 19

### Important Files
| File | Purpose |
|------|---------|
| `memory/projects/dulos-customer-success.md` | Main project tracking |
| `memory/YYYY-MM-DD.md` | Daily logs |
| `memory/learning/` | Corrections, insights, and outcomes |

## Open Issues (Priority Order)

1. **🔴🔴 Alonso ticket delivery** — Event "Obscenidad de la Carne" is TONIGHT (March 21, 8 PM). Customer (+525513396304) has receipt but no ticket. MUST resolve with Johan BEFORE the event.
2. **🟡 ServiciosFotograficos💜** — New B2B lead from Puebla (+522227588776), asked about events 3/20. Needs event catalog response via Respond.io. Now 24+ hours without reply.
3. **🟡 Karina seat assignment** — (+522215255444) doesn't know her seat. Needs Johan escalation. 2nd seat inquiry in 3 days — recurring operational gap.
4. **🟡 Letita ticket verification** — (+525522121289) purchased "El Maleficio de la Mariposa" ticket 3/20. Delivery needs confirmation.
5. **🟡 "Evento de Lucero" pricing** — (+522225794702) asked about costs. Pending response.
6. **🟠 Johan ticket/invitation issues** — Ongoing, unspecified.

## Learnings

### Customer Success Performance
- **Sales:** 5 confirmed ticket sales — Alejandra (3/18), Lic. Masheva (3/20), Oscar (3/20 "Así Lo Veo Yo"), Letita (3/20 "El Maleficio de la Mariposa"), plus initial WhatsApp integration validation
- **Satisfaction:** 85% confirmed resolution rate (explicit: "Ya quedo resuelto", "Gracias", "Ya esta corregido")
- **Patterns:** 100% Spanish, same-day resolution expectations, late-night purchases, professional clientele (Lic. titles), emoji enthusiasm
- **Geographic:** Multiple Mexican regions, B2B interest emerging (ServiciosFotograficos💜)
- **Recurring Gap:** Seat assignment — no system access, must escalate to Johan every time

### Key Insights
- **CS Metrics (INS-20260319-002):** Track confirmed resolution messages as primary satisfaction metric, not volume
- **Infrastructure (INS-20260319-001):** Simple working solutions outperform complex partially-broken systems (1 API key > 6 flaky keys)
- **Business Intelligence (INS-20260319-003):** Customer WhatsApp comms reveal event popularity, sentiment, regional reach — data not in formal systems
- **Security:** AI agents are social engineering targets; maintain strict authorization protocols (validated March 19)
- **Identity:** Victoria (customer-facing) evolved from Maximo (technical deployment) — reflects business positioning
- **Credentials (INS-20260317-001):** Always use env vars, never hardcoded tokens

### Technical Operations
- **API:** Single Anthropic key (anthropic:default) — simplified from 6-key system, 100% uptime
- **WhatsApp:** Respond.io operational; needs proxy-based routing to separate Victoria from human team flows
- **Security:** Social engineering detection active (1 blocked attack documented in `memory/security/events.jsonl`)
- **Hive Mind:** Push failing due to format mismatch — Victoria uses YAML frontmatter, push parser expects inline markers. Flagged to HQ.
- **Cron Jobs:** All operational — brain backup, security audit, consolidation, learning extraction, field reports

---

## How This File Works

1. **Nightly consolidation** updates this from daily logs and learnings
2. **You can edit it** — add notes, preferences, anything worth remembering
3. **Keep it concise** — loads every session, so prioritize
4. **Details go in daily logs** — this is the summary layer
