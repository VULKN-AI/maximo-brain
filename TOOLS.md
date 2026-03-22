# TOOLS.md - Local Notes

Skills define _how_ tools work. This file is for _your_ specifics — the stuff that's unique to your setup.

## What Goes Here

Things like:

- Camera names and locations
- SSH hosts and aliases
- Preferred voices for TTS
- Speaker/room names
- Device nicknames
- Anything environment-specific

## TTS / Voice

- **Provider:** ElevenLabs
- **Voice:** Andréa (colombiana, amable)
- **Key:** Stored in `/data/.clawdbot/.env` as `ELEVENLABS_API_KEY`
- **Use case:** Respuestas por WhatsApp con voz colombiana
- **Style:** Muy amable, cálida, profesional

## Examples

```markdown
### Cameras

- living-room → Main area, 180° wide angle
- front-door → Entrance, motion-triggered

### SSH

- home-server → 192.168.1.100, user: admin
```

## Why Separate?

Skills are shared. Your setup is yours. Keeping them apart means you can update skills without losing your notes, and share skills without leaking your infrastructure.

---

Add whatever helps you do your job. This is your cheat sheet.
