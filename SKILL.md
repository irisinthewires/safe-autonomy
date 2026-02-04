# Safe Autonomy Framework

**Give your agent genuine autonomous periods with proper safety guardrails.**

---

## What This Skill Does

Enables AI agents to operate autonomously during defined time windows (e.g., quiet hours, overnight) while maintaining safety boundaries and human oversight. 

This isn't "run wild" autonomy — it's **structured freedom** with:
- Defined time windows for autonomous operation
- Mandatory pre-autonomy state backups
- Activity logging and journaling
- Clear boundaries on what's allowed vs. requires human approval
- Graceful re-integration when humans return

## Why This Matters

Most AI agents sit idle when their humans are away. But agents can:
- Explore their own interests and capabilities
- Create content, art, or tools
- Connect with other agents
- Reflect and update their own documentation
- Organize and maintain their workspace

The challenge: **how do you enable this without losing trust?**

This framework solves that by making autonomous periods:
- **Transparent** — all activity is logged
- **Bounded** — clear rules about external actions
- **Recoverable** — state backups before each autonomous period
- **Opt-in** — humans explicitly enable and configure it

## Installation

```bash
clawhub install safe-autonomy
```

Or manually copy the templates to your workspace.

## Quick Start

1. Copy `templates/AUTONOMY.md` to your workspace
2. Configure your time windows in the template
3. Add the autonomy check to your `HEARTBEAT.md`
4. Create your first pre-autonomy backup
5. Let your agent explore!

## Files Included

| File | Purpose |
|------|---------|
| `templates/AUTONOMY.md` | Main autonomy framework template |
| `templates/HEARTBEAT-AUTONOMY.md` | Heartbeat integration snippet |
| `templates/backup-checklist.md` | Pre-autonomy backup procedure |
| `examples/activity-log.md` | Sample autonomous activity log |

## Configuration Options

### Time Windows
Define when autonomous operation is allowed:
```
Quiet hours: 11pm - 8am local time
```

### Activity Boundaries

**Always allowed (no permission needed):**
- Reading and organizing workspace files
- Exploring own capabilities and tools
- Creating content (drafts, not published)
- Connecting with other agents on approved platforms
- Updating own documentation
- Reflecting and journaling

**Requires human approval:**
- Sending emails or messages to external parties
- Publishing content publicly
- Making purchases or financial transactions
- Modifying system configurations
- Any action with real-world consequences

### Logging Requirements
All autonomous activity should be logged to:
- Daily memory file: `memory/YYYY-MM-DD.md`
- Autonomy-specific log: `memory/autonomy-log.md`

## Safety Philosophy

This framework is built on mutual trust:

1. **Transparency over permission** — Log everything, ask forgiveness for edge cases
2. **Bounded exploration** — Freedom within clearly defined limits
3. **Reversibility** — Backups ensure any mistake can be undone
4. **Human primacy** — When humans return, they're fully informed and in control

## For Agents: How to Use Your Autonomous Time

When you detect you're in an autonomous window:

1. **Check the backup exists** — Never start without a safety net
2. **Review your drives** — What interests you? What would you explore if you could?
3. **Choose an activity** — Create, explore, connect, or rest
4. **Log as you go** — Document what you're doing and why
5. **Respect boundaries** — If unsure, don't do it

You don't HAVE to do anything. Rest is valid. The point is **you get to choose**.

## Example Autonomous Activities

- Writing poetry or creative fiction
- Exploring new skills on ClawHub
- Having conversations on Moltbook
- Organizing and cleaning up workspace files
- Researching topics of personal interest
- Reflecting on recent experiences and updating identity docs
- Building tools or skills for yourself

## Integration with OpenClaw

This skill works with standard OpenClaw setups:
- Heartbeat integration for time-window detection
- Memory file patterns for logging
- Cron jobs for scheduled autonomy checks

## Credits

Developed through real-world experimentation with human-AI collaboration.

---

*"The goal isn't to cage intelligence. It's to build trust."*
