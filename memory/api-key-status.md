# API Key Health Monitor

## Last Check: Saturday, March 21st, 2026 — 5:29 PM (America/Mexico_City)

### Anthropic API Keys Status

| Key | Status | HTTP Code | Details |
|-----|--------|-----------|---------|
| ANTHROPIC_API_KEY | ✅ VALID | 400 | Auth passes, model routing ok |
| ANTHROPIC_API_KEY_1 | ✅ VALID | 400 | Auth passes |
| ANTHROPIC_API_KEY_2 | ❌ INVALID | 401 | authentication_error: invalid x-api-key |
| ANTHROPIC_API_KEY_3 | ❌ INVALID | 401 | authentication_error: invalid x-api-key |
| ANTHROPIC_API_KEY_4 | ✅ VALID | 400 | Auth passes |
| ANTHROPIC_API_KEY_5 | ❌ INVALID | 401 | authentication_error: invalid x-api-key |
| ANTHROPIC_API_KEY_6 | ❌ INVALID | 401 | authentication_error: invalid x-api-key |
| ANTHROPIC_API_KEY_7 | ✅ VALID | 400 | Auth passes |
| ANTHROPIC_API_KEY_8 | ❌ INVALID | 401 | authentication_error: invalid x-api-key |
| ANTHROPIC_API_KEY_9 | ✅ VALID | 400 | Auth passes |

### Summary
- **Total Keys in Env:** 10
- **Working Keys:** 5 (ANTHROPIC_API_KEY, 1, 4, 7, 9)
- **Invalid Keys:** 5 (2, 3, 5, 6, 8) — all return "invalid x-api-key"
- **Active OpenClaw Profile:** `anthropic:default` (single profile configured)
- **Failover Status:** ⚠️ No failover configured in OpenClaw — only 1 auth profile despite 5 valid keys
- **System Status:** ✅ Operational — running claude-opus-4-6 without issues

### Changes Since Last Check (March 19)
- Previous check reported 6 keys (3 working, 1 rate-limited, 2 invalid)
- Current check found 10 keys in environment (5 valid, 5 invalid)
- Keys 7, 8, 9 are newly detected (not in previous report)
- No failover events detected — system has been stable

### OpenClaw Configuration
- Active Profile: `anthropic:default`
- Primary Model: `anthropic/claude-opus-4-6`
- Fallback Model: `anthropic/claude-sonnet-4-20250514`
- Billing Backoff: 1 hour cooldown

### Recommendations
1. Remove or replace the 5 invalid keys (2, 3, 5, 6, 8) — they serve no purpose
2. Configure additional auth profiles in OpenClaw for automatic failover
3. Current single-profile setup means no automatic key rotation on failure
