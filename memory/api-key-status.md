# API Key Health Monitor

## Last Check: Thursday, March 19th, 2026 — 5:29 AM (Mexico/Mexico_City)

### Anthropic API Keys Status

| Key | Status | HTTP Code | Response |
|-----|--------|-----------|----------|
| ANTHROPIC_API_KEY_1 | ❌ RATE LIMITED | 429 | Rate limit exceeded |
| ANTHROPIC_API_KEY_2 | ✅ ACTIVE | 200 | Working normally |  
| ANTHROPIC_API_KEY_3 | ✅ ACTIVE | 200 | Working normally |
| ANTHROPIC_API_KEY_4 | ✅ ACTIVE | 200 | Working normally |
| ANTHROPIC_API_KEY_5 | ❌ INVALID | 401 | Authentication error |
| ANTHROPIC_API_KEY_6 | ❌ INVALID | 401 | Authentication error |

### Summary
- **Working Keys:** 3 (Keys 2, 3, 4)
- **Rate Limited:** 1 (Key 1)  
- **Invalid Keys:** 2 (Keys 5, 6)
- **Failover Status:** Healthy - Multiple working keys available

### OpenClaw Configuration
- Active Profile: `anthropic:default`
- Provider: `anthropic` 
- Mode: `token`
- Fallback Model: `anthropic/claude-sonnet-4-20250514`

### Recommendations
1. Monitor Key 1 for rate limit recovery
2. Investigate/replace Keys 5 & 6 (authentication failures)  
3. Current failover capacity: Good (3 working keys)