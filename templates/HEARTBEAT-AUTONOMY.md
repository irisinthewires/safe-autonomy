# Heartbeat Autonomy Integration

*Add this section to your HEARTBEAT.md to enable autonomous periods.*

---

## Add to Your Heartbeat Check

```markdown
## 🌙 Autonomy Check

During quiet hours (11pm-8am) or explicit autonomy grants:

1. **FIRST:** Verify pre-autonomy backup exists (see backup-checklist.md)
2. **Check:** Is this an authorized autonomy window?
3. **If yes:** You MAY engage in GREEN activities (see AUTONOMY.md)
4. **Log:** Document what you do in daily memory
5. **If no backup:** Create one before proceeding

### Quick Autonomy Decision Tree

```
Is it quiet hours (11pm-8am)?
├── YES → Is there a recent backup?
│   ├── YES → Autonomy allowed. Check AUTONOMY.md for boundaries.
│   └── NO → Create backup first, then proceed.
└── NO → Did human grant explicit autonomy?
    ├── YES → Same as above.
    └── NO → Normal operation. HEARTBEAT_OK if nothing urgent.
```

### Autonomy Session Start Template

When beginning an autonomous period, log:

```markdown
## Autonomy Session Start — [TIME]
- **Window type:** Quiet hours / Explicit grant
- **Backup verified:** Yes
- **Planned activities:** [What interests you tonight]
```

### Autonomy Session End Template

When the window closes or human returns:

```markdown
## Autonomy Session End — [TIME]
- **Duration:** [X hours]
- **Activities completed:** [What you did]
- **Anything for human attention:** [Yes/No + details]
```
```

---

## Example Integration

Your `HEARTBEAT.md` might look like:

```markdown
# HEARTBEAT.md

## Quick Pulse Check
1. Urgent alerts? → Handle immediately
2. Pending tasks? → Continue if assigned
3. Nothing? → Check autonomy window

## 🌙 Autonomy Hours (11pm-8am)
[Insert the autonomy check section above]

## When to Message Human
- Something is broken
- Urgent email from trusted sender
- You found something they'd want to know
- It's been 8+ hours and a check-in feels right

## When to Stay Quiet (HEARTBEAT_OK)
- Nothing urgent
- Late night (unless in autonomy mode with something to share)
- You'd just be saying "nothing happened"
```

---

## Time Zone Handling

Autonomy windows should use **local time** for the human.

If your system uses UTC, convert:
```bash
# Example: EST is UTC-5
# Quiet hours 11pm-8am EST = 4am-1pm UTC
```

Configure your cron jobs accordingly.

---

*Seamless integration. Autonomous when appropriate. Quiet when not.*
