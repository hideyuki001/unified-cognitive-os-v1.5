# Unified Cognitive OS v1.5 — Operational Enforcement Layer

**v1.5 is the operational enforcement layer for v1.4 conservation laws.**  
It implements a strict execution pipeline:

**Red Flag Detection → Stopline Enforcement → (Repair OR Stop)**

## What v1.5 Is
- Operational enforcement layer for v1.4 conservation laws
- Red Flag → Stopline → Repair execution pipeline
- JRO integration with **STRICT non-expansion constraints**
- Minimal, auditable judgment repairs

## What v1.5 Is NOT
- Not a judgment optimization system
- Not an ambiguity resolution engine
- Not a certainty improvement mechanism
- Not a flexible repair framework

## Non-Negotiables (Design Boundaries)
- Detect Red Flags without suppression
- Enforce Stoplines without bypass
- Apply **ONE** operator per segment
- Audit repairs for integrity violations
- STOP when repair fails audit

Forbidden:
- Stacking multiple JRO operators
- Applying repair before Stopline check
- Overriding audit failures
- Expanding certainty/scope during repair

## Relationship to v1.4
- v1.4 defines **WHAT is forbidden** (conservation laws / manifold constraints).
- v1.5 defines **HOW violations are handled** (detect → stop → repair).

If you only need policy (constraints), v1.4 is enough.  
If you need operational handling and auditable repairs, use v1.5.

## Command Interface (Conceptual)
```bash
# Full pipeline with repair enabled
/unified-execute-v1.5 <context> --full-pipeline --model=flux --repair-enabled

# Repair-only analysis (requires Red Flag + Stopline reports)
/jro-analyze <red_flag_report> <stopline_verdict> --classify-operators

# Post-repair audit
/repair-audit <repair_report> <original_evaluation> --strict-mode

# Red flag detection (v1.2)
/red-flag-detect-v1.2 <evaluation_report> --include-manifold

# Stopline check (v1.1)
/stopline-check-v1.1 <red_flag_report> <manifold_report> --priority=manifold
Status
Complete specification: Repair-ready

Next milestone: v1.6 (graduated rubrics + repair telemetry)

## License
MIT (recommended)

## Author
Hideyuki Okabe
