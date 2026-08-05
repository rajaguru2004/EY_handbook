# Topic 9 — Data Interpretation

### EY Placement Aptitude Handbook · Priority Rank #1 · 🔴 CRITICAL

> **Questions in this file are original, modelled on publicly reported EY test patterns. They are not claimed to be actual previous-year EY questions.**

---

## Contents

1. [Why This Topic Matters for EY](#1-why-this-topic-matters-for-ey)
2. [Core Concepts](#2-core-concepts)
3. [Formula Bank](#3-formula-bank)
4. [Shortcuts & Tricks](#4-shortcuts--tricks)
5. [Solved Examples](#5-solved-examples)
6. [Practice Questions (50, in 10 sets)](#6-practice-questions)
7. [Detailed Solutions](#7-detailed-solutions)
8. [Quick Revision Sheet](#8-quick-revision-sheet)
9. [Common Mistakes](#9-common-mistakes)

---

## 1. Why This Topic Matters for EY

**This is the single most important topic in the entire handbook.**

**Weightage:** 20–25% of the quantitative section under Patterns A and B — and in **Pattern C it is effectively 100% of the numerical section**. The "Numerical Reasoning" block in vendor-hosted EY assessments consists almost entirely of chart-and-table questions with very little standalone arithmetic.

**Why EY leans on DI so heavily:** the firm's actual work is reading financial statements, audit exhibits, client dashboards and management reports. A DI question is the closest an aptitude test gets to simulating the job. Expect the data to be dressed in business language — revenue, headcount, market share, cost centres, rejection rates.

**Question styles reported:**

| Exhibit type | Frequency | What it tests |
|---|---|---|
| **Tables** | Very high | Reading, summation, ratios, ranking |
| **Bar charts** (simple, grouped, stacked) | Very high | Comparison, percentage change |
| **Pie charts** | High | Share-to-absolute conversion, central angles |
| **Line graphs** | High | Trends, growth rates, peaks and troughs |
| **Caselets** (paragraph, no chart) | Medium | Set logic, Venn reasoning |
| **Two-exhibit cross-reference** | Medium | Combining a count table with a rate table |
| **Growth-rate tables** (% change given) | Medium | Chained multipliers |

**Prerequisites:** [Percentages](01-percentages.md), [Ratio & Proportion](03-ratio-proportion-partnership.md), [Averages](04-averages-mixtures-alligation.md). DI is not a new skill — it is those three skills applied under time pressure to messy data.

---

## 2. Core Concepts

### 2.1 What DI actually tests

DI questions almost never require difficult mathematics. They test three things:

1. **Reading accuracy** — did you take the right number from the right cell?
2. **Speed of approximation** — can you get within 2% fast enough?
3. **Resistance to traps** — units, bases, "which is greater" reversals.

**The overwhelming majority of DI errors are reading errors, not arithmetic errors.** Budget your attention accordingly.

### 2.2 The 20-second exhibit scan (do this before reading any question)

```
□  What is the UNIT?          ₹ crore? lakh? thousands? tonnes? percent?
□  What is the TIME RANGE?    which years/months are covered?
□  What are the CATEGORIES?   how many rows/columns/sectors?
□  Is anything a PERCENTAGE   (share of total) rather than an absolute?
□  Are there TWO exhibits?    if so, what links them?
□  Any FOOTNOTES?             "*excluding tax", "provisional", "estimated"
```

This scan costs 20 seconds and prevents the single most expensive mistake in DI — answering a whole 5-question set with the wrong scale.

### 2.3 The five question archetypes

Nearly every DI question is one of these:

| # | Archetype | Method |
|---|---|---|
| **1** | **Direct read / total** | Locate the values, add |
| **2** | **Percentage of total** | Part ÷ Whole × 100 |
| **3** | **Percentage change** | (New − Old) ÷ **Old** × 100 |
| **4** | **Ratio between two entries** | Divide, simplify |
| **5** | **Comparison / ranking** | Compare *rates*, not absolutes |

Archetype 5 is where most marks are lost — see §2.7.

### 2.4 Reading each exhibit type

**Tables** — the most information-dense exhibit. Check whether the last row/column is a **total** (often it is, and it saves you an addition).

**Bar charts** — read values off the axis. If bars are **stacked**, the segment value is the *difference* between gridline positions, not the top position.

**Pie charts** — sectors are always **shares of a whole**. To get an absolute value you *must* know the total.

$$\text{Absolute value} = \frac{\text{Sector \%}}{100} \times \text{Total}$$

$$\text{Central angle} = \frac{\text{Sector \%}}{100} \times 360° \qquad\text{equivalently}\qquad 1\% = 3.6°$$

**Line graphs** — the *slope* carries the information. A steep rise means high growth; a flat segment means no change. For "largest increase" questions, compare **vertical jumps**; for "largest percentage increase", compare **jump ÷ starting value**.

**Caselets** — no chart at all, just a paragraph. Extract the numbers into your own table before answering anything. Most caselets are set-theory problems in disguise (see §2.8).

### 2.5 Percentage change — the base rule

$$\text{\% change} = \frac{\text{New} - \text{Old}}{\text{Old}} \times 100$$

**The denominator is always the earlier / original value.** In a DI set spanning five years, this means the base changes for every year-on-year computation.

> Revenue 200 → 250: increase = 50/**200** = 25%
> Revenue 250 → 200: decrease = 50/**250** = 20%

### 2.6 Growth-rate chains

When a table gives **percentage growth over the previous year** rather than absolute values, convert each to a multiplier and chain them.

| Year | Growth | Multiplier |
|---|---|---|
| 2021 | +20% | × 1.20 |
| 2022 | +25% | × 1.25 |
| 2023 | −10% | × 0.90 |
| 2024 | +20% | × 1.20 |

Starting from ₹500 crore in 2020:
$$500 \to 600 \to 750 \to 675 \to 810$$

**Never add the growth percentages.** 20 + 25 − 10 + 20 = 55% would suggest ₹775 crore; the true figure is ₹810 crore (a 62% total rise).

### 2.7 ⭐ Rate vs absolute — the classic DI trap

> *"Which machine has the lowest rejection rate?"*

A machine that rejected 45 items may have a **lower** rate than one that rejected 80, if it produced far fewer items.

$$\text{Rate} = \frac{\text{Rejects}}{\text{Produced}} \times 100$$

| Machine | Produced | Rejected | Rate |
|---|---|---|---|
| M1 | 2,000 | 80 | 4.0% |
| M3 | 1,500 | **45** | **3.0%** ← lowest rate |
| M4 | 4,000 | 200 | 5.0% |

M3 has the fewest rejects *and* the lowest rate here — but that alignment is coincidental. **Always compute the rate.** The question wording ("rate", "proportion", "per cent of", "efficiency") is your signal.

### 2.8 Caselets and set logic

Caselet DI frequently reduces to two-set or three-set Venn logic.

**Two sets:**
$$n(A \cup B) = n(A) + n(B) - n(A \cap B)$$
$$\text{Only A} = n(A) - n(A \cap B)$$
$$\text{Neither} = \text{Total} - n(A \cup B)$$

> 500 people; 280 like tea, 220 like coffee, 100 like both.
> At least one = 280 + 220 − 100 = **400**
> Only tea = 180 · Only coffee = 120 · Both = 100 · **Neither = 100**

**Three sets:**
$$n(A \cup B \cup C) = \sum n(A) - \sum n(A\cap B) + n(A\cap B\cap C)$$

### 2.9 Approximation discipline

DI options are usually spaced 5–15% apart. Exact arithmetic is almost never needed.

**Round to two significant figures, compute, then check the options.**

> "1,847 is what percent of 8,932?"
> ≈ 1,850/8,900 ≈ 1,800/9,000 = **20%**
> (Exact: 20.68% — close enough to distinguish options at 18%, 21%, 24%.)

**When NOT to approximate:** when two options are within 2% of each other. That is a signal the setter expects exact work — do it exactly.

---

## 3. Formula Bank

| # | Concept | Formula |
|---|---|---|
| 1 | Percentage of total | $\dfrac{\text{Part}}{\text{Whole}} \times 100$ |
| 2 | Percentage change | $\dfrac{\text{New} - \text{Old}}{\text{Old}} \times 100$ |
| 3 | Value after *x*% change | $\text{Old} \times \left(1 \pm \dfrac{x}{100}\right)$ |
| 4 | Reverse a percentage change | $\text{Old} = \dfrac{\text{New}}{1 \pm x/100}$ |
| 5 | Pie: sector value | $\dfrac{\text{Sector \%}}{100} \times \text{Total}$ |
| 6 | Pie: central angle | $\dfrac{\text{Sector \%}}{100} \times 360°$; $1\% = 3.6°$ |
| 7 | Pie: percentage from angle | $\dfrac{\text{Angle}}{360°} \times 100$ |
| 8 | Average | $\dfrac{\text{Sum}}{\text{Count}}$ |
| 9 | Weighted average | $\dfrac{\sum n_i A_i}{\sum n_i}$ |
| 10 | Ratio between entries | $\dfrac{A}{B}$, then simplify |
| 11 | A is *x*% more than B | $\dfrac{A-B}{B} \times 100$ |
| 12 | Rate (rejection, defect, pass) | $\dfrac{\text{Sub-count}}{\text{Total}} \times 100$ |
| 13 | Compound growth chain | $P \times \prod\left(1 + \dfrac{g_i}{100}\right)$ |
| 14 | CAGR over *n* years | $\left[\left(\dfrac{A}{P}\right)^{1/n} - 1\right] \times 100$ |
| 15 | Two-set union | $n(A) + n(B) - n(A\cap B)$ |
| 16 | Only A | $n(A) - n(A\cap B)$ |
| 17 | Neither | $\text{Total} - n(A\cup B)$ |
| 18 | Three-set union | $\sum n(A) - \sum n(A\cap B) + n(A\cap B\cap C)$ |
| 19 | Cross-exhibit total | $\sum (\text{count}_i \times \text{rate}_i)$ |
| 20 | Share of a component in a chained total | $\dfrac{\text{count}_i \times \text{rate}_i}{\sum(\text{count} \times \text{rate})} \times 100$ |

---

## 4. Shortcuts & Tricks

### 4.1 Fraction–percentage conversions (memorise; they carry DI)

| Fraction | % | Fraction | % |
|---|---|---|---|
| 1/2 | 50% | 1/9 | 11.11% |
| 1/3 | 33.33% | 1/10 | 10% |
| 1/4 | 25% | 1/11 | 9.09% |
| 1/5 | 20% | 1/12 | 8.33% |
| 1/6 | 16.67% | 1/15 | 6.67% |
| 1/7 | 14.29% | 1/16 | 6.25% |
| 1/8 | 12.5% | 1/20 | 5% |

When you see 660 out of 1,200, recognise it as 11/20 = **55%** rather than long-dividing.

### 4.2 The percentage-change ladder (mental method)

To find what percent A is of B, or how much A exceeds B, anchor on easy fractions of B.

> **"200 is what percent more than 160?"**
```
10% of 160 = 16
20% of 160 = 32
25% of 160 = 40   ←  and 200 − 160 = 40
                       Answer: 25%
```

### 4.3 Ratio comparison without dividing

To compare a/b against c/d, **cross-multiply**:

$$\frac{a}{b} \text{ vs } \frac{c}{d} \quad \longrightarrow \quad ad \text{ vs } bc$$

> Which is the higher rejection rate: 80/2,000 or 45/1,500?
> Cross-multiply: 80 × 1,500 = 120,000 vs 45 × 2,000 = 90,000.
> Left side is larger ⇒ **80/2,000 is the higher rate** ✓

This is far faster than computing both percentages, especially with awkward numbers.

### 4.4 Percentage points vs percentage

> A market share moves **from 20% to 25%**.
> - It rose **5 percentage points**.
> - It rose **25 percent** (5/20 × 100).

DI questions exploit this constantly. Read whether the question says "percent" or "percentage points".

### 4.5 The pie-chart angle table

| % | Angle | | % | Angle |
|---|---|---|---|---|
| 5% | 18° | | 25% | 90° |
| 10% | 36° | | 30% | 108° |
| 12.5% | 45° | | 33.33% | 120° |
| 15% | 54° | | 40% | 144° |
| 20% | 72° | | 50% | 180° |

**Rule: 1% = 3.6°, and 10% = 36°.** Everything else scales from there.

### 4.6 The "highest growth" scan

For "which year/region grew fastest", do **not** compute every percentage. Instead:

```
1.  Eyeball the absolute jumps. Discard any category with a small jump
    AND a large base — it cannot win.
2.  Shortlist 2–3 candidates: big jump, small base.
3.  Compute only those.
```

> Jumps of 40 (from 160), 40 (from 200), 32 (from 128), 48 (from 152).
> The 40-from-200 case has the biggest base and a mid-sized jump — discard it.
> Compare the rest: 25%, 25%, 31.6% ⇒ **the 48-from-152 wins.**

### 4.7 Cross-exhibit questions

When one table gives **counts** and another gives **rates** (salary per head, defect rate, price per unit), the combined quantity is the **product**:

$$\text{Total} = \text{Count} \times \text{Rate}$$

Build a third column mentally:

| Dept | Headcount | Avg salary (₹k) | **Salary bill (₹k)** |
|---|---|---|---|
| IT | 400 | 60 | **24,000** |
| Finance | 200 | 50 | **10,000** |
| HR | 100 | 40 | **4,000** |
| Ops | 300 | 40 | **12,000** |
| **Total** | **1,000** | — | **50,000** |

Note the company-wide *average* salary is 50,000/1,000 = ₹50k — **not** the simple mean of 60, 50, 40 and 40 (= ₹47.5k). It must be weighted by headcount.

### 4.8 Order of attack within a set

Not all five questions in a set are equally hard. Sequence them:

```
1.  Direct read / single-value questions       (10–15 s each)
2.  Simple totals and averages                 (20 s)
3.  Percentage change between two entries      (25 s)
4.  Ratios and shares                          (30 s)
5.  "Which is highest/lowest" comparisons      (45 s — do LAST)
```

Banking easy marks first means a hard comparison question can be abandoned without cost.

### 4.9 Sanity checks

```
✓ Percentages of a whole must sum to 100
✓ Central angles must sum to 360°
✓ A part can never exceed its whole
✓ If category totals are given, your computed total must match
✓ Growth chains: compare against the naive sum — compounding gives MORE
   for all-positive chains
✓ A weighted average must lie between the smallest and largest component
```

---

## 5. Solved Examples

### Example A — Table

**Exhibit: Revenue of XYZ Ltd (₹ crore)**

| Year | Revenue |
|---|---|
| 2020 | 320 |
| 2021 | 400 |
| 2022 | 440 |
| 2023 | 550 |
| 2024 | 660 |

---

**Q1. Find the total revenue over the five years.**

**Step 1 — Add, grouping for convenience.**
$$320 + 400 = 720$$
$$440 + 550 = 990$$
$$720 + 990 + 660 = 2{,}370$$

**Answer: ₹2,370 crore**

---

**Q2. Find the percentage increase from 2020 to 2021.**

**Step 1 — Identify old and new.** Old = 320 (the base), New = 400.

**Step 2 — Apply the formula.**
$$\frac{400 - 320}{320} \times 100 = \frac{80}{320} \times 100 = \frac{1}{4} \times 100 = 25\%$$

**Answer: 25%**

---

**Q3. In which year was the year-on-year percentage growth the highest?**

**Step 1 — Compute the jump and base for each year.**

| Year | Jump | Base | Growth |
|---|---|---|---|
| 2021 | 80 | 320 | 25.0% |
| 2022 | 40 | 400 | 10.0% |
| 2023 | 110 | 440 | **25.0%** |
| 2024 | 110 | 550 | 20.0% |

**Step 2 — Compare.** 2021 and 2023 tie at 25%; both exceed 2022 and 2024.

**Answer: 2021 and 2023 (both 25%)**

> **Method note:** 2022 could be discarded on sight — a *smaller* jump on a *larger* base cannot beat 2021. Eliminating before computing is the core DI speed skill.

---

**Q4. The 2024 revenue is what percentage of the 2020 revenue?**

$$\frac{660}{320} \times 100 = 206.25\%$$

**Answer: 206.25%**

> **Read the wording.** "*Is what percentage of*" ⇒ 206.25%. "*Is what percentage more than*" ⇒ 106.25%. The two differ by exactly 100.

---

### Example B — Pie chart

**Exhibit: Breakdown of a company's ₹1,200 crore annual expenditure**

```
        Raw materials  35%  ████████████████████
        Salaries       25%  ██████████████
        Marketing      15%  ████████
        Logistics      12%  ███████
        R&D            08%  ████
        Admin          05%  ███
        ─────────────────────────────────────
        TOTAL         100%   =  ₹1,200 crore
```

---

**Q5. How much is spent on raw materials?**

$$0.35 \times 1{,}200 = ₹420 \text{ crore}$$

**Answer: ₹420 crore**

---

**Q6. By how much does expenditure on salaries exceed that on logistics?**

**Step 1 — Work in percentage points first.**
$$25\% - 12\% = 13 \text{ percentage points}$$

**Step 2 — Convert to rupees.**
$$0.13 \times 1{,}200 = ₹156 \text{ crore}$$

**Answer: ₹156 crore**

> **Efficiency note:** subtracting the percentages *before* multiplying halves the arithmetic. Computing ₹300 crore and ₹144 crore separately and then subtracting gives the same answer but takes twice as long.

---

**Q7. What is the central angle of the Marketing sector?**

$$\frac{15}{100} \times 360° = 54°$$

**Answer: 54°**

*(Or use 1% = 3.6°: 15 × 3.6 = 54° ✓)*

---

**Q8. Salaries expenditure is what percent of raw-materials expenditure?**

Since both are shares of the same total, work directly with the percentages:
$$\frac{25}{35} \times 100 = \frac{5}{7} \times 100 = 71.43\%$$

**Answer: ≈ 71.43%**

> **Shortcut:** you never need to convert to rupees. Ratios between pie sectors equal the ratios of their percentages.

---

### Example C — Cross-exhibit (two tables)

**Exhibit 1: Units produced (thousands)**

| Plant | Units |
|---|---|
| A | 50 |
| B | 30 |
| C | 20 |

**Exhibit 2: Cost per unit (₹)**

| Plant | Cost/unit |
|---|---|
| A | 80 |
| B | 100 |
| C | 150 |

---

**Q9. Which plant has the highest total production cost?**

**Step 1 — Build the product column.**

| Plant | Units (000) | Cost/unit | **Total cost (₹ '000)** |
|---|---|---|---|
| A | 50 | 80 | **4,000** |
| B | 30 | 100 | **3,000** |
| C | 20 | 150 | **3,000** |

**Step 2 — Compare.**
Plant A at ₹4,000 thousand (₹40 lakh) is the highest.

**Answer: Plant A**

> **Trap:** picking C because it has the highest cost *per unit*. Total cost is count × rate — C's high unit cost is offset by its low volume.

---

**Q10. What is the average cost per unit across all three plants?**

**Step 1 — This must be a WEIGHTED average.**
$$\text{Average} = \frac{\text{Total cost}}{\text{Total units}} = \frac{4{,}000 + 3{,}000 + 3{,}000}{50 + 30 + 20} = \frac{10{,}000}{100} = ₹100$$

**Answer: ₹100 per unit**

> **Trap:** averaging 80, 100 and 150 to get ₹110. That would only be correct if all three plants produced equal volumes. Plant A, the cheapest, produces half the total output — so it pulls the true average down to ₹100.

---

## 6. Practice Questions

**Instructions:** 50 questions across 10 data sets.
Sets 1–3 Easy · Sets 4–7 Medium · Sets 8–10 Hard.
Target: **45 seconds per question**. Full solutions in [Section 7](#7-detailed-solutions).

---

### 🟢 SET 1 — Table (Questions 1–5)

**The table shows the annual revenue of Aarav Industries Ltd.**

| Year | Revenue (₹ crore) |
|---|---|
| 2020 | 200 |
| 2021 | 250 |
| 2022 | 300 |
| 2023 | 420 |
| 2024 | 480 |

**Q1.** What is the total revenue over the five-year period?
(a) ₹1,550 crore  (b) ₹1,600 crore  (c) ₹1,650 crore  (d) ₹1,700 crore

**Q2.** What is the percentage increase in revenue from 2020 to 2021?
(a) 20%  (b) 25%  (c) 30%  (d) 50%

**Q3.** What is the average annual revenue over the period?
(a) ₹310 crore  (b) ₹320 crore  (c) ₹330 crore  (d) ₹340 crore

**Q4.** In which year was the year-on-year percentage growth the highest?
(a) 2021  (b) 2022  (c) 2023  (d) 2024

**Q5.** The 2024 revenue is what percentage of the 2020 revenue?
(a) 140%  (b) 200%  (c) 240%  (d) 280%

---

### 🟢 SET 2 — Bar chart (Questions 6–10)

**Units sold (in thousands) of four products in 2024:**

```
  80 ┤                                   ███
     │                                   ███
  70 ┤                                   ███
     │                                   ███
  60 ┤              ███                  ███
     │              ███                  ███
  50 ┤              ███                  ███
     │   ███        ███                  ███
  40 ┤   ███        ███                  ███
     │   ███        ███                  ███
  30 ┤   ███        ███       ███        ███
     │   ███        ███       ███        ███
  20 ┤   ███        ███       ███        ███
     │   ███        ███       ███        ███
  10 ┤   ███        ███       ███        ███
     │   ███        ███       ███        ███
   0 ┴───────────────────────────────────────
        A(45)      B(60)     C(30)     D(75)
```

**Q6.** What is the total number of units sold across all four products?
(a) 190 thousand  (b) 200 thousand  (c) 210 thousand  (d) 220 thousand

**Q7.** Sales of Product D exceed those of Product C by what percentage?
(a) 60%  (b) 100%  (c) 150%  (d) 250%

**Q8.** Product B's sales are what percentage of the total sales?
(a) 25.00%  (b) 28.57%  (c) 30.00%  (d) 33.33%

**Q9.** What is the ratio of Product A's sales to Product D's sales?
(a) 2 : 3  (b) 3 : 5  (c) 4 : 5  (d) 5 : 3

**Q10.** What are the average sales per product?
(a) 47.5 thousand  (b) 50.0 thousand  (c) 52.5 thousand  (d) 55.0 thousand

---

### 🟢 SET 3 — Pie chart (Questions 11–15)

**A household's monthly budget of ₹40,000 is allocated as follows:**

```
        Rent          30%   ███████████████
        Food          25%   ████████████
        Transport     15%   ███████
        Education     12%   ██████
        Utilities     10%   █████
        Savings       08%   ████
        ──────────────────────────────────
        TOTAL        100%   =  ₹40,000
```

**Q11.** How much is spent on rent?
(a) ₹10,000  (b) ₹11,000  (c) ₹12,000  (d) ₹13,000

**Q12.** How much more is spent on food than on transport?
(a) ₹3,000  (b) ₹3,500  (c) ₹4,000  (d) ₹4,500

**Q13.** What is the combined amount allocated to education, utilities and savings?
(a) ₹10,000  (b) ₹11,000  (c) ₹12,000  (d) ₹14,000

**Q14.** What is the ratio of the transport allocation to the savings allocation?
(a) 3 : 2  (b) 8 : 15  (c) 15 : 8  (d) 5 : 3

**Q15.** What is the central angle of the "Food" sector in the pie chart?
(a) 72°  (b) 80°  (c) 90°  (d) 108°

---

### 🟡 SET 4 — Line graph (Questions 16–20)

**Monthly production (in tonnes) at a factory:**

```
 220 ┤                                        ●
     │                                       ╱
 200 ┤                                     ╱
     │                                   ╱
 180 ┤              ●                  ╱
     │            ╱   ╲              ╱
 160 ┤          ╱       ╲        ● ╱
     │        ╱           ╲    ╱
 150 ┤   ●  ╱               ●╱
     │    ╲╱
 140 ┤     ●
     │
 120 ┤ ●
     │
   0 ┴──────────────────────────────────────
      Jan  Feb  Mar  Apr  May  Jun
      120  150  140  180  160  210
```

**Q16.** What is the total production over the six months?
(a) 920 t  (b) 940 t  (c) 960 t  (d) 980 t

**Q17.** What is the average monthly production?
(a) 150 t  (b) 155 t  (c) 160 t  (d) 165 t

**Q18.** What is the percentage increase in production from January to June?
(a) 65%  (b) 70%  (c) 75%  (d) 90%

**Q19.** In how many months was production strictly above the six-month average?
(a) 1  (b) 2  (c) 3  (d) 4

**Q20.** In which month was the decline from the previous month the largest?
(a) February  (b) March  (c) May  (d) June

---

### 🟡 SET 5 — Table with two dimensions (Questions 21–25)

**Distribution of 1,200 students across streams and gender:**

| Stream | Boys | Girls | Total |
|---|---|---|---|
| Science | 240 | 160 | 400 |
| Commerce | 180 | 220 | 400 |
| Arts | 120 | 280 | 400 |
| **Total** | **540** | **660** | **1,200** |

**Q21.** What percentage of the college's students are girls?
(a) 45%  (b) 50%  (c) 55%  (d) 60%

**Q22.** What is the ratio of boys to girls in the Science stream?
(a) 2 : 3  (b) 3 : 2  (c) 4 : 3  (d) 5 : 4

**Q23.** In which stream is the proportion of girls the highest?
(a) Science  (b) Commerce  (c) Arts  (d) All are equal

**Q24.** Boys in Commerce form what percentage of all boys in the college?
(a) 30.00%  (b) 33.33%  (c) 36.00%  (d) 45.00%

**Q25.** By what percentage do the girls in Arts exceed the girls in Science?
(a) 60%  (b) 75%  (c) 100%  (d) 120%

---

### 🟡 SET 6 — Two exhibits cross-referenced (Questions 26–30)

**Exhibit A — Number of employees by department**

| Department | Employees |
|---|---|
| IT | 400 |
| Finance | 200 |
| HR | 100 |
| Operations | 300 |
| **Total** | **1,000** |

**Exhibit B — Average monthly salary (₹ thousand)**

| Department | Avg salary |
|---|---|
| IT | 60 |
| Finance | 50 |
| HR | 40 |
| Operations | 40 |

**Q26.** What is the total monthly salary bill for the IT department?
(a) ₹180 lakh  (b) ₹200 lakh  (c) ₹240 lakh  (d) ₹260 lakh

**Q27.** Which department has the highest total monthly salary bill?
(a) IT  (b) Finance  (c) HR  (d) Operations

**Q28.** What is the average monthly salary across the whole company?
(a) ₹47,500  (b) ₹48,000  (c) ₹50,000  (d) ₹52,500

**Q29.** The Finance department's salary bill is what percentage of the company's total salary bill?
(a) 18%  (b) 20%  (c) 22%  (d) 25%

**Q30.** What is the ratio of the IT salary bill to the Operations salary bill?
(a) 3 : 2  (b) 2 : 1  (c) 4 : 3  (d) 5 : 3

---

### 🟡 SET 7 — Pie chart plus comparison table (Questions 31–35)

**Exhibit A — Region-wise share of 2024 sales (total ₹800 crore)**

```
        North   25%
        South   30%
        East    20%
        West    25%
        ────────────
        TOTAL  100%   =  ₹800 crore
```

**Exhibit B — 2023 sales by region (₹ crore)**

| Region | 2023 Sales |
|---|---|
| North | 160 |
| South | 200 |
| East | 128 |
| West | 152 |
| **Total** | **640** |

**Q31.** What were the 2024 sales from the South region?
(a) ₹200 crore  (b) ₹220 crore  (c) ₹240 crore  (d) ₹260 crore

**Q32.** Which region recorded the highest percentage growth from 2023 to 2024?
(a) North  (b) South  (c) East  (d) West

**Q33.** What was the overall percentage growth in total company sales from 2023 to 2024?
(a) 20%  (b) 22.5%  (c) 25%  (d) 28%

**Q34.** What is the ratio of North's 2024 sales to East's 2024 sales?
(a) 4 : 3  (b) 5 : 4  (c) 3 : 2  (d) 5 : 3

**Q35.** If East's sales grow by a further 25% in 2025, what will they be?
(a) ₹180 crore  (b) ₹190 crore  (c) ₹200 crore  (d) ₹210 crore

---

### 🔴 SET 8 — Caselet (Questions 36–40)

**Read the following and answer the questions.**

> A survey of **500 people** was conducted about beverage preferences. **280 people** said they like tea and **220 people** said they like coffee. **100 people** said they like both.
>
> Additionally, among those who like **only tea**, 60% are men; among those who like **only coffee**, 40% are men.

**Q36.** How many people like at least one of the two beverages?
(a) 380  (b) 390  (c) 400  (d) 420

**Q37.** How many people like neither tea nor coffee?
(a) 80  (b) 100  (c) 120  (d) 140

**Q38.** How many men like only tea?
(a) 96  (b) 102  (c) 108  (d) 120

**Q39.** How many women like only coffee?
(a) 48  (b) 60  (c) 72  (d) 84

**Q40.** What is the ratio of people who like only tea to those who like only coffee?
(a) 2 : 1  (b) 3 : 2  (c) 4 : 3  (d) 5 : 4

---

### 🔴 SET 9 — Quality-control table (Questions 41–45)

**Production and rejection data for four machines during a shift:**

| Machine | Items produced | Items rejected |
|---|---|---|
| M1 | 2,000 | 80 |
| M2 | 2,500 | 125 |
| M3 | 1,500 | 45 |
| M4 | 4,000 | 200 |

**Q41.** What is the total number of items produced?
(a) 9,000  (b) 9,500  (c) 10,000  (d) 10,500

**Q42.** What is the overall rejection rate?
(a) 4.0%  (b) 4.5%  (c) 5.0%  (d) 5.5%

**Q43.** Which machine has the lowest rejection rate?
(a) M1  (b) M2  (c) M3  (d) M4

**Q44.** How many items produced by M4 were accepted?
(a) 3,600  (b) 3,700  (c) 3,800  (d) 3,900

**Q45.** If M2's rejection rate were reduced to match M3's, how many fewer items would M2 reject?
(a) 40  (b) 45  (c) 50  (d) 55

---

### 🔴 SET 10 — Growth-rate table (Questions 46–50)

**The table gives the annual percentage change in the revenue of Meridian Corp. relative to the previous year. Revenue in 2020 was ₹500 crore.**

| Year | Change over previous year |
|---|---|
| 2021 | +20% |
| 2022 | +25% |
| 2023 | −10% |
| 2024 | +20% |

**Q46.** What was the revenue in 2022?
(a) ₹700 crore  (b) ₹720 crore  (c) ₹750 crore  (d) ₹775 crore

**Q47.** What was the revenue in 2024?
(a) ₹775 crore  (b) ₹790 crore  (c) ₹810 crore  (d) ₹825 crore

**Q48.** What is the overall percentage growth in revenue from 2020 to 2024?
(a) 55%  (b) 58%  (c) 62%  (d) 65%

**Q49.** In which year was the revenue the highest?
(a) 2021  (b) 2022  (c) 2023  (d) 2024

**Q50.** If revenue grows by a further 10% in 2025, what will the 2025 revenue be?
(a) ₹864 crore  (b) ₹875 crore  (c) ₹891 crore  (d) ₹900 crore

---

## 7. Detailed Solutions

### 🟢 SET 1 — Solutions 1–5

---

**Q1. Total revenue over five years. → (c) ₹1,650 crore**

**Step 1 — Add, grouping for easy arithmetic.**
$$200 + 250 = 450$$
$$300 + 420 = 720$$
$$450 + 720 + 480 = 1{,}650$$

**Answer: (c) ₹1,650 crore**

---

**Q2. Percentage increase from 2020 to 2021. → (b) 25%**

**Formula used:** (New − Old)/Old × 100

$$\frac{250 - 200}{200} \times 100 = \frac{50}{200} \times 100 = 25\%$$

> Note the base is **200** (the 2020 figure), not 250.

**Answer: (b) 25%**

---

**Q3. Average annual revenue. → (c) ₹330 crore**

$$\frac{1{,}650}{5} = 330$$

**Answer: (c) ₹330 crore**

---

**Q4. Year with the highest year-on-year growth. → (c) 2023**

**Step 1 — Tabulate jump and base.**

| Year | Jump | Base | Growth |
|---|---|---|---|
| 2021 | 50 | 200 | 25.00% |
| 2022 | 50 | 250 | 20.00% |
| 2023 | 120 | 300 | **40.00%** |
| 2024 | 60 | 420 | 14.29% |

**Step 2 — Identify the maximum.**
2023 at 40% is clearly the highest.

**⚡ Elimination shortcut:** 2023 has the **largest jump (120)** on a **mid-sized base (300)**. 2024's jump of 60 sits on the largest base of 420 — it cannot compete. Only 2021 and 2023 needed checking.

**Answer: (c) 2023**

---

**Q5. 2024 revenue as a percentage of 2020 revenue. → (c) 240%**

$$\frac{480}{200} \times 100 = 240\%$$

> **Wording check:** "is what percentage **of**" ⇒ 240%. Had it asked "is what percentage **more than**", the answer would be 140%.

**Answer: (c) 240%**

---

### 🟢 SET 2 — Solutions 6–10

---

**Q6. Total units sold. → (c) 210 thousand**

$$45 + 60 + 30 + 75 = 210 \text{ thousand}$$

**Answer: (c) 210 thousand**

---

**Q7. D exceeds C by what percentage? → (c) 150%**

**Formula used:** (D − C)/C × 100 — the base is **C**, the item being compared against.

$$\frac{75 - 30}{30} \times 100 = \frac{45}{30} \times 100 = 150\%$$

> **Trap:** computing 45/75 = 60% (option a). That would answer "C is what percent less than D" — the other direction, with a different base.

**Answer: (c) 150%**

---

**Q8. B as a percentage of total. → (b) 28.57%**

$$\frac{60}{210} \times 100 = \frac{2}{7} \times 100 = 28.57\%$$

**⚡ Shortcut:** 60/210 simplifies to 2/7, and 1/7 = 14.29%, so 2/7 = 28.57% ✓

**Answer: (b) 28.57%**

---

**Q9. Ratio of A to D. → (b) 3 : 5**

$$45 : 75$$

Divide both by their HCF, 15:
$$3 : 5$$

**Answer: (b) 3 : 5**

---

**Q10. Average sales per product. → (c) 52.5 thousand**

$$\frac{210}{4} = 52.5 \text{ thousand}$$

**Answer: (c) 52.5 thousand**

---

### 🟢 SET 3 — Solutions 11–15

---

**Q11. Amount spent on rent. → (c) ₹12,000**

$$0.30 \times 40{,}000 = ₹12{,}000$$

**Answer: (c) ₹12,000**

---

**Q12. Food exceeds transport by how much? → (c) ₹4,000**

**Step 1 — Subtract the percentages first (faster).**
$$25\% - 15\% = 10 \text{ percentage points}$$

**Step 2 — Convert to rupees.**
$$0.10 \times 40{,}000 = ₹4{,}000$$

**Cross-check:** Food = ₹10,000, Transport = ₹6,000, difference = ₹4,000 ✓

**Answer: (c) ₹4,000**

---

**Q13. Education + Utilities + Savings. → (c) ₹12,000**

**Step 1 — Add the percentages.**
$$12\% + 10\% + 8\% = 30\%$$

**Step 2 — Convert.**
$$0.30 \times 40{,}000 = ₹12{,}000$$

**Answer: (c) ₹12,000**

---

**Q14. Ratio of transport to savings. → (c) 15 : 8**

Since both are shares of the same total, use the percentages directly:
$$15 : 8$$

*(In rupees: ₹6,000 : ₹3,200 = 15 : 8 ✓)*

> **Order matters.** The question asks transport **to** savings, so transport comes first. Option (b) reverses it.

**Answer: (c) 15 : 8**

---

**Q15. Central angle of the Food sector. → (c) 90°**

**Formula used:** Angle = (Sector % / 100) × 360°

$$\frac{25}{100} \times 360° = 90°$$

*(Or use 1% = 3.6°: 25 × 3.6 = 90° ✓)*

**Answer: (c) 90°**

---

### 🟡 SET 4 — Solutions 16–20

---

**Q16. Total production over six months. → (c) 960 t**

$$120 + 150 + 140 + 180 + 160 + 210$$

**Grouping:**
$$(120 + 180) + (150 + 210) + (140 + 160) = 300 + 360 + 300 = 960$$

**Answer: (c) 960 t**

---

**Q17. Average monthly production. → (c) 160 t**

$$\frac{960}{6} = 160 \text{ tonnes}$$

**Answer: (c) 160 t**

---

**Q18. Percentage increase from January to June. → (c) 75%**

$$\frac{210 - 120}{120} \times 100 = \frac{90}{120} \times 100 = \frac{3}{4} \times 100 = 75\%$$

**Answer: (c) 75%**

---

**Q19. Months strictly above the average of 160 t. → (b) 2**

**Step 1 — Compare each month against 160.**

| Month | Production | Above 160? |
|---|---|---|
| Jan | 120 | ✗ |
| Feb | 150 | ✗ |
| Mar | 140 | ✗ |
| Apr | 180 | ✓ |
| May | 160 | ✗ (equal, not above) |
| Jun | 210 | ✓ |

**Step 2 — Count.** Two months.

> **The word "strictly" matters.** May is exactly at the average, so it does not qualify. Counting it would give 3 — a deliberately planted option.

**Answer: (b) 2**

---

**Q20. Month with the largest decline from the previous month. → (c) May**

**Step 1 — Compute all month-on-month changes.**

| Transition | Change |
|---|---|
| Jan → Feb | +30 |
| Feb → Mar | **−10** |
| Mar → Apr | +40 |
| Apr → May | **−20** |
| May → Jun | +50 |

**Step 2 — Compare only the declines.**
Two months declined: March (−10) and May (−20). May's fall is larger.

**Answer: (c) May**

---

### 🟡 SET 5 — Solutions 21–25

---

**Q21. Percentage of students who are girls. → (c) 55%**

$$\frac{660}{1{,}200} \times 100 = 55\%$$

**⚡ Shortcut:** 660/1,200 = 66/120 = 11/20, and 11/20 = 55% ✓

**Answer: (c) 55%**

---

**Q22. Ratio of boys to girls in Science. → (b) 3 : 2**

$$240 : 160$$

Divide both by 80:
$$3 : 2$$

**Answer: (b) 3 : 2**

---

**Q23. Stream with the highest proportion of girls. → (c) Arts**

**Step 1 — Compute each proportion.** All streams have 400 students, which simplifies the comparison considerably.

| Stream | Girls | Total | Proportion |
|---|---|---|---|
| Science | 160 | 400 | 40% |
| Commerce | 220 | 400 | 55% |
| Arts | **280** | 400 | **70%** |

**Step 2 — Identify the maximum.** Arts, at 70%.

> **When all denominators are equal**, comparing the raw counts is sufficient — 280 is the largest. But *verify* the denominators are equal before taking that shortcut; if they differ, you must compute the rates.

**Answer: (c) Arts**

---

**Q24. Commerce boys as a percentage of all boys. → (b) 33.33%**

$$\frac{180}{540} \times 100 = \frac{1}{3} \times 100 = 33.33\%$$

> **Note the denominator.** The question asks for a share of *all boys* (540), not of the Commerce stream (400) or the whole college (1,200). Using 400 would give 45%; using 1,200 would give 15% — both are offered as distractors in similar questions.

**Answer: (b) 33.33%**

---

**Q25. Arts girls exceed Science girls by what percentage? → (b) 75%**

**Formula used:** (Arts − Science)/**Science** × 100 — the base is the quantity being exceeded.

$$\frac{280 - 160}{160} \times 100 = \frac{120}{160} \times 100 = 75\%$$

**Answer: (b) 75%**

---

### 🟡 SET 6 — Solutions 26–30

---

**Q26. IT department's total monthly salary bill. → (c) ₹240 lakh**

**Formula used:** Total = Headcount × Average salary

$$400 \times ₹60{,}000 = ₹2{,}40{,}00{,}000 = ₹240 \text{ lakh} = ₹2.4 \text{ crore}$$

*(In thousands: 400 × 60 = 24,000 thousand = ₹240 lakh.)*

**Answer: (c) ₹240 lakh**

---

**Q27. Department with the highest total salary bill. → (a) IT**

**Step 1 — Build the product column.**

| Department | Employees | Avg salary (₹k) | **Salary bill (₹k)** |
|---|---|---|---|
| IT | 400 | 60 | **24,000** |
| Finance | 200 | 50 | 10,000 |
| HR | 100 | 40 | 4,000 |
| Operations | 300 | 40 | 12,000 |
| **Total** | **1,000** | — | **50,000** |

**Step 2 — Compare.** IT's ₹24,000 thousand is the largest — nearly half the company's entire payroll.

**Answer: (a) IT**

---

**Q28. Company-wide average monthly salary. → (c) ₹50,000**

**This must be a weighted average.**

$$\text{Average} = \frac{\text{Total salary bill}}{\text{Total headcount}} = \frac{50{,}000 \text{ thousand}}{1{,}000} = 50 \text{ thousand} = ₹50{,}000$$

> **Trap:** taking the simple mean of the four salaries: (60 + 50 + 40 + 40)/4 = ₹47,500 — option (a). That would only be correct if all four departments had equal headcount. IT alone has 400 of the 1,000 employees and the highest salary, so it pulls the true average *up* to ₹50,000.

**Answer: (c) ₹50,000**

---

**Q29. Finance's share of the total salary bill. → (b) 20%**

$$\frac{10{,}000}{50{,}000} \times 100 = 20\%$$

> **Note:** Finance has 20% of the headcount *and* 20% of the payroll — a coincidence arising because its average salary (₹50k) exactly equals the company average. IT, by contrast, has 40% of the headcount but 48% of the payroll.

**Answer: (b) 20%**

---

**Q30. Ratio of IT's salary bill to Operations'. → (b) 2 : 1**

$$24{,}000 : 12{,}000 = 2 : 1$$

**Answer: (b) 2 : 1**

---

### 🟡 SET 7 — Solutions 31–35

---

**Q31. South region's 2024 sales. → (c) ₹240 crore**

$$0.30 \times 800 = ₹240 \text{ crore}$$

**Answer: (c) ₹240 crore**

---

**Q32. Region with the highest 2023→2024 growth. → (d) West**

**Step 1 — Convert the 2024 percentages into absolute figures.**

| Region | 2024 share | 2024 sales |
|---|---|---|
| North | 25% | ₹200 cr |
| South | 30% | ₹240 cr |
| East | 20% | ₹160 cr |
| West | 25% | ₹200 cr |

**Step 2 — Compute the growth for each region.**

| Region | 2023 | 2024 | Jump | Growth |
|---|---|---|---|---|
| North | 160 | 200 | 40 | 25.00% |
| South | 200 | 240 | 40 | 20.00% |
| East | 128 | 160 | 32 | 25.00% |
| West | 152 | 200 | **48** | **31.58%** |

**Step 3 — Identify the maximum.**
$$\text{West} = \frac{48}{152} \times 100 = 31.58\%$$

**⚡ Elimination shortcut:** West has the **largest jump (48)** on the **second-smallest base (152)** — a strong candidate immediately. South (jump 40 on base 200) can be discarded on sight.

**Answer: (d) West**

---

**Q33. Overall percentage growth in total sales. → (c) 25%**

$$\frac{800 - 640}{640} \times 100 = \frac{160}{640} \times 100 = \frac{1}{4} \times 100 = 25\%$$

**Answer: (c) 25%**

---

**Q34. Ratio of North's to East's 2024 sales. → (b) 5 : 4**

**Method 1 — Use the pie percentages directly.**
$$25\% : 20\% = 5 : 4$$

**Method 2 — Use the absolute figures.**
$$200 : 160 = 5 : 4$$

> Since both are shares of the same total, the percentages give the ratio immediately — no conversion needed.

**Answer: (b) 5 : 4**

---

**Q35. East's sales after a further 25% growth. → (c) ₹200 crore**

**Step 1 — East's 2024 sales.**
$$0.20 \times 800 = ₹160 \text{ crore}$$

**Step 2 — Apply a 25% increase.**
$$160 \times 1.25 = ₹200 \text{ crore}$$

**Answer: (c) ₹200 crore**

---

### 🔴 SET 8 — Solutions 36–40

---

**Q36. People who like at least one beverage. → (c) 400**

**Formula used:** n(A ∪ B) = n(A) + n(B) − n(A ∩ B)

$$= 280 + 220 - 100 = 400$$

> **Why subtract 100?** The 100 people who like both were counted once in the tea group and again in the coffee group. Subtracting removes the double count.

**Answer: (c) 400**

---

**Q37. People who like neither. → (b) 100**

$$\text{Neither} = \text{Total} - n(A \cup B) = 500 - 400 = 100$$

**Full breakdown:**

```
┌─────────────────── 500 surveyed ───────────────────┐
│                                                     │
│   ┌────── TEA (280) ──────┐                        │
│   │                       │                        │
│   │   Only tea            │  Only coffee           │
│   │     180        ┌──────┼──────┐   120           │
│   │                │ BOTH │      │                 │
│   │                │ 100  │      │                 │
│   │                └──────┼──────┘                 │
│   └───────────────────────┘  COFFEE (220)          │
│                                                     │
│              NEITHER:  100                          │
└─────────────────────────────────────────────────────┘
```

**Check:** 180 + 100 + 120 + 100 = 500 ✓

**Answer: (b) 100**

---

**Q38. Men who like only tea. → (c) 108**

**Step 1 — Find how many like only tea.**
$$280 - 100 = 180$$

**Step 2 — Apply the 60% figure.**
$$0.60 \times 180 = 108$$

> **The critical word is "only".** The 60% applies to the *only tea* group (180 people), not to the whole tea group (280). Using 280 would give 168 — the intended trap.

**Answer: (c) 108**

---

**Q39. Women who like only coffee. → (c) 72**

**Step 1 — Find how many like only coffee.**
$$220 - 100 = 120$$

**Step 2 — If 40% are men, then 60% are women.**
$$0.60 \times 120 = 72$$

> **Two-step trap:** the passage gives the *men's* percentage; the question asks for *women*. Take the complement before multiplying.

**Answer: (c) 72**

---

**Q40. Ratio of only-tea to only-coffee. → (b) 3 : 2**

$$180 : 120$$

Divide both by 60:
$$3 : 2$$

**Answer: (b) 3 : 2**

---

### 🔴 SET 9 — Solutions 41–45

---

**Q41. Total items produced. → (c) 10,000**

$$2{,}000 + 2{,}500 + 1{,}500 + 4{,}000 = 10{,}000$$

**Answer: (c) 10,000**

---

**Q42. Overall rejection rate. → (b) 4.5%**

**Step 1 — Total rejects.**
$$80 + 125 + 45 + 200 = 450$$

**Step 2 — Divide by total production.**
$$\frac{450}{10{,}000} \times 100 = 4.5\%$$

> **Trap:** averaging the four individual rates (4%, 5%, 3%, 5%) to get 4.25%. The machines produce different volumes, so the overall rate must be computed from the totals — M4 alone accounts for 40% of production, and its 5% rate carries more weight.

**Answer: (b) 4.5%**

---

**Q43. Machine with the lowest rejection rate. → (c) M3**

**Step 1 — Compute each rate.**

| Machine | Rejected | Produced | Rate |
|---|---|---|---|
| M1 | 80 | 2,000 | 4.0% |
| M2 | 125 | 2,500 | 5.0% |
| M3 | 45 | 1,500 | **3.0%** |
| M4 | 200 | 4,000 | 5.0% |

**Step 2 — Identify the minimum.** M3 at 3.0%.

**⚡ Cross-multiplication check (M1 vs M3):**
$$\frac{80}{2000} \text{ vs } \frac{45}{1500} \implies 80 \times 1500 = 120{,}000 \text{ vs } 45 \times 2000 = 90{,}000$$
The left side is larger, so M1's rate exceeds M3's ✓

**Answer: (c) M3**

---

**Q44. Items accepted from M4. → (c) 3,800**

$$4{,}000 - 200 = 3{,}800$$

**Answer: (c) 3,800**

---

**Q45. Reduction in M2's rejects if its rate matched M3's. → (c) 50**

**Step 1 — M3's rejection rate.**
$$\frac{45}{1{,}500} \times 100 = 3\%$$

**Step 2 — Apply that rate to M2's production.**
$$0.03 \times 2{,}500 = 75 \text{ rejects}$$

**Step 3 — Compute the reduction.**
$$125 - 75 = 50 \text{ fewer rejects}$$

**Answer: (c) 50**

> **Structure of this question type:** apply *one entity's rate* to *another entity's volume*. Always compute the rate first, then multiply by the second volume — never transfer the raw count.

---

### 🔴 SET 10 — Solutions 46–50

---

**Q46. Revenue in 2022. → (c) ₹750 crore**

**Step 1 — Chain the multipliers from the 2020 base.**
$$2021: \quad 500 \times 1.20 = 600$$
$$2022: \quad 600 \times 1.25 = 750$$

**Answer: (c) ₹750 crore**

> **Trap:** applying both growth rates to the original ₹500 crore, giving 500 × 1.45 = ₹725 crore. Each year's growth applies to the *previous year's* revenue, not the base year's.

---

**Q47. Revenue in 2024. → (c) ₹810 crore**

**Full chain:**

| Year | Change | Multiplier | Revenue (₹ cr) |
|---|---|---|---|
| 2020 | — | — | 500 |
| 2021 | +20% | × 1.20 | **600** |
| 2022 | +25% | × 1.25 | **750** |
| 2023 | −10% | × 0.90 | **675** |
| 2024 | +20% | × 1.20 | **810** |

**Answer: (c) ₹810 crore**

---

**Q48. Overall growth from 2020 to 2024. → (c) 62%**

**Step 1 — Compare the endpoints.**
$$\frac{810 - 500}{500} \times 100 = \frac{310}{500} \times 100 = 62\%$$

**Multiplier cross-check:**
$$1.20 \times 1.25 \times 0.90 \times 1.20 = 1.62 \implies +62\% \checkmark$$

> **Trap:** adding the yearly percentages: 20 + 25 − 10 + 20 = 55% — option (a). Growth rates compound; they never simply add. The compounding effect adds a further 7 percentage points here.

**Answer: (c) 62%**

---

**Q49. Year with the highest revenue. → (d) 2024**

From the table in Q47:
$$500 \to 600 \to 750 \to 675 \to \mathbf{810}$$

The highest figure is **₹810 crore in 2024**.

> **Note the dip.** 2023 saw a decline to ₹675 crore, below 2022's ₹750 crore. The revenue path is not monotonic, so you must build the full series rather than assuming the last year is automatically the largest — here it happens to be, but only because the 2024 recovery exceeded the 2023 fall.

**Answer: (d) 2024**

---

**Q50. Revenue in 2025 after a further 10% growth. → (c) ₹891 crore**

$$810 \times 1.10 = 891$$

**Working:** 10% of 810 = 81, so 810 + 81 = ₹891 crore.

**Answer: (c) ₹891 crore**

---

## 8. Quick Revision Sheet

> **One page. Read 48 hours after study, and again the night before the test.**

### The 20-second exhibit scan (do this FIRST, every set)

```
□ UNITS?         ₹ crore / lakh / thousands / tonnes / %
□ TIME RANGE?    which years or months
□ CATEGORIES?    how many rows, columns, sectors
□ ABSOLUTE or %? is any exhibit a SHARE rather than a value
□ TWO exhibits?  what links them
□ FOOTNOTES?     "excluding tax", "estimated", "provisional"
```

### Core formulas

```
% of total        =  Part / Whole × 100
% change          =  (New − Old) / OLD × 100      ← base is always OLD
A exceeds B by    =  (A − B) / B × 100            ← base is B
Value after ±x%   =  Old × (1 ± x/100)
Reverse a change  =  New ÷ (1 ± x/100)            ← DIVIDE

Pie sector value  =  (Sector% / 100) × Total
Pie central angle =  Sector% × 3.6°               (10% = 36°, 25% = 90%)
% from angle      =  Angle / 360 × 100
```

### Cross-exhibit and weighted quantities

```
Count table  ×  Rate table   →   Total = Count × Rate

Weighted average = Σ(count × rate) / Σ(count)
    NEVER the simple mean of the rates
    Result lies CLOSER to the larger group's value
```

### Growth chains (% change given, not values)

```
Convert to multipliers and MULTIPLY:
    +20%, +25%, −10%, +20%   →   1.20 × 1.25 × 0.90 × 1.20 = 1.62
    Total growth = 62%,  NOT 20+25−10+20 = 55%
```

### Set logic (caselets)

```
n(A ∪ B)  =  n(A) + n(B) − n(A ∩ B)
Only A    =  n(A) − n(A ∩ B)
Neither   =  Total − n(A ∪ B)

Three sets: Σn(A) − Σn(A∩B) + n(A∩B∩C)
```

### Speed tools

```
FRACTION → %
  1/2 50%   1/3 33.33%  1/4 25%    1/5 20%    1/6 16.67%
  1/7 14.29% 1/8 12.5%  1/9 11.11% 1/10 10%   1/11 9.09%
  1/12 8.33% 1/16 6.25% 1/20 5%    11/20 55%  2/7 28.57%

COMPARE a/b vs c/d  →  cross-multiply:  ad vs bc
    80/2000 vs 45/1500  →  120,000 vs 90,000  →  first is larger

"HIGHEST GROWTH" SCAN
    1. Discard: small jump on a large base
    2. Shortlist: large jump on a small base
    3. Compute only the 2–3 shortlisted
```

### Order of attack within a set

```
1.  Direct reads / totals            10–20 s
2.  Averages                         20 s
3.  Percentage change (two entries)  25 s
4.  Ratios and shares                30 s
5.  "Which is highest/lowest"        45 s  ← ALWAYS LAST
```

### Sanity checks

```
✓ Percentages of a whole sum to 100
✓ Central angles sum to 360°
✓ A part never exceeds its whole
✓ Your computed total must match any given total
✓ A weighted average lies between the min and max component
✓ All-positive growth chains beat the naive sum of the percentages
```

---

## 9. Common Mistakes

| # | Mistake | Example | Correction |
|---|---|---|---|
| 1 | **Ignoring units** | Reading ₹ crore as ₹ lakh | Scan the units before the questions |
| 2 | **Wrong base in % change** | 200→250 computed as 50/250 | Base is the **old** value: 50/200 = 25% |
| 3 | **Wrong base in "exceeds by"** | D exceeds C: using 45/75 | Base is C: 45/30 = 150% |
| 4 | **Averaging rates unweighted** | Rates 4,5,3,5 ⇒ 4.25% | Use totals: 450/10,000 = 4.5% |
| 5 | **Simple mean of salaries** | (60+50+40+40)/4 = 47.5 | Weight by headcount: 50,000/1,000 = 50 |
| 6 | **Adding growth percentages** | 20+25−10+20 = 55% | Multiply: 1.2×1.25×0.9×1.2 ⇒ 62% |
| 7 | **Growth applied to the base year** | 500 × 1.45 for two years | Chain: 500→600→750 |
| 8 | **"Only" ignored in caselets** | 60% of all 280 tea-likers | 60% of the 180 *only-tea* group |
| 9 | **Complement not taken** | Men's % used for a women's question | Women = 100% − men's % |
| 10 | **Absolute compared instead of rate** | Fewest rejects ⇒ best machine | Compute rejects ÷ produced |
| 11 | **"Strictly above" read as "at least"** | Counting a value equal to the average | Equal ≠ above |
| 12 | **Ratio order reversed** | "Transport to savings" given as 8:15 | Keep the stated order: 15:8 |
| 13 | **"% of" vs "% more than"** | 480/200 answered as 140% | "of" ⇒ 240%; "more than" ⇒ 140% |
| 14 | **Percentage points vs percent** | 20%→25% called "a 5% rise" | 5 percentage points = a 25% rise |
| 15 | **Wrong denominator chosen** | Commerce boys ÷ Commerce total | Question asked ÷ **all boys** |

---

## Practice Answer Key

| Q | Ans | Q | Ans | Q | Ans | Q | Ans | Q | Ans |
|---|---|---|---|---|---|---|---|---|---|
| 1 | c | 11 | c | 21 | c | 31 | c | 41 | c |
| 2 | b | 12 | c | 22 | b | 32 | d | 42 | b |
| 3 | c | 13 | c | 23 | c | 33 | c | 43 | c |
| 4 | c | 14 | c | 24 | b | 34 | b | 44 | c |
| 5 | c | 15 | c | 25 | b | 35 | c | 45 | c |
| 6 | c | 16 | c | 26 | c | 36 | c | 46 | c |
| 7 | c | 17 | c | 27 | a | 37 | b | 47 | c |
| 8 | b | 18 | c | 28 | c | 38 | c | 48 | c |
| 9 | b | 19 | b | 29 | b | 39 | c | 49 | d |
| 10 | c | 20 | c | 30 | b | 40 | b | 50 | c |

**Scoring guide:** 45+/50 → strong. 35–44 → solid; drill the rate-vs-absolute distinction and growth chains. Below 35 → re-read Sections 2.5–2.7 and redo Sets 6, 7, 9 and 10.

> **Timing benchmark:** a full 5-question DI set should take **3–4 minutes**. If a set is taking more than 5 minutes, you are computing exactly where approximation would do.

---

**⬅️ Back:** [Topic 8 — Number System, LCM & HCF](08-number-system-lcm-hcf.md) · **➡️ Next:** [Topic 10 — Permutation, Combination & Probability](10-permutation-combination-probability.md)
