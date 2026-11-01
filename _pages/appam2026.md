---
permalink: /appam2026/
title: "Pandemic Proximity"
author_profile: true
---

**Did COVID-19 Redraw the Geography of Korea's National R&D Collaboration?**

Haseon Jeong · Center for Data Analysis Innovation, Office of Innovation Strategy, Korea Institute of S&T Evaluation and Planning (KISTEP)
APPAM 2026 · Poster Session

Short answer
======
No clear jump in 2020, but distance trends for new partnerships **steepened afterward**, including
for **universities and SMEs** — a pandemic-era acceleration.

Why it matters
======
Proximity has long been treated as a precondition for R&D collaboration. If remote collaboration
became routine during the pandemic, the distance constraint on choosing partners may have
loosened — but for whom?

- **RQ1** Did partners chosen after 2020 sit farther away?
- **RQ2** Which institutions and research stages drove the change?
- **RQ3** What structurally shapes collaboration distance?

Data
======
Korea's national R&D project micro-data (NTIS), 2015–2024: lead institution ↔ domestic partner,
**route (road) distance** in km.

| 131,813 | 65,602 | 292,966 | 10 yrs |
|:---:|:---:|:---:|:---:|
| new-tie records (main unit) | projects | all tie-year records | 2015–2024 |

**Why new ties?** Of 77,200 multi-year ties, only 5.7% ever change distance. A tie's distance is
fixed when the partner is chosen, so we focus on partner selection. A new tie is a project × partner
pair in its first year (history from 2012).

Design
======
ln(1+km)<sub>ijt</sub> = β<sub>1</sub>Year<sub>t</sub> + β<sub>2</sub>Post<sub>t</sub> + β<sub>3</sub>(Year<sub>t</sub>−2020)·Post<sub>t</sub> + X<sub>ijt</sub>γ + μ<sub>region</sub> + ε

- Interrupted time series: β<sub>2</sub> = 2020 departure from pre-trend, β<sub>3</sub> = slope change
- Event study, ref. 2019; SEs clustered by project
- X: institution type, research stage, ln(budget), private funding share; region FE

Findings
======

### 1. No clear 2020 jump — the trend steepened afterward

![Mean route distance of newly formed vs. continuing ties, 2015–2024]({{ site.baseurl }}/images/appam2026/fig1_distance.png)
*Mean route distance of newly formed vs. continuing ties, 2015–2024.*

![Event study, new ties, with controls]({{ site.baseurl }}/images/appam2026/fig2_event_study.png)
*Event study, new ties, with controls (ref. 2019, 95% CI).*

- 2020 vs. pre-trend: +0.006 (n.s.)
- Yearly slope, ln(1 + km): −0.018 → +0.055 (Δ +0.073\*\*\*)
- 2024 vs. 2019: ≈ +19% (event study)

**Not a causal estimate:** pre-2020 years differ from 2019 (joint F = 15.9, p < .001).
Inter-regional share of new ties rose 69% → 75% in 2020, but not after controls (−2 pp) —
consistent with a shift in which projects started.

### 2. Trend slopes shifted upward for universities and SMEs and downward for GRIs; the change for large firms was inconclusive

![Change in yearly slope after 2020 by institution type and research stage]({{ site.baseurl }}/images/appam2026/fig3_slope_change.png)
*Change in yearly slope after 2020 (not level), new ties; pooled model with group interactions.
Blue/orange: p < .05; gray: n.s.; † p < .1.*

| Mean km, new ties | 2015–19 | 2020–24 |
|---|---:|---:|
| SME | 104.7 | 123.8 |
| University | 121.5 | 152.9 |
| Gov't research inst. | 173.6 | 153.8 |
| Large firm | 165.6 | 166.0 |

Mean distances of short- and long-reach institutions converged. Mean distance rose at every
stage; the slope increase was largest for applied research (vs. basic p = .013, vs. development
p = .017).

### 3. Gaps persist across institutions and stages

![Level differences in route distance by institution type and research stage]({{ site.baseurl }}/images/appam2026/fig4_levels.png)
*Level differences (not changes): OLS on new ties with year FE, N = 130,890 (923 missing budget
or region), R² = 0.09.*

SMEs remain the most local (≈ 33% shorter than large firms, conditional on controls), and distance
falls from basic to development research. Bigger budgets go with farther partners; private
co-funding with closer ones.

Robustness — post-2020 slope change
======

| Specification | β<sub>3</sub> / yr |
|---|---:|
| New ties, controls (main) | +0.073\*\*\* |
| New ties, no controls | +0.029\*\*\* |
| Official new-project flag (excl. 2020) | +0.069\*\*\* |
| Excluding 2024 | +0.073\*\*\* |
| Quadratic time trend | +0.065\* |
| Break year 2021 (instead of 2020) | +0.071\*\*\* |

Also positive: all tie-year records +0.052\*\*\*; inter-regional tie share (LPM) +0.022\*\*\*.

**Limitations.** Pre-trends are not flat (F = 15.9), so we report a pandemic-era acceleration — a
change observed in that period, not a causal effect. Placebo breaks within 2015–19 (2017, 2018;
new ties) are also statistically significant, limiting the interpretation of the estimated trend
change as specific to the pandemic period. 2022–24 overlaps other R&D policy changes (e.g., the
2024 budget restructuring).

Takeaways
======
1. **Distance gaps across institution types narrowed:** after 2020, distances to new partners rose
   for SMEs and universities, the institutions with the shortest reach before 2020. Whether this
   widened access is the next question.
2. **Gaps persist:** SMEs and development-stage projects remain the most local.
3. **Policy options to evaluate:** matching intermediaries for SMEs, minimum-scale consortia,
   stage-differentiated incentives for development projects.

Materials
======
- Data: NTIS National R&D project micro-data, 2015–2024
- [Handout (1 page, PDF)]({{ site.baseurl }}/files/APPAM2026_handout_Jeong.pdf)
- [Poster (PDF, 90×44 in)]({{ site.baseurl }}/files/APPAM2026_poster_Jeong.pdf)
- Contact: [summerj@kistep.re.kr](mailto:summerj@kistep.re.kr)
