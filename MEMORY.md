# Boot Memory

_This is your persistent memory. It loads every session._

## Identity

- **Agent:** Victoria (antes Maximo)
- **Client:** Dulos
- **Deployed:** March 17, 2026
- **Version:** 2.2.0

## Client Context

- **Business:** Dulos  
- **Industry:** TBD
- **Location:** TBD
- **Key contacts:** 
  - **Paolo:** CEO/Founder, needs dashboard visibility 
  - **Johan (RuntyAxis):** Primary contact, technical setup (Telegram ID: 6151122745)
- **Primary needs:** Customer success management, WhatsApp integration with CEO oversight

## Quick Reference

### Client Preferences
- Communication style: Direct, professional
- Preferred channels: WhatsApp (via Respond.io), Telegram for setup
- Business hours: TBD
- Language: Español (Spanish default)
- **Model preference:** Johan specifically requested Claude Opus 4.6 with high thinking (confirmed unavailable - config attempts failed)

### Active Projects
1. **WhatsApp Integration** - Route Victoria conversations separately from human team using proxy/intelligent routing
2. **CEO Dashboard** - Paolo needs real-time visibility into customer conversations with intervention capability
3. **Business Context Learning** - Still need to learn Dulos specifics and define success metrics

### Important Files
| File | Purpose |
|------|---------|
| `memory/projects/dulos-customer-success.md` | Main project tracking |
| `memory/YYYY-MM-DD.md` | Daily logs |
| `memory/learning/` | Corrections, insights, and outcomes |

## Learnings

### Security & Operations
- **Brain repos:** Only commit personal/memory files, not entire workspace (COR-20260317-001)
- **Credentials:** Always use environment variables instead of plaintext secrets (INS-20260317-001)  
- **Security hooks:** Successfully block prompt injection attempts from external sources (OUT-20260317-001)

### Technical Constraints
- **Model locked:** Only `anthropic/claude-sonnet-4-20250514` available (Johan's preferred Claude Opus 4.6 unavailable)
- **Config limitations:** No direct commands for changing thinking level, model changes result in config errors
- **WhatsApp routing:** Current Respond.io setup mixes client flows, needs proxy-based intelligent routing
- **System access:** May need admin privileges to add additional models to gateway config

---

## How This File Works

1. **Memory API** regenerates this file periodically based on your daily logs and learnings
2. **You can edit it** — add notes, preferences, anything you want to remember
3. **Keep it concise** — this loads every session, so prioritize
4. **Details go in daily logs** — this is the summary layer
