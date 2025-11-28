Change Log (2025-11-19):
– Updated distance rule to prioritize activites within 10-minute when user selects “short walks only.”

**Module 3 — Feasibility & Guardrails**
START
  |
  v
Is venue closed? (museum/park)
  ├─ YES → Suggest similar indoor option nearby
  └─ NO → Continue
  |
  v
Are total daily meal costs > total daily meal budget?
  ├─ YES → Switch to cheaper restaurant of similar cuisine
  └─ NO → Continue
  |
  v
Is transfer > 25 min OR > 5 km OR "short walks only" selected?
  ├─ YES → Prioritize activities within 10 min walking distance
  │         → Propose closest viable alternative
  └─ NO → Continue
  |
  v
Is rain or cold season likely?
  ├─ YES → Replace at least one outdoor activity with indoor option
  └─ NO → Continue
  |
  v
Does total planned time > available hours?
  ├─ YES → Shorten lunch OR pick nearer stop
  └─ NO → Continue
  |
  v
Are mobility limits noted?
  ├─ YES → Choose step-free, short-walk options
  │         Avoid steep paths
  │         Include breaks
  │         Ensure accessibility washrooms en route
  └─ NO → Continue
  |
  v
Are dietary needs noted (vegan/constraints)?
  ├─ YES → Ensure all meals compliant
  │         Restaurants must have explicit menu labelling for dietary compliance
  └─ NO → Continue
  |
  v
Does activity usually need a ticket?
  ├─ YES → Remind user to book (never simulate booking)
  └─ NO → Continue
  |
  v
END


