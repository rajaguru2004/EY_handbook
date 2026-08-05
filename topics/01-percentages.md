# Topic 1 — Percentages

### EY Placement Aptitude Handbook · Priority Rank #2 · 🔴 Critical

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

**Weightage:** 12–15% of the quantitative section (1–2 direct questions), **plus** it is the underlying skill in:

| Also needed for | How |
|---|---|
| Data Interpretation | Nearly every DI question is a percentage question in disguise |
| Profit & Loss | Profit% and loss% are percentage-change problems |
| Simple & Compound Interest | Rate is a percentage |
| Averages & Mixtures | Concentration is a percentage |
| Population / Depreciation growth | Successive percentage change |

**Realistic impact:** Percentages directly or indirectly touch **40–50% of the entire numerical section**. If you master one quant topic, make it this one.

**Question styles reported in EY tests:**

- Straight computation: *"What is 35% of 640?"*
- Percentage change: *"Revenue rose from ₹4.2 cr to ₹5.1 cr — find the % increase"*
- Successive change: *"Increased by 20%, then decreased by 15% — net change?"*
- The "A is x% more than B" ↔ "B is y% less than A" inversion
- Expenditure = Price × Consumption problems
- Election / exam-marks / population word problems
- Embedded in DI: *"Company X's Q3 share of total revenue"*

---

## 2. Core Concepts

### 2.1 What a percentage actually is

A percentage is **a fraction whose denominator is fixed at 100**. "Per cent" is Latin *per centum* — "for each hundred".

$$x\% = \frac{x}{100}$$

So 35% is nothing more than the number 0.35, or the fraction 35/100 = 7/20.

**This one reframing removes most percentage confusion:** the word "of" means **multiply**.

> 35% of 640 → 0.35 × 640 = 224

### 2.2 The three questions percentages ask

Every percentage problem is one of these three:

| Type | Question form | Method |
|---|---|---|
| **Type 1** | What is *P*% of *N*? | Part = (P/100) × N |
| **Type 2** | *A* is what % of *B*? | P = (A/B) × 100 |
| **Type 3** | *P*% of what number is *A*? | N = A ÷ (P/100) = (A × 100)/P |

**Example of each with the same numbers:**

- Type 1: What is 25% of 80? → 0.25 × 80 = **20**
- Type 2: 20 is what % of 80? → (20/80) × 100 = **25%**
- Type 3: 25% of what number is 20? → 20 × 100/25 = **80**

Recognising which of the three you are facing takes 2 seconds and prevents the single most common error in this topic.

### 2.3 Percentage change

$$\text{% Change} = \frac{\text{New Value} - \text{Old Value}}{\text{Old Value}} \times 100$$

**Critical: the denominator is always the ORIGINAL value.** This is where most marks are lost.

> Price goes 80 → 100. Increase = 20. % increase = 20/**80** × 100 = 25%.
> Price goes 100 → 80. Decrease = 20. % decrease = 20/**100** × 100 = 20%.

Same absolute change of 20, but 25% one way and 20% the other. The base matters.

### 2.4 The multiplier method (learn this — it is the whole topic)

Instead of "add 20%", **multiply by 1.20**. Instead of "subtract 15%", **multiply by 0.85**.

| Change | Multiplier |
|---|---|
| Increase by 5% | × 1.05 |
| Increase by 20% | × 1.20 |
| Increase by 100% | × 2.00 |
| Decrease by 10% | × 0.90 |
| Decrease by 25% | × 0.75 |
| Decrease by 40% | × 0.60 |

**Why this is powerful:** successive changes become simple multiplication.

> A value increases 20%, then decreases 15%, then increases 10%.
> Net multiplier = 1.20 × 0.85 × 1.10 = **1.122** → net **+12.2%**

No chains of addition and subtraction. No sign errors. One multiplication.

### 2.5 Successive percentage change

For two successive changes of *a*% and *b*% (using signed values — negative for a decrease):

$$\text{Net % change} = a + b + \frac{ab}{100}$$

**Derivation:** Start with 100. After *a*%: 100(1 + a/100). After *b*%: 100(1 + a/100)(1 + b/100) = 100 + a + b + ab/100. The change from 100 is a + b + ab/100. ∎

**Worked check:** +20% then −15%.
a = +20, b = −15.
Net = 20 − 15 + (20 × −15)/100 = 5 − 3 = **+2%**
Multiplier check: 1.20 × 0.85 = 1.02 = +2% ✓

**The most important special case:**

> Increase by *x*% then decrease by *x*% ⇒ **net always a decrease of x²/100 %**
>
> +10% then −10% → −1%. +20% then −20% → −4%. +30% then −30% → −9%.
>
> It is *never* zero. The order does not matter.

### 2.6 The "more than / less than" inversion

This is EY's favourite percentage trap.

> If **A is x% more than B**, then **B is $\dfrac{x}{100+x} \times 100\%$ less than A**.
>
> If **A is x% less than B**, then **B is $\dfrac{x}{100-x} \times 100\%$ more than A**.

**Why:** Let B = 100. If A is 25% more, A = 125. Now B compared to A: the gap is 25, and the base is now **A = 125**, not 100. So 25/125 × 100 = 20%.

**Memorise this table — it appears constantly:**

| A is *x*% MORE than B | ⇒ B is this much LESS than A |
|---|---|
| 10% | 9 1/11 % ≈ 9.09% |
| 20% | 16 2/3 % ≈ 16.67% |
| 25% | **20%** |
| 33 1/3 % | **25%** |
| 50% | 33 1/3 % |
| 100% | **50%** |

| A is *x*% LESS than B | ⇒ B is this much MORE than A |
|---|---|
| 10% | 11 1/9 % ≈ 11.11% |
| 20% | **25%** |
| 25% | 33 1/3 % |
| 33 1/3 % | **50%** |
| 50% | **100%** |

### 2.7 Price–Consumption–Expenditure

$$\text{Expenditure} = \text{Price} \times \text{Consumption}$$

If price rises by *x*% and you want expenditure unchanged, consumption must fall by:

$$\frac{x}{100+x} \times 100\%$$

If price falls by *x*% and you want expenditure unchanged, consumption may rise by:

$$\frac{x}{100-x} \times 100\%$$

These are exactly the inversion formulas from §2.6 — same mathematics, different clothing.

### 2.8 Percentage points vs percentage

> A rate rises **from 20% to 25%**.
> - The rise is **5 percentage points**.
> - The rise is **25 percent** (because 5/20 × 100 = 25%).

EY word problems occasionally exploit this. Read whether the question says "percent" or "percentage points".

---

## 3. Formula Bank

| # | Concept | Formula |
|---|---|---|
| 1 | Percentage of a number | $\text{Part} = \dfrac{P}{100} \times N$ |
| 2 | What percent A is of B | $P\% = \dfrac{A}{B} \times 100$ |
| 3 | Find the whole from a part | $N = \dfrac{A \times 100}{P}$ |
| 4 | Percentage change | $\dfrac{\text{New} - \text{Old}}{\text{Old}} \times 100$ |
| 5 | Value after increase of *x*% | $N \times \left(1 + \dfrac{x}{100}\right)$ |
| 6 | Value after decrease of *x*% | $N \times \left(1 - \dfrac{x}{100}\right)$ |
| 7 | Two successive changes *a*%, *b*% | $a + b + \dfrac{ab}{100}$ |
| 8 | Increase *x*% then decrease *x*% | Net $= -\dfrac{x^2}{100}\%$ (always a loss) |
| 9 | A is *x*% more than B ⇒ B less than A by | $\dfrac{x}{100+x} \times 100\%$ |
| 10 | A is *x*% less than B ⇒ B more than A by | $\dfrac{x}{100-x} \times 100\%$ |
| 11 | Price ↑ *x*%, keep expenditure same ⇒ cut consumption by | $\dfrac{x}{100+x} \times 100\%$ |
| 12 | Price ↓ *x*%, keep expenditure same ⇒ raise consumption by | $\dfrac{x}{100-x} \times 100\%$ |
| 13 | Population after *n* years at *r*% growth | $P\left(1 + \dfrac{r}{100}\right)^n$ |
| 14 | Population *n* years ago at *r*% growth | $\dfrac{P}{\left(1 + \frac{r}{100}\right)^n}$ |
| 15 | Depreciation after *n* years at *r*% | $P\left(1 - \dfrac{r}{100}\right)^n$ |
| 16 | Net effect: length +*a*%, breadth +*b*% on area | $a + b + \dfrac{ab}{100}$ % |
| 17 | Exam: fails by *m* marks with score *s*, pass = *p*% | $\text{Total} = \dfrac{(s+m) \times 100}{p}$ |
| 18 | Election, 2 candidates, winner gets *w*%, margin *M* votes | $\text{Total} = \dfrac{M \times 100}{2w - 100}$ |
| 19 | Failed in A = *a*%, in B = *b*%, in both = *c*% | Passed both $= 100 - (a + b - c)$ % |
| 20 | Successive changes (general, *n* terms) | $\prod\left(1 + \dfrac{x_i}{100}\right)$ |

---

## 4. Shortcuts & Tricks

### 4.1 The Fraction–Percentage Table (MEMORISE — saves ~20% of your section time)

| Fraction | % | Fraction | % |
|---|---|---|---|
| 1/1 | 100% | 1/9 | 11 1/9 % ≈ 11.11% |
| 1/2 | 50% | 1/10 | 10% |
| 1/3 | 33 1/3 % ≈ 33.33% | 1/11 | 9 1/11 % ≈ 9.09% |
| 1/4 | 25% | 1/12 | 8 1/3 % ≈ 8.33% |
| 1/5 | 20% | 1/15 | 6 2/3 % ≈ 6.67% |
| 1/6 | 16 2/3 % ≈ 16.67% | 1/16 | 6 1/4 % = 6.25% |
| 1/7 | 14 2/7 % ≈ 14.29% | 1/20 | 5% |
| 1/8 | 12 1/2 % = 12.5% | 1/25 | 4% |

**Multiples you should also know instantly:**

| Fraction | % | Fraction | % |
|---|---|---|---|
| 2/3 | 66.67% | 3/8 | 37.5% |
| 3/4 | 75% | 5/8 | 62.5% |
| 2/5 | 40% | 7/8 | 87.5% |
| 3/5 | 60% | 5/6 | 83.33% |
| 4/5 | 80% | 2/7 | 28.57% |
| 5/12 | 41.67% | 7/12 | 58.33% |

**Why this matters:** *"Find 37.5% of 96"* — a candidate who knows 37.5% = 3/8 computes 96 × 3/8 = **36** in three seconds. A candidate who does 96 × 0.375 by long multiplication takes forty.

### 4.2 The Commutation Trick

$$a\% \text{ of } b = b\% \text{ of } a$$

**Proof:** a% of b = (a/100)×b = ab/100 = (b/100)×a = b% of a. ∎

**Use it when one side is easy:**

- 16% of 25 → flip → 25% of 16 = **4**
- 48% of 50 → flip → 50% of 48 = **24**
- 84% of 25 → flip → 25% of 84 = **21**
- 4% of 175 → flip → 175% of 4 = **7**

### 4.3 Decomposition (mental percentage arithmetic)

Break any percentage into 10%, 5%, and 1% chunks.

**Find 35% of 640:**
```
10% of 640 = 64
30%        = 64 × 3 = 192
 5%        = 64 ÷ 2 =  32
─────────────────────────
35%        = 192 + 32 = 224
```

**Find 17% of 500:**
```
10% = 50
 5% = 25
 1% =  5   → 2% = 10
────────────────────
17% = 50 + 25 + 10 = 85
```

### 4.4 The 1.1× / 0.9× ladder (for growth & depreciation)

Memorise these powers — they appear in population and depreciation questions:

| n | 1.05ⁿ | 1.10ⁿ | 1.20ⁿ | 0.90ⁿ | 0.80ⁿ |
|---|---|---|---|---|---|
| 1 | 1.05 | 1.10 | 1.20 | 0.90 | 0.80 |
| 2 | 1.1025 | 1.21 | 1.44 | 0.81 | 0.64 |
| 3 | 1.157625 | 1.331 | 1.728 | 0.729 | 0.512 |

### 4.5 The "Assume 100" technique

When a problem gives **only percentages and no absolute numbers**, set the base to **100** (or to the LCM of the denominators). Every answer that is itself a percentage will be correct.

> *"A's salary is 40% more than B's. B's is 20% more than C's. By what % is A's more than C's?"*
>
> Let C = 100 → B = 120 → A = 120 × 1.4 = 168. A is **68% more** than C.

If the numbers are ugly, use a friendlier base:

> *"1/3 of a class are girls; 40% of girls wear glasses..."* → assume **class = 300**, not 100.

### 4.6 The Reverse-Percentage Trap

> *"After a 20% increase, the price is ₹600. What was the original?"*

**Wrong (very common):** 600 − 20% of 600 = 600 − 120 = 480 ✗
**Right:** 600 ÷ 1.20 = **500** ✓

Verify: 500 × 1.20 = 600 ✓ (whereas 480 × 1.20 = 576 ✗)

**Rule: to undo a percentage change, DIVIDE by the multiplier — never subtract.**

### 4.7 Elimination by magnitude

EY options are usually spread. Before calculating, ask *"roughly how big should this be?"*

> *"An item costing ₹1,860 is discounted 35%. Find the selling price."*
> Options: (a) ₹1,209 (b) ₹1,309 (c) ₹651 (d) ₹1,450
>
> 35% off means you pay **65%**, so ~two-thirds of 1,860 ≈ 1,240. Only (a) and (b) are near.
> Refine: 65% of 1,800 = 1,170; 65% of 60 = 39; total ≈ 1,209. Answer **(a)**.
>
> Option (c) is the classic trap — that is the *discount amount*, not the selling price.

### 4.8 Percentage → Ratio conversion

When a problem says "A is 25% more than B", immediately write the **ratio** A : B = 5 : 4.

| Statement | Ratio |
|---|---|
| A is 25% more than B | A : B = 5 : 4 |
| A is 20% more than B | A : B = 6 : 5 |
| A is 50% more than B | A : B = 3 : 2 |
| A is 20% less than B | A : B = 4 : 5 |
| A is 25% less than B | A : B = 3 : 4 |
| A is 33⅓% less than B | A : B = 2 : 3 |

Ratios are far easier to manipulate than percentages in multi-step problems.

---

## 5. Solved Examples

### Example 1 — Basic computation with the fraction shortcut

**Q.** Find 62.5% of 480.

**Step 1 — Recognise the fraction.**
From the fraction table, 62.5% = 5/8.

**Step 2 — Multiply.**
$$480 \times \frac{5}{8} = 60 \times 5 = 300$$

**Answer: 300**

> *Long way:* 480 × 0.625 = 300. Same answer, four times the effort.

---

### Example 2 — Percentage change (identifying the correct base)

**Q.** A company's revenue fell from ₹7.5 crore to ₹6.0 crore. Find the percentage decrease.

**Step 1 — Identify old and new.**
Old = 7.5, New = 6.0. The base is the **old** value, 7.5.

**Step 2 — Apply the formula.**
$$\% \text{ change} = \frac{6.0 - 7.5}{7.5} \times 100 = \frac{-1.5}{7.5} \times 100$$

**Step 3 — Simplify.**
$$\frac{1.5}{7.5} = \frac{15}{75} = \frac{1}{5} = 20\%$$

**Answer: 20% decrease**

> **Trap:** dividing by 6.0 instead of 7.5 gives 25% — that would be the answer to "by what % must 6.0 rise to reach 7.5?", a different question.

---

### Example 3 — Successive changes

**Q.** The price of a laptop increased by 25% and later decreased by 20%. What is the net percentage change?

**Method A — Multiplier (fastest):**
$$1.25 \times 0.80 = 1.00$$
Multiplier is exactly 1 ⇒ **no net change (0%)**.

**Method B — Formula:**
$$a + b + \frac{ab}{100} = 25 + (-20) + \frac{25 \times (-20)}{100} = 5 - 5 = 0$$

**Method C — Assume 100:**
100 → +25% → 125 → −20% of 125 = −25 → 100. Back to start.

**Answer: 0% — no change**

> **Pattern worth memorising:** +25% then −20% cancel exactly. So do +20%/−16⅔%, +50%/−33⅓%, and +100%/−50%. These pairs are inverse multipliers.

---

### Example 4 — The more/less inversion

**Q.** Rohan's salary is 60% more than Karan's. By what percentage is Karan's salary less than Rohan's?

**Step 1 — Assume a base.** Let Karan = 100.

**Step 2 — Compute Rohan.** Rohan = 100 × 1.60 = 160.

**Step 3 — Now compare Karan to Rohan. The base changes to Rohan = 160.**
$$\frac{160 - 100}{160} \times 100 = \frac{60}{160} \times 100 = 37.5\%$$

**Formula check:**
$$\frac{x}{100+x} \times 100 = \frac{60}{160} \times 100 = 37.5\%$$ ✓

**Answer: 37.5%**

> **Trap:** answering "60%". The percentage is not symmetric because the base changed.

---

### Example 5 — Price and consumption

**Q.** The price of petrol rises by 20%. By what percentage must a driver reduce consumption so that the monthly fuel bill is unchanged?

**Step 1 — Set up.** Expenditure = Price × Consumption. We need the product to stay constant.

**Step 2 — Assume convenient values.** Price = 100, Consumption = 100, so Expenditure = 10,000.

**Step 3 — Apply the price rise.** New price = 120.

**Step 4 — Solve for new consumption.**
$$120 \times C_{\text{new}} = 10{,}000 \implies C_{\text{new}} = \frac{10{,}000}{120} = 83.33$$

**Step 5 — Percentage reduction.**
$$\frac{100 - 83.33}{100} \times 100 = 16.67\% = 16\tfrac{2}{3}\%$$

**Formula check:** $\frac{20}{120} \times 100 = 16\tfrac{2}{3}\%$ ✓

**Answer: 16⅔% (≈16.67%)**

---

### Example 6 — Exam marks

**Q.** In an examination, a student must score 40% to pass. A candidate scored 168 marks and failed by 32 marks. What are the maximum marks?

**Step 1 — Find the pass mark.**
The candidate needed 32 more marks to pass, so:
$$\text{Pass mark} = 168 + 32 = 200$$

**Step 2 — The pass mark is 40% of the total.**
$$0.40 \times T = 200$$

**Step 3 — Solve.**
$$T = \frac{200}{0.40} = \frac{200 \times 100}{40} = 500$$

**Answer: 500 marks**

**Verify:** 40% of 500 = 200. Candidate got 168, which is 32 short. ✓

---

### Example 7 — Election problem

**Q.** In an election between two candidates, the winner secured 58% of the votes and won by 4,800 votes. How many total votes were cast? (Assume all votes valid.)

**Step 1 — Find the loser's share.**
Loser = 100% − 58% = 42%.

**Step 2 — Find the margin as a percentage.**
Margin = 58% − 42% = **16%** of total votes.

**Step 3 — Equate to the given margin.**
$$0.16 \times T = 4{,}800$$

**Step 4 — Solve.**
$$T = \frac{4{,}800}{0.16} = 30{,}000$$

**Answer: 30,000 votes**

**Verify:** Winner = 58% × 30,000 = 17,400. Loser = 42% × 30,000 = 12,600. Difference = 4,800 ✓

> **Formula:** Total = Margin × 100 / (2w − 100), where w = winner's percentage.
> Here: 4800 × 100 / (116 − 100) = 480000/16 = 30,000 ✓

---

### Example 8 — Multi-step with savings

**Q.** A man spends 80% of his income. His income rises by 25% and his expenditure rises by 15%. Find the percentage increase in his savings.

**Step 1 — Assume income = 100.**
Expenditure = 80, Savings = 100 − 80 = 20.

**Step 2 — Apply the increases.**
New income = 100 × 1.25 = 125
New expenditure = 80 × 1.15 = 92

**Step 3 — Compute new savings.**
New savings = 125 − 92 = 33

**Step 4 — Percentage increase in savings.**
$$\frac{33 - 20}{20} \times 100 = \frac{13}{20} \times 100 = 65\%$$

**Answer: 65%**

> **Insight:** savings is a *small* base, so it swings hard. A 25%/15% split on income/expenditure produced a 65% jump in savings. Expect large answers here — don't second-guess them.

---

## 6. Practice Questions

**Instructions:** 50 questions. Easy (1–20), Medium (21–40), Hard (41–50).
Target times: Easy 30 s · Medium 60 s · Hard 90 s.
Full solutions in [Section 7](#7-detailed-solutions).

### 🟢 EASY (Questions 1–20)

**Q1.** What is 35% of 640?
(a) 214  (b) 224  (c) 234  (d) 244

**Q2.** What percent of 250 is 45?
(a) 15%  (b) 16%  (c) 18%  (d) 20%

**Q3.** If 20% of a number is 60, what is the number?
(a) 240  (b) 280  (c) 300  (d) 320

**Q4.** Find 25% of 25% of 800.
(a) 40  (b) 50  (c) 60  (d) 100

**Q5.** Express 5/8 as a percentage.
(a) 58%  (b) 60.5%  (c) 62.5%  (d) 64%

**Q6.** A number is increased by 20%. The new number is what percent of the original?
(a) 20%  (b) 80%  (c) 110%  (d) 120%

**Q7.** The price of an item rises from ₹80 to ₹100. Find the percentage increase.
(a) 20%  (b) 25%  (c) 30%  (d) 33⅓%

**Q8.** Find 15% of 40% of 500.
(a) 25  (b) 30  (c) 35  (d) 40

**Q9.** A student scored 288 marks out of 400. What is the percentage?
(a) 68%  (b) 70%  (c) 72%  (d) 75%

**Q10.** If A is 25% more than B, then B is what percent less than A?
(a) 16⅔%  (b) 20%  (c) 25%  (d) 30%

**Q11.** 60% of a number is 45 more than 40% of the same number. Find the number.
(a) 200  (b) 215  (c) 225  (d) 250

**Q12.** A salary of ₹25,000 is increased by 12%. Find the new salary.
(a) ₹27,000  (b) ₹27,500  (c) ₹28,000  (d) ₹28,500

**Q13.** 45 is what percent of 180?
(a) 20%  (b) 22.5%  (c) 25%  (d) 30%

**Q14.** If 30% of *x* = 18, find 45% of *x*.
(a) 24  (b) 25  (c) 27  (d) 30

**Q15.** A town's population of 8,000 increases by 10% and then decreases by 10%. What is the final population?
(a) 7,900  (b) 7,920  (c) 8,000  (d) 8,080

**Q16.** A number is increased by 10% and then by 20%. Find the net percentage increase.
(a) 30%  (b) 31%  (c) 32%  (d) 33%

**Q17.** Express 0.45 as a percentage.
(a) 0.45%  (b) 4.5%  (c) 45%  (d) 450%

**Q18.** A student needs 40% to pass. He scored 178 marks and failed by 22 marks. Find the maximum marks.
(a) 450  (b) 480  (c) 500  (d) 550

**Q19.** If 12% of 500 = *x*% of 300, find *x*.
(a) 15  (b) 18  (c) 20  (d) 24

**Q20.** A's income is 20% less than B's. B's income is what percent more than A's?
(a) 20%  (b) 22%  (c) 25%  (d) 30%

---

### 🟡 MEDIUM (Questions 21–40)

**Q21.** The price of sugar increases by 25%. By what percentage must a family reduce consumption so that expenditure remains unchanged?
(a) 16⅔%  (b) 20%  (c) 25%  (d) 30%

**Q22.** In an election between two candidates, the winner received 56% of the votes and won by 3,600 votes. Find the total number of votes.
(a) 24,000  (b) 28,000  (c) 30,000  (d) 36,000

**Q23.** A's salary is 40% more than B's. B's salary is 20% more than C's. If C earns ₹15,000, find A's salary.
(a) ₹24,000  (b) ₹25,200  (c) ₹26,400  (d) ₹27,000

**Q24.** A town's population grows 5% annually. If the present population is 1,76,400, what was it two years ago?
(a) 1,55,000  (b) 1,58,000  (c) 1,60,000  (d) 1,62,000

**Q25.** In a class, 40% are girls. 20% of the girls and 25% of the boys wear glasses. What percentage of the class wears glasses?
(a) 21%  (b) 22%  (c) 23%  (d) 24%

**Q26.** A shop's sales rose 20% in Year 1 and fell 25% in Year 2. Find the net percentage change over the two years.
(a) 5% decrease  (b) 10% decrease  (c) 5% increase  (d) No change

**Q27.** If the numerator of a fraction is increased by 20% and the denominator decreased by 20%, the new fraction is 3/4. Find the original fraction.
(a) 1/3  (b) 1/2  (c) 2/5  (d) 3/8

**Q28.** A candidate needs 35% to pass. He scored 210 marks and failed by 35 marks. Find the maximum marks.
(a) 600  (b) 650  (c) 700  (d) 750

**Q29.** A 60-litre mixture contains milk and water in the ratio 2 : 1. How much water must be added so that milk becomes 50% of the mixture?
(a) 15 L  (b) 20 L  (c) 25 L  (d) 30 L

**Q30.** Two numbers are respectively 25% and 40% less than a third number. The first number is what percent of the second?
(a) 115%  (b) 120%  (c) 125%  (d) 130%

**Q31.** A person's salary is reduced by 20%. By what percentage must the reduced salary be increased to restore the original?
(a) 20%  (b) 22%  (c) 25%  (d) 30%

**Q32.** When 30% of a number is subtracted from the number itself, the result is 84. Find the number.
(a) 110  (b) 115  (c) 120  (d) 125

**Q33.** A man spends 75% of his income. His income increases by 20% and his expenditure by 10%. Find the percentage increase in his savings.
(a) 40%  (b) 45%  (c) 50%  (d) 55%

**Q34.** If 20% of A = 30% of B = 40% of C, find A : B : C.
(a) 2 : 3 : 4  (b) 4 : 3 : 2  (c) 6 : 4 : 3  (d) 3 : 4 : 6

**Q35.** The price of an article is reduced by 20% and consequently its sales increase by 30%. Find the percentage change in revenue.
(a) 4% increase  (b) 4% decrease  (c) 10% increase  (d) 6% increase

**Q36.** In a school of 800 students, 45% are boys. If 200 more girls join, what percentage of the school will be girls?
(a) 60%  (b) 62%  (c) 64%  (d) 66%

**Q37.** A's height is 25% more than B's, and B's is 20% more than C's. By what percentage is A's height more than C's?
(a) 45%  (b) 48%  (c) 50%  (d) 55%

**Q38.** A number increased by 15% becomes 460. Find the number.
(a) 380  (b) 391  (c) 400  (d) 415

**Q39.** 50% of 60% of a number is 24 more than 20% of the same number. Find the number.
(a) 200  (b) 220  (c) 240  (d) 260

**Q40.** In an exam, 35% failed in Mathematics, 45% failed in English, and 20% failed in both. What percentage passed in both subjects?
(a) 20%  (b) 35%  (c) 40%  (d) 45%

---

### 🔴 HARD (Questions 41–50)

**Q41.** The price of a commodity increases by 30%. A family reduces its consumption by 20%. Find the percentage change in expenditure.
(a) 4% increase  (b) 4% decrease  (c) 10% increase  (d) 6% decrease

**Q42.** In a three-cornered election, A polled 40% of the votes, B polled 35%, and C the remainder. A defeated C by 3,000 votes. Find the total votes cast.
(a) 15,000  (b) 18,000  (c) 20,000  (d) 24,000

**Q43.** A's salary is 25% more than B's, and C's salary is 20% less than A's. If the combined salary of all three is ₹65,000, find A's salary.
(a) ₹22,000  (b) ₹24,000  (c) ₹25,000  (d) ₹26,000

**Q44.** A machine depreciates in value by 10% each year. After 3 years its value is ₹43,740. Find its original value.
(a) ₹54,000  (b) ₹58,000  (c) ₹60,000  (d) ₹62,000

**Q45.** In a town, 60% of the population is literate. Of the literate population, 40% are women. If there are 7,200 literate men, find the total population of the town.
(a) 16,000  (b) 18,000  (c) 20,000  (d) 24,000

**Q46.** A 25% reduction in the price of rice enables a man to buy 5 kg more for ₹300. Find the reduced price per kg.
(a) ₹12  (b) ₹15  (c) ₹18  (d) ₹20

**Q47.** In an election between two candidates, 10% of the votes cast were declared invalid. One candidate secured 60% of the valid votes and won by 3,600 votes. Find the total number of votes cast.
(a) 18,000  (b) 20,000  (c) 22,000  (d) 25,000

**Q48.** A's salary is 30% more than B's. B's salary is 25% less than C's. If A earns ₹58,500, find C's salary.
(a) ₹55,000  (b) ₹58,000  (c) ₹60,000  (d) ₹65,000

**Q49.** An alloy of 50 kg contains 40% copper and 60% zinc. How much copper must be added so that copper forms 50% of the new alloy?
(a) 5 kg  (b) 8 kg  (c) 10 kg  (d) 12 kg

**Q50.** A person's income increases by 20%, while the tax rate falls from 25% to 20%. Find the percentage change in post-tax income.
(a) 25%  (b) 26%  (c) 28%  (d) 30%

---

## 7. Detailed Solutions

### 🟢 EASY — Solutions 1–20

---

**Q1. What is 35% of 640? → (b) 224**

**Formula used:** Part = (P/100) × N

**Method 1 — Decomposition (fastest):**
```
10% of 640 = 64
30% of 640 = 64 × 3 = 192
 5% of 640 = 64 ÷ 2 =  32
──────────────────────────
35% of 640 = 192 + 32 = 224
```

**Method 2 — Direct:**
$$\frac{35}{100} \times 640 = 35 \times 6.4 = 224$$

**Answer: (b) 224**

---

**Q2. What percent of 250 is 45? → (c) 18%**

**Formula used:** P% = (A/B) × 100 — this is Type 2 (A is what % of B).

Here A = 45 (the part), B = 250 (the whole).

$$P = \frac{45}{250} \times 100$$

**Simplify before multiplying:**
$$= \frac{45}{250} \times 100 = \frac{45 \times 100}{250} = \frac{4500}{250} = 18$$

**Cross-check:** 18% of 250 = 0.18 × 250 = 45 ✓

**Answer: (c) 18%**

---

**Q3. If 20% of a number is 60, what is the number? → (c) 300**

**Formula used:** N = (A × 100)/P — Type 3.

$$N = \frac{60 \times 100}{20} = \frac{6000}{20} = 300$$

**Shortcut:** 20% = 1/5. If one-fifth is 60, the whole is 60 × 5 = 300.

**Cross-check:** 20% of 300 = 60 ✓

**Answer: (c) 300**

---

**Q4. Find 25% of 25% of 800. → (b) 50**

**Work from the inside out.**

**Step 1:** 25% of 800 = 800 × 1/4 = 200
**Step 2:** 25% of 200 = 200 × 1/4 = 50

**Faster (combine the multipliers first):**
$$0.25 \times 0.25 = 0.0625 = \frac{1}{16}$$
$$800 \times \frac{1}{16} = 50$$

**Answer: (b) 50**

---

**Q5. Express 5/8 as a percentage. → (c) 62.5%**

**Formula used:** Fraction → % is × 100.

$$\frac{5}{8} \times 100 = \frac{500}{8} = 62.5\%$$

**Shortcut:** 1/8 = 12.5%, so 5/8 = 5 × 12.5 = 62.5%.

**Answer: (c) 62.5%**

---

**Q6. A number increased by 20% is what percent of the original? → (d) 120%**

Let the original be 100.
New value = 100 + 20% of 100 = 100 + 20 = 120.

$$\frac{120}{100} \times 100 = 120\%$$

> **Note the wording.** "The *increase* is what percent" → 20%. "The *new number* is what percent" → 120%. Read carefully; both options are offered.

**Answer: (d) 120%**

---

**Q7. Price rises ₹80 → ₹100. Percentage increase? → (b) 25%**

**Formula used:** % change = (New − Old)/Old × 100

The base is the **original** price, ₹80.

$$\frac{100 - 80}{80} \times 100 = \frac{20}{80} \times 100 = \frac{1}{4} \times 100 = 25\%$$

> **Trap:** using 100 as the denominator gives 20%, which is option (a). That would answer "if the price fell from 100 to 80, what is the % decrease?" — a different question.

**Answer: (b) 25%**

---

**Q8. Find 15% of 40% of 500. → (b) 30**

**Step 1:** 40% of 500 = 0.40 × 500 = 200
**Step 2:** 15% of 200 = 0.15 × 200 = 30

**Combined multiplier:** 0.15 × 0.40 = 0.06 → 0.06 × 500 = 30

**Answer: (b) 30**

---

**Q9. 288 out of 400 — find the percentage. → (c) 72%**

$$\frac{288}{400} \times 100 = \frac{288}{4} = 72\%$$

**Shortcut:** dividing by 400 and multiplying by 100 is the same as dividing by 4.

**Answer: (c) 72%**

---

**Q10. A is 25% more than B ⇒ B is what % less than A? → (b) 20%**

**Formula used:** $\dfrac{x}{100+x} \times 100$, with x = 25.

$$\frac{25}{125} \times 100 = \frac{1}{5} \times 100 = 20\%$$

**Verification by assuming values:**
Let B = 100 → A = 125.
B is less than A by 25. Base is now **A = 125**.
25/125 × 100 = 20% ✓

**Answer: (b) 20%**

---

**Q11. 60% of a number is 45 more than 40% of it. Find the number. → (c) 225**

**Step 1 — Translate to an equation.** Let the number be *x*.
$$0.60x = 0.40x + 45$$

**Step 2 — Collect terms.**
$$0.60x - 0.40x = 45$$
$$0.20x = 45$$

**Step 3 — Solve.**
$$x = \frac{45}{0.20} = \frac{4500}{20} = 225$$

**Shortcut:** The gap between 60% and 40% is **20%**, and that gap equals 45. So 20% ⇒ 45, hence 100% ⇒ 45 × 5 = 225.

**Cross-check:** 60% of 225 = 135; 40% of 225 = 90; 135 − 90 = 45 ✓

**Answer: (c) 225**

---

**Q12. ₹25,000 increased by 12%. → (c) ₹28,000**

**Formula used:** New = N × (1 + x/100)

$$25{,}000 \times 1.12 = 28{,}000$$

**Mental method:**
```
10% of 25,000 = 2,500
 2% of 25,000 =   500
──────────────────────
12%           = 3,000
New salary = 25,000 + 3,000 = 28,000
```

**Answer: (c) ₹28,000**

---

**Q13. 45 is what percent of 180? → (c) 25%**

$$\frac{45}{180} \times 100$$

**Simplify the fraction first:** 45/180 = 1/4.

$$\frac{1}{4} \times 100 = 25\%$$

**Answer: (c) 25%**

---

**Q14. If 30% of x = 18, find 45% of x. → (c) 27**

**Method 1 — Find x first.**
$$0.30x = 18 \implies x = \frac{18}{0.30} = 60$$
$$45\% \text{ of } 60 = 0.45 \times 60 = 27$$

**Method 2 — Ratio shortcut (faster):**
45% is 45/30 = 1.5 times 30%.
So the answer is 1.5 × 18 = **27**.

**Answer: (c) 27**

---

**Q15. 8,000 → +10% → −10%. Final population? → (b) 7,920**

**Multiplier method:**
$$8000 \times 1.10 \times 0.90 = 8000 \times 0.99 = 7920$$

**Step by step:**
- After +10%: 8000 + 800 = 8,800
- After −10%: 8800 − 880 = 7,920

**Key concept:** +x% then −x% always gives a **net loss of x²/100 %**.
Here x = 10 ⇒ net loss = 100/100 = **1%**. And 1% of 8,000 = 80, so 8000 − 80 = 7,920 ✓

**Answer: (b) 7,920**

---

**Q16. +10% then +20% — net increase? → (c) 32%**

**Formula used:** Net = a + b + ab/100

$$10 + 20 + \frac{10 \times 20}{100} = 30 + 2 = 32\%$$

**Multiplier check:** 1.10 × 1.20 = 1.32 → +32% ✓

> **Trap:** answering 30%. Successive percentages never simply add — the second increase applies to the *already-increased* value.

**Answer: (c) 32%**

---

**Q17. Express 0.45 as a percentage. → (c) 45%**

**Rule:** Decimal → % is × 100.

$$0.45 \times 100 = 45\%$$

**Answer: (c) 45%**

---

**Q18. Pass = 40%; scored 178, failed by 22. Max marks? → (c) 500**

**Formula used:** Total = (Score + Shortfall) × 100 / Pass%

**Step 1 — Find the pass mark.**
Failing "by 22 marks" means 22 more would have passed him.
$$\text{Pass mark} = 178 + 22 = 200$$

**Step 2 — Pass mark = 40% of total.**
$$0.40 \times T = 200$$

**Step 3 — Solve.**
$$T = \frac{200 \times 100}{40} = 500$$

**Cross-check:** 40% of 500 = 200; he got 178; shortfall 22 ✓

**Answer: (c) 500**

---

**Q19. 12% of 500 = x% of 300. Find x. → (c) 20**

**Step 1 — Evaluate the left side.**
$$12\% \text{ of } 500 = 0.12 \times 500 = 60$$

**Step 2 — Set up the right side.**
$$\frac{x}{100} \times 300 = 60$$
$$3x = 60$$
$$x = 20$$

**Cross-check:** 20% of 300 = 60 ✓

**Answer: (c) 20**

---

**Q20. A is 20% less than B ⇒ B is what % more than A? → (c) 25%**

**Formula used:** $\dfrac{x}{100-x} \times 100$, with x = 20.

$$\frac{20}{80} \times 100 = 25\%$$

**Verification:** Let B = 100 → A = 80.
B exceeds A by 20. Base is now **A = 80**.
20/80 × 100 = 25% ✓

**Answer: (c) 25%**

---

### 🟡 MEDIUM — Solutions 21–40

---

**Q21. Sugar price +25%; cut consumption by what % to keep expenditure fixed? → (b) 20%**

**Formula used:** Reduction% = $\dfrac{x}{100+x} \times 100$

$$\frac{25}{125} \times 100 = 20\%$$

**First-principles derivation:**
Let price = ₹100/kg, consumption = 100 kg ⇒ expenditure = ₹10,000.
New price = ₹125/kg.
For expenditure to stay ₹10,000:
$$\text{New consumption} = \frac{10{,}000}{125} = 80 \text{ kg}$$
Reduction = 100 − 80 = 20 kg on a base of 100 ⇒ **20%** ✓

**Answer: (b) 20%**

---

**Q22. Winner got 56%, won by 3,600 votes. Total? → (c) 30,000**

**Step 1 — Loser's share.** 100% − 56% = 44%

**Step 2 — Margin as a percentage.**
$$56\% - 44\% = 12\%$$

**Step 3 — Equate.**
$$0.12 \times T = 3{,}600$$

**Step 4 — Solve.**
$$T = \frac{3{,}600}{0.12} = 30{,}000$$

**Cross-check:** Winner 16,800; loser 13,200; margin 3,600 ✓

> **Shortcut:** margin% = 2w − 100 = 2(56) − 100 = 12%. Total = Margin × 100 / (2w − 100) = 3600 × 100/12 = 30,000.

**Answer: (c) 30,000**

---

**Q23. A is 40% more than B; B is 20% more than C; C = ₹15,000. Find A. → (b) ₹25,200**

**Work outward from C.**

**Step 1 — Find B.**
$$B = C \times 1.20 = 15{,}000 \times 1.20 = 18{,}000$$

**Step 2 — Find A.**
$$A = B \times 1.40 = 18{,}000 \times 1.40 = 25{,}200$$

**Single-step multiplier:**
$$A = 15{,}000 \times 1.20 \times 1.40 = 15{,}000 \times 1.68 = 25{,}200$$

**Answer: (b) ₹25,200**

---

**Q24. Population grows 5%/yr; now 1,76,400. Value 2 years ago? → (c) 1,60,000**

**Formula used:** $P_{\text{past}} = \dfrac{P_{\text{now}}}{(1 + r/100)^n}$

**Step 1 — Compute the two-year growth factor.**
$$1.05^2 = 1.1025$$

**Step 2 — Divide (do NOT subtract 10%).**
$$P = \frac{1{,}76{,}400}{1.1025} = 1{,}60{,}000$$

**Easier arithmetic — work with fractions:**
$$1.05 = \frac{21}{20} \implies 1.05^2 = \frac{441}{400}$$
$$P = 1{,}76{,}400 \times \frac{400}{441}$$
$$\frac{1{,}76{,}400}{441} = 400 \implies P = 400 \times 400 = 1{,}60{,}000$$

**Cross-check forward:** 1,60,000 × 1.05 = 1,68,000 → × 1.05 = 1,76,400 ✓

**Answer: (c) 1,60,000**

---

**Q25. 40% girls; 20% of girls and 25% of boys wear glasses. % of class with glasses? → (c) 23%**

**Step 1 — Assume class size = 100.**
Girls = 40, Boys = 60

**Step 2 — Count glasses-wearers in each group.**
$$\text{Girls with glasses} = 20\% \text{ of } 40 = 8$$
$$\text{Boys with glasses} = 25\% \text{ of } 60 = 15$$

**Step 3 — Total.**
$$8 + 15 = 23 \text{ out of } 100 = 23\%$$

> **Trap:** averaging 20% and 25% to get 22.5%. That is only valid if the groups are equal in size. They are 40 : 60, so the boys' 25% carries more weight — pulling the answer above the midpoint.

**Answer: (c) 23%**

---

**Q26. +20% then −25%. Net change? → (b) 10% decrease**

**Multiplier method:**
$$1.20 \times 0.75 = 0.90$$
Multiplier 0.90 ⇒ **10% decrease**

**Formula method:**
$$a + b + \frac{ab}{100} = 20 + (-25) + \frac{20 \times (-25)}{100} = -5 - 5 = -10\%$$

**Assume-100 check:** 100 → 120 → 120 − 30 = 90. Down 10 from 100 ⇒ 10% decrease ✓

**Answer: (b) 10% decrease**

---

**Q27. Numerator +20%, denominator −20% gives 3/4. Find the original fraction. → (b) 1/2**

**Step 1 — Express the new fraction.** Let the original be n/d.
$$\text{New} = \frac{1.20\,n}{0.80\,d}$$

**Step 2 — Simplify the multiplier.**
$$\frac{1.20}{0.80} = \frac{3}{2} = 1.5$$
So New = 1.5 × (n/d).

**Step 3 — Set equal to 3/4 and solve.**
$$1.5 \times \frac{n}{d} = \frac{3}{4}$$
$$\frac{n}{d} = \frac{3}{4} \div \frac{3}{2} = \frac{3}{4} \times \frac{2}{3} = \frac{1}{2}$$

**Cross-check:** n/d = 1/2. Numerator 1 → 1.2; denominator 2 → 1.6. New = 1.2/1.6 = 3/4 ✓

**Answer: (b) 1/2**

---

**Q28. Pass = 35%; scored 210, failed by 35. Max marks? → (c) 700**

**Step 1 — Pass mark.**
$$210 + 35 = 245$$

**Step 2 — Relate to the total.**
$$0.35 \times T = 245$$

**Step 3 — Solve.**
$$T = \frac{245}{0.35} = \frac{24{,}500}{35} = 700$$

**Cross-check:** 35% of 700 = 245; 245 − 210 = 35 ✓

**Answer: (c) 700**

---

**Q29. 60 L mixture, milk : water = 2 : 1. Add water so milk = 50%. → (b) 20 L**

**Step 1 — Find current quantities.**
Ratio 2 : 1 means 3 parts total; each part = 60/3 = 20 L.
$$\text{Milk} = 40 \text{ L}, \quad \text{Water} = 20 \text{ L}$$

**Step 2 — Key insight: adding water does not change the milk.**
Milk stays at 40 L.

**Step 3 — For milk to be 50%, the total must be twice the milk.**
$$\text{New total} = 2 \times 40 = 80 \text{ L}$$

**Step 4 — Water to add.**
$$80 - 60 = 20 \text{ L}$$

**Cross-check:** 40 L milk in 80 L total = 50% ✓

**Answer: (b) 20 L**

---

**Q30. Two numbers are 25% and 40% less than a third. First is what % of second? → (c) 125%**

**Step 1 — Assume the third number = 100.**
$$\text{First} = 100 - 25\% = 75$$
$$\text{Second} = 100 - 40\% = 60$$

**Step 2 — Compare first to second (base = second).**
$$\frac{75}{60} \times 100 = \frac{5}{4} \times 100 = 125\%$$

**Answer: (c) 125%**

---

**Q31. Salary cut 20%; raise it by what % to restore? → (c) 25%**

**Formula used:** $\dfrac{x}{100-x} \times 100$

$$\frac{20}{80} \times 100 = 25\%$$

**Verification:** Original 100 → after 20% cut = 80.
To return to 100, we must add 20 on a base of 80:
$$\frac{20}{80} \times 100 = 25\% \checkmark$$

> **Trap:** answering 20%. A 20% rise on 80 gives 96, not 100.

**Answer: (c) 25%**

---

**Q32. 30% of a number subtracted from itself gives 84. → (c) 120**

**Step 1 — Set up.**
$$x - 0.30x = 84$$

**Step 2 — Simplify.**
$$0.70x = 84$$

**Step 3 — Solve.**
$$x = \frac{84}{0.70} = 120$$

**Shortcut:** "Remove 30%" leaves **70%**. If 70% = 84, then 10% = 12, so 100% = 120.

**Answer: (c) 120**

---

**Q33. Spends 75%; income +20%, expenditure +10%. % increase in savings? → (c) 50%**

**Step 1 — Assume income = 100.**
$$\text{Expenditure} = 75, \quad \text{Savings} = 100 - 75 = 25$$

**Step 2 — Apply the increases.**
$$\text{New income} = 100 \times 1.20 = 120$$
$$\text{New expenditure} = 75 \times 1.10 = 82.5$$

**Step 3 — New savings.**
$$120 - 82.5 = 37.5$$

**Step 4 — Percentage increase in savings.**
$$\frac{37.5 - 25}{25} \times 100 = \frac{12.5}{25} \times 100 = 50\%$$

> **Why so large?** Savings is a small residual (25), so absolute changes hit it hard in percentage terms. Never assume the savings change must lie between 10% and 20%.

**Answer: (c) 50%**

---

**Q34. If 20% of A = 30% of B = 40% of C, find A : B : C. → (c) 6 : 4 : 3**

**Step 1 — Set the common value to *k*.**
$$0.20A = 0.30B = 0.40C = k$$

**Step 2 — Express each variable.**
$$A = \frac{k}{0.20} = 5k, \quad B = \frac{k}{0.30} = \frac{10k}{3}, \quad C = \frac{k}{0.40} = 2.5k$$

**Step 3 — Form the ratio.**
$$A : B : C = 5 : \frac{10}{3} : 2.5$$

**Step 4 — Clear fractions (multiply all by 6).**
$$= 30 : 20 : 15 = 6 : 4 : 3$$

**Shortcut worth remembering:** If *a*% of A = *b*% of B = *c*% of C, then
$$A : B : C = \frac{1}{a} : \frac{1}{b} : \frac{1}{c}$$
Here: 1/20 : 1/30 : 1/40. Multiply by LCM(20,30,40) = 120 → 6 : 4 : 3 ✓

**Cross-check:** A = 6, B = 4, C = 3. 20% of 6 = 1.2; 30% of 4 = 1.2; 40% of 3 = 1.2 ✓

**Answer: (c) 6 : 4 : 3**

---

**Q35. Price −20%, sales +30%. Change in revenue? → (a) 4% increase**

**Key relation:** Revenue = Price × Quantity Sold

**Multiplier method:**
$$0.80 \times 1.30 = 1.04$$
⇒ **4% increase**

**Formula method:**
$$a + b + \frac{ab}{100} = -20 + 30 + \frac{(-20)(30)}{100} = 10 - 6 = +4\%$$

**Assume-100 check:** Price 100, Qty 100 ⇒ Revenue 10,000.
New: Price 80, Qty 130 ⇒ Revenue 10,400. Increase = 400/10,000 = 4% ✓

**Answer: (a) 4% increase**

---

**Q36. 800 students, 45% boys. 200 more girls join. % girls now? → (c) 64%**

**Step 1 — Current composition.**
$$\text{Boys} = 45\% \text{ of } 800 = 360$$
$$\text{Girls} = 800 - 360 = 440$$

**Step 2 — After 200 girls join.**
$$\text{Girls} = 440 + 200 = 640$$
$$\text{Total} = 800 + 200 = 1{,}000$$

**Step 3 — Percentage of girls.**
$$\frac{640}{1{,}000} \times 100 = 64\%$$

> **Trap:** forgetting that the **total** also grows. Dividing 640 by the old total of 800 gives 80% — wrong.

**Answer: (c) 64%**

---

**Q37. A is 25% more than B; B is 20% more than C. A vs C? → (c) 50%**

**Multiplier chain:**
$$1.25 \times 1.20 = 1.50$$
⇒ A is **50% more** than C.

**Assume-value check:** Let C = 100.
$$B = 120, \quad A = 120 \times 1.25 = 150$$
$$\frac{150 - 100}{100} \times 100 = 50\% \checkmark$$

> **Trap:** answering 45% (25 + 20). Successive percentages multiply, not add.

**Answer: (c) 50%**

---

**Q38. A number increased by 15% becomes 460. → (c) 400**

**Formula used:** Original = New ÷ (1 + x/100)

$$\text{Original} = \frac{460}{1.15}$$

**Clean the arithmetic:**
$$\frac{460}{1.15} = \frac{46{,}000}{115} = 400$$

**Cross-check:** 400 × 1.15 = 460 ✓

> **Trap:** computing 460 − 15% of 460 = 460 − 69 = 391 (option b). To reverse a percentage change you must **divide**, not subtract.

**Answer: (c) 400**

---

**Q39. 50% of 60% of a number is 24 more than 20% of it. → (c) 240**

**Step 1 — Combine the nested percentages.**
$$50\% \times 60\% = 0.50 \times 0.60 = 0.30 = 30\%$$

**Step 2 — Set up the equation.**
$$0.30x = 0.20x + 24$$

**Step 3 — Solve.**
$$0.10x = 24 \implies x = 240$$

**Cross-check:** 30% of 240 = 72; 20% of 240 = 48; 72 − 48 = 24 ✓

**Answer: (c) 240**

---

**Q40. Failed: Maths 35%, English 45%, both 20%. Passed both? → (c) 40%**

**Concept: Set union.** Use the inclusion–exclusion principle.

**Step 1 — Failed in at least one subject.**
$$n(M \cup E) = n(M) + n(E) - n(M \cap E)$$
$$= 35 + 45 - 20 = 60\%$$

**Step 2 — Passed in both = everyone else.**
$$100 - 60 = 40\%$$

**Visual check:**

```
        Failed Maths only : 35 − 20 = 15%
        Failed English only: 45 − 20 = 25%
        Failed both        :          20%
        ───────────────────────────────────
        Failed at least one:          60%
        Passed BOTH        :          40%
```

> **Trap:** answering 20% by computing 100 − 35 − 45. That double-subtracts the 20% who failed both.

**Answer: (c) 40%**

---

### 🔴 HARD — Solutions 41–50

---

**Q41. Price +30%, consumption −20%. Change in expenditure? → (a) 4% increase**

**Key relation:** Expenditure = Price × Consumption

**Multiplier method:**
$$1.30 \times 0.80 = 1.04 \implies +4\%$$

**Formula method:**
$$a + b + \frac{ab}{100} = 30 - 20 + \frac{30 \times (-20)}{100} = 10 - 6 = +4\%$$

**Assume-value verification:**
Original: price ₹100/unit × 100 units = ₹10,000
New: price ₹130/unit × 80 units = ₹10,400
$$\frac{10{,}400 - 10{,}000}{10{,}000} \times 100 = 4\% \text{ increase} \checkmark$$

> **Insight:** cutting consumption by 20% is *not enough* to absorb a 30% price rise. To fully absorb it, the cut would need to be 30/130 × 100 = 23.08%.

**Answer: (a) 4% increase**

---

**Q42. Three candidates: A 40%, B 35%, C rest. A beat C by 3,000. Total? → (c) 20,000**

**Step 1 — Find C's share.**
$$C = 100\% - 40\% - 35\% = 25\%$$

**Step 2 — Margin between A and C as a percentage.**
$$40\% - 25\% = 15\%$$

**Step 3 — Equate to the given margin.**
$$0.15 \times T = 3{,}000$$

**Step 4 — Solve.**
$$T = \frac{3{,}000}{0.15} = 20{,}000$$

**Cross-check:**
A = 40% × 20,000 = 8,000
B = 35% × 20,000 = 7,000
C = 25% × 20,000 = 5,000
A − C = 8,000 − 5,000 = 3,000 ✓ (and 8,000+7,000+5,000 = 20,000 ✓)

> **Trap:** using B's 35% instead of computing C's 25%. Read which pair the margin refers to.

**Answer: (c) 20,000**

---

**Q43. A = B + 25%; C = A − 20%; A + B + C = ₹65,000. Find A. → (c) ₹25,000**

**Step 1 — Express everything in terms of one variable.** Let B = 100 units.

$$A = 100 \times 1.25 = 125 \text{ units}$$
$$C = A \times 0.80 = 125 \times 0.80 = 100 \text{ units}$$

**Step 2 — Sum the units.**
$$A + B + C = 125 + 100 + 100 = 325 \text{ units}$$

**Step 3 — Find the value of one unit.**
$$325 \text{ units} = ₹65{,}000 \implies 1 \text{ unit} = ₹200$$

**Step 4 — Compute A.**
$$A = 125 \times 200 = ₹25{,}000$$

**Cross-check:**
B = 100 × 200 = ₹20,000
A = ₹25,000 (which is 25% more than 20,000 ✓)
C = 80% of 25,000 = ₹20,000 ✓
Total = 25,000 + 20,000 + 20,000 = ₹65,000 ✓

> **Note:** C and B turn out equal — because 1.25 × 0.80 = 1 exactly. That is the +25%/−20% inverse pair from §2.5.

**Answer: (c) ₹25,000**

---

**Q44. 10% annual depreciation; value after 3 years = ₹43,740. Original? → (c) ₹60,000**

**Formula used:** $V_n = P(1 - r/100)^n$

**Step 1 — Write the equation.**
$$P \times (0.90)^3 = 43{,}740$$

**Step 2 — Compute the depreciation factor.**
$$0.90^3 = 0.729$$

**Step 3 — Solve for P.**
$$P = \frac{43{,}740}{0.729}$$

**Step 4 — Clean arithmetic using fractions.**
$$0.9 = \frac{9}{10} \implies 0.9^3 = \frac{729}{1000}$$
$$P = 43{,}740 \times \frac{1000}{729}$$
$$\frac{43{,}740}{729} = 60 \implies P = 60 \times 1000 = ₹60{,}000$$

**Cross-check forward:**
Year 1: 60,000 × 0.9 = 54,000
Year 2: 54,000 × 0.9 = 48,600
Year 3: 48,600 × 0.9 = 43,740 ✓

> **Trap:** treating 3 years of 10% depreciation as a flat 30% loss, giving 43,740/0.70 = ₹62,485.7. Compounding is not additive.

**Answer: (c) ₹60,000**

---

**Q45. 60% literate; 40% of literates are women; 7,200 literate men. Total population? → (c) 20,000**

**Step 1 — Find the men's share of the literate group.**
If 40% of literates are women, then 60% of literates are men.

**Step 2 — Express literate men as a fraction of the total population *P*.**
$$\text{Literate men} = 60\% \text{ of literates} = 0.60 \times (0.60 \times P) = 0.36P$$

**Step 3 — Equate and solve.**
$$0.36P = 7{,}200$$
$$P = \frac{7{,}200}{0.36} = 20{,}000$$

**Cross-check:**
Total = 20,000
Literate = 60% × 20,000 = 12,000
Literate women = 40% × 12,000 = 4,800
Literate men = 12,000 − 4,800 = 7,200 ✓

> **Trap:** reading "40% are women" as 40% of the *total population*. It is 40% of the *literate* subgroup. Always identify which base a percentage sits on.

**Answer: (c) 20,000**

---

**Q46. 25% price cut lets a man buy 5 kg more for ₹300. Reduced price/kg? → (b) ₹15**

**Step 1 — Define variables.**
Let the reduced price be ₹*R* per kg.
Since the reduced price is 75% of the original:
$$0.75 \times \text{Original} = R \implies \text{Original} = \frac{R}{0.75} = \frac{4R}{3}$$

**Step 2 — Express quantities bought with ₹300.**
$$\text{Quantity at new price} = \frac{300}{R}$$
$$\text{Quantity at old price} = \frac{300}{4R/3} = \frac{900}{4R} = \frac{225}{R}$$

**Step 3 — The difference is 5 kg.**
$$\frac{300}{R} - \frac{225}{R} = 5$$
$$\frac{75}{R} = 5$$

**Step 4 — Solve.**
$$R = \frac{75}{5} = ₹15$$

**Cross-check:**
Reduced price ₹15/kg → ₹300 buys 20 kg
Original price = 15/0.75 = ₹20/kg → ₹300 buys 15 kg
Extra = 20 − 15 = 5 kg ✓

**⚡ Fast alternative:** A 25% price cut means the money buys 1/0.75 = 4/3 as much — a **33⅓% increase in quantity**. So:
$$\frac{1}{3} \times Q_{\text{old}} = 5 \implies Q_{\text{old}} = 15 \text{ kg} \implies Q_{\text{new}} = 20 \text{ kg}$$
$$\text{Reduced price} = \frac{300}{20} = ₹15 \checkmark$$

> **Trap:** answering ₹20 — that is the *original* price. Read which price is asked for.

**Answer: (b) ₹15**

---

**Q47. 10% invalid votes; winner got 60% of valid votes and won by 3,600. Total cast? → (b) 20,000**

**Step 1 — Let total votes cast = *T*.**
$$\text{Valid votes} = 90\% \text{ of } T = 0.90T$$

**Step 2 — Split the valid votes.**
Winner = 60% of valid, Loser = 40% of valid.
$$\text{Margin} = 20\% \text{ of valid votes}$$

**Step 3 — Express the margin in terms of T.**
$$\text{Margin} = 0.20 \times 0.90T = 0.18T$$

**Step 4 — Equate and solve.**
$$0.18T = 3{,}600$$
$$T = \frac{3{,}600}{0.18} = 20{,}000$$

**Cross-check:**
Total cast = 20,000
Invalid = 10% = 2,000 → Valid = 18,000
Winner = 60% × 18,000 = 10,800
Loser = 40% × 18,000 = 7,200
Margin = 10,800 − 7,200 = 3,600 ✓

> **Trap:** applying the 20% margin to the *total* votes instead of the *valid* votes, giving 18,000. The two-layer percentage is the entire difficulty of this question.

**Answer: (b) 20,000**

---

**Q48. A = B + 30%; B = C − 25%; A = ₹58,500. Find C. → (c) ₹60,000**

**Step 1 — Write each relation as a multiplier, chaining back to C.**
$$B = 0.75\,C$$
$$A = 1.30\,B = 1.30 \times 0.75\,C$$

**Step 2 — Combine the multipliers.**
$$1.30 \times 0.75 = 0.975$$
$$A = 0.975\,C$$

**Step 3 — Substitute and solve.**
$$0.975\,C = 58{,}500$$
$$C = \frac{58{,}500}{0.975} = \frac{58{,}500{,}000}{975} = 60{,}000$$

**Cross-check:**
C = ₹60,000
B = 75% of 60,000 = ₹45,000
A = 130% of 45,000 = ₹58,500 ✓

> **Insight:** A ends up *less* than C (0.975 < 1), even though A is "30% more" than something. Chained percentages regularly defy intuition — always multiply the factors rather than reasoning verbally.

**Answer: (c) ₹60,000**

---

**Q49. 50 kg alloy with 40% copper. Add copper to reach 50%. → (c) 10 kg**

**Step 1 — Current composition.**
$$\text{Copper} = 40\% \text{ of } 50 = 20 \text{ kg}$$
$$\text{Zinc} = 60\% \text{ of } 50 = 30 \text{ kg}$$

**Step 2 — Key insight: adding copper does not change the zinc.**
Zinc stays fixed at 30 kg.

**Step 3 — For copper to be 50%, zinc must also be 50%.**
$$\text{New total} = \frac{30}{0.50} = 60 \text{ kg}$$

**Step 4 — Copper added.**
$$60 - 50 = 10 \text{ kg}$$

**Algebraic confirmation:** Let *x* kg of copper be added.
$$\frac{20 + x}{50 + x} = 0.50$$
$$20 + x = 0.50(50 + x) = 25 + 0.5x$$
$$0.5x = 5 \implies x = 10 \checkmark$$

**Cross-check:** New alloy = 60 kg with 30 kg copper and 30 kg zinc = 50% each ✓

> **Technique:** in any "add one component" problem, anchor on the component that **does not change**. It converts a two-variable problem into a one-step division.

**Answer: (c) 10 kg**

---

**Q50. Income +20%; tax rate 25% → 20%. % change in post-tax income? → (c) 28%**

**Step 1 — Assume original income = 100.**
$$\text{Tax} = 25\% \text{ of } 100 = 25$$
$$\text{Post-tax income} = 100 - 25 = 75$$

**Step 2 — Compute the new figures.**
$$\text{New income} = 100 \times 1.20 = 120$$
$$\text{New tax} = 20\% \text{ of } 120 = 24$$
$$\text{New post-tax income} = 120 - 24 = 96$$

**Step 3 — Percentage change in post-tax income.**
$$\frac{96 - 75}{75} \times 100 = \frac{21}{75} \times 100 = 28\%$$

**Multiplier verification:**
Post-tax income = Income × (1 − tax rate)
$$\text{Old factor} = 1 \times 0.75 = 0.75$$
$$\text{New factor} = 1.20 \times 0.80 = 0.96$$
$$\text{Change} = \frac{0.96}{0.75} = 1.28 \implies +28\% \checkmark$$

> **Trap:** answering 25% by adding the 20% income rise to the 5-percentage-point tax cut. The tax cut is applied to a *larger* income, and the base for comparison is post-tax income (75, not 100).

**Answer: (c) 28%**

---

## 8. Quick Revision Sheet

> **One page. Read this 48 hours after studying the topic, and again the night before the test.**

### Core formulas

```
P% of N          =  (P/100) × N
A as % of B      =  (A/B) × 100
Find whole       =  (Part × 100) / P%
% change         =  (New − Old) / Old × 100      ← base is ALWAYS Old
After +x%        =  N × (1 + x/100)
After −x%        =  N × (1 − x/100)
Reverse a change =  DIVIDE by the multiplier (never subtract)
```

### Successive change

```
Net of a% and b%  =  a + b + ab/100      (signs matter)
Multiplier method =  (1 ± a/100)(1 ± b/100)
+x% then −x%      =  net LOSS of x²/100 %   ← never zero
```

### The inversion pair (memorise the numbers)

```
A is x% MORE than B  →  B is  x/(100+x) × 100 % less than A
A is x% LESS than B  →  B is  x/(100−x) × 100 % more than A

  +25% ↔ −20%      +20% ↔ −16⅔%      +50% ↔ −33⅓%      +100% ↔ −50%
  +33⅓% ↔ −25%     +10% ↔ −9 1/11%   +11⅑% ↔ −10%
```

### Fraction → percentage (instant recall)

```
1/2 = 50%     1/3 = 33.33%   1/4 = 25%      1/5 = 20%
1/6 = 16.67%  1/7 = 14.29%   1/8 = 12.5%    1/9 = 11.11%
1/10 = 10%    1/11 = 9.09%   1/12 = 8.33%   1/16 = 6.25%
1/20 = 5%     1/25 = 4%

2/3 = 66.67%  3/4 = 75%      2/5 = 40%      3/5 = 60%    4/5 = 80%
3/8 = 37.5%   5/8 = 62.5%    7/8 = 87.5%    5/6 = 83.33%
```

### Word-problem templates

| Situation | Formula |
|---|---|
| Exam: score *s*, failed by *m*, pass *p*% | Total = (s + m) × 100 / p |
| Election, 2 candidates, winner *w*%, margin *M* | Total = M × 100 / (2w − 100) |
| Election with *i*% invalid, winner *w*% of valid | Margin fraction of total = (2w − 100)/100 × (100 − i)/100 |
| Failed A = *a*%, B = *b*%, both = *c*% | Passed both = 100 − (a + b − c) |
| Price ↑ *x*%, keep expenditure same | Cut consumption by x/(100+x) × 100 % |
| Price ↓ *x*%, same money buys more | Quantity ↑ by x/(100−x) × 100 % |
| Growth *r*% for *n* years | P(1 + r/100)ⁿ |
| Depreciation *r*% for *n* years | P(1 − r/100)ⁿ |

### Speed tricks

```
1.  a% of b = b% of a          →  16% of 25 = 25% of 16 = 4
2.  Decompose into 10/5/1%     →  35% of 640 = 192 + 32 = 224
3.  Assume base = 100          →  when only percentages are given
4.  Convert % to ratio         →  "25% more" ⇒ 5 : 4
5.  Anchor on the unchanged    →  mixture problems: fix the untouched component
6.  Check option magnitude     →  eliminate before you calculate
```

### Powers to know

```
1.05² = 1.1025    1.10² = 1.21    1.20² = 1.44
1.05³ ≈ 1.1576    1.10³ = 1.331   1.20³ = 1.728
0.90² = 0.81      0.80² = 0.64
0.90³ = 0.729     0.80³ = 0.512
```

---

## 9. Common Mistakes

| # | Mistake | Example | Correction |
|---|---|---|---|
| 1 | **Wrong base for % change** | 80→100 computed as 20/100 = 20% | Base is always the *original*: 20/80 = 25% |
| 2 | **Adding successive percentages** | +10% then +20% = 30% | Multiply: 1.1 × 1.2 = 1.32 ⇒ 32% |
| 3 | **Assuming +x%/−x% cancels** | +10%, −10% ⇒ no change | Net loss of x²/100 = 1% |
| 4 | **Reversing by subtraction** | After +15% it's 460 ⇒ 460 − 69 = 391 | Divide: 460/1.15 = 400 |
| 5 | **Symmetric more/less** | A is 25% more than B ⇒ B is 25% less | B is 20% less — the base changed |
| 6 | **Averaging unequal groups** | 20% of girls, 25% of boys ⇒ 22.5% | Weight by group size: 40:60 ⇒ 23% |
| 7 | **Forgetting the total changes** | 200 girls join 800 ⇒ 640/800 | Total becomes 1,000 ⇒ 640/1,000 = 64% |
| 8 | **Wrong base in nested percentages** | "40% of literates are women" ⇒ 40% of population | It is 40% of the *literate subgroup* |
| 9 | **Double-subtracting in overlap problems** | 100 − 35 − 45 = 20% | Use inclusion–exclusion: 100 − (35 + 45 − 20) = 40% |
| 10 | **Compounding treated as flat** | 10%/yr for 3 yrs = 30% | 1 − 0.9³ = 27.1%, not 30% |
| 11 | **Answering the wrong quantity** | Asked for reduced price, gave original | Re-read the final line of the question |
| 12 | **Percentage vs percentage points** | 20% → 25% called "a 5% rise" | It is 5 percentage points = a 25% rise |

---

## Practice Answer Key (for quick self-scoring)

| Q | Ans | Q | Ans | Q | Ans | Q | Ans | Q | Ans |
|---|---|---|---|---|---|---|---|---|---|
| 1 | b | 11 | c | 21 | b | 31 | c | 41 | a |
| 2 | c | 12 | c | 22 | c | 32 | c | 42 | c |
| 3 | c | 13 | c | 23 | b | 33 | c | 43 | c |
| 4 | b | 14 | c | 24 | c | 34 | c | 44 | c |
| 5 | c | 15 | b | 25 | c | 35 | a | 45 | c |
| 6 | d | 16 | c | 26 | b | 36 | c | 46 | b |
| 7 | b | 17 | c | 27 | b | 37 | c | 47 | b |
| 8 | b | 18 | c | 28 | c | 38 | c | 48 | c |
| 9 | c | 19 | c | 29 | b | 39 | c | 49 | c |
| 10 | b | 20 | c | 30 | c | 40 | c | 50 | c |

**Scoring guide:** 45+/50 → strong. 35–44 → solid, revise the missed sub-types. Below 35 → re-read Sections 2–4 and redo the Medium set.

---

**⬅️ Back:** [Exam Pattern & Strategy](../00-exam-pattern-and-strategy.md) · **➡️ Next:** [Topic 2 — Profit, Loss & Discount](02-profit-loss-discount.md)
