# Head & Neck Re-Irradiation Plan Recommendation

Evidence-based re-irradiation plan selection for recurrent head and neck cancer — SBRT + immunotherapy regimens, Quad-Shot, and cumulative BED calculation.

## What This Skill Does

Given a brief patient history (primary site, prior RT details, recurrent disease extent, available drugs), this skill:

1. **Calculates cumulative BED** from the prior RT course with gap repair correction
2. **Screens 4 re-irradiation options**: Quad-Shot + IO, Q3w low-dose + IO, conventional 2 Gy/fx, SBRT continuous
3. **Generates a comparative table** with tumor EQD2, late tissue safety, and immune effect for each option
4. **Recommends the optimal regimen** with rationale, risk warnings, and execution parameters

## Evidence Base

| Regimen | Evidence | PMID |
|---------|----------|------|
| **Quad-Shot** (3.7 Gy × 4 BID Q4w) + Pembrolizumab | JAMA Otolaryngol 2026 | 42313403 |
| **Q3w single fraction** (3.5 Gy × 1 Q3w) + IO/ADC | Shanghai Ninth People's Hospital | — |
| **Conventional** (2 Gy/fx) | Standard re-RT | — |
| **SBRT** (5-6 Gy × 5) + IO | Multiple phase I/II | 37105404, 38892731 |

## Key Clinical Logic

```
Prior RT → residual EQD2 (gap repair)
  + Candidate regimen EQD2
  = Cumulative late EQD2

  ≤40 Gy → any option
  40-50 → Quad-Shot acceptable, SBRT limited
  50-60 → only Q3w or conventional
  >60 → conventional only (≤15 fx)
```

## Immunogenic Cell Death Threshold

- <4 Gy/fx → ICD signal may be sub-threshold
- 4-6 Gy/fx → weak-moderate ICD
- **6-12 Gy/fx → optimal ICD window**
- >12 Gy/fx → may kill infiltrating T cells

## Quick Install

```bash
hermes skills install https://raw.githubusercontent.com/antica1/head-neck-reirradiation/master/SKILL.md
```

## Trigger Keywords

`reirradiation` `recurrent head neck` `SBRT second course` `Quad-Shot` `immunotherapy radiosensitization` `ADC SBRT` `再程放疗`

## Author

Zhu Guopei, MD — Shanghai Ninth People's Hospital. Contact: antica@gmail.com

## License

MIT
