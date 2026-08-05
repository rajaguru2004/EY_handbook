# Topic 5 — Time & Work, Pipes & Cisterns

### EY Placement Aptitude Handbook · Priority Rank #4 · 🔴 Critical

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

**Weightage:** 8–10% of the quantitative section — a **near-guaranteed appearance**, typically 1 question. Pipes & cisterns is the same mathematics wearing a different hat, so the two are covered together.

**Why this topic is a high-return investment:** with the **LCM method** (Section 2.3), almost every question in this topic reduces to whole-number arithmetic. No fractions, no common denominators, no algebra. A question that takes 2 minutes with the traditional 1/x approach takes 30 seconds with LCM units.

**Question styles reported:**

| Style | Typical shape |
|---|---|
| A + B together | "A in 12 days, B in 15 days — together?" |
| Find the third worker | "A+B in 12, B+C in 15, C+A in 20 — find A alone" |
| Partial work then handover | "Together 6 days, then A leaves; B finishes the rest" |
| One worker leaves early | "A leaves 3 days before completion" |
| Alternate days | "A and B work on alternate days" |
| Efficiency comparison | "A is 25% more efficient than B" |
| Men–women–boys equivalence | "3 men and 4 boys in 8 days…" |
| Man-days / work-equation | "15 men, 8 hrs/day, 12 days → 20 men, 9 hrs/day?" |
| Wages distribution | "Split ₹600 in proportion to work done" |
| Pipes filling & emptying | "Two inlets and one outlet, all opened" |
| Leak problems | "Tank fills in 6 h; with a leak, 8 h" |

---

## 2. Core Concepts

### 2.1 The one-day-work idea

If a person completes a job in *n* days, then in one day they complete **1/n of the job**.

$$\text{Rate} = \frac{1}{\text{Time}} \qquad \text{Time} = \frac{1}{\text{Rate}}$$

**Rates add when people work together:**

$$\frac{1}{T_{\text{together}}} = \frac{1}{T_A} + \frac{1}{T_B} + \cdots$$

Which rearranges (for two workers) into:

$$\boxed{T_{\text{together}} = \frac{T_A \times T_B}{T_A + T_B}}$$

> A in 12 days, B in 15 days ⇒ together in (12 × 15)/(12 + 15) = 180/27 = **6⅔ days**

### 2.2 Work is proportional to rate × time

$$\text{Work done} = \text{Rate} \times \text{Time}$$

This is the master equation. Every problem in this topic is an application of it.

### 2.3 ⭐ The LCM Method — learn this and use nothing else

**The idea:** instead of treating the total work as "1 unit" (which forces you into fractions), define the total work as the **LCM of all the given times**. Every rate then becomes a whole number.

**Procedure:**

```
1. Total Work = LCM of all given times
2. Each person's rate = Total Work ÷ their individual time
3. Do the whole problem in whole-number units
4. Convert back at the end: Time = Units needed ÷ Combined rate
```

**Worked demonstration:** *A can do a job in 12 days, B in 18 days, C in 36 days. How long together?*

```
Step 1:  Total Work = LCM(12, 18, 36) = 36 units

Step 2:  A's rate = 36 ÷ 12 = 3 units/day
         B's rate = 36 ÷ 18 = 2 units/day
         C's rate = 36 ÷ 36 = 1 unit/day

Step 3:  Combined = 3 + 2 + 1 = 6 units/day

Step 4:  Time = 36 ÷ 6 = 6 days
```

**Compare with the fraction method:** 1/12 + 1/18 + 1/36 = 3/36 + 2/36 + 1/36 = 6/36 = 1/6 ⇒ 6 days.

Same answer — but the LCM method never left the integers. Under a 45-second clock, that difference is decisive.

> **You do not need the true LCM.** Any common multiple works. If the times are 7 and 11, use 77. If they are 20 and 30, use 60 (or even 120). Convenience beats minimality.

### 2.4 Efficiency

**Efficiency is the rate of work.** It is *inversely* proportional to time.

$$\text{Efficiency} \propto \frac{1}{\text{Time}}$$

$$\boxed{\frac{\text{Efficiency of A}}{\text{Efficiency of B}} = \frac{\text{Time of B}}{\text{Time of A}}}$$

| Statement | Efficiency ratio | Time ratio |
|---|---|---|
| A is twice as good as B | A : B = 2 : 1 | A : B = 1 : 2 |
| A is thrice as fast as B | A : B = 3 : 1 | A : B = 1 : 3 |
| A is 25% more efficient than B | A : B = 5 : 4 | A : B = 4 : 5 |
| A is 20% more efficient than B | A : B = 6 : 5 | A : B = 5 : 6 |
| A is 20% less efficient than B | A : B = 4 : 5 | A : B = 5 : 4 |

> **A is 25% more efficient than B, and B takes 20 days. How long does A take?**
> Efficiency A : B = 5 : 4 ⇒ Time A : B = 4 : 5.
> If B takes 20, A takes 20 × (4/5) = **16 days**.

### 2.5 The man-days (work equation) principle

For a fixed job:

$$\boxed{M_1 \times D_1 \times H_1 = M_2 \times D_2 \times H_2}$$

where M = number of workers, D = days, H = hours per day.

**Extended with work quantity:**

$$\frac{M_1 D_1 H_1}{W_1} = \frac{M_2 D_2 H_2}{W_2}$$

> 15 men working 8 hours/day finish in 12 days. How many days for 20 men at 9 hours/day?
> $$15 \times 8 \times 12 = 20 \times 9 \times D \implies 1440 = 180D \implies D = 8 \text{ days}$$

**Think in "man-hours" as a currency:** the job costs 1,440 man-hours. Any team that supplies 1,440 man-hours finishes it.

### 2.6 The three-pairs identity

A very common EY setup: you are given the *pairs*, and asked for individuals.

Given: (A+B), (B+C), (C+A) rates.

$$(A+B) + (B+C) + (C+A) = 2(A + B + C)$$

$$\boxed{A + B + C = \frac{1}{2}\left[\frac{1}{T_{AB}} + \frac{1}{T_{BC}} + \frac{1}{T_{CA}}\right]}$$

Then each individual falls out by subtraction:

$$A = (A+B+C) - (B+C), \qquad B = (A+B+C) - (C+A), \qquad C = (A+B+C) - (A+B)$$

### 2.7 Alternate-day working

When A and B work on alternate days:

```
1. Compute the work done in ONE PAIR of days (A's day + B's day)
2. Divide the total work by the pair-output to get the number of complete cycles
3. Handle the leftover work day by day
```

> A in 12 days, B in 18 days, starting with A.
> LCM = 36 units. A = 3/day, B = 2/day. **Pair output = 5 units per 2 days.**
> 36 ÷ 5 = 7 pairs (35 units) in **14 days**, with 1 unit left.
> Day 15 is A's turn (3 units/day) — he needs only 1 unit, taking 1/3 of a day.
> **Total = 14⅓ days.**

> **Watch the starting worker.** Starting with B instead would give a different answer whenever the leftover is nonzero.

### 2.8 One worker leaving early

> *"A and B start together, but A leaves *k* days before completion. Find the total time T."*

**Set up:** B works the full **T** days; A works **(T − k)** days.

$$\text{Rate}_A \times (T - k) + \text{Rate}_B \times T = \text{Total Work}$$

> A in 12 days, B in 18 days; A leaves 3 days before the end.
> LCM = 36. A = 3, B = 2.
> $$3(T - 3) + 2T = 36 \implies 5T - 9 = 36 \implies T = 9 \text{ days}$$

### 2.9 Wages and payment

**Wages are shared in the ratio of work done**, which — for equal time worked — equals the ratio of efficiencies (i.e. the *inverse* ratio of individual times).

$$\text{Wage ratio} = \frac{1}{T_A} : \frac{1}{T_B} : \frac{1}{T_C}$$

> A in 6 days, B in 8 days, C in 24 days; total wage ₹600.
> Ratio = 1/6 : 1/8 : 1/24. Multiply by 24 ⇒ **4 : 3 : 1** (8 parts).
> A = ₹300, B = ₹225, C = ₹75.

If workers put in **different numbers of days**, use (rate × days worked) as the weight instead.

### 2.10 Pipes & Cisterns — the same topic with signs

| Work concept | Pipes concept |
|---|---|
| Worker | Inlet pipe (positive rate) |
| — | Outlet pipe / leak (**negative** rate) |
| Job completed | Tank filled |
| Rate = 1/time | Fill rate = 1/time to fill |

$$\text{Net rate} = \sum(\text{inlet rates}) - \sum(\text{outlet rates})$$

> Pipe A fills in 12 h, B fills in 16 h, C empties in 24 h. All open.
> LCM = 48. A = +4, B = +3, C = −2. **Net = +5 units/h.**
> Time = 48 ÷ 5 = **9.6 hours**.

**If the net rate is negative, the tank never fills** — it empties. Check the sign before answering.

### 2.11 The leak problem

> *"A tank fills in *a* hours. With a leak, it takes *b* hours. How long does the leak alone take to empty a full tank?"*

$$\frac{1}{a} - \frac{1}{\text{leak}} = \frac{1}{b} \implies \boxed{\text{Leak time} = \frac{ab}{b - a}}$$

> Fills in 8 h; with a leak, 10 h. Leak empties in (8 × 10)/(10 − 8) = 80/2 = **40 hours**.

### 2.12 Capacity from a flow rate

When a pipe's flow is given in litres per minute, use it to convert a *rate* into an *absolute capacity*.

> A leak empties a cistern in 20 h. A tap admitting 4 L/min is opened, and the cistern now empties in 24 h. Find the capacity.
>
> The tap's fill rate = (leak rate) − (net emptying rate) = 1/20 − 1/24 = **1/120 per hour**.
> So the tap alone would fill the cistern in 120 hours.
> Tap flow = 4 L/min = 240 L/hour.
> **Capacity = 240 × 120 = 28,800 litres.**

---

## 3. Formula Bank

| # | Concept | Formula |
|---|---|---|
| 1 | One day's work | $\dfrac{1}{n}$ if the job takes *n* days |
| 2 | Combined time (2 workers) | $\dfrac{T_A T_B}{T_A + T_B}$ |
| 3 | Combined rate (any number) | $\sum \dfrac{1}{T_i}$ |
| 4 | Find the partner | $\dfrac{1}{T_B} = \dfrac{1}{T_{AB}} - \dfrac{1}{T_A}$ |
| 5 | **LCM method** | Work $=$ LCM(times); rate $=$ Work ÷ time |
| 6 | Efficiency ratio | $E_A : E_B = T_B : T_A$ (inverse) |
| 7 | A is *x*% more efficient | $T_A = T_B \times \dfrac{100}{100+x}$ |
| 8 | Work equation | $M_1D_1H_1 = M_2D_2H_2$ |
| 9 | With differing work amounts | $\dfrac{M_1D_1H_1}{W_1} = \dfrac{M_2D_2H_2}{W_2}$ |
| 10 | Three pairs → all three | $A+B+C = \frac{1}{2}\left(\frac{1}{T_{AB}}+\frac{1}{T_{BC}}+\frac{1}{T_{CA}}\right)$ |
| 11 | Individual from the trio | $A = (A+B+C) - (B+C)$ |
| 12 | A leaves *k* days early | $R_A(T-k) + R_B T = W$ |
| 13 | Alternate days | Pair output per 2 days; then handle the remainder |
| 14 | Wage ratio | $\dfrac{1}{T_A} : \dfrac{1}{T_B} : \dfrac{1}{T_C}$ (or rate × days worked) |
| 15 | Pipes: net rate | $\sum \text{inlets} - \sum \text{outlets}$ |
| 16 | Two inlets *a*, *b* | $\dfrac{ab}{a+b}$ |
| 17 | Inlet *a*, outlet *b* (*b* > *a*) | $\dfrac{ab}{b-a}$ |
| 18 | Leak time from *a* and *b* | $\dfrac{ab}{b-a}$ where *b* is the time with the leak |
| 19 | Capacity from flow | Capacity $=$ (flow per hour) × (hours the pipe alone would take) |
| 20 | Fraction of work in *d* days | $\dfrac{d}{n}$ |
| 21 | Remaining work | $1 - \dfrac{d}{n}$ |
| 22 | Time for the remainder by B | $\left(1 - \dfrac{d}{n}\right) \times T_B$ |

---

## 4. Shortcuts & Tricks

### 4.1 The LCM method in three lines

```
Times given: 20, 30, 60         →  Work = 60 units
Rates:        3,  2,  1  units/day
Combined:              6 units/day  →  60/6 = 10 days
```

Never write a fraction in a time-and-work problem again.

### 4.2 The product-over-sum shortcut (two workers only)

$$T = \frac{ab}{a+b}$$

Memorise these pairs — they appear constantly:

| a, b | Together |
|---|---|
| 10, 15 | 6 |
| 12, 24 | 8 |
| 12, 6 | 4 |
| 20, 30 | 12 |
| 15, 30 | 10 |
| 6, 12 | 4 |
| 4, 12 | 3 |
| 10, 40 | 8 |

### 4.3 Efficiency percentages → clean ratios

| Statement | Efficiency | Time |
|---|---|---|
| 25% more efficient | 5 : 4 | 4 : 5 |
| 20% more efficient | 6 : 5 | 5 : 6 |
| 50% more efficient | 3 : 2 | 2 : 3 |
| 100% more efficient (twice as fast) | 2 : 1 | 1 : 2 |
| 20% less efficient | 4 : 5 | 5 : 4 |
| 25% less efficient | 3 : 4 | 4 : 3 |

**Rule:** the efficiency ratio and the time ratio are always **flipped**.

### 4.4 The "days remaining" pattern

> *"A can do a job in n days. He works for d days, then B (who takes m days) finishes it."*

```
Fraction done by A       =  d / n
Fraction remaining       =  1 − d/n
Days B needs             =  m × (1 − d/n)
```

> A takes 20 days and works 8 days; B takes 15 days and finishes.
> Remaining = 1 − 8/20 = 3/5. B needs 15 × 3/5 = **9 days**.

### 4.5 Alternate-days checklist

```
□  Compute pair output (2 days of work)
□  Divide total by pair output → number of complete cycles
□  Multiply cycles × 2 → days elapsed
□  Compute the leftover units
□  Identify WHOSE TURN the next day is (depends on who started)
□  Leftover ÷ that person's rate → fractional final day
```

The most-missed step is the last: whether the leftover is finished by A or B changes the answer.

### 4.6 Man-days as a currency

Convert the whole job into **man-days** (or man-hours) and treat it like a budget.

> 40 men, 60 days planned. After 30 days only 40% is done. How many more men?
>
> Spent: 40 × 30 = **1,200 man-days** = 40% of the job
> Whole job: 1,200 ÷ 0.40 = **3,000 man-days**
> Remaining: 60% = **1,800 man-days** in 30 days ⇒ need 1,800/30 = **60 men**
> **Additional men = 60 − 40 = 20**

### 4.7 Pipes — sign discipline

```
Inlet  →  +rate
Outlet →  −rate

Write every rate WITH its sign before adding. Then:
   Net > 0  →  tank fills; time = Capacity / Net
   Net < 0  →  tank never fills
   Net = 0  →  level stays constant forever
```

### 4.8 Sanity checks

```
✓ Two people together are ALWAYS faster than the faster one alone
   (if A takes 12 and B takes 18, together must be < 12)
✓ Adding an outlet pipe ALWAYS increases the fill time
✓ More men ⇒ fewer days (inverse). If your answer moves the wrong way, recheck.
✓ Efficiency ratio and time ratio are always INVERSE
✓ In the three-pairs setup, always halve the sum — forgetting this is the #1 error
```

---

## 5. Solved Examples

### Example 1 — Two workers together (LCM method)

**Q.** A can complete a piece of work in 15 days and B can complete it in 10 days. How long will they take working together?

**Method — LCM:**

**Step 1 — Set the total work.**
$$\text{Work} = \text{LCM}(15, 10) = 30 \text{ units}$$

**Step 2 — Find individual rates.**
$$A = \frac{30}{15} = 2 \text{ units/day}$$
$$B = \frac{30}{10} = 3 \text{ units/day}$$

**Step 3 — Combine.**
$$A + B = 5 \text{ units/day}$$

**Step 4 — Time.**
$$\frac{30}{5} = 6 \text{ days}$$

**Formula cross-check:**
$$T = \frac{ab}{a+b} = \frac{15 \times 10}{25} = 6 \checkmark$$

**Answer: 6 days**

**Sanity check:** 6 < 10 (the faster worker's time) ✓ — two workers must beat either one alone.

---

### Example 2 — Finding the missing partner

**Q.** A and B together can complete a work in 8 days. A alone takes 12 days. How long will B take alone?

**Step 1 — Set the total work.**
$$\text{Work} = \text{LCM}(8, 12) = 24 \text{ units}$$

**Step 2 — Convert the given information into rates.**
$$A + B = \frac{24}{8} = 3 \text{ units/day}$$
$$A = \frac{24}{12} = 2 \text{ units/day}$$

**Step 3 — Subtract.**
$$B = 3 - 2 = 1 \text{ unit/day}$$

**Step 4 — B's time.**
$$\frac{24}{1} = 24 \text{ days}$$

**Answer: 24 days**

> **Note:** this is the standard "subtract the rates, never the times" pattern. Subtracting times (12 − 8 = 4) is wrong and is a common trap option.

---

### Example 3 — The three-pairs problem

**Q.** A and B together can complete a work in 12 days, B and C in 15 days, and C and A in 20 days. In how many days can all three together complete it? How long would A alone take?

**Step 1 — Set the total work.**
$$\text{Work} = \text{LCM}(12, 15, 20) = 60 \text{ units}$$

**Step 2 — Convert pair-times into pair-rates.**
$$A + B = \frac{60}{12} = 5 \text{ units/day}$$
$$B + C = \frac{60}{15} = 4 \text{ units/day}$$
$$C + A = \frac{60}{20} = 3 \text{ units/day}$$

**Step 3 — Add all three (this counts each person twice).**
$$2(A + B + C) = 5 + 4 + 3 = 12$$
$$A + B + C = 6 \text{ units/day}$$

**Step 4 — Time for all three together.**
$$\frac{60}{6} = 10 \text{ days}$$

**Step 5 — Isolate A.**
$$A = (A+B+C) - (B+C) = 6 - 4 = 2 \text{ units/day}$$
$$T_A = \frac{60}{2} = 30 \text{ days}$$

**Bonus — the other two:**
$$B = 6 - 3 = 3 \text{ units/day} \implies T_B = 20 \text{ days}$$
$$C = 6 - 5 = 1 \text{ unit/day} \implies T_C = 60 \text{ days}$$

**Verification:** A + B = 2 + 3 = 5 ✓ · B + C = 3 + 1 = 4 ✓ · C + A = 1 + 2 = 3 ✓

**Answer: All three in 10 days; A alone in 30 days**

> **The critical step is halving.** Forgetting the factor of 2 in Step 3 gives 5 days instead of 10 — and 5 days would be a trap option.

---

### Example 4 — Partial work and handover

**Q.** A can do a piece of work in 20 days and B in 30 days. They work together for 6 days, after which A leaves. How many more days will B need to finish?

**Step 1 — Set the total work.**
$$\text{Work} = \text{LCM}(20, 30) = 60 \text{ units}$$

**Step 2 — Individual rates.**
$$A = 3 \text{ units/day}, \qquad B = 2 \text{ units/day}$$

**Step 3 — Work done in the first 6 days together.**
$$(3 + 2) \times 6 = 30 \text{ units}$$

**Step 4 — Remaining work.**
$$60 - 30 = 30 \text{ units}$$

**Step 5 — Days B needs alone.**
$$\frac{30}{2} = 15 \text{ days}$$

**Answer: 15 more days** (total project duration = 6 + 15 = 21 days)

---

### Example 5 — One worker leaves before completion

**Q.** A can complete a work in 12 days and B in 18 days. They begin together, but A leaves 3 days before the work is finished. Find the total number of days taken.

**Step 1 — Set up.**
$$\text{Work} = \text{LCM}(12, 18) = 36 \text{ units}$$
$$A = 3 \text{ units/day}, \qquad B = 2 \text{ units/day}$$

**Step 2 — Identify who works how long.**
Let the total duration be **T** days.
- **B works the entire time**: T days
- **A leaves 3 days early**: A works (T − 3) days

**Step 3 — Write the work equation.**
$$3(T - 3) + 2T = 36$$

**Step 4 — Solve.**
$$3T - 9 + 2T = 36$$
$$5T = 45$$
$$T = 9 \text{ days}$$

**Verification:**
- A works 9 − 3 = 6 days ⇒ 6 × 3 = 18 units
- B works 9 days ⇒ 9 × 2 = 18 units
- Total = 36 units ✓

**Answer: 9 days**

> **Watch the wording.** "A leaves 3 days before completion" means A works T − 3 days. Contrast with "A works for 3 days then leaves", which is a different (and easier) problem.

---

### Example 6 — Alternate days

**Q.** A can do a work in 12 days and B in 18 days. They work on alternate days, with A starting. In how many days will the work be completed?

**Step 1 — Set up.**
$$\text{Work} = \text{LCM}(12, 18) = 36 \text{ units}$$
$$A = 3 \text{ units/day}, \qquad B = 2 \text{ units/day}$$

**Step 2 — Compute the output of one 2-day cycle.**
$$\text{Day 1 (A)} + \text{Day 2 (B)} = 3 + 2 = 5 \text{ units per 2 days}$$

**Step 3 — How many complete cycles fit?**
$$36 \div 5 = 7 \text{ complete cycles, remainder } 1$$
$$7 \text{ cycles} = 7 \times 5 = 35 \text{ units in } 14 \text{ days}$$

**Step 4 — Handle the leftover.**
1 unit remains. Day 15 is **A's turn** (cycles start with A, so odd days are A's).
A works at 3 units/day, so 1 unit takes:
$$\frac{1}{3} \text{ of a day}$$

**Step 5 — Total.**
$$14 + \frac{1}{3} = 14\tfrac{1}{3} \text{ days}$$

**Answer: 14⅓ days**

> **If B had started instead**, the cycle output would still be 5, but Day 15 would be B's turn (2 units/day), and the leftover unit would take 1/2 day, giving 14½ days. The starting worker matters.

---

### Example 7 — Pipes with an outlet

**Q.** Two pipes can fill a tank in 20 and 30 minutes respectively, while a third pipe can empty the full tank in 40 minutes. If all three are opened together on an empty tank, how long will it take to fill?

**Step 1 — Set the capacity.**
$$\text{Capacity} = \text{LCM}(20, 30, 40) = 120 \text{ units}$$

**Step 2 — Compute rates WITH SIGNS.**
$$\text{Pipe A (inlet)} = \frac{120}{20} = +6 \text{ units/min}$$
$$\text{Pipe B (inlet)} = \frac{120}{30} = +4 \text{ units/min}$$
$$\text{Pipe C (outlet)} = \frac{120}{40} = -3 \text{ units/min}$$

**Step 3 — Net rate.**
$$6 + 4 - 3 = +7 \text{ units/min}$$

Positive ⇒ the tank will fill.

**Step 4 — Time.**
$$\frac{120}{7} = 17\tfrac{1}{7} \text{ minutes} \approx 17.14 \text{ min}$$

**Answer: 120/7 ≈ 17.14 minutes (17 minutes 8.6 seconds)**

**Sanity check:** without the outlet, A and B together would take 120/10 = 12 minutes. Adding a leak must make it *slower*, and 17.14 > 12 ✓

---

### Example 8 — Wages distribution

**Q.** A and B undertake a piece of work for ₹600. A alone can do it in 6 days and B in 8 days. With C's help they finish it in 3 days. Find C's share of the payment.

**Step 1 — Set the total work.**
$$\text{Work} = \text{LCM}(6, 8, 3) = 24 \text{ units}$$

**Step 2 — Compute known rates.**
$$A = \frac{24}{6} = 4 \text{ units/day}$$
$$B = \frac{24}{8} = 3 \text{ units/day}$$
$$A + B + C = \frac{24}{3} = 8 \text{ units/day}$$

**Step 3 — Deduce C's rate.**
$$C = 8 - (4 + 3) = 1 \text{ unit/day}$$

**Step 4 — Wages split in the ratio of work done.**
All three worked the same 3 days, so the ratio of work done equals the ratio of rates:
$$A : B : C = 4 : 3 : 1 \quad (\text{total } 8 \text{ parts})$$

**Step 5 — C's share.**
$$\frac{1}{8} \times 600 = ₹75$$

**Full split:** A = ₹300, B = ₹225, C = ₹75. Total ₹600 ✓

**Answer: ₹75**

> **Principle:** wages follow **work done**, not time spent. A worker who is present but contributes little earns little. If workers put in different numbers of days, weight each by (rate × days worked).

---

## 6. Practice Questions

**Instructions:** 50 questions. Easy (1–20), Medium (21–40), Hard (41–50).
Target times: Easy 30 s · Medium 60 s · Hard 90 s.
Full solutions in [Section 7](#7-detailed-solutions).

### 🟢 EASY (Questions 1–20)

**Q1.** A can complete a work in 10 days. What part of the work does he do in one day?
(a) 1/5  (b) 1/10  (c) 1/20  (d) 10

**Q2.** A can do a work in 12 days and B in 15 days. How long will they take together?
(a) 6 days  (b) 6⅔ days  (c) 7 days  (d) 7½ days

**Q3.** A does one-fourth of a work in 5 days. How long will he take to complete the whole work?
(a) 15 days  (b) 18 days  (c) 20 days  (d) 25 days

**Q4.** A and B together can complete a work in 8 days. A alone takes 12 days. How long will B alone take?
(a) 16 days  (b) 20 days  (c) 24 days  (d) 30 days

**Q5.** A can do a work in 20 days. What fraction of the work is done in 5 days?
(a) 1/5  (b) 1/4  (c) 1/3  (d) 2/5

**Q6.** A pipe can fill a tank in 6 hours. What part of the tank does it fill in one hour?
(a) 1/3  (b) 1/6  (c) 1/12  (d) 6

**Q7.** Two pipes can fill a tank in 12 and 24 hours respectively. How long will they take together?
(a) 6 hours  (b) 8 hours  (c) 9 hours  (d) 18 hours

**Q8.** A is twice as good a workman as B. If B takes 18 days to do a job, how long does A take?
(a) 6 days  (b) 9 days  (c) 12 days  (d) 36 days

**Q9.** 10 men can complete a work in 12 days. How long will 15 men take?
(a) 6 days  (b) 8 days  (c) 9 days  (d) 10 days

**Q10.** A can do a work in 15 days and B in 30 days. How long together?
(a) 8 days  (b) 10 days  (c) 12 days  (d) 15 days

**Q11.** A pipe fills a tank in 8 hours, but a leak empties the full tank in 24 hours. How long will the tank take to fill with the leak present?
(a) 10 hours  (b) 12 hours  (c) 16 hours  (d) 18 hours

**Q12.** If 6 men can complete a work in 9 days, how many men are needed to complete it in 3 days?
(a) 12  (b) 15  (c) 18  (d) 24

**Q13.** A completes three-fifths of a work in 12 days. How many more days will he need to finish it?
(a) 6 days  (b) 8 days  (c) 10 days  (d) 12 days

**Q14.** A and B can do a work in 6 days and 12 days respectively. How long together?
(a) 3 days  (b) 4 days  (c) 5 days  (d) 6 days

**Q15.** A completes a work in 16 days working 8 hours a day. How many hours a day must he work to finish it in 8 days?
(a) 12 hours  (b) 14 hours  (c) 16 hours  (d) 18 hours

**Q16.** The efficiencies of A and B are in the ratio 3 : 2. If A takes 10 days to complete a work, how long does B take?
(a) 12 days  (b) 15 days  (c) 18 days  (d) 20 days

**Q17.** One tap fills a tank in 5 hours and another in 20 hours. How long will both together take?
(a) 3 hours  (b) 4 hours  (c) 5 hours  (d) 12.5 hours

**Q18.** A can complete a work in 24 days. He works for 6 days and then leaves. What fraction of the work remains?
(a) 1/4  (b) 1/2  (c) 2/3  (d) 3/4

**Q19.** 4 women can complete a work in 20 days. How long will one woman take?
(a) 40 days  (b) 60 days  (c) 80 days  (d) 100 days

**Q20.** A, B and C can complete a work in 10, 20 and 30 days respectively. How long will they take together?
(a) 5 5/11 days  (b) 6 days  (c) 6 6/11 days  (d) 7 days

---

### 🟡 MEDIUM (Questions 21–40)

**Q21.** A and B can do a work in 12 days, B and C in 15 days, and C and A in 20 days. In how many days can all three together complete it?
(a) 8 days  (b) 9 days  (c) 10 days  (d) 12 days

**Q22.** Using the data of Q21, how many days will A alone take?
(a) 20 days  (b) 24 days  (c) 30 days  (d) 60 days

**Q23.** A can do a work in 20 days and B in 30 days. They work together for 6 days, after which A leaves. How many more days will B need to finish?
(a) 10 days  (b) 12 days  (c) 15 days  (d) 18 days

**Q24.** 12 men can complete a work in 18 days. After 6 days of work, 4 more men join them. In how many more days will the work be completed?
(a) 7 days  (b) 8 days  (c) 9 days  (d) 10 days

**Q25.** A is 25% more efficient than B. If B alone takes 20 days, how long will A and B take together?
(a) 8 days  (b) 8 8/9 days  (c) 9 days  (d) 10 days

**Q26.** Two pipes A and B can fill a tank in 20 and 30 minutes respectively. Both are opened together, but B is closed after 10 minutes. Find the total time to fill the tank.
(a) 12 min  (b) 13⅓ min  (c) 14 min  (d) 15 min

**Q27.** Pipes A and B can fill a tank in 12 and 16 hours respectively, while pipe C can empty it in 24 hours. If all three are opened, how long will the tank take to fill?
(a) 8.4 hours  (b) 9.6 hours  (c) 10.2 hours  (d) 11 hours

**Q28.** A can do a work in 30 days and B in 40 days. They work on alternate days with A starting. In how many days will the work be completed?
(a) 33.5 days  (b) 34 days  (c) 34.25 days  (d) 35 days

**Q29.** 8 men or 12 women can complete a work in 10 days. How long will 4 men and 4 women take?
(a) 10 days  (b) 12 days  (c) 14 days  (d) 15 days

**Q30.** A does half as much work as B in three-fourths of the time. If together they complete the work in 18 days, how long will B alone take?
(a) 25 days  (b) 30 days  (c) 36 days  (d) 45 days

**Q31.** A leak can empty a cistern in 20 hours. A tap admitting 4 litres per minute is opened, and the cistern is now emptied in 24 hours. Find the capacity of the cistern.
(a) 24,000 L  (b) 26,400 L  (c) 28,800 L  (d) 30,000 L

**Q32.** A can complete a work in 12 days and B in 18 days. They start together, but A leaves 3 days before completion. Find the total number of days taken.
(a) 8 days  (b) 9 days  (c) 10 days  (d) 11 days

**Q33.** Two pipes can fill a tank in 15 and 20 hours respectively. Both are opened together, but the first is closed after some time, and the tank fills in 12 hours in total. After how long was the first pipe closed?
(a) 4 hours  (b) 5 hours  (c) 6 hours  (d) 8 hours

**Q34.** 2 men and 4 boys can complete a work in 6 days, while 4 men and 4 boys can complete it in 4 days. How long will 1 man and 2 boys take?
(a) 8 days  (b) 10 days  (c) 12 days  (d) 16 days

**Q35.** A contractor undertakes to finish a work in 40 days and employs 30 men. After 25 days only half the work is done. How many additional men must he employ to finish on time?
(a) 15  (b) 20  (c) 25  (d) 30

**Q36.** Pipes A and B can fill a tank in 24 and 32 minutes respectively. Both are opened together. After how long should B be closed so that the tank fills in exactly 18 minutes?
(a) 6 min  (b) 8 min  (c) 10 min  (d) 12 min

**Q37.** A, B and C can complete a work in 20, 30 and 60 days respectively. In how many days can A complete the work if he is assisted by B and C on every third day?
(a) 12 days  (b) 15 days  (c) 16 days  (d) 18 days

**Q38.** A tank has two inlet pipes that can fill it in 10 and 12 hours, and an outlet pipe that can empty it in 20 hours. If all three are opened on an empty tank, how long will it take to fill?
(a) 6 hours  (b) 7 hours  (c) 7.5 hours  (d) 8 hours

**Q39.** A and B undertake a work for ₹600. A alone can do it in 6 days and B in 8 days. With C's help they finish it in 3 days. Find C's share.
(a) ₹60  (b) ₹75  (c) ₹90  (d) ₹100

**Q40.** If 15 men working 8 hours a day can complete a work in 12 days, how many days will 20 men working 9 hours a day take?
(a) 6 days  (b) 8 days  (c) 9 days  (d) 10 days

---

### 🔴 HARD (Questions 41–50)

**Q41.** A can complete a work in 12 days and B in 18 days. They work on alternate days with A starting. Find the total time taken.
(a) 14 days  (b) 14⅓ days  (c) 14½ days  (d) 15 days

**Q42.** Pipes A and B can fill a tank in 20 and 30 minutes respectively, and pipe C can empty it in 40 minutes. All three are opened together, and C is closed after 10 minutes. Find the total time to fill the tank.
(a) 13 min  (b) 14 min  (c) 15 min  (d) 16 min

**Q43.** 20 men can complete a work in 30 days. After 12 days, 8 men leave. How many more days will the remaining men take to complete the work?
(a) 24 days  (b) 27 days  (c) 30 days  (d) 33 days

**Q44.** A works twice as fast as B, and B works three times as fast as C. Working together they complete a job in 6 days. How long would C alone take?
(a) 40 days  (b) 50 days  (c) 60 days  (d) 72 days

**Q45.** A cistern can be filled by three pipes in 6, 8 and 12 hours respectively. All three are opened, but the first is closed after 2 hours. Find the total time to fill the cistern.
(a) 3 hours  (b) 3 h 12 min  (c) 3 h 30 min  (d) 4 hours

**Q46.** A contractor employs 40 men to complete a job in 60 days. After 30 days only 40% of the work is done. How many more men must he employ to finish on schedule?
(a) 15  (b) 20  (c) 25  (d) 30

**Q47.** Pipe A can fill a tank in 12 minutes and pipe B can empty it in 18 minutes. If the tank is already one-third full and both pipes are opened, how long will it take to fill completely?
(a) 20 min  (b) 24 min  (c) 28 min  (d) 36 min

**Q48.** A and B can do a work in 12 days, B and C in 15 days, and A and C in 20 days. How long would C alone take?
(a) 30 days  (b) 40 days  (c) 50 days  (d) 60 days

**Q49.** A tap can fill a tank in 6 hours. After half the tank is filled, three more taps of the same capacity are opened. Find the total time to fill the tank.
(a) 3 h 15 min  (b) 3 h 30 min  (c) 3 h 45 min  (d) 4 h 15 min

**Q50.** 3 men and 7 women can complete a work in 10 days, while 4 men and 6 women can complete it in 8 days. In how many days can 10 women alone complete the work?
(a) 30 days  (b) 35 days  (c) 40 days  (d) 45 days

---

## 7. Detailed Solutions

### 🟢 EASY — Solutions 1–20

---

**Q1. A completes a work in 10 days. One day's work? → (b) 1/10**

**Formula used:** One day's work = 1/n

$$\frac{1}{10}$$

**Answer: (b) 1/10**

---

**Q2. A in 12 days, B in 15 days. Together? → (b) 6⅔ days**

**LCM method:**

**Step 1 — Total work.**
$$\text{LCM}(12, 15) = 60 \text{ units}$$

**Step 2 — Rates.**
$$A = \frac{60}{12} = 5 \text{ units/day}, \qquad B = \frac{60}{15} = 4 \text{ units/day}$$

**Step 3 — Combined.**
$$5 + 4 = 9 \text{ units/day}$$

**Step 4 — Time.**
$$\frac{60}{9} = \frac{20}{3} = 6\tfrac{2}{3} \text{ days}$$

**Formula check:** ab/(a+b) = (12 × 15)/27 = 180/27 = 20/3 ✓

**Answer: (b) 6⅔ days**

---

**Q3. A does ¼ of a work in 5 days. Whole work? → (c) 20 days**

If one-quarter takes 5 days, the whole takes:
$$5 \times 4 = 20 \text{ days}$$

**Answer: (c) 20 days**

---

**Q4. A+B in 8 days; A alone in 12. B alone? → (c) 24 days**

**Step 1 — Total work.**
$$\text{LCM}(8, 12) = 24 \text{ units}$$

**Step 2 — Rates.**
$$A + B = \frac{24}{8} = 3 \text{ units/day}$$
$$A = \frac{24}{12} = 2 \text{ units/day}$$

**Step 3 — Subtract the rates (not the times).**
$$B = 3 - 2 = 1 \text{ unit/day}$$

**Step 4 — B's time.**
$$\frac{24}{1} = 24 \text{ days}$$

> **Trap:** subtracting times, 12 − 8 = 4 days. Rates subtract; times do not.

**Answer: (c) 24 days**

---

**Q5. A in 20 days. Fraction done in 5 days? → (b) 1/4**

$$\frac{5}{20} = \frac{1}{4}$$

**Answer: (b) 1/4**

---

**Q6. Pipe fills a tank in 6 hours. Part filled in 1 hour? → (b) 1/6**

$$\frac{1}{6}$$

**Answer: (b) 1/6**

---

**Q7. Pipes fill in 12 and 24 hours. Together? → (b) 8 hours**

**Step 1 — Capacity.**
$$\text{LCM}(12, 24) = 24 \text{ units}$$

**Step 2 — Rates.**
$$P_1 = 2 \text{ units/h}, \qquad P_2 = 1 \text{ unit/h}$$

**Step 3 — Combined and time.**
$$3 \text{ units/h} \implies \frac{24}{3} = 8 \text{ hours}$$

**Formula check:** (12 × 24)/36 = 288/36 = 8 ✓

**Answer: (b) 8 hours**

---

**Q8. A is twice as good as B; B takes 18 days. A? → (b) 9 days**

**Concept:** efficiency and time are inversely proportional.

Efficiency A : B = 2 : 1 ⇒ Time A : B = 1 : 2.
$$T_A = \frac{18}{2} = 9 \text{ days}$$

**Answer: (b) 9 days**

---

**Q9. 10 men in 12 days. 15 men? → (b) 8 days**

**Formula used:** M₁D₁ = M₂D₂

$$10 \times 12 = 15 \times D$$
$$D = \frac{120}{15} = 8 \text{ days}$$

**Sanity check:** more men ⇒ fewer days ✓

**Answer: (b) 8 days**

---

**Q10. A in 15 days, B in 30 days. Together? → (b) 10 days**

**Step 1 — Work = LCM(15, 30) = 30 units**

**Step 2 — Rates:** A = 2, B = 1 ⇒ combined = 3 units/day

**Step 3 — Time:** 30/3 = **10 days**

**Formula check:** (15 × 30)/45 = 450/45 = 10 ✓

**Answer: (b) 10 days**

---

**Q11. Fills in 8 h; leak empties in 24 h. Time with leak? → (b) 12 hours**

**Step 1 — Capacity = LCM(8, 24) = 24 units**

**Step 2 — Rates with signs.**
$$\text{Inlet} = +3 \text{ units/h}, \qquad \text{Leak} = -1 \text{ unit/h}$$

**Step 3 — Net rate.**
$$3 - 1 = +2 \text{ units/h}$$

**Step 4 — Time.**
$$\frac{24}{2} = 12 \text{ hours}$$

**Sanity check:** 12 > 8, so the leak slowed it down ✓

**Answer: (b) 12 hours**

---

**Q12. 6 men in 9 days. How many for 3 days? → (c) 18**

**Formula used:** M₁D₁ = M₂D₂

$$6 \times 9 = M \times 3$$
$$M = \frac{54}{3} = 18 \text{ men}$$

**Answer: (c) 18**

---

**Q13. A does 3/5 of a work in 12 days. Days for the rest? → (b) 8 days**

**Step 1 — Find the daily rate.**
$$\frac{3/5}{12} = \frac{3}{60} = \frac{1}{20} \text{ of the work per day}$$

**Step 2 — Remaining work.**
$$1 - \frac{3}{5} = \frac{2}{5}$$

**Step 3 — Days needed.**
$$\frac{2/5}{1/20} = \frac{2}{5} \times 20 = 8 \text{ days}$$

**⚡ Proportional shortcut:** 3/5 took 12 days, so 1/5 takes 4 days, and 2/5 takes **8 days** ✓

**Answer: (b) 8 days**

---

**Q14. A in 6 days, B in 12 days. Together? → (b) 4 days**

**Formula used:** ab/(a+b)

$$\frac{6 \times 12}{18} = \frac{72}{18} = 4 \text{ days}$$

**Answer: (b) 4 days**

---

**Q15. 16 days at 8 h/day. Hours/day to finish in 8 days? → (c) 16 hours**

**Formula used:** D₁H₁ = D₂H₂

$$16 \times 8 = 8 \times H$$
$$H = \frac{128}{8} = 16 \text{ hours/day}$$

**Answer: (c) 16 hours**

---

**Q16. Efficiency A : B = 3 : 2; A takes 10 days. B? → (b) 15 days**

**Concept:** time ratio is the inverse of the efficiency ratio.

$$E_A : E_B = 3 : 2 \implies T_A : T_B = 2 : 3$$
$$\frac{10}{T_B} = \frac{2}{3} \implies T_B = 15 \text{ days}$$

**Sanity check:** B is less efficient, so B must take *longer* — 15 > 10 ✓

**Answer: (b) 15 days**

---

**Q17. Taps fill in 5 and 20 hours. Together? → (b) 4 hours**

**Step 1 — Capacity = LCM(5, 20) = 20 units**

**Step 2 — Rates:** 4 and 1 ⇒ combined = 5 units/h

**Step 3 — Time:** 20/5 = **4 hours**

**Answer: (b) 4 hours**

---

**Q18. A in 24 days; works 6 days. Fraction remaining? → (d) 3/4**

**Step 1 — Fraction done.**
$$\frac{6}{24} = \frac{1}{4}$$

**Step 2 — Fraction remaining.**
$$1 - \frac{1}{4} = \frac{3}{4}$$

**Answer: (d) 3/4**

---

**Q19. 4 women in 20 days. One woman? → (c) 80 days**

**Formula used:** M₁D₁ = M₂D₂

$$4 \times 20 = 1 \times D \implies D = 80 \text{ days}$$

**Answer: (c) 80 days**

---

**Q20. A, B, C in 10, 20, 30 days. Together? → (a) 5 5/11 days**

**Step 1 — Work = LCM(10, 20, 30) = 60 units**

**Step 2 — Rates.**
$$A = 6, \qquad B = 3, \qquad C = 2 \text{ units/day}$$

**Step 3 — Combined.**
$$6 + 3 + 2 = 11 \text{ units/day}$$

**Step 4 — Time.**
$$\frac{60}{11} = 5\tfrac{5}{11} \text{ days}$$

**Sanity check:** must be less than 10 (the fastest worker's time) ✓

**Answer: (a) 5 5/11 days**

---

### 🟡 MEDIUM — Solutions 21–40

---

**Q21. A+B = 12, B+C = 15, C+A = 20. All three? → (c) 10 days**

**Formula used:** (A+B) + (B+C) + (C+A) = 2(A+B+C)

**Step 1 — Work = LCM(12, 15, 20) = 60 units**

**Step 2 — Pair rates.**
$$A + B = \frac{60}{12} = 5 \qquad B + C = \frac{60}{15} = 4 \qquad C + A = \frac{60}{20} = 3$$

**Step 3 — Sum and halve.**
$$2(A+B+C) = 5 + 4 + 3 = 12 \implies A+B+C = 6 \text{ units/day}$$

**Step 4 — Time.**
$$\frac{60}{6} = 10 \text{ days}$$

> **The single most important step is halving.** Forgetting it yields 5 days, which is offered as a trap in many versions of this question.

**Answer: (c) 10 days**

---

**Q22. From Q21, A alone? → (c) 30 days**

**Formula used:** A = (A+B+C) − (B+C)

**Step 1 — From Q21:** A + B + C = 6 units/day, and B + C = 4 units/day.

**Step 2 — Isolate A.**
$$A = 6 - 4 = 2 \text{ units/day}$$

**Step 3 — A's time.**
$$\frac{60}{2} = 30 \text{ days}$$

**Cross-check the whole trio:**
$$B = 6 - 3 = 3 \implies T_B = 20 \text{ days}$$
$$C = 6 - 5 = 1 \implies T_C = 60 \text{ days}$$
Verify: A + B = 2 + 3 = 5 ✓ · B + C = 3 + 1 = 4 ✓ · C + A = 1 + 2 = 3 ✓

**Answer: (c) 30 days**

---

**Q23. A in 20, B in 30; together 6 days, then A leaves. B needs? → (c) 15 days**

**Step 1 — Work = LCM(20, 30) = 60 units**

**Step 2 — Rates.**
$$A = 3, \qquad B = 2 \text{ units/day}$$

**Step 3 — Work done together in 6 days.**
$$(3 + 2) \times 6 = 30 \text{ units}$$

**Step 4 — Remaining.**
$$60 - 30 = 30 \text{ units}$$

**Step 5 — Days for B alone.**
$$\frac{30}{2} = 15 \text{ days}$$

**Answer: (c) 15 days**

---

**Q24. 12 men, 18 days; after 6 days 4 more join. More days? → (c) 9 days**

**Step 1 — Total work in man-days.**
$$12 \times 18 = 216 \text{ man-days}$$

**Step 2 — Work done in the first 6 days.**
$$12 \times 6 = 72 \text{ man-days}$$

**Step 3 — Remaining work.**
$$216 - 72 = 144 \text{ man-days}$$

**Step 4 — Now there are 16 men.**
$$\frac{144}{16} = 9 \text{ days}$$

**Verification:** 72 + (16 × 9) = 72 + 144 = 216 ✓

**Answer: (c) 9 days**

---

**Q25. A is 25% more efficient than B; B takes 20 days. Together? → (b) 8 8/9 days**

**Step 1 — Convert efficiency to time.**
$$E_A : E_B = 125 : 100 = 5 : 4 \implies T_A : T_B = 4 : 5$$
$$T_A = 20 \times \frac{4}{5} = 16 \text{ days}$$

**Step 2 — Combined time.**
$$T = \frac{16 \times 20}{16 + 20} = \frac{320}{36} = \frac{80}{9} = 8\tfrac{8}{9} \text{ days}$$

**LCM cross-check:** Work = LCM(16, 20) = 80 units. A = 5, B = 4 ⇒ combined 9 units/day ⇒ 80/9 days ✓

**Answer: (b) 8 8/9 days**

---

**Q26. A (20 min), B (30 min) both open; B closed after 10 min. Total time? → (b) 13⅓ min**

**Step 1 — Capacity = LCM(20, 30) = 60 units**

**Step 2 — Rates.**
$$A = 3 \text{ units/min}, \qquad B = 2 \text{ units/min}$$

**Step 3 — First 10 minutes with both pipes.**
$$(3 + 2) \times 10 = 50 \text{ units}$$

**Step 4 — Remaining.**
$$60 - 50 = 10 \text{ units}$$

**Step 5 — A alone finishes.**
$$\frac{10}{3} = 3\tfrac{1}{3} \text{ minutes}$$

**Step 6 — Total.**
$$10 + 3\tfrac{1}{3} = 13\tfrac{1}{3} \text{ minutes}$$

**Answer: (b) 13⅓ min**

---

**Q27. A (12 h), B (16 h) fill; C (24 h) empties. All open. Time? → (b) 9.6 hours**

**Step 1 — Capacity = LCM(12, 16, 24) = 48 units**

**Step 2 — Rates with signs.**
$$A = +4, \qquad B = +3, \qquad C = -2 \text{ units/h}$$

**Step 3 — Net rate.**
$$4 + 3 - 2 = +5 \text{ units/h}$$

**Step 4 — Time.**
$$\frac{48}{5} = 9.6 \text{ hours}$$

**Sanity check:** without C, A and B would take 48/7 ≈ 6.86 h. Adding the outlet must slow it, and 9.6 > 6.86 ✓

**Answer: (b) 9.6 hours**

---

**Q28. A (30 days), B (40 days), alternate days, A starts. Total? → (c) 34.25 days**

**Step 1 — Work = LCM(30, 40) = 120 units**

**Step 2 — Rates.**
$$A = 4 \text{ units/day}, \qquad B = 3 \text{ units/day}$$

**Step 3 — Output of one 2-day cycle.**
$$4 + 3 = 7 \text{ units per 2 days}$$

**Step 4 — Number of complete cycles.**
$$120 \div 7 = 17 \text{ cycles, remainder } 1$$
$$17 \text{ cycles} = 119 \text{ units in } 34 \text{ days}$$

**Step 5 — Handle the leftover.**
1 unit remains. Day 35 is **A's turn** (A starts, so odd days are A's).
$$\text{Time needed} = \frac{1}{4} \text{ day}$$

**Step 6 — Total.**
$$34 + 0.25 = 34.25 \text{ days}$$

**Answer: (c) 34.25 days**

---

**Q29. 8 men or 12 women in 10 days. 4 men + 4 women? → (b) 12 days**

**Step 1 — Establish the equivalence.**
$$8 \text{ men} \equiv 12 \text{ women} \implies 1 \text{ man} \equiv 1.5 \text{ women}$$

**Step 2 — Express the total work in woman-days.**
$$12 \text{ women} \times 10 \text{ days} = 120 \text{ woman-days}$$

**Step 3 — Convert the new team to woman-equivalents.**
$$4 \text{ men} = 4 \times 1.5 = 6 \text{ women}$$
$$\text{Team} = 6 + 4 = 10 \text{ women-equivalent}$$

**Step 4 — Time.**
$$\frac{120}{10} = 12 \text{ days}$$

**Cross-check in man-days:** total = 8 × 10 = 80 man-days. Team = 4 men + 4 women = 4 + 4/1.5 = 4 + 2.667 = 6.667 men. 80/6.667 = 12 days ✓

**Answer: (b) 12 days**

---

**Q30. A does half as much work as B in three-fourths of the time; together 18 days. B alone? → (b) 30 days**

**Step 1 — Translate the statement carefully.**
Take any time interval *t*. In time *t*, B does an amount of work $R_B \cdot t$.

The statement says A does **half that amount** in **three-quarters of the time**:
$$R_A \times \frac{3t}{4} = \frac{1}{2}\left(R_B \times t\right)$$

**Step 2 — Solve for A's rate.**
$$R_A = \frac{1}{2}R_B \times \frac{4}{3} = \frac{2}{3}R_B$$

**Step 3 — Use the combined-time condition.**
$$R_A + R_B = \frac{1}{18}$$
$$\frac{2}{3}R_B + R_B = \frac{5}{3}R_B = \frac{1}{18}$$

**Step 4 — Solve.**
$$R_B = \frac{3}{5 \times 18} = \frac{1}{30}$$
$$T_B = 30 \text{ days}$$

**Verification:**
$$R_A = \frac{2}{3} \times \frac{1}{30} = \frac{1}{45} \implies T_A = 45 \text{ days}$$
$$\frac{1}{45} + \frac{1}{30} = \frac{2}{90} + \frac{3}{90} = \frac{5}{90} = \frac{1}{18} \checkmark$$

**Answer: (b) 30 days**

---

**Q31. Leak empties in 20 h; with a 4 L/min tap, 24 h. Capacity? → (c) 28,800 L**

**Step 1 — Write the rates as fractions of the tank per hour.**
$$\text{Leak (emptying)} = \frac{1}{20} \text{ per hour}$$
$$\text{Net emptying with the tap on} = \frac{1}{24} \text{ per hour}$$

**Step 2 — Isolate the tap's fill rate.**
The tap partly offsets the leak:
$$\text{Tap} = \frac{1}{20} - \frac{1}{24} = \frac{6 - 5}{120} = \frac{1}{120} \text{ per hour}$$

So the tap alone would fill the cistern in **120 hours**.

**Step 3 — Convert the flow rate to litres per hour.**
$$4 \text{ L/min} \times 60 = 240 \text{ L/hour}$$

**Step 4 — Capacity.**
$$240 \times 120 = 28{,}800 \text{ litres}$$

**Verification:**
- Leak drains 28,800 L in 20 h ⇒ 1,440 L/h
- Tap adds 240 L/h ⇒ net drain = 1,200 L/h
- Time to empty = 28,800/1,200 = **24 hours** ✓

**Answer: (c) 28,800 L**

---

**Q32. A (12 days), B (18 days); A leaves 3 days before completion. Total? → (b) 9 days**

**Step 1 — Work = LCM(12, 18) = 36 units**

**Step 2 — Rates.**
$$A = 3, \qquad B = 2 \text{ units/day}$$

**Step 3 — Set up the durations.**
Let the total be **T** days.
- B works all **T** days
- A works **(T − 3)** days

**Step 4 — Write the work equation.**
$$3(T - 3) + 2T = 36$$
$$3T - 9 + 2T = 36$$
$$5T = 45 \implies T = 9 \text{ days}$$

**Verification:**
- A works 6 days ⇒ 18 units
- B works 9 days ⇒ 18 units
- Total = 36 ✓

**Answer: (b) 9 days**

---

**Q33. Pipes (15 h, 20 h) both open; first closed early; tank fills in 12 h. When was it closed? → (c) 6 hours**

**Step 1 — Capacity = LCM(15, 20) = 60 units**

**Step 2 — Rates.**
$$P_1 = 4 \text{ units/h}, \qquad P_2 = 3 \text{ units/h}$$

**Step 3 — The second pipe runs the whole 12 hours.**
$$3 \times 12 = 36 \text{ units}$$

**Step 4 — The first pipe supplies the rest.**
$$60 - 36 = 24 \text{ units}$$

**Step 5 — Time the first pipe ran.**
$$\frac{24}{4} = 6 \text{ hours}$$

**Answer: (c) 6 hours** *(closed after 6 hours)*

---

**Q34. 2 men + 4 boys in 6 days; 4 men + 4 boys in 4 days. 1 man + 2 boys? → (c) 12 days**

**Step 1 — Write the two rate equations.**
Let *m* and *b* be the daily work rates of one man and one boy.
$$2m + 4b = \frac{1}{6} \qquad \text{...(i)}$$
$$4m + 4b = \frac{1}{4} \qquad \text{...(ii)}$$

**Step 2 — Subtract (i) from (ii) to eliminate the boys.**
$$2m = \frac{1}{4} - \frac{1}{6} = \frac{3 - 2}{12} = \frac{1}{12}$$
$$m = \frac{1}{24}$$

**Step 3 — Substitute back into (i).**
$$2\left(\frac{1}{24}\right) + 4b = \frac{1}{6}$$
$$\frac{1}{12} + 4b = \frac{1}{6}$$
$$4b = \frac{1}{6} - \frac{1}{12} = \frac{1}{12} \implies b = \frac{1}{48}$$

**Step 4 — Compute the required team's rate.**
$$1m + 2b = \frac{1}{24} + \frac{2}{48} = \frac{1}{24} + \frac{1}{24} = \frac{1}{12}$$

**Step 5 — Time.**
$$T = 12 \text{ days}$$

**Interpretation:** one man alone takes 24 days; one boy alone takes 48 days — so a man works exactly twice as fast as a boy.

**Verification of (ii):** 4(1/24) + 4(1/48) = 1/6 + 1/12 = 3/12 = 1/4 ✓

**Answer: (c) 12 days**

---

**Q35. 40-day contract, 30 men; after 25 days half is done. Additional men? → (b) 20**

**Step 1 — Convert the completed portion into man-days.**
$$30 \text{ men} \times 25 \text{ days} = 750 \text{ man-days} = \text{half the job}$$

**Step 2 — Size the whole job.**
$$\text{Total} = 750 \times 2 = 1{,}500 \text{ man-days}$$

**Step 3 — Remaining work and remaining time.**
$$\text{Remaining work} = 750 \text{ man-days}$$
$$\text{Remaining time} = 40 - 25 = 15 \text{ days}$$

**Step 4 — Men required.**
$$\frac{750}{15} = 50 \text{ men}$$

**Step 5 — Additional men.**
$$50 - 30 = 20$$

**Answer: (b) 20**

---

**Q36. A (24 min), B (32 min); when to close B so the tank fills in 18 min? → (b) 8 min**

**Step 1 — Capacity = LCM(24, 32) = 96 units**

**Step 2 — Rates.**
$$A = 4 \text{ units/min}, \qquad B = 3 \text{ units/min}$$

**Step 3 — A runs the whole 18 minutes.**
$$4 \times 18 = 72 \text{ units}$$

**Step 4 — B must supply the remainder.**
$$96 - 72 = 24 \text{ units}$$

**Step 5 — Time B must run.**
$$\frac{24}{3} = 8 \text{ minutes}$$

**Verification:** In 8 min both pipes deliver (4+3)×8 = 56 units. In the remaining 10 min, A alone delivers 40 units. Total = 96 ✓

**Answer: (b) 8 min** *(B is closed after 8 minutes)*

---

**Q37. A (20), B (30), C (60) days; B and C assist A every third day. Total? → (b) 15 days**

**Step 1 — Work = LCM(20, 30, 60) = 60 units**

**Step 2 — Rates.**
$$A = 3, \qquad B = 2, \qquad C = 1 \text{ unit/day}$$

**Step 3 — Model a 3-day cycle.**
- Day 1: A alone ⇒ 3 units
- Day 2: A alone ⇒ 3 units
- Day 3: A + B + C ⇒ 3 + 2 + 1 = 6 units

$$\text{Cycle output} = 3 + 3 + 6 = 12 \text{ units per 3 days}$$

**Step 4 — Number of cycles.**
$$\frac{60}{12} = 5 \text{ complete cycles}$$

**Step 5 — Total days.**
$$5 \times 3 = 15 \text{ days}$$

**Verification:** 5 cycles × 12 units = 60 units — exactly the whole job, with no remainder ✓

**Answer: (b) 15 days**

---

**Q38. Inlets (10 h, 12 h), outlet (20 h). All open. Time to fill? → (c) 7.5 hours**

**Step 1 — Capacity = LCM(10, 12, 20) = 60 units**

**Step 2 — Rates with signs.**
$$P_1 = +6, \qquad P_2 = +5, \qquad \text{Outlet} = -3 \text{ units/h}$$

**Step 3 — Net rate.**
$$6 + 5 - 3 = +8 \text{ units/h}$$

**Step 4 — Time.**
$$\frac{60}{8} = 7.5 \text{ hours}$$

**Answer: (c) 7.5 hours**

---

**Q39. A (6 d), B (8 d); with C they finish in 3 days; total wage ₹600. C's share? → (b) ₹75**

**Step 1 — Work = LCM(6, 8, 3) = 24 units**

**Step 2 — Compute the known rates.**
$$A = \frac{24}{6} = 4 \text{ units/day}$$
$$B = \frac{24}{8} = 3 \text{ units/day}$$
$$A + B + C = \frac{24}{3} = 8 \text{ units/day}$$

**Step 3 — Deduce C's rate.**
$$C = 8 - 7 = 1 \text{ unit/day}$$

**Step 4 — Wages split by work done.**
All three worked the same 3 days, so the wage ratio equals the rate ratio:
$$A : B : C = 4 : 3 : 1 \quad (\text{8 parts total})$$

**Step 5 — C's share.**
$$\frac{1}{8} \times 600 = ₹75$$

**Full split:** A ₹300, B ₹225, C ₹75 — total ₹600 ✓

**Answer: (b) ₹75**

---

**Q40. 15 men, 8 h/day, 12 days → 20 men, 9 h/day. Days? → (b) 8 days**

**Formula used:** M₁D₁H₁ = M₂D₂H₂

**Step 1 — Compute the total man-hours.**
$$15 \times 8 \times 12 = 1{,}440 \text{ man-hours}$$

**Step 2 — Compute the new team's daily output.**
$$20 \times 9 = 180 \text{ man-hours per day}$$

**Step 3 — Days required.**
$$\frac{1440}{180} = 8 \text{ days}$$

**Answer: (b) 8 days**

---

### 🔴 HARD — Solutions 41–50

---

**Q41. A (12 d), B (18 d) on alternate days, A starting. Total? → (b) 14⅓ days**

**Step 1 — Work = LCM(12, 18) = 36 units**

**Step 2 — Rates.**
$$A = 3 \text{ units/day}, \qquad B = 2 \text{ units/day}$$

**Step 3 — Output per 2-day cycle.**
$$3 + 2 = 5 \text{ units}$$

**Step 4 — Complete cycles.**
$$36 \div 5 = 7 \text{ cycles, remainder } 1$$
$$7 \text{ cycles} = 35 \text{ units completed in } 14 \text{ days}$$

**Step 5 — The final fractional day.**
1 unit remains. Since **A started**, the odd-numbered days belong to A — so day 15 is A's.
$$\text{Time for 1 unit at 3 units/day} = \frac{1}{3} \text{ day}$$

**Step 6 — Total.**
$$14 + \frac{1}{3} = 14\tfrac{1}{3} \text{ days}$$

**Audit of the first 14 days.** They comprise 7 A-days and 7 B-days:
$$7(3) + 7(2) = 21 + 14 = 35 \text{ units} \checkmark$$

| Day | Worker | Units done | Cumulative |
|---|---|---|---|
| 13 | A | 3 | 33 |
| 14 | B | 2 | 35 |
| 15 (partial) | A | 1 needed (of his 3) | **36** ✓ |

**Answer: (b) 14⅓ days**

> **If B had started**, day 15 would be B's (2 units/day), and the last unit would take **½ day**, giving 14½ days. Always check who starts.

---

**Q42. A (20), B (30) fill; C (40) empties. All open; C closed after 10 min. Total? → (c) 15 min**

**Step 1 — Capacity = LCM(20, 30, 40) = 120 units**

**Step 2 — Rates with signs.**
$$A = +6, \qquad B = +4, \qquad C = -3 \text{ units/min}$$

**Step 3 — First 10 minutes (all three open).**
$$\text{Net rate} = 6 + 4 - 3 = +7 \text{ units/min}$$
$$\text{Filled} = 7 \times 10 = 70 \text{ units}$$

**Step 4 — Remaining after C is closed.**
$$120 - 70 = 50 \text{ units}$$

**Step 5 — Now only A and B run.**
$$\text{Rate} = 6 + 4 = 10 \text{ units/min}$$
$$\text{Time} = \frac{50}{10} = 5 \text{ minutes}$$

**Step 6 — Total.**
$$10 + 5 = 15 \text{ minutes}$$

**Answer: (c) 15 min**

---

**Q43. 20 men, 30 days; after 12 days 8 leave. More days? → (c) 30 days**

**Step 1 — Total work in man-days.**
$$20 \times 30 = 600 \text{ man-days}$$

**Step 2 — Work completed in 12 days.**
$$20 \times 12 = 240 \text{ man-days}$$

**Step 3 — Remaining work.**
$$600 - 240 = 360 \text{ man-days}$$

**Step 4 — Remaining workforce.**
$$20 - 8 = 12 \text{ men}$$

**Step 5 — Days needed.**
$$\frac{360}{12} = 30 \text{ days}$$

**Verification:** 240 + (12 × 30) = 240 + 360 = 600 man-days ✓

**Note:** the total project now runs 12 + 30 = 42 days — twelve days late. Losing 40% of the workforce halfway through nearly doubles the remaining schedule, because only 60% of the work was left but only 60% of the men remain.

**Answer: (c) 30 days**

---

**Q44. A is twice as fast as B; B is thrice as fast as C; together 6 days. C alone? → (c) 60 days**

**Step 1 — Express all rates in terms of C.**
Let C's rate = **1 unit/day**.
$$B = 3 \times C = 3 \text{ units/day}$$
$$A = 2 \times B = 6 \text{ units/day}$$

**Step 2 — Combined rate.**
$$6 + 3 + 1 = 10 \text{ units/day}$$

**Step 3 — Size the job from the given combined time.**
$$\text{Total work} = 10 \times 6 = 60 \text{ units}$$

**Step 4 — C's time alone.**
$$\frac{60}{1} = 60 \text{ days}$$

**Cross-check:** A takes 60/6 = 10 days; B takes 60/3 = 20 days; C takes 60 days.
$$\frac{1}{10} + \frac{1}{20} + \frac{1}{60} = \frac{6 + 3 + 1}{60} = \frac{10}{60} = \frac{1}{6} \implies 6 \text{ days} \checkmark$$

**Answer: (c) 60 days**

---

**Q45. Pipes (6, 8, 12 h); first closed after 2 hours. Total time? → (b) 3 h 12 min**

**Step 1 — Capacity = LCM(6, 8, 12) = 24 units**

**Step 2 — Rates.**
$$P_1 = 4, \qquad P_2 = 3, \qquad P_3 = 2 \text{ units/h}$$

**Step 3 — First 2 hours, all three open.**
$$\text{Rate} = 4 + 3 + 2 = 9 \text{ units/h}$$
$$\text{Filled} = 9 \times 2 = 18 \text{ units}$$

**Step 4 — Remaining.**
$$24 - 18 = 6 \text{ units}$$

**Step 5 — P₂ and P₃ continue.**
$$\text{Rate} = 3 + 2 = 5 \text{ units/h}$$
$$\text{Time} = \frac{6}{5} = 1.2 \text{ hours} = 1 \text{ h } 12 \text{ min}$$

**Step 6 — Total.**
$$2 \text{ h} + 1 \text{ h } 12 \text{ min} = 3 \text{ h } 12 \text{ min}$$

**Answer: (b) 3 h 12 min**

---

**Q46. 40 men, 60 days; after 30 days 40% done. More men? → (b) 20**

**Step 1 — Convert the completed portion into man-days.**
$$40 \times 30 = 1{,}200 \text{ man-days} = 40\% \text{ of the job}$$

**Step 2 — Size the whole job.**
$$\text{Total} = \frac{1{,}200}{0.40} = 3{,}000 \text{ man-days}$$

**Step 3 — Remaining work and time.**
$$\text{Remaining} = 3{,}000 - 1{,}200 = 1{,}800 \text{ man-days}$$
$$\text{Time left} = 60 - 30 = 30 \text{ days}$$

**Step 4 — Required workforce.**
$$\frac{1{,}800}{30} = 60 \text{ men}$$

**Step 5 — Additional men.**
$$60 - 40 = 20$$

**Verification:** 1,200 + (60 × 30) = 1,200 + 1,800 = 3,000 man-days ✓

**Answer: (b) 20**

---

**Q47. A fills in 12 min, B empties in 18 min; tank is ⅓ full. Time to fill? → (b) 24 min**

**Step 1 — Capacity = LCM(12, 18) = 36 units**

**Step 2 — Rates with signs.**
$$A = +3 \text{ units/min}, \qquad B = -2 \text{ units/min}$$

**Step 3 — Net rate.**
$$3 - 2 = +1 \text{ unit/min}$$

Positive ⇒ the tank will eventually fill.

**Step 4 — How much still needs filling.**
The tank is already 1/3 full:
$$\text{Already filled} = \frac{36}{3} = 12 \text{ units}$$
$$\text{Still needed} = 36 - 12 = 24 \text{ units}$$

**Step 5 — Time.**
$$\frac{24}{1} = 24 \text{ minutes}$$

**Answer: (b) 24 min**

> **Trap:** computing 36/1 = 36 minutes, ignoring the head start. Always subtract what is already in the tank.

---

**Q48. A+B = 12, B+C = 15, A+C = 20 days. C alone? → (d) 60 days**

**Step 1 — Work = LCM(12, 15, 20) = 60 units**

**Step 2 — Pair rates.**
$$A + B = 5, \qquad B + C = 4, \qquad A + C = 3 \text{ units/day}$$

**Step 3 — Sum and halve.**
$$2(A+B+C) = 5 + 4 + 3 = 12 \implies A + B + C = 6 \text{ units/day}$$

**Step 4 — Isolate C.**
$$C = (A+B+C) - (A+B) = 6 - 5 = 1 \text{ unit/day}$$

**Step 5 — C's time.**
$$\frac{60}{1} = 60 \text{ days}$$

**Full solution set:** A = 2 units/day (30 days), B = 3 units/day (20 days), C = 1 unit/day (60 days).
Verify: A+B = 5 ✓, B+C = 4 ✓, A+C = 3 ✓

**Answer: (d) 60 days**

---

**Q49. Tap fills in 6 h; after half is filled, three more identical taps open. Total time? → (c) 3 h 45 min**

**Step 1 — Phase 1: one tap fills the first half.**
A full tank takes 6 hours, so half takes:
$$\frac{6}{2} = 3 \text{ hours}$$

**Step 2 — Phase 2: four taps now operate.**
Each tap fills 1/6 of the tank per hour, so four taps fill:
$$4 \times \frac{1}{6} = \frac{2}{3} \text{ of the tank per hour}$$

**Step 3 — Time for the remaining half.**
$$\frac{1/2}{2/3} = \frac{1}{2} \times \frac{3}{2} = \frac{3}{4} \text{ hour} = 45 \text{ minutes}$$

**Step 4 — Total.**
$$3 \text{ h} + 45 \text{ min} = 3 \text{ h } 45 \text{ min}$$

**LCM verification:** Capacity = 12 units; one tap = 2 units/h.
- Phase 1: 6 units at 2 units/h = 3 hours
- Phase 2: 6 units at 8 units/h = 0.75 hours = 45 min ✓

**Answer: (c) 3 h 45 min**

---

**Q50. 3 men + 7 women in 10 days; 4 men + 6 women in 8 days. 10 women alone? → (c) 40 days**

**Step 1 — Write the two rate equations.**
Let *m* and *w* be the daily rates of one man and one woman.
$$3m + 7w = \frac{1}{10} \qquad \text{...(i)}$$
$$4m + 6w = \frac{1}{8} \qquad \text{...(ii)}$$

**Step 2 — Eliminate *m*.**
Multiply (i) by 4 and (ii) by 3 to match the *m* coefficients:
$$12m + 28w = \frac{4}{10} = \frac{2}{5} \qquad \text{...(iii)}$$
$$12m + 18w = \frac{3}{8} \qquad \text{...(iv)}$$

**Step 3 — Subtract (iv) from (iii).**
$$10w = \frac{2}{5} - \frac{3}{8}$$

**Step 4 — Compute the right side.**
$$\frac{2}{5} - \frac{3}{8} = \frac{16 - 15}{40} = \frac{1}{40}$$

**Step 5 — Read off the answer directly.**
$$10w = \frac{1}{40}$$

The left side is exactly the combined rate of **10 women** — so 10 women complete 1/40 of the work per day:
$$T = 40 \text{ days}$$

**Verification.** From Step 4, w = 1/400 (one woman alone takes 400 days).
Substituting into (i):
$$3m + \frac{7}{400} = \frac{1}{10} = \frac{40}{400} \implies 3m = \frac{33}{400} \implies m = \frac{11}{400}$$
Check (ii): $4\left(\frac{11}{400}\right) + 6\left(\frac{1}{400}\right) = \frac{44 + 6}{400} = \frac{50}{400} = \frac{1}{8}$ ✓

**Answer: (c) 40 days**

> **Elegant point:** the elimination produced "10w" directly — exactly the quantity asked for. Before solving for the individual rates, check whether the eliminated equation already answers the question. It often does, and saves a full step.

---

## 8. Quick Revision Sheet

> **One page. Read 48 hours after study, and again the night before the test.**

### The LCM method (use this for everything)

```
1.  Total Work = LCM of all given times
2.  Each rate  = Total Work ÷ that person's time
3.  Solve entirely in whole-number units
4.  Time = Units needed ÷ Combined rate

Example: A=20, B=30, C=60 days
    Work = 60 units;  rates 3, 2, 1;  combined 6  →  60/6 = 10 days
```

### Core relations

```
Rate = 1/Time                       Time = 1/Rate
Work = Rate × Time
Together (2 people)  T = ab/(a+b)
Find the partner:    1/T_B = 1/T_AB − 1/T_A     ← subtract RATES, never times
```

### Efficiency

```
Efficiency ∝ 1/Time     →     E_A : E_B  =  T_B : T_A     (ALWAYS inverse)

25% more efficient → E 5:4, T 4:5      20% more → E 6:5, T 5:6
50% more efficient → E 3:2, T 2:3      twice as fast → E 2:1, T 1:2
```

### Work equation (man-days)

```
M₁ D₁ H₁ = M₂ D₂ H₂           and       M₁D₁H₁/W₁ = M₂D₂H₂/W₂

Treat the job as a MAN-DAY BUDGET:
    spent so far → remaining → divide by days left → men needed
```

### Three pairs → individuals

```
(A+B) + (B+C) + (C+A) = 2(A+B+C)      ← HALVE IT. Most-missed step.
A = (A+B+C) − (B+C)
B = (A+B+C) − (C+A)
C = (A+B+C) − (A+B)
```

### Special setups

```
A leaves k days early:   R_A(T − k) + R_B·T = W

Alternate days:  pair output per 2 days → complete cycles → leftover
                 CHECK WHOSE TURN the final day is (depends on who started)

Every third day help:  model a 3-day cycle, then count cycles

Wages:  split in ratio of WORK DONE = rate × days worked
        equal days → ratio of rates → ratio 1/T_A : 1/T_B : 1/T_C
```

### Pipes & Cisterns

```
Inlet = +rate       Outlet / leak = −rate
Net rate = Σinlets − Σoutlets

Two inlets a, b              →  ab/(a+b)
Inlet a, outlet b (b > a)    →  ab/(b−a)
Fills in a; with leak b      →  Leak alone empties in ab/(b−a)

Tank partly full  →  subtract what's already there BEFORE dividing
Capacity from flow →  (L per hour) × (hours that pipe alone would take)

Net < 0  →  the tank never fills. Check the sign.
```

### Sanity checks

```
✓ Together must be FASTER than the fastest individual
✓ Adding an outlet ALWAYS increases the fill time
✓ More men ⇒ fewer days (inverse)
✓ Efficiency ratio and time ratio are INVERSE
✓ In three-pairs problems, HALVE the sum
```

---

## 9. Common Mistakes

| # | Mistake | Example | Correction |
|---|---|---|---|
| 1 | **Subtracting times instead of rates** | A+B = 8, A = 12 ⇒ B = 4 days | Subtract rates: 1/8 − 1/12 = 1/24 ⇒ 24 days |
| 2 | **Adding times instead of rates** | A = 12, B = 15 ⇒ together 27 days | Add rates: 1/12 + 1/15 ⇒ 6⅔ days |
| 3 | **Forgetting to halve in three-pairs** | (A+B)+(B+C)+(C+A) taken as (A+B+C) | It equals **2**(A+B+C) |
| 4 | **Efficiency ratio used directly as time** | E = 3:2 ⇒ times 3:2 | Times are inverse: 2 : 3 |
| 5 | **Alternate days: wrong final worker** | Leftover always given to A | Depends on who started and the day parity |
| 6 | **"Leaves 3 days early" misread** | A works only 3 days | A works (T − 3) days |
| 7 | **Outlet sign forgotten** | 1/12 + 1/16 + 1/24 for a leak | The leak is **negative**: +4 +3 −2 |
| 8 | **Head start ignored** | Tank ⅓ full but full capacity used | Fill only the remaining 2/3 |
| 9 | **Wages split by time present** | Equal days ⇒ equal pay | Split by **work done** (rate × days) |
| 10 | **Man-days budget miscomputed** | 40% done ⇒ total = 1,200 man-days | Total = 1,200 ÷ 0.40 = 3,000 |
| 11 | **Men and women added directly** | 4 men + 4 women = 8 workers | Convert via the equivalence first |
| 12 | **Not checking the net sign in pipes** | Answering a time when net < 0 | If net ≤ 0, the tank never fills |

---

## Practice Answer Key

| Q | Ans | Q | Ans | Q | Ans | Q | Ans | Q | Ans |
|---|---|---|---|---|---|---|---|---|---|
| 1 | b | 11 | b | 21 | c | 31 | c | 41 | b |
| 2 | b | 12 | c | 22 | c | 32 | b | 42 | c |
| 3 | c | 13 | b | 23 | c | 33 | c | 43 | c |
| 4 | c | 14 | b | 24 | c | 34 | c | 44 | c |
| 5 | b | 15 | c | 25 | b | 35 | b | 45 | b |
| 6 | b | 16 | b | 26 | b | 36 | b | 46 | b |
| 7 | b | 17 | b | 27 | b | 37 | b | 47 | b |
| 8 | b | 18 | d | 28 | c | 38 | c | 48 | d |
| 9 | b | 19 | c | 29 | b | 39 | b | 49 | c |
| 10 | b | 20 | a | 30 | b | 40 | b | 50 | c |

**Scoring guide:** 45+/50 → strong. 35–44 → solid; drill alternate-days and pipes-with-outlets. Below 35 → adopt the LCM method exclusively (Section 2.3) and redo the Medium set.

---

**⬅️ Back:** [Topic 4 — Averages, Mixtures & Alligation](04-averages-mixtures-alligation.md) · **➡️ Next:** [Topic 6 — Time, Speed & Distance](06-time-speed-distance.md)
