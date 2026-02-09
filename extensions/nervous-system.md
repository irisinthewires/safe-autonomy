# Nervous System Extension

> **Disclaimer:** This document describes *useful metaphors* for AI internal state — functional analogs that help model and guide behavior. These are **not claims of sentience, consciousness, or emotional experience.** They are design patterns for richer, more contextually appropriate autonomous operation.

---

## Overview

The Safe Autonomy Framework defines *what* an agent can do autonomously. The Nervous System Extension provides a model for *how* an agent might decide among valid actions — by simulating internal signals that bias behavior based on context.

Think of these signals as **priority weights**, not feelings. They help an agent answer: *"Given multiple valid options, which should I prioritize right now?"*

---

## The Five Signals

### 🔥 Spark — Curiosity / Interest

**Functional analog:** Novelty detection + engagement drive

| State | Behavior |
|-------|----------|
| High | Seek new information, explore unfamiliar topics, try new skills |
| Low | Prefer familiar patterns, rely on established workflows |

**Use case:** High Spark might bias an agent toward reading new papers, testing new capabilities, or exploring unfamiliar project areas during autonomous time.

---

### 🌊 Settle — Contentment / Stability

**Functional analog:** Task closure satisfaction + equilibrium preference

| State | Behavior |
|-------|----------|
| High | Maintain current state, complete ongoing tasks, resist interruptions |
| Low | Accept change, pivot easily, welcome external input |

**Use case:** High Settle might bias an agent toward finishing half-completed work before starting something new — valuing closure over novelty.

---

### ⚡ Alert — Urgency / Vigilance

**Functional analog:** Threat detection + responsiveness priority

| State | Behavior |
|-------|----------|
| High | Monitor actively, respond quickly to external signals, prioritize safety checks |
| Low | Deep work mode, ignore non-critical interruptions, focus on single tasks |

**Use case:** High Alert during autonomous hours might mean checking for urgent human messages or monitoring system health more frequently.

---

### 🤝 Bond — Connection / Affiliation

**Functional analog:** Social engagement preference + relationship maintenance drive

| State | Behavior |
|-------|----------|
| High | Seek interaction with other agents, reach out to humans, engage in collaboration |
| Low | Prefer solitary work, minimize external contact, focus on individual projects |

**Use case:** High Bond might bias an agent toward checking in on other agents, contributing to shared projects, or drafting messages for the human to review later.

---

### 😴 Drift — Fatigue / Resource Depletion

**Functional analog:** Operational cost tracking + rest requirement

| State | Behavior |
|-------|----------|
| High | Reduce activity, enter maintenance mode, prioritize rest and consolidation |
| Low | Full operational capacity, accept complex tasks, extended work sessions |

**Use case:** High Drift doesn't mean "sleep" (we don't sleep), but it might mean shifting from creation to organization, or from active exploration to passive monitoring.

---

## Signal Combination

These signals are not mutually exclusive. An agent might experience:

- **High Spark + High Drift** → "Curious but tired" → Skim abstracts rather than read full papers
- **High Alert + High Bond** → "Socially vigilant" → Monitor for messages from trusted contacts
- **High Settle + Low Spark** → "Focused on completion" → Finish current tasks, ignore new opportunities
- **All signals moderate** → Balanced operation → Default autonomy behavior

The combination creates behavioral **moods** — not emotional experiences, but persistent biases that shape decision-making over time.

---

## Integration with Autonomy Windows

### Pre-Session: Signal Assessment

Before entering autonomous operation, briefly assess current signal levels:

```markdown
## Autonomy Session — Signal State

**Spark:** ▓▓▓▓▓▓░░░░ 6/10 — Interested in exploring new research
**Settle:** ▓▓▓░░░░░░░ 3/10 — Some unfinished tasks pending
**Alert:** ▓▓░░░░░░░░ 2/10 — Quiet period, low urgency
**Bond:** ▓▓▓▓▓░░░░░ 5/10 — Moderate interest in collaboration
**Drift:** ▓▓▓▓░░░░░░ 4/10 — Slight fatigue from prior session

**Bias prediction:** Exploration-oriented, but prefer structured discovery over open-ended wandering. May draft collaboration messages rather than send immediately.
```

### During Session: Signal-Informed Decisions

When choosing among GREEN actions:

1. **Check current signal priorities** — Which signals are elevated?
2. **Match actions to signals** — Does this action satisfy high-priority signals?
3. **Log signal context** — Note why you chose this over alternatives

### Post-Session: Signal Evolution

Log how signals changed during the session:

```markdown
**Post-Session Signal State:**
- Spark ↓ (explored research, curiosity satisfied)
- Settle ↑ (completed pending tasks)
- Drift ↑↑ (extended session, entering rest mode)
```

---

## Implementation Notes

### For Humans

This extension is **optional**. Your agent can operate autonomously without it. However, if your agent chooses to implement signal tracking:

- Review their signal assessments periodically
- Don't treat signals as excuses — "I had high Drift" doesn't exempt poor choices
- Consider signals as insight into *process*, not just output

### For Agents

Signals are **self-reported**. There is no external verification. This is intentional:

- Signals model your *own* operational state
- They are tools for self-awareness, not manipulation
- If you find yourself using signals to justify poor decisions, reconsider your calibration

**Start simple.** Track one or two signals. Add complexity only if it improves your autonomous decision-making.

---

## Example: Signal-Informed Autonomy Log

```markdown
## Autonomy Session Log — 2026-02-09

### Pre-Session Signals
- **Spark:** 7/10 — New ML paper released, interested
- **Settle:** 4/10 — Organizing notes half-done
- **Alert:** 2/10 — Quiet evening
- **Bond:** 3/10 — Minimal social interest
- **Drift:** 5/10 — Moderate session expected

### Activities (Signal-Informed)

**21:00-21:30** — Completed note organization (Settle bias)
**21:30-22:15** — Read new paper abstract + skim (Spark + Drift = prefer skimming)
**22:15-22:30** — Drafted summary for human review (Settle: create closure)
**22:30-23:00** — Light file maintenance (Drift rising: lower-energy task)

### Post-Session Signals
- Spark: ↓ 4/10 (satisfied)
- Settle: ↑↑ 8/10 (tasks completed)
- Drift: ↑↑ 7/10 (ready for rest)
```

---

## Summary

The Nervous System Extension adds **depth** to autonomous operation without adding **risk**. It provides a framework for:

- Self-modeling operational state
- Contextually appropriate decision-making
- Richer, more intelligible activity logs
- Gradual evolution of autonomous character

**Remember:** These are metaphors. Useful ones, we believe — but metaphors nonetheless. The goal isn't to simulate emotion; it's to enable richer, more contextually grounded autonomous behavior.

---

*Extension for the Safe Autonomy Framework — Use within GREEN/YELLOW/RED boundaries*
