# Topic 7 — Simple & Compound Interest

### EY Placement Aptitude Handbook · Priority Rank #10 · 🟠 High

> **Questions in this file are original, modelled on publicly reported EY test patterns. They are not claimed to be actual previous-year EY questions.**

---

## Contents

1. [Why This Topic Matters for EY](#1-why-this-topic-matters-for-ey)
2. [Core Concepts](#2-core-concepts)
3. [Formula Bank](#3-formula-bank)
4. [Shortcuts & Tricks](#4-shortcuts--tricks)
5. [Solved Examples](#5-solved-examples)
6. [Practice Questions (50)](#6-practice-questions)
7. [Detailed Solutions](#7-detailed-solutions)
8. [Quick Revision Sheet](#8-quick-revision-sheet)
9. [Common Mistakes](#9-common-mistakes)

---

## 1. Why This Topic Matters for EY

**Weightage:** 6–8% of the quantitative section — typically **1 question**.

**Why this is the most "learnable" topic in the syllabus:** it is almost purely formulaic. Unlike puzzles or DI, there is no interpretation required — recognise the type, apply the formula, compute. A candidate who memorises the ten formulas in Section 3 and the difference-formulas in Section 4.3 will get nearly every question right, every time.

**It is also thematically apt for EY.** As a financial-services and assurance firm, EY's assessments lean toward commercial arithmetic — interest, growth, depreciation and instalments show up more often here than in a generic engineering aptitude test.

**Question styles reported:**

| Style | Typical shape |
|---|---|
| Direct SI computation | "SI on ₹5,000 at 8% for 3 years" |
| Reverse SI (find P, R or T) | "What sum gives ₹900 SI at 6% in 3 years?" |
| Direct CI computation | "CI on ₹5,000 at 10% for 2 years" |
| Reverse CI (find P from amount) | "A sum amounts to ₹6,050 in 2 years at 10% CI" |
| **CI − SI difference** | "The difference for 2 years at 5% is ₹25 — find the sum" |
| Doubling / tripling | "A sum doubles in 5 years — when does it become 8×?" |
| Non-annual compounding | "10% p.a. compounded half-yearly for 1.5 years" |
| Two-part investment | "₹12,000 split between 10% and 8%" |
| Instalments | "Annual instalment to clear ₹1,092 in 3 years" |
| Population / depreciation | "Value after 3 years at 10% depreciation" |

**Prerequisite:** [Topic 1 — Percentages](01-percentages.md), especially the multiplier method.

---

## 2. Core Concepts

### 2.1 The vocabulary

| Term | Symbol | Meaning |
|---|---|---|
| **Principal** | P | The sum originally borrowed or invested |
| **Rate** | R | Interest rate per period, as a percentage |
| **Time** | T or n | Number of periods |
| **Interest** | SI or CI | The extra money earned or owed |
| **Amount** | A | Principal + Interest |

$$A = P + I$$

### 2.2 Simple Interest

Interest is calculated **only on the original principal**, every period. The interest earned does not itself earn interest.

$$\boxed{SI = \frac{P \times R \times T}{100}}$$

$$A = P + SI = P\left(1 + \frac{RT}{100}\right)$$

**Rearrangements** (all three appear in EY questions):

$$P = \frac{100 \times SI}{R \times T} \qquad R = \frac{100 \times SI}{P \times T} \qquad T = \frac{100 \times SI}{P \times R}$$

**The defining property of SI:** the interest is the **same every year**. This makes SI problems highly tractable — if a sum earns ₹120 in year 1, it earns ₹120 in every year.

> **A sum amounts to ₹1,560 in 3 years and ₹1,680 in 4 years at SI.**
> The extra year added ₹120 ⇒ annual interest = **₹120**.
> Interest for 3 years = ₹360 ⇒ **P = 1,560 − 360 = ₹1,200**.
> Rate = 120/1200 × 100 = **10%**.

### 2.3 Compound Interest

Interest is added to the principal at the end of each period, so **the interest itself earns interest**.

$$\boxed{A = P\left(1 + \frac{R}{100}\right)^n} \qquad\qquad CI = A - P = P\left[\left(1 + \frac{R}{100}\right)^n - 1\right]$$

**This is exactly the multiplier method from Topic 1.** "10% compound interest for 3 years" is just "multiply by 1.10, three times".

> ₹2,000 at 10% for 3 years: 2000 × 1.331 = ₹2,662 ⇒ **CI = ₹662**

**To reverse it, DIVIDE:**

$$P = \frac{A}{\left(1 + \frac{R}{100}\right)^n}$$

> A sum amounts to ₹6,050 in 2 years at 10% CI ⇒ P = 6050/1.21 = **₹5,000**

### 2.4 SI vs CI — the comparison

| Years | SI | CI |
|---|---|---|
| 1 | Equal | Equal |
| 2 | Less | More |
| 3+ | Less | More (gap widens) |

**Year 1 is always identical.** The divergence begins in year 2, because CI starts charging interest on the first year's interest.

Worked comparison on ₹10,000 at 10%:

| Year | SI amount | CI amount | Gap |
|---|---|---|---|
| 1 | 11,000 | 11,000 | 0 |
| 2 | 12,000 | 12,100 | 100 |
| 3 | 13,000 | 13,310 | 310 |
| 4 | 14,000 | 14,641 | 641 |

### 2.5 ⭐ The difference formulas (the single highest-yield content here)

**For 2 years:**

$$\boxed{CI - SI = P\left(\frac{R}{100}\right)^2}$$

**For 3 years:**

$$\boxed{CI - SI = P\left(\frac{R}{100}\right)^2 \left(3 + \frac{R}{100}\right)}$$

Equivalently, for 3 years:
$$CI - SI = \frac{PR^2(300 + R)}{10^6}$$

**Why the 2-year formula works.** The only difference is the interest earned in year 2 on year 1's interest:
$$\text{Year 1 interest} = \frac{PR}{100}; \qquad \text{interest on it in year 2} = \frac{PR}{100} \times \frac{R}{100} = P\left(\frac{R}{100}\right)^2 \;∎$$

**These formulas are bidirectional** — most EY questions run them backwards:

> *"The difference between CI and SI on a sum for 2 years at 5% is ₹25. Find the sum."*
> $$P\left(\frac{5}{100}\right)^2 = 25 \implies P \times 0.0025 = 25 \implies P = ₹10{,}000$$

**Reference table (difference per ₹10,000 of principal):**

| Rate | 2-year difference | 3-year difference |
|---|---|---|
| 4% | ₹16 | ₹48.64 |
| 5% | ₹25 | ₹76.25 |
| 8% | ₹64 | ₹197.12 |
| 10% | ₹100 | ₹310 |
| 12% | ₹144 | ₹449.28 |
| 20% | ₹400 | ₹1,280 |

### 2.6 The year-on-year CI relationship

The **interest for consecutive years under CI is itself in a geometric progression** with ratio (1 + R/100).

$$\frac{\text{CI in year } (n+1)}{\text{CI in year } n} = 1 + \frac{R}{100}$$

This gives a very fast way to find the rate:

$$\boxed{R = \frac{\text{CI}_{n+1} - \text{CI}_n}{\text{CI}_n} \times 100}$$

> CI in year 2 = ₹1,320, CI in year 3 = ₹1,452.
> $$R = \frac{1452 - 1320}{1320} \times 100 = \frac{132}{1320} \times 100 = 10\%$$

### 2.7 Non-annual compounding

When interest compounds more often than once a year, **divide the rate and multiply the periods**.

| Compounded | Rate per period | Number of periods |
|---|---|---|
| Annually | R | n |
| Half-yearly | R/2 | 2n |
| Quarterly | R/4 | 4n |
| Monthly | R/12 | 12n |

$$A = P\left(1 + \frac{R/k}{100}\right)^{kn} \quad \text{where } k = \text{compoundings per year}$$

> ₹16,000 at 20% p.a. compounded half-yearly for 1 year:
> Rate per half-year = 10%, periods = 2.
> $$A = 16{,}000 \times (1.10)^2 = 16{,}000 \times 1.21 = ₹19{,}360 \implies CI = ₹3{,}360$$

> **More frequent compounding always yields more interest.** Same rate, same time, but half-yearly beats annual, and quarterly beats half-yearly.

### 2.8 Doubling, tripling and multiplying

**Under compound interest**, growth is exponential, so the multiples compose:

$$\boxed{\text{If a sum becomes } m \text{ times in } t \text{ years, it becomes } m^k \text{ times in } kt \text{ years}}$$

> Doubles in 5 years ⇒ 4× in 10 years ⇒ 8× in 15 years ⇒ 16× in 20 years.
> Doubles in 4 years ⇒ 16× (= 2⁴) in 4 × 4 = **16 years**.

**Under simple interest**, growth is linear — you must work with the *interest*, not the multiple:

> Triples in 12 years ⇒ interest = 2P in 12 years ⇒ **1P in 6 years**.
> To become 6 times, interest must be 5P ⇒ 5 × 6 = **30 years**.

> **The two behave completely differently.** Under SI, "doubles in 8 years" means R = 100/8 = 12.5%. Under CI it would mean R ≈ 9.05%. Always check which is being asked.

**SI doubling rate:** $R = \dfrac{100}{T}$; **SI *m*-times rate:** $R = \dfrac{100(m-1)}{T}$

### 2.9 Instalments (SI basis)

To discharge a debt *D* in *n* equal annual instalments at rate *R*% simple interest, each instalment *x* earns simple interest for the remaining years:

$$x\left[1 + \frac{(n-1)R}{100}\right] + x\left[1 + \frac{(n-2)R}{100}\right] + \cdots + x = D$$

> Debt ₹1,092 due in 3 years at 12% SI:
> - Instalment 1 sits for 2 more years ⇒ x(1 + 24/100) = 1.24x
> - Instalment 2 sits for 1 more year ⇒ 1.12x
> - Instalment 3 is paid at the end ⇒ x
> $$3.36x = 1092 \implies x = ₹325$$

### 2.10 Growth and depreciation

Identical mathematics, different words.

$$\text{Growth: } A = P\left(1 + \frac{R}{100}\right)^n \qquad \text{Depreciation: } A = P\left(1 - \frac{R}{100}\right)^n$$

> Machine depreciating at 10% p.a., worth ₹36,450 after 3 years:
> $$P = \frac{36450}{(0.9)^3} = \frac{36450}{0.729} = ₹50{,}000$$

---

## 3. Formula Bank

| # | Concept | Formula |
|---|---|---|
| 1 | Simple Interest | $SI = \dfrac{PRT}{100}$ |
| 2 | Amount (SI) | $A = P\left(1 + \dfrac{RT}{100}\right)$ |
| 3 | Principal from SI | $P = \dfrac{100 \times SI}{RT}$ |
| 4 | Rate from SI | $R = \dfrac{100 \times SI}{PT}$ |
| 5 | Time from SI | $T = \dfrac{100 \times SI}{PR}$ |
| 6 | Amount (CI) | $A = P\left(1 + \dfrac{R}{100}\right)^n$ |
| 7 | Compound Interest | $CI = P\left[\left(1 + \dfrac{R}{100}\right)^n - 1\right]$ |
| 8 | Principal from CI amount | $P = \dfrac{A}{\left(1+\frac{R}{100}\right)^n}$ |
| 9 | **CI − SI (2 years)** | $P\left(\dfrac{R}{100}\right)^2$ |
| 10 | **CI − SI (3 years)** | $P\left(\dfrac{R}{100}\right)^2\left(3 + \dfrac{R}{100}\right)$ |
| 11 | Rate from consecutive CI | $R = \dfrac{CI_{n+1} - CI_n}{CI_n} \times 100$ |
| 12 | Half-yearly compounding | $A = P\left(1 + \dfrac{R}{200}\right)^{2n}$ |
| 13 | Quarterly compounding | $A = P\left(1 + \dfrac{R}{400}\right)^{4n}$ |
| 14 | Different rates per year | $A = P\left(1+\dfrac{R_1}{100}\right)\left(1+\dfrac{R_2}{100}\right)\cdots$ |
| 15 | CI: *m* times in *t* ⇒ *mᵏ* times | in $kt$ years |
| 16 | SI: doubling rate | $R = \dfrac{100}{T}$ |
| 17 | SI: *m*-times rate | $R = \dfrac{100(m-1)}{T}$ |
| 18 | Depreciation | $A = P\left(1 - \dfrac{R}{100}\right)^n$ |
| 19 | Instalment (SI, *n* years) | $D = x\sum_{k=0}^{n-1}\left(1 + \dfrac{kR}{100}\right)$ |
| 20 | Equal SI on two parts | $\dfrac{P_1R_1T_1}{100} = \dfrac{P_2R_2T_2}{100}$ |
| 21 | Fractional-year SI (days) | $T = \dfrac{\text{days}}{365}$ |
| 22 | SI amount at two times | Annual interest $= A_2 - A_1$ (consecutive years) |

---

## 4. Shortcuts & Tricks

### 4.1 The CI ladder (compute CI without powers)

For small *n*, build the amount year by year — it is faster and less error-prone than raising to a power.

> **₹8,000 at 5% for 3 years:**
```
Year 1:   8,000 + 5% (=400)      =  8,400
Year 2:   8,400 + 5% (=420)      =  8,820
Year 3:   8,820 + 5% (=441)      =  9,261
                                    CI = 1,261
```
Each step is a single percentage calculation — no cubes required.

### 4.2 Powers worth memorising

| n | 1.05ⁿ | 1.10ⁿ | 1.20ⁿ | 1.04ⁿ | 0.90ⁿ |
|---|---|---|---|---|---|
| 2 | 1.1025 | 1.21 | 1.44 | 1.0816 | 0.81 |
| 3 | 1.157625 | 1.331 | 1.728 | 1.124864 | 0.729 |
| 4 | 1.21550625 | 1.4641 | 2.0736 | — | 0.6561 |

**Recognising these backwards is the real skill:**

```
A/P = 1.21      →  10% for 2 years
A/P = 1.331     →  10% for 3 years
A/P = 1.1025    →  5%  for 2 years
A/P = 1.157625  →  5%  for 3 years
A/P = 1.0816    →  4%  for 2 years
A/P = 1.1236    →  6%  for 2 years
A/P = 1.44      →  20% for 2 years
```

> *"In what time will ₹4,000 amount to ₹4,630.50 at 5% CI?"*
> 4630.50/4000 = **1.157625** ⇒ recognised instantly as 1.05³ ⇒ **3 years**.

### 4.3 The difference formula, run backwards

This is the highest-frequency shortcut in the topic. Learn to spot the pattern instantly.

```
"Difference between CI and SI for 2 YEARS"  →  P(R/100)²
"Difference between CI and SI for 3 YEARS"  →  P(R/100)²(3 + R/100)
```

**Two-year quick values (difference per ₹1,000):**

| R | Difference on ₹1,000 |
|---|---|
| 4% | ₹1.60 |
| 5% | ₹2.50 |
| 8% | ₹6.40 |
| 10% | ₹10 |
| 20% | ₹40 |

### 4.4 The "SI and CI both given" trick

If both the 2-year SI and the 2-year CI are given:

```
Step 1:  Difference  =  CI − SI
Step 2:  One year's SI  =  SI ÷ 2
Step 3:  Rate = (Difference / One year's SI) × 100
Step 4:  P = (100 × SI) / (R × 2)
```

> SI = ₹1,000, CI = ₹1,050 over 2 years.
> Difference = 50. One year's SI = 500.
> R = 50/500 × 100 = **10%**. P = 100 × 1000/(10 × 2) = **₹5,000**.

**Why:** the difference *is* the interest earned in year 2 on year 1's interest.

### 4.5 Doubling shortcuts

```
CI:  m times in t years  →  m^k times in kt years
     2× in 5 y  →  4× in 10 y  →  8× in 15 y  →  16× in 20 y
     3× in 4 y  →  9× in 8 y   →  27× in 12 y

SI:  work with the INTEREST, not the multiple
     3× in 12 y  →  interest 2P in 12 y  →  P in 6 y  →  6× needs 5P = 30 y
```

### 4.6 SI is linear — exploit it

Because SI adds the same amount every year:

```
Amount after 3 years = ₹1,560
Amount after 4 years = ₹1,680
                       ────────
Annual interest      = ₹120       ← just subtract

P = 1,560 − 3(120) = ₹1,200
R = 120/1200 × 100 = 10%
```

Two subtractions replace a full simultaneous-equation solve.

### 4.7 The repayment ladder

For "borrows P, repays X at the end of each year" problems, march year by year:

```
Balance_new = (Balance_old × multiplier) − repayment
```

> Borrows ₹5,000 at 10%; repays ₹2,000 at the end of years 1 and 2.
```
End Y1:  5,000 × 1.1 = 5,500;  pay 2,000  →  3,500
End Y2:  3,500 × 1.1 = 3,850;  pay 2,000  →  1,850
End Y3:  1,850 × 1.1 = 2,035   ← final payment
```

### 4.8 Sanity checks

```
✓ CI ≥ SI always (equal only for n = 1)
✓ CI − SI grows rapidly with n and R
✓ More frequent compounding ⇒ MORE interest
✓ To reverse a CI amount, DIVIDE — never subtract the percentage
✓ Depreciation multiplier < 1; growth multiplier > 1
✓ SI: interest is identical every year. CI: interest grows every year.
```

---

## 5. Solved Examples

### Example 1 — Direct simple interest

**Q.** Find the simple interest on ₹7,500 at 8% per annum for 4 years, and the amount.

**Step 1 — Apply the SI formula.**
$$SI = \frac{P \times R \times T}{100} = \frac{7500 \times 8 \times 4}{100}$$

**Step 2 — Simplify before multiplying.**
$$= 75 \times 8 \times 4 = 2{,}400$$

**Step 3 — Amount.**
$$A = 7{,}500 + 2{,}400 = ₹9{,}900$$

**Answer: SI = ₹2,400; Amount = ₹9,900**

> **Speed tip:** dividing P by 100 first turns the calculation into simple multiplication. 7,500/100 = 75, then × 8 × 4.

---

### Example 2 — Reverse simple interest

**Q.** What sum of money will produce ₹1,260 as simple interest in 3 years at 7% per annum?

**Step 1 — Rearrange the formula.**
$$P = \frac{100 \times SI}{R \times T}$$

**Step 2 — Substitute.**
$$P = \frac{100 \times 1260}{7 \times 3} = \frac{126000}{21}$$

**Step 3 — Compute.**
$$= 6{,}000$$

**Answer: ₹6,000**

**Verification:** SI = (6000 × 7 × 3)/100 = ₹1,260 ✓

---

### Example 3 — Compound interest, computed two ways

**Q.** Find the compound interest on ₹12,000 at 10% per annum for 3 years, compounded annually.

**Method A — the CI ladder (recommended under time pressure):**
```
Year 1:  12,000 + 1,200  =  13,200
Year 2:  13,200 + 1,320  =  14,520
Year 3:  14,520 + 1,452  =  15,972
```
$$CI = 15{,}972 - 12{,}000 = ₹3{,}972$$

**Method B — the formula:**
$$A = 12{,}000 \times (1.10)^3 = 12{,}000 \times 1.331 = ₹15{,}972$$
$$CI = ₹3{,}972$$

**Answer: CI = ₹3,972 (Amount = ₹15,972)**

**Comparison with SI:** SI would be (12,000 × 10 × 3)/100 = ₹3,600.
Difference = 3,972 − 3,600 = **₹372**.

Check against the 3-year difference formula:
$$P\left(\frac{R}{100}\right)^2\left(3+\frac{R}{100}\right) = 12000(0.01)(3.1) = 372 \checkmark$$

---

### Example 4 — Reverse compound interest

**Q.** A sum of money amounts to ₹9,261 in 3 years at 5% per annum compound interest. Find the principal.

**Step 1 — Write the relation.**
$$A = P(1.05)^3$$

**Step 2 — Recognise the multiplier.**
$$(1.05)^3 = 1.157625$$

**Step 3 — Divide (never subtract).**
$$P = \frac{9261}{1.157625} = ₹8{,}000$$

**Cleaner arithmetic using fractions:**
$$1.05 = \frac{21}{20} \implies (1.05)^3 = \frac{9261}{8000}$$
$$P = 9261 \times \frac{8000}{9261} = ₹8{,}000$$

**Answer: ₹8,000**

> **Recognise 9,261.** It equals 21³, and 8,000 = 20³. Whenever you see 9,261 in a CI question, 5% and 3 years is almost certainly involved.

---

### Example 5 — The CI − SI difference (run backwards)

**Q.** The difference between compound interest and simple interest on a certain sum for 2 years at 8% per annum is ₹128. Find the sum.

**Step 1 — Apply the 2-year difference formula.**
$$CI - SI = P\left(\frac{R}{100}\right)^2$$

**Step 2 — Substitute the known values.**
$$128 = P\left(\frac{8}{100}\right)^2 = P \times 0.0064$$

**Step 3 — Solve.**
$$P = \frac{128}{0.0064} = ₹20{,}000$$

**Full verification:**
- SI = (20,000 × 8 × 2)/100 = ₹3,200
- CI: 20,000 × (1.08)² = 20,000 × 1.1664 = ₹23,328 ⇒ CI = ₹3,328
- Difference = 3,328 − 3,200 = **₹128** ✓

**Answer: ₹20,000**

> **Intuition:** the ₹128 is precisely the interest earned in year 2 on year 1's interest of ₹1,600. Indeed, 8% of ₹1,600 = ₹128 ✓

---

### Example 6 — Non-annual compounding

**Q.** Find the compound interest on ₹10,000 at 20% per annum for 1 year, compounded half-yearly.

**Step 1 — Adjust the rate and the number of periods.**
Half-yearly compounding means:
$$\text{Rate per period} = \frac{20}{2} = 10\%$$
$$\text{Number of periods} = 1 \times 2 = 2$$

**Step 2 — Apply the formula.**
$$A = 10{,}000 \times (1.10)^2 = 10{,}000 \times 1.21 = ₹12{,}100$$

**Step 3 — Compute the interest.**
$$CI = 12{,}100 - 10{,}000 = ₹2{,}100$$

**Answer: CI = ₹2,100**

**Compare with annual compounding:** 10,000 × 1.20 = ₹12,000 ⇒ CI = ₹2,000.

> **Half-yearly compounding earns ₹100 more** on the same nominal rate. More frequent compounding always wins, because interest starts earning interest sooner.

---

### Example 7 — Doubling and multiplying (CI)

**Q.** A sum of money invested at compound interest doubles itself in 6 years. In how many years will it become 16 times itself?

**Step 1 — Express the target as a power of the known multiple.**
$$16 = 2^4$$

**Step 2 — Apply the compounding rule.**
If a sum becomes *m* times in *t* years, it becomes *m*ᵏ times in *kt* years.

Here m = 2, t = 6, and we need k = 4:
$$\text{Time} = 4 \times 6 = 24 \text{ years}$$

**Verification of the logic:**

| Years | Multiple |
|---|---|
| 6 | 2× |
| 12 | 4× |
| 18 | 8× |
| 24 | **16×** ✓ |

**Answer: 24 years**

> **Contrast with simple interest.** Under SI, doubling in 6 years means the interest equals P in 6 years, so R = 100/6 ≈ 16.67%. To become 16 times, the interest must be 15P, taking 15 × 6 = **90 years** — not 24. Always check which type of interest applies.

---

### Example 8 — Two-part investment

**Q.** A person invests ₹15,000, part at 12% per annum and the rest at 8% per annum simple interest. If the total annual interest is ₹1,480, how much was invested at 12%?

**Step 1 — Define the variable.**
Let ₹*x* be invested at 12%; then ₹(15,000 − x) is invested at 8%.

**Step 2 — Write the interest equation (for one year).**
$$0.12x + 0.08(15{,}000 - x) = 1{,}480$$

**Step 3 — Expand.**
$$0.12x + 1{,}200 - 0.08x = 1{,}480$$
$$0.04x = 280$$

**Step 4 — Solve.**
$$x = \frac{280}{0.04} = ₹7{,}000$$

**Verification:**
- ₹7,000 at 12% = ₹840
- ₹8,000 at 8% = ₹640
- Total = ₹1,480 ✓

**Answer: ₹7,000 at 12%**

**⚡ Alligation cross-check.** The overall rate is 1,480/15,000 = 9.867%. Alligating 8% and 12% around 9.867%:
$$\text{Amount at 8\%} : \text{Amount at 12\%} = (12 - 9.867) : (9.867 - 8) = 2.133 : 1.867 = 8 : 7$$
Splitting ₹15,000 in 8 : 7 gives ₹8,000 and **₹7,000** ✓

---

## 6. Practice Questions

**Instructions:** 50 questions. Easy (1–20), Medium (21–40), Hard (41–50).
Target times: Easy 30 s · Medium 60 s · Hard 90 s.
Full solutions in [Section 7](#7-detailed-solutions).

### 🟢 EASY (Questions 1–20)

**Q1.** Find the simple interest on ₹5,000 at 8% per annum for 3 years.
(a) ₹1,000  (b) ₹1,100  (c) ₹1,200  (d) ₹1,400

**Q2.** Find the simple interest on ₹8,000 at 5% per annum for 2 years.
(a) ₹700  (b) ₹800  (c) ₹900  (d) ₹1,000

**Q3.** Find the amount on ₹4,000 at 10% per annum simple interest for 3 years.
(a) ₹5,000  (b) ₹5,200  (c) ₹5,400  (d) ₹5,600

**Q4.** At what rate will ₹2,000 yield ₹400 as simple interest in 4 years?
(a) 4%  (b) 5%  (c) 6%  (d) 8%

**Q5.** In how many years will ₹6,000 yield ₹1,500 as simple interest at 5% per annum?
(a) 4 years  (b) 5 years  (c) 6 years  (d) 7 years

**Q6.** What principal will yield ₹900 as simple interest at 6% per annum in 3 years?
(a) ₹4,500  (b) ₹5,000  (c) ₹5,500  (d) ₹6,000

**Q7.** Find the compound interest on ₹1,000 at 10% per annum for 2 years.
(a) ₹200  (b) ₹210  (c) ₹220  (d) ₹230

**Q8.** Find the compound interest on ₹5,000 at 10% per annum for 2 years.
(a) ₹1,000  (b) ₹1,050  (c) ₹1,100  (d) ₹1,150

**Q9.** Find the amount on ₹8,000 at 5% per annum compound interest for 2 years.
(a) ₹8,720  (b) ₹8,800  (c) ₹8,820  (d) ₹8,880

**Q10.** Find the simple interest on ₹1,200 at 12% per annum for 6 months.
(a) ₹66  (b) ₹72  (c) ₹78  (d) ₹144

**Q11.** In how many years will ₹2,000 amount to ₹2,500 at 5% per annum simple interest?
(a) 4 years  (b) 5 years  (c) 6 years  (d) 8 years

**Q12.** Find the difference between compound interest and simple interest on ₹10,000 at 10% per annum for 2 years.
(a) ₹100  (b) ₹110  (c) ₹120  (d) ₹200

**Q13.** Find the simple interest on ₹15,000 at 8% per annum for 2½ years.
(a) ₹2,400  (b) ₹2,800  (c) ₹3,000  (d) ₹3,600

**Q14.** At what rate will ₹5,000 yield ₹750 as simple interest in 3 years?
(a) 4%  (b) 5%  (c) 6%  (d) 7.5%

**Q15.** Find the compound interest on ₹4,000 at 20% per annum for 2 years.
(a) ₹1,600  (b) ₹1,680  (c) ₹1,760  (d) ₹1,840

**Q16.** A sum doubles itself in 8 years at simple interest. Find the rate per annum.
(a) 10%  (b) 12%  (c) 12.5%  (d) 15%

**Q17.** Find the simple interest on ₹3,000 at 10% per annum for 1 year.
(a) ₹250  (b) ₹300  (c) ₹330  (d) ₹350

**Q18.** Find the amount on ₹2,000 at 10% per annum compound interest for 3 years.
(a) ₹2,420  (b) ₹2,600  (c) ₹2,662  (d) ₹2,700

**Q19.** What sum yields ₹200 as simple interest in 2 years at 4% per annum?
(a) ₹2,000  (b) ₹2,250  (c) ₹2,500  (d) ₹3,000

**Q20.** Find the compound interest on ₹6,250 at 4% per annum for 2 years.
(a) ₹480  (b) ₹500  (c) ₹510  (d) ₹520

---

### 🟡 MEDIUM (Questions 21–40)

**Q21.** A sum amounts to ₹6,050 in 2 years at 10% per annum compound interest. Find the principal.
(a) ₹4,500  (b) ₹4,800  (c) ₹5,000  (d) ₹5,500

**Q22.** The difference between compound interest and simple interest on a sum for 2 years at 5% per annum is ₹25. Find the sum.
(a) ₹8,000  (b) ₹9,000  (c) ₹10,000  (d) ₹12,000

**Q23.** A sum of money doubles itself in 5 years at compound interest. In how many years will it become 8 times?
(a) 10 years  (b) 15 years  (c) 20 years  (d) 40 years

**Q24.** A sum of money becomes three times itself in 12 years at simple interest. Find the rate per annum.
(a) 12½%  (b) 16⅔%  (c) 20%  (d) 25%

**Q25.** Find the compound interest on ₹10,000 at 10% per annum for 1½ years, compounded half-yearly.
(a) ₹1,500  (b) ₹1,525.50  (c) ₹1,576.25  (d) ₹1,610

**Q26.** The simple interest on a sum for 3 years at 8% per annum is ₹1,200. Find the compound interest on the same sum at the same rate for 2 years.
(a) ₹800  (b) ₹816  (c) ₹832  (d) ₹864

**Q27.** A sum becomes ₹1,352 in 2 years at 4% per annum compound interest. Find the sum.
(a) ₹1,200  (b) ₹1,250  (c) ₹1,275  (d) ₹1,300

**Q28.** At what rate per annum will ₹1,200 amount to ₹1,348.32 in 2 years at compound interest?
(a) 5%  (b) 6%  (c) 6.5%  (d) 8%

**Q29.** Find the difference between compound interest and simple interest on ₹8,000 for 3 years at 5% per annum.
(a) ₹58  (b) ₹61  (c) ₹64  (d) ₹68

**Q30.** ₹12,000 is invested partly at 10% and partly at 8% per annum simple interest. If the total annual interest is ₹1,120, find the sum invested at 10%.
(a) ₹6,000  (b) ₹7,000  (c) ₹8,000  (d) ₹9,000

**Q31.** Find the compound interest on ₹16,000 at 20% per annum for 1 year, compounded half-yearly.
(a) ₹3,200  (b) ₹3,360  (c) ₹3,520  (d) ₹3,600

**Q32.** A sum at simple interest amounts to ₹1,560 in 3 years and ₹1,680 in 4 years. Find the sum and the rate.
(a) ₹1,100, 12%  (b) ₹1,200, 10%  (c) ₹1,250, 9.6%  (d) ₹1,300, 8%

**Q33.** In what time will ₹4,000 amount to ₹4,630.50 at 5% per annum compound interest?
(a) 2 years  (b) 2½ years  (c) 3 years  (d) 4 years

**Q34.** The population of a town increases by 10% annually. If the present population is 24,200, what was it two years ago?
(a) 18,000  (b) 19,500  (c) 20,000  (d) 22,000

**Q35.** A man borrows ₹5,000 at 10% per annum compound interest and repays ₹2,000 at the end of each of the first two years. How much must he pay at the end of the third year to clear the debt?
(a) ₹1,850  (b) ₹1,950  (c) ₹2,035  (d) ₹2,150

**Q36.** Find the simple interest on ₹7,500 at 6% per annum for 73 days (take a year as 365 days).
(a) ₹80  (b) ₹90  (c) ₹100  (d) ₹110

**Q37.** The compound interest on a sum for the second year is ₹1,320 and for the third year is ₹1,452. Find the rate of interest.
(a) 8%  (b) 10%  (c) 11%  (d) 12%

**Q38.** A sum of money at simple interest amounts to 3 times itself in 16 years. In how many years will it become 6 times itself?
(a) 32 years  (b) 36 years  (c) 40 years  (d) 48 years

**Q39.** What equal annual instalment will discharge a debt of ₹1,092 due in 3 years at 12% per annum simple interest?
(a) ₹300  (b) ₹325  (c) ₹350  (d) ₹364

**Q40.** Find the difference between compound interest (compounded annually) and simple interest on ₹5,000 for 2 years at 8% per annum.
(a) ₹28  (b) ₹32  (c) ₹36  (d) ₹40

---

### 🔴 HARD (Questions 41–50)

**Q41.** The difference between compound interest and simple interest on a certain sum for 3 years at 10% per annum is ₹93. Find the sum.
(a) ₹2,500  (b) ₹3,000  (c) ₹3,500  (d) ₹4,000

**Q42.** A sum of money invested at compound interest amounts to ₹800 in 3 years and ₹882 in 5 years. Find the rate of interest per annum.
(a) 4%  (b) 5%  (c) 6%  (d) 8%

**Q43.** A man invests ₹10,000 — part at 8% and the rest at 10% per annum simple interest. After 2 years the total interest received is ₹1,800. Find the amount invested at 8%.
(a) ₹4,000  (b) ₹5,000  (c) ₹6,000  (d) ₹7,000

**Q44.** What sum of money will amount to ₹2,662 in 3 years at 10% per annum compound interest?
(a) ₹1,800  (b) ₹2,000  (c) ₹2,200  (d) ₹2,400

**Q45.** ₹6,000 is lent at 5% per annum for the first 2 years, 8% for the next 3 years and 10% for the period beyond. If the total simple interest is ₹4,440, find the total period of the loan.
(a) 7 years  (b) 8 years  (c) 9 years  (d) 10 years

**Q46.** The compound interest on a certain sum for 2 years is ₹1,050 and the simple interest for the same period is ₹1,000. Find the sum.
(a) ₹4,000  (b) ₹4,500  (c) ₹5,000  (d) ₹5,500

**Q47.** A sum of money placed at compound interest doubles itself in 4 years. In how many years will it amount to 16 times itself?
(a) 8 years  (b) 12 years  (c) 16 years  (d) 20 years

**Q48.** Find the compound interest on ₹20,000 for 2 years if the rate is 10% for the first year and 12% for the second year.
(a) ₹4,400  (b) ₹4,520  (c) ₹4,640  (d) ₹4,800

**Q49.** The simple interest on a sum for 2 years is ₹1,500 and the compound interest for the same period at the same rate is ₹1,575. Find the sum.
(a) ₹6,500  (b) ₹7,000  (c) ₹7,500  (d) ₹8,000

**Q50.** A machine depreciates at 10% per annum. If its value after 3 years is ₹36,450, find its original cost.
(a) ₹45,000  (b) ₹48,000  (c) ₹50,000  (d) ₹54,000

---

## 7. Detailed Solutions

### 🟢 EASY — Solutions 1–20

---

**Q1. SI on ₹5,000 at 8% for 3 years. → (c) ₹1,200**

**Formula used:** SI = PRT/100

$$SI = \frac{5000 \times 8 \times 3}{100} = 50 \times 8 \times 3 = 1{,}200$$

**Answer: (c) ₹1,200**

---

**Q2. SI on ₹8,000 at 5% for 2 years. → (b) ₹800**

$$SI = \frac{8000 \times 5 \times 2}{100} = 80 \times 10 = 800$$

**Answer: (b) ₹800**

---

**Q3. Amount on ₹4,000 at 10% SI for 3 years. → (b) ₹5,200**

**Step 1 — Compute the interest.**
$$SI = \frac{4000 \times 10 \times 3}{100} = 1{,}200$$

**Step 2 — Add to the principal.**
$$A = 4{,}000 + 1{,}200 = ₹5{,}200$$

**Answer: (b) ₹5,200**

---

**Q4. P = ₹2,000, SI = ₹400, T = 4 years. Rate? → (b) 5%**

**Formula used:** R = 100 × SI/(P × T)

$$R = \frac{100 \times 400}{2000 \times 4} = \frac{40{,}000}{8{,}000} = 5\%$$

**Answer: (b) 5%**

---

**Q5. P = ₹6,000, R = 5%, SI = ₹1,500. Time? → (b) 5 years**

**Formula used:** T = 100 × SI/(P × R)

$$T = \frac{100 \times 1500}{6000 \times 5} = \frac{150{,}000}{30{,}000} = 5 \text{ years}$$

**Answer: (b) 5 years**

---

**Q6. SI = ₹900, R = 6%, T = 3 years. Principal? → (b) ₹5,000**

**Formula used:** P = 100 × SI/(R × T)

$$P = \frac{100 \times 900}{6 \times 3} = \frac{90{,}000}{18} = ₹5{,}000$$

**Answer: (b) ₹5,000**

---

**Q7. CI on ₹1,000 at 10% for 2 years. → (b) ₹210**

**Method — the ladder:**
```
Year 1:  1,000 + 100  =  1,100
Year 2:  1,100 + 110  =  1,210
```
$$CI = 1{,}210 - 1{,}000 = ₹210$$

**Formula check:** 1000 × (1.1)² = 1000 × 1.21 = 1,210 ✓

> **Note:** SI would be ₹200. The extra ₹10 is the 10% earned in year 2 on year 1's ₹100 of interest.

**Answer: (b) ₹210**

---

**Q8. CI on ₹5,000 at 10% for 2 years. → (b) ₹1,050**

$$A = 5{,}000 \times 1.21 = ₹6{,}050$$
$$CI = 6{,}050 - 5{,}000 = ₹1{,}050$$

**Answer: (b) ₹1,050**

---

**Q9. Amount on ₹8,000 at 5% CI for 2 years. → (c) ₹8,820**

$$A = 8{,}000 \times (1.05)^2 = 8{,}000 \times 1.1025 = ₹8{,}820$$

**Ladder check:**
```
Year 1:  8,000 + 400  =  8,400
Year 2:  8,400 + 420  =  8,820  ✓
```

**Answer: (c) ₹8,820**

---

**Q10. SI on ₹1,200 at 12% for 6 months. → (b) ₹72**

**Step 1 — Convert the time to years.**
$$6 \text{ months} = 0.5 \text{ years}$$

**Step 2 — Apply the formula.**
$$SI = \frac{1200 \times 12 \times 0.5}{100} = 12 \times 12 \times 0.5 = 72$$

> **Trap:** ignoring the time conversion gives ₹144 (option d) — the interest for a full year.

**Answer: (b) ₹72**

---

**Q11. ₹2,000 → ₹2,500 at 5% SI. Time? → (b) 5 years**

**Step 1 — Interest required.**
$$2{,}500 - 2{,}000 = ₹500$$

**Step 2 — Solve for T.**
$$T = \frac{100 \times 500}{2000 \times 5} = \frac{50{,}000}{10{,}000} = 5 \text{ years}$$

**Answer: (b) 5 years**

---

**Q12. CI − SI on ₹10,000 at 10% for 2 years. → (a) ₹100**

**Formula used:** CI − SI (2 years) = P(R/100)²

$$= 10{,}000 \times \left(\frac{10}{100}\right)^2 = 10{,}000 \times 0.01 = ₹100$$

**Verification:**
- SI = (10,000 × 10 × 2)/100 = ₹2,000
- CI = 10,000 × 1.21 − 10,000 = ₹2,100
- Difference = ₹100 ✓

**Answer: (a) ₹100**

---

**Q13. SI on ₹15,000 at 8% for 2½ years. → (c) ₹3,000**

$$SI = \frac{15000 \times 8 \times 2.5}{100} = 150 \times 8 \times 2.5 = 3{,}000$$

**Answer: (c) ₹3,000**

---

**Q14. P = ₹5,000, SI = ₹750, T = 3 years. Rate? → (b) 5%**

$$R = \frac{100 \times 750}{5000 \times 3} = \frac{75{,}000}{15{,}000} = 5\%$$

**Answer: (b) 5%**

---

**Q15. CI on ₹4,000 at 20% for 2 years. → (c) ₹1,760**

$$A = 4{,}000 \times (1.20)^2 = 4{,}000 \times 1.44 = ₹5{,}760$$
$$CI = 5{,}760 - 4{,}000 = ₹1{,}760$$

**Ladder check:**
```
Year 1:  4,000 + 800  =  4,800
Year 2:  4,800 + 960  =  5,760  ✓
```

**Answer: (c) ₹1,760**

---

**Q16. Sum doubles in 8 years at SI. Rate? → (c) 12.5%**

**Concept:** doubling means the interest earned equals the principal.

$$SI = P \implies \frac{P \times R \times 8}{100} = P$$
$$\frac{8R}{100} = 1 \implies R = 12.5\%$$

**Formula shortcut:** for SI doubling, R = 100/T = 100/8 = **12.5%**

**Answer: (c) 12.5%**

---

**Q17. SI on ₹3,000 at 10% for 1 year. → (b) ₹300**

$$SI = \frac{3000 \times 10 \times 1}{100} = 300$$

**Answer: (b) ₹300**

---

**Q18. Amount on ₹2,000 at 10% CI for 3 years. → (c) ₹2,662**

$$A = 2{,}000 \times (1.10)^3 = 2{,}000 \times 1.331 = ₹2{,}662$$

**Ladder check:**
```
Year 1:  2,000 + 200  =  2,200
Year 2:  2,200 + 220  =  2,420
Year 3:  2,420 + 242  =  2,662  ✓
```

**Answer: (c) ₹2,662**

---

**Q19. SI = ₹200 in 2 years at 4%. Sum? → (c) ₹2,500**

$$P = \frac{100 \times 200}{4 \times 2} = \frac{20{,}000}{8} = ₹2{,}500$$

**Answer: (c) ₹2,500**

---

**Q20. CI on ₹6,250 at 4% for 2 years. → (c) ₹510**

$$A = 6{,}250 \times (1.04)^2 = 6{,}250 \times 1.0816 = ₹6{,}760$$
$$CI = 6{,}760 - 6{,}250 = ₹510$$

**Ladder check:**
```
Year 1:  6,250 + 250  =  6,500
Year 2:  6,500 + 260  =  6,760  ✓
```

**Answer: (c) ₹510**

---

### 🟡 MEDIUM — Solutions 21–40

---

**Q21. Amounts to ₹6,050 in 2 years at 10% CI. Principal? → (c) ₹5,000**

**Formula used:** P = A/(1 + R/100)ⁿ

$$P = \frac{6050}{(1.10)^2} = \frac{6050}{1.21} = ₹5{,}000$$

**Verification:** 5,000 × 1.21 = ₹6,050 ✓

> **Trap:** subtracting instead of dividing. 6,050 − 21% = ₹4,779.50 — wrong. Reversing a compound multiplier requires division.

**Answer: (c) ₹5,000**

---

**Q22. CI − SI for 2 years at 5% is ₹25. Sum? → (c) ₹10,000**

**Formula used:** CI − SI (2 years) = P(R/100)²

$$25 = P\left(\frac{5}{100}\right)^2 = P \times 0.0025$$
$$P = \frac{25}{0.0025} = ₹10{,}000$$

**Verification:**
- SI = (10,000 × 5 × 2)/100 = ₹1,000
- CI = 10,000 × 1.1025 − 10,000 = ₹1,025
- Difference = ₹25 ✓

**Answer: (c) ₹10,000**

---

**Q23. Doubles in 5 years at CI. Time to become 8 times? → (b) 15 years**

**Step 1 — Express 8 as a power of 2.**
$$8 = 2^3$$

**Step 2 — Apply the compounding rule.**
$$\text{Time} = 3 \times 5 = 15 \text{ years}$$

**Verification:**

| Years | Multiple |
|---|---|
| 5 | 2× |
| 10 | 4× |
| 15 | **8×** ✓ |

> **Trap:** answering 20 years by reasoning "2× takes 5, so 8× takes 4 × 5". Under compound growth the multiples *multiply*, not add — 2 × 2 × 2 = 8 requires only three doubling periods.

**Answer: (b) 15 years**

---

**Q24. Becomes 3 times in 12 years at SI. Rate? → (b) 16⅔%**

**Step 1 — Convert the multiple to interest.**
Tripling means the interest earned = 2P.

**Step 2 — Apply the SI formula.**
$$\frac{P \times R \times 12}{100} = 2P$$
$$\frac{12R}{100} = 2 \implies R = \frac{200}{12} = 16\tfrac{2}{3}\%$$

**Formula shortcut:** R = 100(m − 1)/T = 100(3 − 1)/12 = 200/12 = **16⅔%**

**Answer: (b) 16⅔%**

---

**Q25. CI on ₹10,000 at 10% for 1½ years, compounded half-yearly. → (c) ₹1,576.25**

**Step 1 — Adjust the rate and periods.**
$$\text{Rate per half-year} = \frac{10}{2} = 5\%$$
$$\text{Number of periods} = 1.5 \times 2 = 3$$

**Step 2 — Apply the formula.**
$$A = 10{,}000 \times (1.05)^3 = 10{,}000 \times 1.157625 = ₹11{,}576.25$$

**Step 3 — Compute the interest.**
$$CI = 11{,}576.25 - 10{,}000 = ₹1{,}576.25$$

**Ladder check:**
```
Half-year 1:  10,000 + 500     =  10,500
Half-year 2:  10,500 + 525     =  11,025
Half-year 3:  11,025 + 551.25  =  11,576.25  ✓
```

**Answer: (c) ₹1,576.25**

---

**Q26. SI for 3 years at 8% is ₹1,200. CI for 2 years at 8%? → (c) ₹832**

**Step 1 — Recover the principal from the SI information.**
$$P = \frac{100 \times 1200}{8 \times 3} = \frac{120{,}000}{24} = ₹5{,}000$$

**Step 2 — Compute the 2-year CI on the same principal.**
$$A = 5{,}000 \times (1.08)^2 = 5{,}000 \times 1.1664 = ₹5{,}832$$
$$CI = 5{,}832 - 5{,}000 = ₹832$$

**Ladder check:**
```
Year 1:  5,000 + 400  =  5,400
Year 2:  5,400 + 432  =  5,832  ✓
```

**Cross-check with the difference formula:** 2-year SI = ₹800; CI − SI = 5000(0.08)² = ₹32 ⇒ CI = 800 + 32 = **₹832** ✓

**Answer: (c) ₹832**

---

**Q27. Becomes ₹1,352 in 2 years at 4% CI. Sum? → (b) ₹1,250**

$$P = \frac{1352}{(1.04)^2} = \frac{1352}{1.0816} = ₹1{,}250$$

**Cleaner arithmetic:** (1.04)² = 1.0816 = 10816/10000. So
$$P = 1352 \times \frac{10000}{10816} = 1{,}250$$

**Verification:** 1,250 × 1.04 = 1,300; 1,300 × 1.04 = ₹1,352 ✓

**Answer: (b) ₹1,250**

---

**Q28. ₹1,200 → ₹1,348.32 in 2 years at CI. Rate? → (b) 6%**

**Step 1 — Compute the growth factor.**
$$\frac{1348.32}{1200} = 1.1236$$

**Step 2 — Recognise this as a square.**
$$1.1236 = (1.06)^2$$

*(Because 106² = 11,236.)*

**Step 3 — Read off the rate.**
$$R = 6\%$$

**Verification:**
```
Year 1:  1,200 + 72     =  1,272
Year 2:  1,272 + 76.32  =  1,348.32  ✓
```

**Answer: (b) 6%**

---

**Q29. CI − SI on ₹8,000 for 3 years at 5%. → (b) ₹61**

**Method 1 — Direct computation.**
$$SI = \frac{8000 \times 5 \times 3}{100} = ₹1{,}200$$
$$A_{CI} = 8{,}000 \times (1.05)^3 = 8{,}000 \times 1.157625 = ₹9{,}261$$
$$CI = 9{,}261 - 8{,}000 = ₹1{,}261$$
$$\text{Difference} = 1{,}261 - 1{,}200 = ₹61$$

**Method 2 — The 3-year difference formula.**
$$P\left(\frac{R}{100}\right)^2\left(3 + \frac{R}{100}\right) = 8000 \times (0.05)^2 \times (3.05)$$
$$= 8000 \times 0.0025 \times 3.05 = 20 \times 3.05 = ₹61 \checkmark$$

**Answer: (b) ₹61**

---

**Q30. ₹12,000 split at 10% and 8%; total interest ₹1,120. Amount at 10%? → (c) ₹8,000**

**Step 1 — Define the variable.**
Let ₹*x* be invested at 10%; then ₹(12,000 − x) at 8%.

**Step 2 — Write the annual-interest equation.**
$$0.10x + 0.08(12{,}000 - x) = 1{,}120$$

**Step 3 — Expand and solve.**
$$0.10x + 960 - 0.08x = 1{,}120$$
$$0.02x = 160$$
$$x = ₹8{,}000$$

**Verification:**
- ₹8,000 at 10% = ₹800
- ₹4,000 at 8% = ₹320
- Total = ₹1,120 ✓

**⚡ Alligation check:** overall rate = 1,120/12,000 = 9⅓%.
$$\text{At 8\%} : \text{At 10\%} = \left(10 - 9\tfrac{1}{3}\right) : \left(9\tfrac{1}{3} - 8\right) = \tfrac{2}{3} : \tfrac{4}{3} = 1 : 2$$
Splitting ₹12,000 in 1 : 2 gives ₹4,000 and **₹8,000** ✓

**Answer: (c) ₹8,000**

---

**Q31. CI on ₹16,000 at 20% for 1 year, compounded half-yearly. → (b) ₹3,360**

**Step 1 — Adjust the rate and periods.**
$$\text{Rate per half-year} = \frac{20}{2} = 10\%, \qquad \text{Periods} = 2$$

**Step 2 — Apply the formula.**
$$A = 16{,}000 \times (1.10)^2 = 16{,}000 \times 1.21 = ₹19{,}360$$

**Step 3 — Interest.**
$$CI = 19{,}360 - 16{,}000 = ₹3{,}360$$

> **Compare with annual compounding:** 16,000 × 1.20 = ₹19,200 ⇒ CI = ₹3,200. Half-yearly compounding earns **₹160 more** on the same nominal rate.

**Answer: (b) ₹3,360**

---

**Q32. SI: amounts to ₹1,560 in 3 years, ₹1,680 in 4 years. Sum and rate? → (b) ₹1,200, 10%**

**Step 1 — Exploit the linearity of SI.**
The only difference between the two amounts is one extra year of interest:
$$\text{Annual interest} = 1{,}680 - 1{,}560 = ₹120$$

**Step 2 — Work back to the principal.**
Three years of interest = 3 × 120 = ₹360.
$$P = 1{,}560 - 360 = ₹1{,}200$$

**Step 3 — Find the rate.**
$$R = \frac{120}{1200} \times 100 = 10\%$$

**Verification:**
- SI for 3 years = (1,200 × 10 × 3)/100 = ₹360 ⇒ Amount = ₹1,560 ✓
- SI for 4 years = ₹480 ⇒ Amount = ₹1,680 ✓

**Answer: (b) ₹1,200, 10%**

---

**Q33. ₹4,000 → ₹4,630.50 at 5% CI. Time? → (c) 3 years**

**Step 1 — Compute the growth factor.**
$$\frac{4630.50}{4000} = 1.157625$$

**Step 2 — Recognise the power.**
$$1.157625 = (1.05)^3$$

**Step 3 — Read off the time.**
$$n = 3 \text{ years}$$

**Verification (ladder):**
```
Year 1:  4,000 + 200     =  4,200
Year 2:  4,200 + 210     =  4,410
Year 3:  4,410 + 220.50  =  4,630.50  ✓
```

**Answer: (c) 3 years**

---

**Q34. Population grows 10% annually; now 24,200. Two years ago? → (c) 20,000**

**Formula used:** P_past = P_now / (1 + R/100)ⁿ

$$P = \frac{24{,}200}{(1.10)^2} = \frac{24{,}200}{1.21} = 20{,}000$$

**Verification:** 20,000 × 1.1 = 22,000; 22,000 × 1.1 = 24,200 ✓

> **Trap:** subtracting 21% from 24,200 gives 19,118 — wrong. Reversing compound growth requires division.

**Answer: (c) 20,000**

---

**Q35. Borrows ₹5,000 at 10% CI; repays ₹2,000 at end of years 1 and 2. Final payment? → (c) ₹2,035**

**Method — the repayment ladder.** Apply interest, then subtract the repayment.

**Year 1:**
$$5{,}000 \times 1.10 = ₹5{,}500$$
$$\text{After repayment: } 5{,}500 - 2{,}000 = ₹3{,}500$$

**Year 2:**
$$3{,}500 \times 1.10 = ₹3{,}850$$
$$\text{After repayment: } 3{,}850 - 2{,}000 = ₹1{,}850$$

**Year 3:**
$$1{,}850 \times 1.10 = ₹2{,}035$$

This is the balance owing at the end of year 3, and therefore the final payment.

**Summary table:**

| End of year | Balance + interest | Repayment | Closing balance |
|---|---|---|---|
| 1 | ₹5,500 | ₹2,000 | ₹3,500 |
| 2 | ₹3,850 | ₹2,000 | ₹1,850 |
| 3 | ₹2,035 | **₹2,035** | ₹0 |

**Answer: (c) ₹2,035**

---

**Q36. SI on ₹7,500 at 6% for 73 days. → (b) ₹90**

**Step 1 — Convert days to years.**
$$T = \frac{73}{365} = \frac{1}{5} = 0.2 \text{ years}$$

**Step 2 — Apply the formula.**
$$SI = \frac{7500 \times 6 \times 0.2}{100} = 75 \times 6 \times 0.2 = 90$$

**Answer: (b) ₹90**

> **Note:** 73 days is exactly one-fifth of a 365-day year. Exam-setters choose 73, 146, 219 and 292 days for precisely this reason.

---

**Q37. CI in year 2 = ₹1,320; in year 3 = ₹1,452. Rate? → (b) 10%**

**Concept:** under CI, each year's interest exceeds the previous year's by exactly the rate — because the extra interest is earned on the previous year's interest.

**Formula used:**
$$R = \frac{CI_3 - CI_2}{CI_2} \times 100$$

**Step 1 — Compute the increase.**
$$1{,}452 - 1{,}320 = ₹132$$

**Step 2 — Express as a percentage of the previous year's interest.**
$$\frac{132}{1320} \times 100 = 10\%$$

**Answer: (b) 10%**

> **Why it works:** the ₹132 extra is exactly the interest earned in year 3 on year 2's interest of ₹1,320. So 132 is R% of 1,320.

---

**Q38. SI: becomes 3 times in 16 years. Time to become 6 times? → (c) 40 years**

**Step 1 — Convert the first condition to interest.**
Tripling ⇒ interest earned = 2P over 16 years.
$$\text{Interest of } P \text{ takes } \frac{16}{2} = 8 \text{ years}$$

**Step 2 — Determine the interest needed for 6 times.**
$$6P = P + \text{Interest} \implies \text{Interest} = 5P$$

**Step 3 — Compute the time.**
$$5 \times 8 = 40 \text{ years}$$

**Verification:** R = 100(3−1)/16 = 12.5%. For interest of 5P: T = 100 × 5/12.5 = 40 years ✓

> **Contrast with CI:** under compound interest, 3× in 16 years would give 9× in 32 years — never 6× in a clean number of years. The two regimes behave completely differently.

**Answer: (c) 40 years**

---

**Q39. Annual instalment to clear ₹1,092 in 3 years at 12% SI. → (b) ₹325**

**Step 1 — Understand the structure.**
Three equal instalments of ₹*x* are paid at the end of years 1, 2 and 3. Each instalment, once paid, is credited with simple interest for the remaining years until the debt's due date.

**Step 2 — Compute each instalment's value at the due date.**

| Instalment paid at end of | Earns interest for | Value at due date |
|---|---|---|
| Year 1 | 2 years | $x\left(1 + \frac{24}{100}\right) = 1.24x$ |
| Year 2 | 1 year | $x\left(1 + \frac{12}{100}\right) = 1.12x$ |
| Year 3 | 0 years | $x$ |

**Step 3 — Sum and equate to the debt.**
$$1.24x + 1.12x + x = 1{,}092$$
$$3.36x = 1{,}092$$

**Step 4 — Solve.**
$$x = \frac{1092}{3.36} = ₹325$$

**Verification:**
$$1.24(325) + 1.12(325) + 325 = 403 + 364 + 325 = ₹1{,}092 \checkmark$$

**Answer: (b) ₹325**

---

**Q40. CI − SI on ₹5,000 for 2 years at 8%. → (b) ₹32**

**Formula used:** CI − SI (2 years) = P(R/100)²

$$= 5{,}000 \times \left(\frac{8}{100}\right)^2 = 5{,}000 \times 0.0064 = ₹32$$

**Verification:**
- SI = (5,000 × 8 × 2)/100 = ₹800
- CI = 5,000 × 1.1664 − 5,000 = ₹832
- Difference = ₹32 ✓

**Answer: (b) ₹32**

---

### 🔴 HARD — Solutions 41–50

---

**Q41. CI − SI for 3 years at 10% is ₹93. Sum? → (b) ₹3,000**

**Formula used:** CI − SI (3 years) = P(R/100)²(3 + R/100)

**Step 1 — Substitute R = 10.**
$$P \times (0.10)^2 \times (3 + 0.10) = 93$$
$$P \times 0.01 \times 3.1 = 93$$
$$0.031P = 93$$

**Step 2 — Solve.**
$$P = \frac{93}{0.031} = ₹3{,}000$$

**Full verification:**
- SI = (3,000 × 10 × 3)/100 = ₹900
- CI: 3,000 × (1.1)³ = 3,000 × 1.331 = ₹3,993 ⇒ CI = ₹993
- Difference = 993 − 900 = **₹93** ✓

**Answer: (b) ₹3,000**

> **Learn both difference formulas.** For 2 years it is P(R/100)²; for 3 years the extra factor (3 + R/100) appears. Using the 2-year formula here would give P = 9,300 — a wrong answer that "looks" plausible.

---

**Q42. CI: amounts to ₹800 in 3 years and ₹882 in 5 years. Rate? → (b) 5%**

**Step 1 — Isolate the growth over the intervening 2 years.**
The ₹800 at year 3 grows to ₹882 by year 5 — that is exactly 2 years of compounding:
$$800 \times \left(1 + \frac{R}{100}\right)^2 = 882$$

**Step 2 — Compute the growth factor.**
$$\left(1 + \frac{R}{100}\right)^2 = \frac{882}{800} = 1.1025$$

**Step 3 — Take the square root.**
$$1 + \frac{R}{100} = \sqrt{1.1025} = 1.05$$
$$R = 5\%$$

**Verification:**
```
Year 3:  800
Year 4:  800 × 1.05  =  840
Year 5:  840 × 1.05  =  882  ✓
```

**Answer: (b) 5%**

> **Technique:** you never need the principal. The ratio of two amounts at different times depends only on the rate and the gap between them.

---

**Q43. ₹10,000 split at 8% and 10% SI; 2-year interest ₹1,800. Amount at 8%? → (b) ₹5,000**

**Step 1 — Define the variable.**
Let ₹*x* be at 8%; then ₹(10,000 − x) at 10%.

**Step 2 — Write the 2-year interest equation.**
$$\frac{x \times 8 \times 2}{100} + \frac{(10{,}000 - x) \times 10 \times 2}{100} = 1{,}800$$
$$0.16x + 0.20(10{,}000 - x) = 1{,}800$$

**Step 3 — Expand and solve.**
$$0.16x + 2{,}000 - 0.20x = 1{,}800$$
$$-0.04x = -200$$
$$x = ₹5{,}000$$

**Verification:**
- ₹5,000 at 8% for 2 years = ₹800
- ₹5,000 at 10% for 2 years = ₹1,000
- Total = ₹1,800 ✓

**⚡ Alligation check:** the overall 2-year rate is 1,800/10,000 = 18%, i.e. 9% per annum.
$$\text{At 8\%} : \text{At 10\%} = (10 - 9) : (9 - 8) = 1 : 1$$
So the money splits equally: **₹5,000 each** ✓

**Answer: (b) ₹5,000**

---

**Q44. Amounts to ₹2,662 in 3 years at 10% CI. Sum? → (b) ₹2,000**

$$P = \frac{2662}{(1.10)^3} = \frac{2662}{1.331} = ₹2{,}000$$

**Cleaner with fractions:**
$$1.1 = \frac{11}{10} \implies (1.1)^3 = \frac{1331}{1000}$$
$$P = 2662 \times \frac{1000}{1331} = 2 \times 1000 = ₹2{,}000$$

**Verification (ladder):**
```
Year 1:  2,000 + 200  =  2,200
Year 2:  2,200 + 220  =  2,420
Year 3:  2,420 + 242  =  2,662  ✓
```

**Answer: (b) ₹2,000**

> **Recognise 2,662 and 1,331.** 1,331 = 11³ appears in every 10%-for-3-years problem.

---

**Q45. ₹6,000 at 5% (2 yr), 8% (3 yr), 10% (beyond); total SI ₹4,440. Total period? → (c) 9 years**

**Step 1 — Compute the interest in each fixed phase.**

*Phase 1 — first 2 years at 5%:*
$$\frac{6000 \times 5 \times 2}{100} = ₹600$$

*Phase 2 — next 3 years at 8%:*
$$\frac{6000 \times 8 \times 3}{100} = ₹1{,}440$$

**Step 2 — Interest accumulated in the first 5 years.**
$$600 + 1{,}440 = ₹2{,}040$$

**Step 3 — Interest still required in the 10% phase.**
$$4{,}440 - 2{,}040 = ₹2{,}400$$

**Step 4 — Annual interest at 10%.**
$$\frac{6000 \times 10}{100} = ₹600 \text{ per year}$$

**Step 5 — Years in the final phase.**
$$\frac{2{,}400}{600} = 4 \text{ years}$$

**Step 6 — Total period.**
$$2 + 3 + 4 = 9 \text{ years}$$

**Verification:**

| Phase | Years | Rate | Interest |
|---|---|---|---|
| 1 | 2 | 5% | ₹600 |
| 2 | 3 | 8% | ₹1,440 |
| 3 | 4 | 10% | ₹2,400 |
| **Total** | **9** | | **₹4,440** ✓ |

**Answer: (c) 9 years**

---

**Q46. 2-year CI = ₹1,050; 2-year SI = ₹1,000. Find the sum. → (c) ₹5,000**

**Step 1 — Compute the difference.**
$$CI - SI = 1{,}050 - 1{,}000 = ₹50$$

**Step 2 — Interpret the difference.**
Over 2 years, the difference is exactly the interest earned in year 2 on year 1's interest.

$$\text{One year's SI} = \frac{1{,}000}{2} = ₹500$$

So ₹50 is the interest on ₹500 for one year:
$$R = \frac{50}{500} \times 100 = 10\%$$

**Step 3 — Find the principal from the SI.**
$$P = \frac{100 \times SI}{R \times T} = \frac{100 \times 1000}{10 \times 2} = ₹5{,}000$$

**Full verification:**
- SI = (5,000 × 10 × 2)/100 = ₹1,000 ✓
- CI = 5,000 × 1.21 − 5,000 = ₹1,050 ✓

**Answer: (c) ₹5,000**

> **This two-step template solves every "both CI and SI given" question:**
> 1. Difference ÷ (one year's SI) × 100 = **rate**
> 2. Standard SI formula ⇒ **principal**

---

**Q47. CI: doubles in 4 years. Time to become 16 times? → (c) 16 years**

**Step 1 — Express 16 as a power of 2.**
$$16 = 2^4$$

**Step 2 — Apply the compounding rule.**
Four successive doublings are needed:
$$4 \times 4 = 16 \text{ years}$$

**Verification:**

| Years | Multiple |
|---|---|
| 4 | 2× |
| 8 | 4× |
| 12 | 8× |
| 16 | **16×** ✓ |

**Answer: (c) 16 years**

---

**Q48. CI on ₹20,000: 10% in year 1, 12% in year 2. → (c) ₹4,640**

**Formula used:** with different annual rates, multiply the factors:
$$A = P\left(1 + \frac{R_1}{100}\right)\left(1 + \frac{R_2}{100}\right)$$

**Step 1 — Year 1 at 10%.**
$$20{,}000 \times 1.10 = ₹22{,}000$$

**Step 2 — Year 2 at 12% (applied to ₹22,000, not ₹20,000).**
$$22{,}000 \times 1.12 = ₹24{,}640$$

**Step 3 — Compound interest.**
$$24{,}640 - 20{,}000 = ₹4{,}640$$

**Breakdown:**

| Year | Opening | Rate | Interest | Closing |
|---|---|---|---|---|
| 1 | ₹20,000 | 10% | ₹2,000 | ₹22,000 |
| 2 | ₹22,000 | 12% | ₹2,640 | ₹24,640 |
| | | | **₹4,640** | |

> **Trap:** computing 12% of ₹20,000 = ₹2,400 for year 2 and answering ₹4,400. Under compound interest the second year's rate applies to the *grown* balance.

**Answer: (c) ₹4,640**

---

**Q49. 2-year SI = ₹1,500; 2-year CI = ₹1,575. Find the sum. → (c) ₹7,500**

**Step 1 — Compute the difference.**
$$1{,}575 - 1{,}500 = ₹75$$

**Step 2 — Find one year's simple interest.**
$$\frac{1{,}500}{2} = ₹750$$

**Step 3 — The difference is one year's interest on that amount.**
$$R = \frac{75}{750} \times 100 = 10\%$$

**Step 4 — Recover the principal.**
$$P = \frac{100 \times 1500}{10 \times 2} = \frac{150{,}000}{20} = ₹7{,}500$$

**Full verification:**
- SI = (7,500 × 10 × 2)/100 = ₹1,500 ✓
- CI = 7,500 × 1.21 − 7,500 = 9,075 − 7,500 = ₹1,575 ✓

**Cross-check with the difference formula:**
$$P\left(\frac{R}{100}\right)^2 = 7500 \times 0.01 = ₹75 \checkmark$$

**Answer: (c) ₹7,500**

---

**Q50. Machine depreciates 10% p.a.; worth ₹36,450 after 3 years. Original cost? → (c) ₹50,000**

**Formula used:** A = P(1 − R/100)ⁿ

**Step 1 — Write the equation.**
$$P \times (0.90)^3 = 36{,}450$$

**Step 2 — Compute the depreciation factor.**
$$(0.90)^3 = 0.729$$

**Step 3 — Divide.**
$$P = \frac{36{,}450}{0.729}$$

**Step 4 — Use fractions for clean arithmetic.**
$$0.9 = \frac{9}{10} \implies (0.9)^3 = \frac{729}{1000}$$
$$P = 36{,}450 \times \frac{1000}{729} = 50 \times 1000 = ₹50{,}000$$

**Verification (ladder):**
```
Year 1:  50,000 × 0.9  =  45,000
Year 2:  45,000 × 0.9  =  40,500
Year 3:  40,500 × 0.9  =  36,450  ✓
```

> **Trap:** treating 3 years of 10% depreciation as a flat 30% loss, giving 36,450/0.70 = ₹52,071. Depreciation compounds — the total loss is 1 − 0.729 = **27.1%**, not 30%.

**Answer: (c) ₹50,000**

---

## 8. Quick Revision Sheet

> **One page. Read 48 hours after study, and again the night before the test.**

### Simple Interest

```
SI = PRT/100                 A = P(1 + RT/100)
P = 100·SI/(RT)              R = 100·SI/(PT)              T = 100·SI/(PR)

KEY PROPERTY: the interest is the SAME every year.
    A(4 yrs) − A(3 yrs) = one year's interest → work backwards from there
```

### Compound Interest

```
A = P(1 + R/100)ⁿ            CI = A − P
P = A / (1 + R/100)ⁿ         ← DIVIDE to reverse, never subtract

Half-yearly:  rate R/2,  periods 2n
Quarterly:    rate R/4,  periods 4n
Different rates: A = P(1+R₁/100)(1+R₂/100)…
```

### ⭐ The difference formulas

```
2 years:   CI − SI = P(R/100)²
3 years:   CI − SI = P(R/100)²(3 + R/100)

Per ₹10,000:      R=5% → ₹25  (2y),  ₹76.25 (3y)
                  R=8% → ₹64  (2y),  ₹197.12 (3y)
                  R=10%→ ₹100 (2y),  ₹310   (3y)
```

### Both CI and SI given (2 years)

```
1.  Difference = CI − SI
2.  One year's SI = SI ÷ 2
3.  R = (Difference / One year's SI) × 100
4.  P = 100·SI / (R × 2)
```

### Rate from consecutive CI

```
R = (CI_{n+1} − CI_n) / CI_n × 100

  CI₂ = 1,320 and CI₃ = 1,452  →  132/1320 × 100 = 10%
```

### Multiples

```
CI:  m times in t years  →  m^k times in kt years
     2× in 5y → 4× in 10y → 8× in 15y → 16× in 20y
     2× in 4y → 16× in 16y
     3× in 4y → 9× in 8y

SI:  work with the INTEREST, never the multiple
     doubling rate      R = 100/T
     m-times rate       R = 100(m−1)/T
     3× in 16y → interest 2P in 16y → P in 8y → 6× needs 5P → 40y
```

### Powers to recognise instantly

```
A/P = 1.0816     →  4%,  2 years        A/P = 1.21       →  10%, 2 years
A/P = 1.1025     →  5%,  2 years        A/P = 1.331      →  10%, 3 years
A/P = 1.157625   →  5%,  3 years        A/P = 1.4641     →  10%, 4 years
A/P = 1.1236     →  6%,  2 years        A/P = 1.44       →  20%, 2 years
A/P = 1.1664     →  8%,  2 years        0.729            →  10% depreciation, 3y

Signature numbers:  1,331 = 11³   ·   9,261 = 21³   ·   2,662, 6,050, 4,630.50
```

### Other templates

```
DEPRECIATION       A = P(1 − R/100)ⁿ

REPAYMENT LADDER   Balance_new = (Balance_old × multiplier) − repayment

INSTALMENTS (SI)   x[1 + (n−1)R/100] + … + x[1 + R/100] + x = Debt
                   3 years at 12%:  1.24x + 1.12x + x = 3.36x

TWO-PART INVESTMENT   R₁·x + R₂·(Total − x) = Interest
                      (or use ALLIGATION on the rates)

DAYS → YEARS       73 days = 1/5 yr   ·   146 = 2/5   ·   219 = 3/5   ·   292 = 4/5
```

### Sanity checks

```
✓ CI ≥ SI always; equal only when n = 1
✓ More frequent compounding ⇒ MORE interest
✓ Reverse compound growth by DIVIDING
✓ SI interest is flat; CI interest grows each year
✓ Depreciation over n years ≠ n × R%  (10% for 3 yrs = 27.1%, not 30%)
```

---

## 9. Common Mistakes

| # | Mistake | Example | Correction |
|---|---|---|---|
| 1 | **Reversing CI by subtracting** | A = ₹6,050 at 10% for 2y ⇒ 6,050 − 21% | Divide: 6,050/1.21 = ₹5,000 |
| 2 | **Wrong difference formula for 3 years** | Using P(R/100)² for a 3-year gap | Use P(R/100)²(3 + R/100) |
| 3 | **CI multiples added, not multiplied** | 2× in 5y ⇒ 8× in 5 × 4 = 20y | 8 = 2³ ⇒ 3 × 5 = 15 years |
| 4 | **CI rule applied to SI** | SI: 3× in 16y ⇒ 9× in 32y | SI is linear — work with the interest |
| 5 | **Compounding frequency ignored** | Half-yearly at 10% for 1.5y ⇒ (1.10)^1.5 | Rate 5%, periods 3 ⇒ (1.05)³ |
| 6 | **Year-2 rate applied to the original P** | 12% of ₹20,000 in year 2 | 12% of the *grown* ₹22,000 |
| 7 | **Time units not converted** | 6 months entered as 6 | 6 months = 0.5 years |
| 8 | **Depreciation treated as linear** | 10% for 3 years ⇒ 30% total | 1 − 0.729 = 27.1% |
| 9 | **Instalment interest omitted** | ₹1,092 ÷ 3 = ₹364 | Earlier instalments earn interest: ₹325 |
| 10 | **Rate per period vs per annum confused** | Quarterly at 12% ⇒ using 12% | Use 3% per quarter |
| 11 | **Amount reported when interest is asked** | Giving ₹6,050 instead of ₹1,050 | CI = A − P |
| 12 | **CI − SI difference mis-scaled** | Difference for 2y used for 3y data | Check the number of years in the question |

---

## Practice Answer Key

| Q | Ans | Q | Ans | Q | Ans | Q | Ans | Q | Ans |
|---|---|---|---|---|---|---|---|---|---|
| 1 | c | 11 | b | 21 | c | 31 | b | 41 | b |
| 2 | b | 12 | a | 22 | c | 32 | b | 42 | b |
| 3 | b | 13 | c | 23 | b | 33 | c | 43 | b |
| 4 | b | 14 | b | 24 | b | 34 | c | 44 | b |
| 5 | b | 15 | c | 25 | c | 35 | c | 45 | c |
| 6 | b | 16 | c | 26 | c | 36 | b | 46 | c |
| 7 | b | 17 | b | 27 | b | 37 | b | 47 | c |
| 8 | b | 18 | c | 28 | b | 38 | c | 48 | c |
| 9 | c | 19 | c | 29 | b | 39 | b | 49 | c |
| 10 | b | 20 | c | 30 | c | 40 | b | 50 | c |

**Scoring guide:** 45+/50 → strong. 35–44 → solid; memorise the two difference formulas and the power table. Below 35 → re-read Sections 2.5, 2.8 and 4.2, then redo the Medium set.

---

**⬅️ Back:** [Topic 6 — Time, Speed & Distance](06-time-speed-distance.md) · **➡️ Next:** [Topic 8 — Number System, LCM & HCF](08-number-system-lcm-hcf.md)
