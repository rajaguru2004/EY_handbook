# Topic 3 — Ratio, Proportion & Partnership

### EY Placement Aptitude Handbook · Priority Rank #7 · 🟠 High

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

**Weightage:** 7–9% of the quantitative section — typically **1 direct question**, but the *technique* is used far more widely.

**Where ratios show up beyond their own questions:**

| Area | How ratios are used |
|---|---|
| **Pie-chart DI** | Sector shares are ratios; converting to absolute values is the whole question |
| **Mixtures & Alligation** | Concentration is a ratio; alligation is a ratio shortcut |
| **Time & Work** | Efficiency ratios are the inverse of time ratios |
| **Time, Speed & Distance** | Constant distance ⇒ speed and time are in inverse ratio |
| **Partnership** | Profit sharing is capital × time, expressed as a ratio |
| **Ages** | Almost every age problem is a ratio problem |
| **Percentages** | "25% more" is just the ratio 5 : 4 |

**Question styles reported:**

- Combining chained ratios (a:b, b:c → a:b:c)
- Dividing a sum in a given ratio
- "Add/subtract *k* from each term, ratio becomes…"
- Income–expenditure–savings with two ratios
- Partnership profit sharing, including staggered entry and withdrawal
- Coins-in-a-bag (number ratio vs value ratio)
- Mixture ratio adjustments

---

## 2. Core Concepts

### 2.1 What a ratio is

A ratio compares two quantities **of the same kind** by division.

$$a : b = \frac{a}{b}$$

- *a* is the **antecedent**, *b* is the **consequent**
- A ratio has **no units** — you must convert both quantities to the same unit *before* forming the ratio
- Multiplying or dividing both terms by the same non-zero number does not change the ratio: 6 : 8 = 3 : 4

> **Unit trap:** "the ratio of 2 hours to 40 minutes" is **not** 2 : 40. Convert first: 120 min : 40 min = **3 : 1**.

### 2.2 Ratios as parts

If two quantities are in the ratio *a* : *b*, think of them as *a* parts and *b* parts, with **(a + b) parts in total**.

$$\text{Value of one part} = \frac{\text{Total}}{a+b}$$

> Divide ₹600 in the ratio 2 : 3.
> Total parts = 5 ⇒ one part = ₹120 ⇒ shares are ₹240 and ₹360.

This "parts" mindset solves the majority of ratio questions in a single line.

### 2.3 Combining chained ratios

Given a : b and b : c, make the **common term equal** by scaling.

> a : b = 3 : 4 and b : c = 8 : 9
>
> *b* is 4 in the first and 8 in the second. LCM = 8.
> Scale the first by 2: a : b = 6 : 8
> Now a : b : c = **6 : 8 : 9**

**Fast method for three-link chains:**

$$a : b : c = (a_1 \times a_2) : (b_1 \times a_2) : (b_2 \times b_1)$$

where a₁:b₁ is the first ratio and a₂:b₂ the second. Or simply:

```
a : b = 3 : 4
b : c =     8 : 9
─────────────────────
a : b : c = 3×8 : 4×8 : 4×9  =  24 : 32 : 36  =  6 : 8 : 9
```

Multiply the first ratio through by the second's antecedent, and the second ratio through by the first's consequent.

**For four terms (a:b, b:c, c:d), just find a:d directly:**

$$\frac{a}{d} = \frac{a}{b} \times \frac{b}{c} \times \frac{c}{d}$$

### 2.4 Proportion

Four quantities are in proportion when a : b = c : d, written **a : b :: c : d**.

$$\boxed{a \times d = b \times c} \qquad \text{(product of extremes = product of means)}$$

- *a* and *d* are the **extremes**
- *b* and *c* are the **means**

| Term | Definition | Formula |
|---|---|---|
| **Fourth proportional** to a, b, c | The *d* in a : b :: c : d | $d = \dfrac{b \times c}{a}$ |
| **Third proportional** to a, b | The *c* in a : b :: b : c | $c = \dfrac{b^2}{a}$ |
| **Mean proportional** between a, b | The *x* in a : x :: x : b | $x = \sqrt{ab}$ |

> Fourth proportional to 4, 6, 10 → (6 × 10)/4 = **15**
> Third proportional to 9, 12 → 12²/9 = 144/9 = **16**
> Mean proportional between 4 and 25 → √100 = **10**

### 2.5 Properties of proportion

If a/b = c/d, then all of the following hold:

| Name | Statement |
|---|---|
| **Invertendo** | b/a = d/c |
| **Alternendo** | a/c = b/d |
| **Componendo** | (a+b)/b = (c+d)/d |
| **Dividendo** | (a−b)/b = (c−d)/d |
| **Componendo & Dividendo** | $\dfrac{a+b}{a-b} = \dfrac{c+d}{c-d}$ |

**Componendo–dividendo is the most useful of these** — it collapses equations of the form (px + q)/(rx + s) = m/n into a single step.

### 2.6 The "equal ratios" theorem

If

$$\frac{a}{p} = \frac{b}{q} = \frac{c}{r} = k$$

then

$$\frac{a + b + c}{p + q + r} = k \qquad \text{and more generally} \qquad \frac{\lambda_1 a + \lambda_2 b + \lambda_3 c}{\lambda_1 p + \lambda_2 q + \lambda_3 r} = k$$

for any weights λ. **Any weighted combination of the numerators over the same weighted combination of the denominators equals the common ratio.**

> If a : b = c : d = e : f = 3 : 5, then (2a + 3c + 4e) : (2b + 3d + 4f) = **3 : 5** as well.

### 2.7 Direct and inverse proportion

| Type | Relation | Example |
|---|---|---|
| **Direct** | $x \propto y$, so $x/y$ is constant | More workers ⇒ more work done |
| **Inverse** | $x \propto 1/y$, so $xy$ is constant | More workers ⇒ less time taken |

> **Key inverse-ratio fact used constantly:** if the distance (or work) is fixed, then
> $$\text{Speed ratio} = a : b \implies \text{Time ratio} = b : a$$

### 2.8 Partnership

Partners share profit in the ratio of their **effective capital**:

$$\text{Effective capital} = \text{Amount invested} \times \text{Time invested}$$

$$\boxed{P_1 : P_2 : P_3 = C_1 T_1 : C_2 T_2 : C_3 T_3}$$

**Two special cases:**

| Case | Sharing ratio |
|---|---|
| **Simple partnership** — all invest for the same duration | Ratio of capitals alone |
| **Compound partnership** — different durations | Ratio of capital × time |

**Working vs sleeping partners:** a working partner may first take a fixed salary or a percentage of profit for management. Deduct that **first**, then divide the remainder by effective capital.

**Capital changes mid-year:** split the year into segments and sum.

> B invests ₹30,000 for 6 months, then withdraws ₹10,000 and continues with ₹20,000 for 6 months.
> $$\text{Effective capital} = 30{,}000 \times 6 + 20{,}000 \times 6 = 1{,}80{,}000 + 1{,}20{,}000 = 3{,}00{,}000$$

### 2.9 Number ratio vs value ratio (the coins problem)

When items have **different unit values**, the ratio of *counts* is not the ratio of *money*.

> Coins of 50p, 25p and 10p are in the ratio **5 : 9 : 4** *by number*.
> The ratio **by value** is:
> $$5 \times 50 \;:\; 9 \times 25 \;:\; 4 \times 10 \;=\; 250 : 225 : 40 \;=\; 50 : 45 : 8$$

Always ask which ratio the question gives you, and which it wants.

---

## 3. Formula Bank

| # | Concept | Formula |
|---|---|---|
| 1 | Ratio | $a : b = a/b$ |
| 2 | Value of one part | $\dfrac{\text{Total}}{\text{Sum of ratio terms}}$ |
| 3 | Share of a term | $\dfrac{\text{its ratio term}}{\text{sum of terms}} \times \text{Total}$ |
| 4 | Combining a:b and b:c | Scale to a common *b*, or use $a_1a_2 : b_1a_2 : b_1b_2$ |
| 5 | Chain to a : d | $\dfrac{a}{d} = \dfrac{a}{b}\cdot\dfrac{b}{c}\cdot\dfrac{c}{d}$ |
| 6 | Proportion | $a:b::c:d \iff ad = bc$ |
| 7 | Fourth proportional to a, b, c | $\dfrac{bc}{a}$ |
| 8 | Third proportional to a, b | $\dfrac{b^2}{a}$ |
| 9 | Mean proportional between a, b | $\sqrt{ab}$ |
| 10 | Componendo & dividendo | $\dfrac{a}{b}=\dfrac{c}{d} \implies \dfrac{a+b}{a-b}=\dfrac{c+d}{c-d}$ |
| 11 | Equal-ratio theorem | $\dfrac{a}{p}=\dfrac{b}{q}=\dfrac{c}{r}=k \implies \dfrac{a+b+c}{p+q+r}=k$ |
| 12 | If $ka = lb = mc$ | $a:b:c = \dfrac{1}{k} : \dfrac{1}{l} : \dfrac{1}{m}$ |
| 13 | Duplicate ratio of a : b | $a^2 : b^2$ |
| 14 | Sub-duplicate ratio of a : b | $\sqrt{a} : \sqrt{b}$ |
| 15 | Triplicate ratio of a : b | $a^3 : b^3$ |
| 16 | Compound ratio of a:b and c:d | $ac : bd$ |
| 17 | Inverse proportion | $x_1 y_1 = x_2 y_2$ |
| 18 | Partnership (equal time) | $P_1 : P_2 = C_1 : C_2$ |
| 19 | Partnership (unequal time) | $P_1 : P_2 = C_1T_1 : C_2T_2$ |
| 20 | Working partner | Deduct salary/commission first, then split remainder by capital ratio |
| 21 | Add *x* to both terms of a:b to get c:d | $x = \dfrac{ad - bc}{c - d}$ |
| 22 | Coins ratio: number *n* with value *v* | Value ratio $= n_1v_1 : n_2v_2 : n_3v_3$ |

---

## 4. Shortcuts & Tricks

### 4.1 The "one part" method

The single most useful habit in this topic. Convert the ratio into **parts**, find the value of one part, and read off every answer.

> *"Two numbers are in the ratio 3 : 4 and their difference is 8."*
> Difference in parts = 4 − 3 = **1 part** = 8.
> So the numbers are 3 × 8 = **24** and 4 × 8 = **32**.

> *"A sum is divided among P, Q, R as 3 : 5 : 7. R gets ₹800 more than P."*
> Difference = 7 − 3 = **4 parts** = ₹800 ⇒ 1 part = ₹200.
> Total = 15 parts = **₹3,000**.

Never set up algebra when a "parts" reading works.

### 4.2 The chained-ratio ladder

Write each ratio on its own line, aligned on the shared term, then cross-multiply down the columns.

```
A : B : C : D
2 : 3
    4 : 5
        6 : 7
─────────────────
A : B  = 2 : 3
B : C  = 4 : 5
C : D  = 6 : 7

A : D = (2 × 4 × 6) : (3 × 5 × 7) = 48 : 105 = 16 : 35
```

**Rule for A : D** — multiply all antecedents, multiply all consequents.

For the full A : B : C : D, scale each ratio so shared terms match:
```
A : B = 2 : 3      × 4    →  8 : 12
B : C = 4 : 5      × 3    →      12 : 15
C : D = 6 : 7      × 15/6 →           15 : 17.5   → ×2 throughout
A : B : C : D = 16 : 24 : 30 : 35
```

### 4.3 "ka = lb = mc" → invert

$$ka = lb = mc \implies a : b : c = \frac{1}{k} : \frac{1}{l} : \frac{1}{m}$$

Then clear the fractions by multiplying by the LCM of k, l, m.

> **2A = 3B = 4C** ⇒ A : B : C = 1/2 : 1/3 : 1/4
> LCM(2,3,4) = 12 ⇒ multiply through: **6 : 4 : 3**

**Check:** A = 6, B = 4, C = 3. 2(6) = 12, 3(4) = 12, 4(3) = 12 ✓

### 4.4 The income–expenditure–savings template

Given incomes in ratio *a* : *b*, expenditures in ratio *c* : *d*, and savings *S*₁, *S*₂:

$$a x - c y = S_1$$
$$b x - d y = S_2$$

Solve the two linear equations for *x*. Income of the first = *ax*.

> Incomes 5 : 4, expenditures 3 : 2, each saves ₹2,000.
> 5x − 3y = 2000
> 4x − 2y = 2000 ⇒ 2x − y = 1000 ⇒ y = 2x − 1000
> Substituting: 5x − 6x + 3000 = 2000 ⇒ x = 1000 ⇒ **first income = ₹5,000**

### 4.5 The "add k to both terms" formula

To find what must be added to **both** terms of *a* : *b* to make it *c* : *d*:

$$x = \frac{ad - bc}{c - d}$$

> What must be added to each term of 3 : 5 to make it 5 : 7?
> $$x = \frac{3(7) - 5(5)}{5 - 7} = \frac{21 - 25}{-2} = \frac{-4}{-2} = 2$$
> Check: (3+2) : (5+2) = 5 : 7 ✓

### 4.6 Partnership — build the effective-capital table

Never do partnership problems in your head. Tabulate.

| Partner | Capital | × Months | Effective capital |
|---|---|---|---|
| A | 20,000 | 12 | 2,40,000 |
| B | 30,000 (6 mo) + 20,000 (6 mo) | — | 1,80,000 + 1,20,000 = 3,00,000 |
| C | 25,000 | 8 | 2,00,000 |

Then reduce: 240 : 300 : 200 = **12 : 15 : 10** (sum 37).

Divide the profit into 37 parts.

### 4.7 Mixture-ratio shortcut

When you **add only one component**, the other component stays fixed — anchor on it.

> 45 L mixture, milk : water = 4 : 1. How much water to make it 3 : 2?
> Milk = 36 L and **stays 36 L**.
> For milk : water = 3 : 2 with milk = 36, water must be 36 × (2/3) = 24 L.
> Water present = 9 L ⇒ **add 15 L**.

### 4.8 Ratio ↔ percentage conversions

| Ratio | As a percentage | Common phrasing |
|---|---|---|
| 5 : 4 | first is 25% more | "A is 25% more than B" |
| 6 : 5 | first is 20% more | "A is 20% more than B" |
| 4 : 5 | first is 20% less | "A is 20% less than B" |
| 3 : 4 | first is 25% less | "A is 25% less than B" |
| 3 : 2 | first is 50% more | "A is 50% more than B" |
| 2 : 3 | first is 33⅓% less | "A is 33⅓% less than B" |

Converting a percentage statement into a ratio is almost always the faster route in multi-step problems.

---

## 5. Solved Examples

### Example 1 — Combining chained ratios

**Q.** If A : B = 3 : 4 and B : C = 6 : 7, find A : B : C.

**Step 1 — Identify the shared term.**
B appears as 4 in the first ratio and 6 in the second.

**Step 2 — Make B the same in both. LCM(4, 6) = 12.**
$$A : B = 3 : 4 \quad (\times 3) \quad \to \quad 9 : 12$$
$$B : C = 6 : 7 \quad (\times 2) \quad \to \quad 12 : 14$$

**Step 3 — Merge.**
$$A : B : C = 9 : 12 : 14$$

**Verification:** A/B = 9/12 = 3/4 ✓ and B/C = 12/14 = 6/7 ✓

**Answer: 9 : 12 : 14**

---

### Example 2 — Dividing a sum

**Q.** ₹3,500 is divided among A, B and C such that A : B = 2 : 3 and B : C = 4 : 5. Find each share.

**Step 1 — Combine the ratios.** B is 3 and 4; LCM = 12.
$$A : B = 2 : 3 \ (\times 4) \to 8 : 12$$
$$B : C = 4 : 5 \ (\times 3) \to 12 : 15$$
$$A : B : C = 8 : 12 : 15$$

**Step 2 — Find the value of one part.**
$$\text{Total parts} = 8 + 12 + 15 = 35$$
$$\text{One part} = \frac{3500}{35} = ₹100$$

**Step 3 — Compute shares.**
$$A = 8 \times 100 = ₹800$$
$$B = 12 \times 100 = ₹1{,}200$$
$$C = 15 \times 100 = ₹1{,}500$$

**Check:** 800 + 1,200 + 1,500 = ₹3,500 ✓

**Answer: A = ₹800, B = ₹1,200, C = ₹1,500**

---

### Example 3 — Ratio changes after adding/subtracting

**Q.** Two numbers are in the ratio 3 : 5. If 9 is subtracted from each, the ratio becomes 12 : 23. Find the numbers.

**Step 1 — Represent using a single variable.**
Let the numbers be 3*x* and 5*x*.

**Step 2 — Apply the condition.**
$$\frac{3x - 9}{5x - 9} = \frac{12}{23}$$

**Step 3 — Cross-multiply.**
$$23(3x - 9) = 12(5x - 9)$$
$$69x - 207 = 60x - 108$$

**Step 4 — Solve.**
$$9x = 99 \implies x = 11$$

**Step 5 — Find the numbers.**
$$3x = 33, \qquad 5x = 55$$

**Verification:** (33 − 9) : (55 − 9) = 24 : 46 = 12 : 23 ✓

**Answer: 33 and 55**

> **Technique note:** always introduce a *single* variable *x* using the ratio. Using two separate variables doubles the algebra for no benefit.

---

### Example 4 — Income, expenditure and savings

**Q.** The incomes of two people are in the ratio 4 : 3 and their expenditures are in the ratio 3 : 2. If each saves ₹6,000, find the income of the first person.

**Step 1 — Set up with two variables.**
Incomes: 4*x* and 3*x*
Expenditures: 3*y* and 2*y*

**Step 2 — Write the savings equations.**
$$4x - 3y = 6000 \qquad \text{...(i)}$$
$$3x - 2y = 6000 \qquad \text{...(ii)}$$

**Step 3 — Eliminate *y*.**
Multiply (i) by 2 and (ii) by 3:
$$8x - 6y = 12000 \qquad \text{...(iii)}$$
$$9x - 6y = 18000 \qquad \text{...(iv)}$$

Subtract (iii) from (iv):
$$x = 6000$$

**Step 4 — Compute the first income.**
$$4x = 4 \times 6000 = ₹24{,}000$$

**Full verification:**
From (ii): 3(6000) − 2y = 6000 ⇒ 18,000 − 2y = 6,000 ⇒ y = 6,000
- Incomes: ₹24,000 and ₹18,000 (ratio 4 : 3 ✓)
- Expenditures: 3y = ₹18,000 and 2y = ₹12,000 (ratio 3 : 2 ✓)
- Savings: 24,000 − 18,000 = ₹6,000 ✓ and 18,000 − 12,000 = ₹6,000 ✓

**Answer: ₹24,000**

---

### Example 5 — Simple partnership

**Q.** A, B and C invest ₹8,000, ₹10,000 and ₹12,000 respectively in a business for one year. If the annual profit is ₹9,000, find each partner's share.

**Step 1 — Equal time ⇒ ratio is simply the capital ratio.**
$$8000 : 10000 : 12000 = 8 : 10 : 12 = 4 : 5 : 6$$

**Step 2 — Total parts.**
$$4 + 5 + 6 = 15$$

**Step 3 — Value of one part.**
$$\frac{9000}{15} = ₹600$$

**Step 4 — Shares.**
$$A = 4 \times 600 = ₹2{,}400$$
$$B = 5 \times 600 = ₹3{,}000$$
$$C = 6 \times 600 = ₹3{,}600$$

**Check:** 2,400 + 3,000 + 3,600 = ₹9,000 ✓

**Answer: A ₹2,400, B ₹3,000, C ₹3,600**

---

### Example 6 — Compound partnership (different durations)

**Q.** A starts a business with ₹12,000. Four months later B joins with ₹18,000. Find the ratio in which the year-end profit should be divided.

**Step 1 — Determine each partner's investment period.**
- A invests for the full **12 months**
- B joins after 4 months, so B invests for **12 − 4 = 8 months**

**Step 2 — Compute effective capital (capital × time).**
$$A: \quad 12{,}000 \times 12 = 1{,}44{,}000$$
$$B: \quad 18{,}000 \times 8 = 1{,}44{,}000$$

**Step 3 — Form the ratio.**
$$1{,}44{,}000 : 1{,}44{,}000 = \mathbf{1 : 1}$$

**Answer: 1 : 1 — they share the profit equally**

> **Insight:** B invested 50% more capital, but for only two-thirds of the time. 1.5 × (2/3) = 1, so the two effects exactly cancel. Never judge partnership shares by capital alone.

---

### Example 7 — Coins problem (number ratio vs value ratio)

**Q.** A bag contains 50-paise, 25-paise and 10-paise coins in the ratio 5 : 9 : 4, totalling ₹206. Find the number of 25-paise coins.

**Step 1 — Let the counts be 5x, 9x and 4x.**

**Step 2 — Convert counts to value (in rupees).**
$$\text{50p coins: } 5x \times 0.50 = 2.5x$$
$$\text{25p coins: } 9x \times 0.25 = 2.25x$$
$$\text{10p coins: } 4x \times 0.10 = 0.4x$$

**Step 3 — Sum to the given total.**
$$2.5x + 2.25x + 0.4x = 206$$
$$5.15x = 206$$

**Step 4 — Solve.**
$$x = \frac{206}{5.15} = \frac{20600}{515} = 40$$

**Step 5 — Answer the question asked.**
$$\text{Number of 25p coins} = 9x = 9 \times 40 = 360$$

**Verification:**
- 50p coins: 200 → ₹100
- 25p coins: 360 → ₹90
- 10p coins: 160 → ₹16
- Total = ₹206 ✓

**Answer: 360 coins**

> **The trap:** dividing ₹206 in the ratio 5 : 9 : 4 directly. That ratio is by **count**, not by value. Always convert.

---

### Example 8 — Working partner with a commission

**Q.** A and B invest in the ratio 3 : 2. A is a working partner and receives 15% of the profit for managing the business; the remainder is divided in the investment ratio. If A receives ₹4,800 more than B, find the total profit.

**Step 1 — Let the total profit be P.**

**Step 2 — Deduct A's management commission first.**
$$\text{A's commission} = 0.15P$$
$$\text{Remaining profit} = 0.85P$$

**Step 3 — Divide the remainder in the ratio 3 : 2 (total 5 parts).**
$$\text{A's share of remainder} = \frac{3}{5} \times 0.85P = 0.51P$$
$$\text{B's share} = \frac{2}{5} \times 0.85P = 0.34P$$

**Step 4 — Compute A's total.**
$$\text{A total} = 0.15P + 0.51P = 0.66P$$
$$\text{B total} = 0.34P$$

**Step 5 — Apply the given difference.**
$$0.66P - 0.34P = 4800$$
$$0.32P = 4800$$
$$P = \frac{4800}{0.32} = ₹15{,}000$$

**Verification:**
- Commission = 15% of 15,000 = ₹2,250
- Remainder = ₹12,750, split 3 : 2 ⇒ A ₹7,650, B ₹5,100
- A total = 2,250 + 7,650 = ₹9,900
- Difference = 9,900 − 5,100 = ₹4,800 ✓

**Answer: ₹15,000**

---

## 6. Practice Questions

**Instructions:** 50 questions. Easy (1–20), Medium (21–40), Hard (41–50).
Target times: Easy 30 s · Medium 60 s · Hard 90 s.
Full solutions in [Section 7](#7-detailed-solutions).

### 🟢 EASY (Questions 1–20)

**Q1.** If a : b = 3 : 4 and b : c = 4 : 5, find a : c.
(a) 3 : 5  (b) 4 : 5  (c) 3 : 4  (d) 5 : 3

**Q2.** Divide ₹600 in the ratio 2 : 3.
(a) ₹200, ₹400  (b) ₹240, ₹360  (c) ₹250, ₹350  (d) ₹260, ₹340

**Q3.** Simplify the ratio 45 : 60.
(a) 2 : 3  (b) 3 : 4  (c) 4 : 5  (d) 5 : 6

**Q4.** If 3 : 5 :: x : 20, find x.
(a) 10  (b) 12  (c) 14  (d) 15

**Q5.** Find the ratio of 2 hours to 40 minutes.
(a) 1 : 20  (b) 2 : 40  (c) 3 : 1  (d) 1 : 3

**Q6.** Two numbers are in the ratio 5 : 7 and their sum is 96. Find the larger number.
(a) 40  (b) 48  (c) 56  (d) 60

**Q7.** Find the fourth proportional to 4, 6 and 10.
(a) 12  (b) 14  (c) 15  (d) 18

**Q8.** Find the third proportional to 9 and 12.
(a) 14  (b) 15  (c) 16  (d) 18

**Q9.** Find the mean proportional between 4 and 25.
(a) 8  (b) 10  (c) 12  (d) 14.5

**Q10.** If a : b = 2 : 3, find (2a + 3b) : (a + b).
(a) 11 : 5  (b) 12 : 5  (c) 13 : 5  (d) 14 : 5

**Q11.** Divide ₹1,200 among A, B and C in the ratio 1 : 2 : 3.
(a) ₹200, ₹400, ₹600  (b) ₹150, ₹350, ₹700  (c) ₹250, ₹350, ₹600  (d) ₹300, ₹400, ₹500

**Q12.** Two numbers are in the ratio 3 : 4 and their difference is 8. Find the numbers.
(a) 18, 26  (b) 21, 29  (c) 24, 32  (d) 27, 35

**Q13.** If x : y = 4 : 5, find (x + y) : (y − x).
(a) 7 : 1  (b) 8 : 1  (c) 9 : 1  (d) 10 : 1

**Q14.** A and B invest ₹5,000 and ₹7,000 for the same period. Divide a profit of ₹3,600 between them.
(a) ₹1,400, ₹2,200  (b) ₹1,500, ₹2,100  (c) ₹1,600, ₹2,000  (d) ₹1,200, ₹2,400

**Q15.** Simplify the ratio 0.5 : 1.5.
(a) 1 : 2  (b) 1 : 3  (c) 2 : 3  (d) 1 : 4

**Q16.** If a : b = 3 : 4 and b : c = 2 : 3, find a : b : c.
(a) 3 : 4 : 5  (b) 3 : 4 : 6  (c) 2 : 3 : 4  (d) 3 : 5 : 6

**Q17.** Express the ratio 3 : 8 as a percentage.
(a) 32.5%  (b) 35%  (c) 37.5%  (d) 40%

**Q18.** Find the ratio of 1 km to 400 m.
(a) 1 : 4  (b) 2 : 5  (c) 5 : 2  (d) 4 : 1

**Q19.** What must be added to each term of the ratio 3 : 5 to make it 5 : 7?
(a) 1  (b) 2  (c) 3  (d) 4

**Q20.** Divide 108 into two parts in the ratio 5 : 4.
(a) 55, 53  (b) 58, 50  (c) 60, 48  (d) 62, 46

---

### 🟡 MEDIUM (Questions 21–40)

**Q21.** If A : B = 2 : 3, B : C = 4 : 5 and C : D = 6 : 7, find A : D.
(a) 8 : 35  (b) 16 : 35  (c) 12 : 35  (d) 16 : 45

**Q22.** The sum of three numbers is 98. The ratio of the first to the second is 2 : 3, and of the second to the third is 5 : 8. Find the second number.
(a) 20  (b) 30  (c) 48  (d) 58

**Q23.** ₹5,625 is divided among A, B and C so that A receives half of what B and C together receive, and B receives one-fourth of what A and C together receive. Find A's share.
(a) ₹1,575  (b) ₹1,750  (c) ₹1,875  (d) ₹2,000

**Q24.** Two numbers are in the ratio 3 : 5. If 9 is subtracted from each, the ratio becomes 12 : 23. Find the numbers.
(a) 27, 45  (b) 30, 50  (c) 33, 55  (d) 36, 60

**Q25.** A, B and C invest ₹8,000, ₹10,000 and ₹12,000 respectively for one year. If the profit is ₹9,000, find C's share.
(a) ₹3,000  (b) ₹3,200  (c) ₹3,600  (d) ₹4,000

**Q26.** A starts a business with ₹12,000. Four months later B joins with ₹18,000. In what ratio should the year-end profit be divided?
(a) 1 : 1  (b) 2 : 3  (c) 3 : 2  (d) 4 : 3

**Q27.** The incomes of two people are in the ratio 5 : 4 and their expenditures in the ratio 3 : 2. If each saves ₹2,000, find the income of the first.
(a) ₹4,000  (b) ₹4,500  (c) ₹5,000  (d) ₹5,500

**Q28.** If a : b = 3 : 4 and b : c = 8 : 9, find a : b : c.
(a) 3 : 4 : 9  (b) 6 : 8 : 9  (c) 3 : 8 : 9  (d) 6 : 8 : 12

**Q29.** Divide ₹3,500 among A, B and C such that A : B = 2 : 3 and B : C = 4 : 5.
(a) ₹700, ₹1,200, ₹1,600  (b) ₹800, ₹1,200, ₹1,500  (c) ₹750, ₹1,250, ₹1,500  (d) ₹900, ₹1,100, ₹1,500

**Q30.** If 2A = 3B = 4C, find A : B : C.
(a) 2 : 3 : 4  (b) 4 : 3 : 2  (c) 6 : 4 : 3  (d) 3 : 4 : 6

**Q31.** A invests ₹15,000 for 8 months and B invests ₹12,000 for 10 months. If the profit is ₹8,000, find B's share.
(a) ₹3,600  (b) ₹4,000  (c) ₹4,400  (d) ₹4,800

**Q32.** A bag contains 50-paise, 25-paise and 10-paise coins in the ratio 5 : 9 : 4, amounting to ₹206. Find the number of 25-paise coins.
(a) 200  (b) 320  (c) 360  (d) 400

**Q33.** If x/2 = y/3 = z/5, find (x + y + z)/z.
(a) 1  (b) 2  (c) 3  (d) 5

**Q34.** In a 45-litre mixture, milk and water are in the ratio 4 : 1. How much water must be added to make the ratio 3 : 2?
(a) 12 L  (b) 15 L  (c) 18 L  (d) 20 L

**Q35.** A, B and C enter a partnership. A invests three times as much as B, and B invests two-thirds of what C invests. Find the ratio of their profit shares.
(a) 3 : 2 : 1  (b) 6 : 2 : 3  (c) 6 : 3 : 2  (d) 2 : 3 : 6

**Q36.** Divide ₹1,870 among A, B and C so that A receives one-third of what B receives, and B receives half of what C receives.
(a) ₹170, ₹510, ₹1,190  (b) ₹187, ₹561, ₹1,122  (c) ₹200, ₹600, ₹1,070  (d) ₹190, ₹570, ₹1,110

**Q37.** If (a + b) : (b + c) : (c + a) = 6 : 7 : 8 and a + b + c = 14, find c.
(a) 4  (b) 5  (c) 6  (d) 8

**Q38.** Two vessels contain milk and water in the ratios 4 : 1 and 3 : 2. Equal quantities from each are mixed. Find the ratio of milk to water in the new mixture.
(a) 5 : 3  (b) 6 : 4  (c) 7 : 3  (d) 7 : 5

**Q39.** The ratio of the present ages of A and B is 4 : 5. After 6 years the ratio becomes 5 : 6. Find A's present age.
(a) 20 years  (b) 22 years  (c) 24 years  (d) 26 years

**Q40.** A sum is divided among P, Q and R in the ratio 3 : 5 : 7. If R receives ₹800 more than P, find the total sum.
(a) ₹2,400  (b) ₹2,800  (c) ₹3,000  (d) ₹3,200

---

### 🔴 HARD (Questions 41–50)

**Q41.** A, B and C start a business. A invests ₹20,000 for the whole year. B invests ₹30,000 for the first six months, then withdraws ₹10,000 and continues with the rest. C invests ₹25,000 for the last eight months. If the annual profit is ₹37,000, find B's share.
(a) ₹12,000  (b) ₹13,500  (c) ₹15,000  (d) ₹16,000

**Q42.** The incomes of A and B are in the ratio 4 : 3 and their expenditures in the ratio 3 : 2. If each saves ₹6,000, find A's income.
(a) ₹18,000  (b) ₹20,000  (c) ₹24,000  (d) ₹28,000

**Q43.** ₹6,300 is divided among three friends such that half of A's share, one-third of B's share and one-fourth of C's share are all equal. Find C's share.
(a) ₹1,400  (b) ₹2,100  (c) ₹2,800  (d) ₹3,200

**Q44.** A mixture contains milk and water in the ratio 5 : 1. On adding 5 litres of water, the ratio becomes 5 : 2. Find the quantity of milk in the mixture.
(a) 20 L  (b) 25 L  (c) 30 L  (d) 35 L

**Q45.** A and B invest in the ratio 3 : 2. A, as the working partner, receives 15% of the profit for management, and the remainder is divided in the investment ratio. If A receives ₹4,800 more than B, find the total profit.
(a) ₹12,000  (b) ₹14,000  (c) ₹15,000  (d) ₹18,000

**Q46.** Two numbers are in the ratio 7 : 9. If 12 is added to each, the ratio becomes 5 : 6. Find the smaller number.
(a) 21  (b) 24  (c) 28  (d) 35

**Q47.** In a 60-litre mixture, milk and water are in the ratio 3 : 1. How much of the mixture must be drawn off and replaced by water so that milk and water are in the ratio 1 : 1?
(a) 15 L  (b) 18 L  (c) 20 L  (d) 24 L

**Q48.** A, B and C together subscribe ₹50,000 for a business. A subscribes ₹4,000 more than B, and B subscribes ₹5,000 more than C. Out of a total profit of ₹35,000, find A's share.
(a) ₹13,600  (b) ₹14,700  (c) ₹15,400  (d) ₹16,200

**Q49.** The ratio of boys to girls in a school is 3 : 2. If 20% of the boys and 25% of the girls hold scholarships, what percentage of the students do **not** hold a scholarship?
(a) 72%  (b) 75%  (c) 78%  (d) 80%

**Q50.** If a : b = c : d = e : f = 3 : 5, find (2a + 3c + 4e) : (2b + 3d + 4f).
(a) 2 : 3  (b) 3 : 5  (c) 5 : 3  (d) 9 : 15 reduced to 1 : 2

---

## 7. Detailed Solutions

### 🟢 EASY — Solutions 1–20

---

**Q1. a : b = 3 : 4, b : c = 4 : 5. Find a : c. → (a) 3 : 5**

**Formula used:** a/c = (a/b) × (b/c)

$$\frac{a}{c} = \frac{3}{4} \times \frac{4}{5} = \frac{12}{20} = \frac{3}{5}$$

**Observation:** *b* is already 4 in both ratios, so they chain directly: a : b : c = 3 : 4 : 5.

**Answer: (a) 3 : 5**

---

**Q2. Divide ₹600 in the ratio 2 : 3. → (b) ₹240, ₹360**

**Formula used:** One part = Total / (sum of ratio terms)

**Step 1 — Total parts.**
$$2 + 3 = 5$$

**Step 2 — Value of one part.**
$$\frac{600}{5} = ₹120$$

**Step 3 — Shares.**
$$2 \times 120 = ₹240 \qquad 3 \times 120 = ₹360$$

**Check:** 240 + 360 = ₹600 ✓

**Answer: (b) ₹240, ₹360**

---

**Q3. Simplify 45 : 60. → (b) 3 : 4**

Divide both terms by their HCF.
$$\text{HCF}(45, 60) = 15$$
$$\frac{45}{15} : \frac{60}{15} = 3 : 4$$

**Answer: (b) 3 : 4**

---

**Q4. If 3 : 5 :: x : 20, find x. → (b) 12**

**Formula used:** Product of extremes = product of means, i.e. 3 × 20 = 5 × x

$$60 = 5x \implies x = 12$$

**Alternative:** 5 → 20 means the second ratio is scaled by 4. So x = 3 × 4 = 12 ✓

**Answer: (b) 12**

---

**Q5. Ratio of 2 hours to 40 minutes. → (c) 3 : 1**

**Step 1 — Convert to a common unit.**
$$2 \text{ hours} = 120 \text{ minutes}$$

**Step 2 — Form the ratio.**
$$120 : 40 = 3 : 1$$

> **Trap:** writing 2 : 40 = 1 : 20. A ratio requires identical units on both sides.

**Answer: (c) 3 : 1**

---

**Q6. Two numbers in ratio 5 : 7, sum 96. Larger? → (c) 56**

**Step 1 — Total parts.**
$$5 + 7 = 12$$

**Step 2 — One part.**
$$\frac{96}{12} = 8$$

**Step 3 — Larger number.**
$$7 \times 8 = 56$$

**Check:** 40 + 56 = 96 ✓

**Answer: (c) 56**

---

**Q7. Fourth proportional to 4, 6, 10. → (c) 15**

**Formula used:** For a : b :: c : d, d = bc/a

$$d = \frac{6 \times 10}{4} = \frac{60}{4} = 15$$

**Check:** 4 : 6 = 10 : 15, since 4 × 15 = 60 = 6 × 10 ✓

**Answer: (c) 15**

---

**Q8. Third proportional to 9 and 12. → (c) 16**

**Formula used:** For a : b :: b : c, c = b²/a

$$c = \frac{12^2}{9} = \frac{144}{9} = 16$$

**Check:** 9 : 12 = 12 : 16, since 9 × 16 = 144 = 12 × 12 ✓

**Answer: (c) 16**

---

**Q9. Mean proportional between 4 and 25. → (b) 10**

**Formula used:** x = √(ab)

$$x = \sqrt{4 \times 25} = \sqrt{100} = 10$$

**Check:** 4 : 10 = 10 : 25, since 4 × 25 = 100 = 10 × 10 ✓

**Answer: (b) 10**

---

**Q10. a : b = 2 : 3. Find (2a + 3b) : (a + b). → (c) 13 : 5**

**Method — substitute the simplest values.** Let a = 2, b = 3.

$$2a + 3b = 2(2) + 3(3) = 4 + 9 = 13$$
$$a + b = 2 + 3 = 5$$

$$\text{Ratio} = 13 : 5$$

> **Why substitution is valid:** the expression is homogeneous of degree 1 in a and b, so scaling a and b by any factor leaves the ratio unchanged. Test with a = 4, b = 6: (8 + 18) : (10) = 26 : 10 = 13 : 5 ✓

**Answer: (c) 13 : 5**

---

**Q11. Divide ₹1,200 in the ratio 1 : 2 : 3. → (a) ₹200, ₹400, ₹600**

**Step 1 — Total parts.**
$$1 + 2 + 3 = 6$$

**Step 2 — One part.**
$$\frac{1200}{6} = ₹200$$

**Step 3 — Shares.**
$$₹200, \quad ₹400, \quad ₹600$$

**Check:** 200 + 400 + 600 = ₹1,200 ✓

**Answer: (a) ₹200, ₹400, ₹600**

---

**Q12. Ratio 3 : 4, difference 8. Find the numbers. → (c) 24, 32**

**Step 1 — Difference in parts.**
$$4 - 3 = 1 \text{ part}$$

**Step 2 — One part = the given difference.**
$$1 \text{ part} = 8$$

**Step 3 — Numbers.**
$$3 \times 8 = 24, \qquad 4 \times 8 = 32$$

**Check:** 32 − 24 = 8 ✓ and 24 : 32 = 3 : 4 ✓

**Answer: (c) 24, 32**

---

**Q13. x : y = 4 : 5. Find (x + y) : (y − x). → (c) 9 : 1**

**Substitute x = 4, y = 5.**

$$x + y = 9 \qquad y - x = 1$$
$$\text{Ratio} = 9 : 1$$

**Answer: (c) 9 : 1**

---

**Q14. A ₹5,000, B ₹7,000, same period, profit ₹3,600. → (b) ₹1,500, ₹2,100**

**Formula used:** Equal time ⇒ profit ratio = capital ratio

**Step 1 — Ratio.**
$$5000 : 7000 = 5 : 7$$

**Step 2 — Total parts and one part.**
$$5 + 7 = 12 \implies \frac{3600}{12} = ₹300$$

**Step 3 — Shares.**
$$A = 5 \times 300 = ₹1{,}500 \qquad B = 7 \times 300 = ₹2{,}100$$

**Check:** 1,500 + 2,100 = ₹3,600 ✓

**Answer: (b) ₹1,500, ₹2,100**

---

**Q15. Simplify 0.5 : 1.5. → (b) 1 : 3**

Multiply both terms by 2 to clear decimals:
$$1 : 3$$

**Answer: (b) 1 : 3**

---

**Q16. a : b = 3 : 4, b : c = 2 : 3. Find a : b : c. → (b) 3 : 4 : 6**

**Step 1 — Identify the shared term.** *b* is 4 in the first ratio and 2 in the second.

**Step 2 — Scale the second ratio so b = 4.**
$$b : c = 2 : 3 \quad (\times 2) \quad \to \quad 4 : 6$$

**Step 3 — Merge.**
$$a : b : c = 3 : 4 : 6$$

**Check:** a/b = 3/4 ✓; b/c = 4/6 = 2/3 ✓

**Answer: (b) 3 : 4 : 6**

---

**Q17. Express 3 : 8 as a percentage. → (c) 37.5%**

$$\frac{3}{8} \times 100 = 37.5\%$$

**Shortcut:** 1/8 = 12.5%, so 3/8 = 3 × 12.5 = 37.5% ✓

**Answer: (c) 37.5%**

---

**Q18. Ratio of 1 km to 400 m. → (c) 5 : 2**

**Step 1 — Convert to a common unit.**
$$1 \text{ km} = 1000 \text{ m}$$

**Step 2 — Form and simplify.**
$$1000 : 400 = 10 : 4 = 5 : 2$$

**Answer: (c) 5 : 2**

---

**Q19. What must be added to each term of 3 : 5 to make it 5 : 7? → (b) 2**

**Method 1 — Direct equation.** Let *x* be added to both terms.
$$\frac{3+x}{5+x} = \frac{5}{7}$$
$$7(3+x) = 5(5+x)$$
$$21 + 7x = 25 + 5x$$
$$2x = 4 \implies x = 2$$

**Method 2 — Formula.**
$$x = \frac{ad - bc}{c - d} = \frac{3(7) - 5(5)}{5 - 7} = \frac{21 - 25}{-2} = 2$$

**Check:** (3 + 2) : (5 + 2) = 5 : 7 ✓

**Answer: (b) 2**

---

**Q20. Divide 108 in the ratio 5 : 4. → (c) 60, 48**

**Step 1 — Total parts.**
$$5 + 4 = 9$$

**Step 2 — One part.**
$$\frac{108}{9} = 12$$

**Step 3 — Parts.**
$$5 \times 12 = 60 \qquad 4 \times 12 = 48$$

**Check:** 60 + 48 = 108 ✓

**Answer: (c) 60, 48**

---

### 🟡 MEDIUM — Solutions 21–40

---

**Q21. A:B = 2:3, B:C = 4:5, C:D = 6:7. Find A:D. → (b) 16 : 35**

**Formula used:** A/D = (A/B) × (B/C) × (C/D)

$$\frac{A}{D} = \frac{2}{3} \times \frac{4}{5} \times \frac{6}{7}$$

**Step 1 — Multiply numerators and denominators.**
$$= \frac{2 \times 4 \times 6}{3 \times 5 \times 7} = \frac{48}{105}$$

**Step 2 — Simplify.**
$$\text{HCF}(48, 105) = 3 \implies \frac{16}{35}$$

**Answer: (b) 16 : 35**

---

**Q22. Sum = 98; 1st:2nd = 2:3, 2nd:3rd = 5:8. Find the second. → (b) 30**

**Step 1 — Chain the ratios via the second number.**
The second term is 3 in the first ratio and 5 in the second. LCM(3, 5) = 15.

$$1\text{st} : 2\text{nd} = 2 : 3 \quad (\times 5) \to 10 : 15$$
$$2\text{nd} : 3\text{rd} = 5 : 8 \quad (\times 3) \to 15 : 24$$

**Step 2 — Combined ratio.**
$$1\text{st} : 2\text{nd} : 3\text{rd} = 10 : 15 : 24$$

**Step 3 — Total parts and one part.**
$$10 + 15 + 24 = 49 \implies \text{one part} = \frac{98}{49} = 2$$

**Step 4 — The second number.**
$$15 \times 2 = 30$$

**Check:** Numbers are 20, 30, 48. Sum = 98 ✓; 20 : 30 = 2 : 3 ✓; 30 : 48 = 5 : 8 ✓

**Answer: (b) 30**

---

**Q23. ₹5,625; A = ½(B+C), B = ¼(A+C). Find A's share. → (c) ₹1,875**

**Key technique: convert each condition into a fraction of the TOTAL.**

**Step 1 — Handle A's condition.**
$$A = \frac{1}{2}(B + C)$$
Since B + C = Total − A:
$$A = \frac{1}{2}(\text{Total} - A) \implies 2A = \text{Total} - A \implies 3A = \text{Total}$$
$$A = \frac{1}{3} \times 5625 = ₹1{,}875$$

**Step 2 — Verify with B's condition (for confidence).**
$$B = \frac{1}{4}(A + C) = \frac{1}{4}(\text{Total} - B) \implies 5B = \text{Total} \implies B = \frac{5625}{5} = ₹1{,}125$$

**Step 3 — Deduce C.**
$$C = 5625 - 1875 - 1125 = ₹2{,}625$$

**Verification:**
- A = ½(1,125 + 2,625) = ½(3,750) = ₹1,875 ✓
- B = ¼(1,875 + 2,625) = ¼(4,500) = ₹1,125 ✓

**Answer: (c) ₹1,875**

> **The general trick:** "X gets 1/n of what the others get together" ⇒ **X gets 1/(n+1) of the total.**
> Here A gets 1/2 of the rest ⇒ A gets 1/3 of the total. B gets 1/4 of the rest ⇒ B gets 1/5 of the total.

---

**Q24. Ratio 3 : 5; subtract 9 from each ⇒ 12 : 23. Find the numbers. → (c) 33, 55**

**Step 1 — Introduce one variable.** Let the numbers be 3*x* and 5*x*.

**Step 2 — Apply the condition.**
$$\frac{3x - 9}{5x - 9} = \frac{12}{23}$$

**Step 3 — Cross-multiply.**
$$23(3x - 9) = 12(5x - 9)$$
$$69x - 207 = 60x - 108$$

**Step 4 — Solve.**
$$9x = 99 \implies x = 11$$

**Step 5 — The numbers.**
$$3(11) = 33, \qquad 5(11) = 55$$

**Check:** (33 − 9) : (55 − 9) = 24 : 46 = 12 : 23 ✓

**Answer: (c) 33, 55**

---

**Q25. A ₹8,000, B ₹10,000, C ₹12,000; profit ₹9,000. C's share? → (c) ₹3,600**

**Step 1 — Capital ratio (equal time).**
$$8000 : 10000 : 12000 = 8 : 10 : 12 = 4 : 5 : 6$$

**Step 2 — Total parts.**
$$4 + 5 + 6 = 15$$

**Step 3 — C's share.**
$$\frac{6}{15} \times 9000 = \frac{2}{5} \times 9000 = ₹3{,}600$$

**Full split for confidence:** A ₹2,400, B ₹3,000, C ₹3,600 — total ₹9,000 ✓

**Answer: (c) ₹3,600**

---

**Q26. A ₹12,000 for 12 months; B ₹18,000 joining after 4 months. Profit ratio? → (a) 1 : 1**

**Formula used:** Profit ratio = Capital × Time

**Step 1 — Determine time periods.**
- A: full year = **12 months**
- B: joins after 4 months ⇒ **8 months**

**Step 2 — Effective capitals.**
$$A: 12{,}000 \times 12 = 1{,}44{,}000$$
$$B: 18{,}000 \times 8 = 1{,}44{,}000$$

**Step 3 — Ratio.**
$$1{,}44{,}000 : 1{,}44{,}000 = 1 : 1$$

> **Trap:** answering 2 : 3 from the capitals alone. Time weighting is essential — B's larger capital is exactly offset by the shorter period.

**Answer: (a) 1 : 1**

---

**Q27. Incomes 5 : 4, expenditures 3 : 2, each saves ₹2,000. First income? → (c) ₹5,000**

**Step 1 — Set up variables.**
Incomes: 5*x*, 4*x* · Expenditures: 3*y*, 2*y*

**Step 2 — Savings equations.**
$$5x - 3y = 2000 \qquad \text{...(i)}$$
$$4x - 2y = 2000 \qquad \text{...(ii)}$$

**Step 3 — Simplify (ii).**
$$2x - y = 1000 \implies y = 2x - 1000$$

**Step 4 — Substitute into (i).**
$$5x - 3(2x - 1000) = 2000$$
$$5x - 6x + 3000 = 2000$$
$$-x = -1000 \implies x = 1000$$

**Step 5 — First person's income.**
$$5x = ₹5{,}000$$

**Verification:**
- Incomes: ₹5,000 and ₹4,000 (5 : 4 ✓)
- y = 2(1000) − 1000 = 1000 ⇒ expenditures ₹3,000 and ₹2,000 (3 : 2 ✓)
- Savings: 5,000 − 3,000 = ₹2,000 ✓ and 4,000 − 2,000 = ₹2,000 ✓

**Answer: (c) ₹5,000**

---

**Q28. a : b = 3 : 4, b : c = 8 : 9. Find a : b : c. → (b) 6 : 8 : 9**

**Step 1 — Shared term b: 4 in the first, 8 in the second. LCM = 8.**

**Step 2 — Scale the first ratio by 2.**
$$a : b = 3 : 4 \quad (\times 2) \to 6 : 8$$

**Step 3 — Merge with b : c = 8 : 9.**
$$a : b : c = 6 : 8 : 9$$

**Check:** 6/8 = 3/4 ✓ and 8/9 ✓

**Answer: (b) 6 : 8 : 9**

---

**Q29. ₹3,500 with A:B = 2:3 and B:C = 4:5. → (b) ₹800, ₹1,200, ₹1,500**

**Step 1 — Combine.** B is 3 and 4; LCM = 12.
$$A : B = 2 : 3 \ (\times 4) \to 8 : 12$$
$$B : C = 4 : 5 \ (\times 3) \to 12 : 15$$
$$A : B : C = 8 : 12 : 15$$

**Step 2 — Total parts and one part.**
$$8 + 12 + 15 = 35 \implies \frac{3500}{35} = ₹100$$

**Step 3 — Shares.**
$$A = ₹800, \quad B = ₹1{,}200, \quad C = ₹1{,}500$$

**Check:** Total ₹3,500 ✓; A : B = 800 : 1200 = 2 : 3 ✓; B : C = 1200 : 1500 = 4 : 5 ✓

**Answer: (b) ₹800, ₹1,200, ₹1,500**

---

**Q30. 2A = 3B = 4C. Find A : B : C. → (c) 6 : 4 : 3**

**Formula used:** If kA = lB = mC, then A : B : C = 1/k : 1/l : 1/m

$$A : B : C = \frac{1}{2} : \frac{1}{3} : \frac{1}{4}$$

**Clear fractions** — multiply throughout by LCM(2, 3, 4) = 12:
$$6 : 4 : 3$$

**Verification:** Let A = 6, B = 4, C = 3.
2(6) = 12; 3(4) = 12; 4(3) = 12 ✓ All equal.

> **Common error:** writing 2 : 3 : 4. Note the relationship is *inverse* — the larger the coefficient, the smaller the variable.

**Answer: (c) 6 : 4 : 3**

---

**Q31. A ₹15,000 × 8 months; B ₹12,000 × 10 months; profit ₹8,000. B's share? → (b) ₹4,000**

**Step 1 — Effective capitals.**
$$A: 15{,}000 \times 8 = 1{,}20{,}000$$
$$B: 12{,}000 \times 10 = 1{,}20{,}000$$

**Step 2 — Ratio.**
$$1 : 1$$

**Step 3 — B's share.**
$$\frac{1}{2} \times 8000 = ₹4{,}000$$

**Answer: (b) ₹4,000**

---

**Q32. Coins 50p : 25p : 10p in ratio 5 : 9 : 4, total ₹206. Number of 25p coins? → (c) 360**

**Step 1 — Let the counts be 5x, 9x, 4x.**

**Step 2 — Convert counts to rupee value.**
$$5x \times 0.50 = 2.50x$$
$$9x \times 0.25 = 2.25x$$
$$4x \times 0.10 = 0.40x$$

**Step 3 — Sum and equate.**
$$2.50x + 2.25x + 0.40x = 206$$
$$5.15x = 206$$

**Step 4 — Solve.**
$$x = \frac{206}{5.15} = \frac{20600}{515} = 40$$

**Step 5 — Number of 25p coins.**
$$9x = 9 \times 40 = 360$$

**Verification:**
| Coin | Count | Value |
|---|---|---|
| 50p | 200 | ₹100 |
| 25p | 360 | ₹90 |
| 10p | 160 | ₹16 |
| | | **₹206** ✓ |

> **The trap:** splitting ₹206 in the ratio 5 : 9 : 4. The ratio given is by **number of coins**, not by value.

**Answer: (c) 360**

---

**Q33. x/2 = y/3 = z/5. Find (x + y + z)/z. → (b) 2**

**Step 1 — Introduce the common ratio k.**
$$\frac{x}{2} = \frac{y}{3} = \frac{z}{5} = k \implies x = 2k, \; y = 3k, \; z = 5k$$

**Step 2 — Compute the sum.**
$$x + y + z = 2k + 3k + 5k = 10k$$

**Step 3 — Divide by z.**
$$\frac{10k}{5k} = 2$$

**Answer: (b) 2**

---

**Q34. 45 L, milk : water = 4 : 1. Add water for 3 : 2. → (b) 15 L**

**Step 1 — Current quantities.**
Total parts = 5 ⇒ one part = 45/5 = 9 L
$$\text{Milk} = 4 \times 9 = 36 \text{ L} \qquad \text{Water} = 1 \times 9 = 9 \text{ L}$$

**Step 2 — Key insight: adding water leaves the milk unchanged.**
Milk stays at **36 L**.

**Step 3 — Find the water needed for a 3 : 2 ratio.**
$$\frac{\text{Milk}}{\text{Water}} = \frac{3}{2} \implies \text{Water} = 36 \times \frac{2}{3} = 24 \text{ L}$$

**Step 4 — Water to add.**
$$24 - 9 = 15 \text{ L}$$

**Verification:** New mixture = 36 L milk + 24 L water = 60 L, ratio 36 : 24 = 3 : 2 ✓

**Answer: (b) 15 L**

---

**Q35. A invests 3× B; B invests ⅔ of C. Profit ratio? → (b) 6 : 2 : 3**

**Step 1 — Start from C, the term expressed as a fraction.**
Let C = 3 units (chosen so that ⅔ of C is a whole number).

**Step 2 — Find B.**
$$B = \frac{2}{3} \times 3 = 2 \text{ units}$$

**Step 3 — Find A.**
$$A = 3 \times B = 3 \times 2 = 6 \text{ units}$$

**Step 4 — Form the ratio.**
$$A : B : C = 6 : 2 : 3$$

**Verification:** A = 6, B = 2, C = 3.
- Is A three times B? 6 = 3 × 2 ✓
- Is B two-thirds of C? 2 = (2/3) × 3 ✓

**Answer: (b) 6 : 2 : 3**

---

**Q36. ₹1,870; A = ⅓ of B; B = ½ of C. → (b) ₹187, ₹561, ₹1,122**

**Step 1 — Express everything in terms of the largest, C.**
Let C = 6*k* (chosen so all shares are whole).
$$B = \frac{1}{2} \times 6k = 3k$$
$$A = \frac{1}{3} \times 3k = k$$

**Step 2 — Sum and solve.**
$$k + 3k + 6k = 10k = 1870 \implies k = 187$$

**Step 3 — Shares.**
$$A = ₹187, \quad B = 3 \times 187 = ₹561, \quad C = 6 \times 187 = ₹1{,}122$$

**Verification:**
- Total: 187 + 561 + 1,122 = ₹1,870 ✓
- A = ⅓ of B: 561/3 = 187 ✓
- B = ½ of C: 1,122/2 = 561 ✓

**Answer: (b) ₹187, ₹561, ₹1,122**

---

**Q37. (a+b) : (b+c) : (c+a) = 6 : 7 : 8 and a+b+c = 14. Find c. → (c) 6**

**Step 1 — Note what the three sums add up to.**
$$(a+b) + (b+c) + (c+a) = 2(a+b+c) = 2 \times 14 = 28$$

**Step 2 — Total ratio parts.**
$$6 + 7 + 8 = 21$$

**Step 3 — Value of one part.**
$$\frac{28}{21} = \frac{4}{3}$$

**Step 4 — Find (a + b), then c.**
$$a + b = 6 \times \frac{4}{3} = 8$$
$$c = (a+b+c) - (a+b) = 14 - 8 = 6$$

**Verification:**
$$b + c = 7 \times \tfrac{4}{3} = \tfrac{28}{3}, \qquad c + a = 8 \times \tfrac{4}{3} = \tfrac{32}{3}$$
From a + b = 8 and a + b + c = 14, c = 6 ✓
Then b = (b+c) − c = 28/3 − 6 = 10/3, and a = 8 − 10/3 = 14/3.
Check c + a = 6 + 14/3 = 32/3 ✓

**Answer: (c) 6**

> **Technique:** whenever pairwise sums are given in a ratio, add all of them — you get twice the grand total. That single observation unlocks the problem.

---

**Q38. Vessels with milk:water = 4:1 and 3:2; equal quantities mixed. New ratio? → (c) 7 : 3**

**Step 1 — Take a convenient equal quantity from each vessel.**
Take **5 litres** from each (5 = sum of parts in both ratios).

**Step 2 — Compute the contents of each 5-litre sample.**

| Vessel | Ratio | Milk | Water |
|---|---|---|---|
| I | 4 : 1 | 4 L | 1 L |
| II | 3 : 2 | 3 L | 2 L |
| **Mixed** | | **7 L** | **3 L** |

**Step 3 — New ratio.**
$$\text{Milk} : \text{Water} = 7 : 3$$

**Fraction method (works for any quantities):**
$$\text{Milk fraction} = \frac{1}{2}\left(\frac{4}{5} + \frac{3}{5}\right) = \frac{1}{2} \times \frac{7}{5} = \frac{7}{10}$$
$$\text{Water fraction} = \frac{3}{10} \implies 7 : 3 \checkmark$$

**Answer: (c) 7 : 3**

---

**Q39. Ages 4 : 5 now; 5 : 6 after 6 years. A's present age? → (c) 24 years**

**Step 1 — Represent present ages.**
Let A = 4*x* and B = 5*x*.

**Step 2 — Ages after 6 years.**
$$A = 4x + 6, \qquad B = 5x + 6$$

**Step 3 — Apply the future ratio.**
$$\frac{4x + 6}{5x + 6} = \frac{5}{6}$$

**Step 4 — Cross-multiply.**
$$6(4x + 6) = 5(5x + 6)$$
$$24x + 36 = 25x + 30$$

**Step 5 — Solve.**
$$x = 6$$

**Step 6 — A's present age.**
$$4x = 24 \text{ years}$$

**Verification:** Present ages 24 and 30 (ratio 4 : 5 ✓). After 6 years: 30 and 36, ratio 30 : 36 = 5 : 6 ✓

**Answer: (c) 24 years**

---

**Q40. P : Q : R = 3 : 5 : 7; R gets ₹800 more than P. Total? → (c) ₹3,000**

**Step 1 — Difference in parts.**
$$R - P = 7 - 3 = 4 \text{ parts}$$

**Step 2 — Value of one part.**
$$4 \text{ parts} = ₹800 \implies 1 \text{ part} = ₹200$$

**Step 3 — Total.**
$$(3 + 5 + 7) \times 200 = 15 \times 200 = ₹3{,}000$$

**Verification:** P = ₹600, Q = ₹1,000, R = ₹1,400. R − P = ₹800 ✓; total = ₹3,000 ✓

**Answer: (c) ₹3,000**

---

### 🔴 HARD — Solutions 41–50

---

**Q41. A ₹20,000×12; B ₹30,000 for 6 mo then ₹20,000 for 6 mo; C ₹25,000×8; profit ₹37,000. B's share? → (c) ₹15,000**

**Step 1 — Build the effective-capital table.**

| Partner | Capital × Time | Effective capital |
|---|---|---|
| A | 20,000 × 12 | 2,40,000 |
| B | 30,000 × 6 = 1,80,000<br>20,000 × 6 = 1,20,000 | **3,00,000** |
| C | 25,000 × 8 | 2,00,000 |

*Note on B:* after withdrawing ₹10,000 from ₹30,000, B continues with ₹20,000 for the remaining 6 months.
*Note on C:* "the last eight months" means C invests for 8 months.

**Step 2 — Form and reduce the ratio.**
$$2{,}40{,}000 : 3{,}00{,}000 : 2{,}00{,}000$$

Divide by 20,000:
$$12 : 15 : 10$$

**Step 3 — Total parts.**
$$12 + 15 + 10 = 37$$

**Step 4 — Value of one part.**
$$\frac{37{,}000}{37} = ₹1{,}000$$

**Step 5 — B's share.**
$$15 \times 1000 = ₹15{,}000$$

**Full split:** A = ₹12,000, B = ₹15,000, C = ₹10,000. Total = ₹37,000 ✓

**Answer: (c) ₹15,000**

---

**Q42. Incomes 4 : 3, expenditures 3 : 2, each saves ₹6,000. A's income? → (c) ₹24,000**

**Step 1 — Set up.**
Incomes: 4*x* and 3*x* · Expenditures: 3*y* and 2*y*

**Step 2 — Savings equations.**
$$4x - 3y = 6000 \qquad \text{...(i)}$$
$$3x - 2y = 6000 \qquad \text{...(ii)}$$

**Step 3 — Eliminate y.**
(i) × 2: $\;8x - 6y = 12{,}000$
(ii) × 3: $\;9x - 6y = 18{,}000$

Subtracting the first from the second:
$$x = 6000$$

**Step 4 — A's income.**
$$4x = 4 \times 6000 = ₹24{,}000$$

**Verification:**
From (ii): 3(6,000) − 2y = 6,000 ⇒ y = 6,000
- Incomes: ₹24,000 and ₹18,000 → 4 : 3 ✓
- Expenditures: ₹18,000 and ₹12,000 → 3 : 2 ✓
- Savings: ₹6,000 each ✓

**Answer: (c) ₹24,000**

---

**Q43. ₹6,300; ½A = ⅓B = ¼C. Find C's share. → (c) ₹2,800**

**Step 1 — Set the common value to k.**
$$\frac{A}{2} = \frac{B}{3} = \frac{C}{4} = k$$
$$A = 2k, \quad B = 3k, \quad C = 4k$$

**Step 2 — Sum and solve.**
$$2k + 3k + 4k = 9k = 6300 \implies k = 700$$

**Step 3 — C's share.**
$$C = 4 \times 700 = ₹2{,}800$$

**Verification:** A = ₹1,400, B = ₹2,100, C = ₹2,800. Total = ₹6,300 ✓
Half of A = 700; a third of B = 700; a quarter of C = 700 ✓ All equal.

> **Note the direction:** ½A = ⅓B = ¼C gives A : B : C = **2 : 3 : 4** (direct), whereas 2A = 3B = 4C gives **6 : 4 : 3** (inverse). Read whether the coefficient multiplies or divides.

**Answer: (c) ₹2,800**

---

**Q44. Milk : water = 5 : 1; add 5 L water ⇒ 5 : 2. Find the milk. → (b) 25 L**

**Step 1 — Represent the original mixture.**
Let milk = 5*x* and water = *x*.

**Step 2 — Adding water leaves the milk unchanged.**
$$\text{Milk} = 5x \text{ (unchanged)}, \qquad \text{Water} = x + 5$$

**Step 3 — Apply the new ratio.**
$$\frac{5x}{x + 5} = \frac{5}{2}$$

**Step 4 — Cross-multiply.**
$$10x = 5(x + 5) = 5x + 25$$
$$5x = 25 \implies x = 5$$

**Step 5 — Quantity of milk.**
$$5x = 25 \text{ L}$$

**Verification:** Original: 25 L milk, 5 L water (ratio 5 : 1 ✓).
After adding 5 L water: 25 L milk, 10 L water ⇒ 25 : 10 = 5 : 2 ✓

**Answer: (b) 25 L**

---

**Q45. A : B invest 3 : 2; A takes 15% commission; A gets ₹4,800 more. Total profit? → (c) ₹15,000**

**Step 1 — Let total profit = P. Deduct the commission first.**
$$\text{A's commission} = 0.15P$$
$$\text{Distributable profit} = 0.85P$$

**Step 2 — Split the remainder 3 : 2 (5 parts).**
$$\text{A's investment share} = \frac{3}{5} \times 0.85P = 0.51P$$
$$\text{B's share} = \frac{2}{5} \times 0.85P = 0.34P$$

**Step 3 — A's total earnings.**
$$0.15P + 0.51P = 0.66P$$

**Step 4 — Apply the difference condition.**
$$0.66P - 0.34P = 4800$$
$$0.32P = 4800$$

**Step 5 — Solve.**
$$P = \frac{4800}{0.32} = ₹15{,}000$$

**Verification:**
| Item | Amount |
|---|---|
| Total profit | ₹15,000 |
| A's commission (15%) | ₹2,250 |
| Distributable | ₹12,750 |
| A's investment share (3/5) | ₹7,650 |
| B's share (2/5) | ₹5,100 |
| **A's total** | **₹9,900** |
| **Difference** | 9,900 − 5,100 = **₹4,800** ✓ |

> **Order matters:** the commission comes off the top *before* the capital-ratio split. Splitting first and then adding the commission gives a different (wrong) answer.

**Answer: (c) ₹15,000**

---

**Q46. Ratio 7 : 9; add 12 to each ⇒ 5 : 6. Smaller number? → (c) 28**

**Step 1 — Represent with one variable.**
Numbers are 7*x* and 9*x*.

**Step 2 — Apply the condition.**
$$\frac{7x + 12}{9x + 12} = \frac{5}{6}$$

**Step 3 — Cross-multiply.**
$$6(7x + 12) = 5(9x + 12)$$
$$42x + 72 = 45x + 60$$

**Step 4 — Solve.**
$$12 = 3x \implies x = 4$$

**Step 5 — Smaller number.**
$$7x = 28$$

**Verification:** Numbers 28 and 36. Adding 12: 40 and 48 ⇒ 40 : 48 = 5 : 6 ✓

**Answer: (c) 28**

---

**Q47. 60 L, milk : water = 3 : 1. Replace how much with water for 1 : 1? → (c) 20 L**

**Step 1 — Current quantities.**
Total parts = 4 ⇒ one part = 15 L
$$\text{Milk} = 45 \text{ L}, \qquad \text{Water} = 15 \text{ L}$$

**Step 2 — Understand "drawn off and replaced".**
Removing *x* litres of **mixture** removes milk and water in the current 3 : 1 proportion — so it removes (3/4)*x* litres of milk. Replacing with pure water keeps the **total at 60 L**.

**Step 3 — Target the milk quantity.**
For a 1 : 1 ratio in 60 L, milk must be **30 L**.

**Step 4 — Set up the milk equation.**
$$45 - \frac{3}{4}x = 30$$
$$\frac{3}{4}x = 15$$
$$x = 20 \text{ L}$$

**Verification:**
- Draw off 20 L of mixture ⇒ removes 15 L milk and 5 L water
- Remaining: 30 L milk, 10 L water (total 40 L)
- Add 20 L water ⇒ 30 L milk, 30 L water = 60 L, ratio **1 : 1** ✓

**⚡ Faster route — the milk fraction:** milk must go from 3/4 of the volume to 1/2. Since replacement preserves the total volume, the milk *fraction* is multiplied by (1 − x/60):
$$\frac{3}{4}\left(1 - \frac{x}{60}\right) = \frac{1}{2} \implies 1 - \frac{x}{60} = \frac{2}{3} \implies \frac{x}{60} = \frac{1}{3} \implies x = 20 \checkmark$$

**Answer: (c) 20 L**

---

**Q48. A+B+C = ₹50,000; A = B + 4,000; B = C + 5,000; profit ₹35,000. A's share? → (b) ₹14,700**

**Step 1 — Express everything in terms of C.**
$$B = C + 5{,}000$$
$$A = B + 4{,}000 = C + 9{,}000$$

**Step 2 — Write the total.**
$$(C + 9000) + (C + 5000) + C = 50{,}000$$
$$3C + 14{,}000 = 50{,}000$$
$$3C = 36{,}000 \implies C = ₹12{,}000$$

**Step 3 — Find B and A.**
$$B = 12{,}000 + 5{,}000 = ₹17{,}000$$
$$A = 17{,}000 + 4{,}000 = ₹21{,}000$$

**Step 4 — Form the profit ratio.**
$$21{,}000 : 17{,}000 : 12{,}000 = 21 : 17 : 12 \quad (\text{sum} = 50)$$

**Step 5 — A's share of the profit.**
$$\frac{21}{50} \times 35{,}000 = 21 \times 700 = ₹14{,}700$$

**Verification:**
- Capitals: 21,000 + 17,000 + 12,000 = ₹50,000 ✓
- Shares: A ₹14,700, B = (17/50) × 35,000 = ₹11,900, C = (12/50) × 35,000 = ₹8,400
- Total: 14,700 + 11,900 + 8,400 = ₹35,000 ✓

**Answer: (b) ₹14,700**

---

**Q49. Boys : girls = 3 : 2; 20% of boys and 25% of girls hold scholarships. % without? → (c) 78%**

**Step 1 — Assume a convenient total.**
Let there be 100 students. With a 3 : 2 ratio (5 parts):
$$\text{Boys} = 60, \qquad \text{Girls} = 40$$

**Step 2 — Count scholarship holders.**
$$\text{Boys with scholarship} = 20\% \text{ of } 60 = 12$$
$$\text{Girls with scholarship} = 25\% \text{ of } 40 = 10$$
$$\text{Total} = 22$$

**Step 3 — Compute the complement.**
$$100 - 22 = 78 \implies \mathbf{78\%}$$

> **Trap:** averaging 20% and 25% to 22.5% and answering 77.5%. The groups are unequal (60 vs 40), so the boys' rate carries more weight — the true scholarship rate is 22%, not 22.5%.

**Answer: (c) 78%**

---

**Q50. a:b = c:d = e:f = 3:5. Find (2a + 3c + 4e) : (2b + 3d + 4f). → (b) 3 : 5**

**Formula used:** The equal-ratio (weighted-sum) theorem.

**Step 1 — State the theorem.**
If $\dfrac{a}{b} = \dfrac{c}{d} = \dfrac{e}{f} = k$, then for any weights λ₁, λ₂, λ₃:
$$\frac{\lambda_1 a + \lambda_2 c + \lambda_3 e}{\lambda_1 b + \lambda_2 d + \lambda_3 f} = k$$

**Step 2 — Apply with k = 3/5 and weights 2, 3, 4.**
$$\frac{2a + 3c + 4e}{2b + 3d + 4f} = \frac{3}{5}$$

**Step 3 — Verify with concrete numbers.**
Take a = 3, b = 5; c = 6, d = 10; e = 9, f = 15 (each pair in the ratio 3 : 5).

$$2a + 3c + 4e = 2(3) + 3(6) + 4(9) = 6 + 18 + 36 = 60$$
$$2b + 3d + 4f = 2(5) + 3(10) + 4(15) = 10 + 30 + 60 = 100$$
$$60 : 100 = 3 : 5 \checkmark$$

**Answer: (b) 3 : 5**

> **Why this works:** since a = (3/5)b, c = (3/5)d and e = (3/5)f, every term in the numerator is exactly 3/5 of the matching term in the denominator. Factoring out 3/5 leaves the denominator itself.

---

## 8. Quick Revision Sheet

> **One page. Read 48 hours after study, and again the night before the test.**

### Core operations

```
a : b  =  a/b            (same units required — convert FIRST)
One part = Total / (sum of ratio terms)
Share of a term = (its term / sum of terms) × Total
```

### Combining ratios

```
a:b and b:c  →  scale so b matches, then merge
   3:4 and 8:9   →   6:8 and 8:9   →   6:8:9

a:d from a:b, b:c, c:d  →  multiply antecedents / multiply consequents
   2:3, 4:5, 6:7  →  (2·4·6) : (3·5·7) = 48:105 = 16:35
```

### Proportion

```
a:b :: c:d   ⟺   ad = bc
Fourth proportional to a,b,c   =  bc/a
Third  proportional to a,b     =  b²/a
Mean   proportional of a,b     =  √(ab)

Componendo & Dividendo:  a/b = c/d  →  (a+b)/(a−b) = (c+d)/(c−d)
```

### Key conversions

```
kA = lB = mC       →   A:B:C = 1/k : 1/l : 1/m   (INVERSE)
A/k = B/l = C/m    →   A:B:C = k : l : m          (DIRECT)

2A = 3B = 4C       →   6 : 4 : 3
A/2 = B/3 = C/4    →   2 : 3 : 4
```

### Equal-ratio theorem

```
a/p = b/q = c/r = k   →   (λ₁a + λ₂b + λ₃c)/(λ₁p + λ₂q + λ₃r) = k
```

### Word-problem templates

```
"X gets 1/n of what the others get together"  →  X gets 1/(n+1) of the TOTAL
Add x to both terms of a:b to get c:d         →  x = (ad − bc)/(c − d)
Difference of shares = (difference in parts) × (value of one part)
Pairwise sums (a+b),(b+c),(c+a) given         →  their total = 2(a+b+c)
```

### Income–expenditure–savings

```
Incomes a:b, Expenditures c:d, Savings S₁ and S₂
    ax − cy = S₁
    bx − dy = S₂     →  solve for x, then income₁ = ax
```

### Partnership

```
Profit ratio = Capital × Time  (build a TABLE, always)

Same duration      →  ratio of capitals
Different duration →  ratio of capital × months
Capital changes    →  sum the segments:  C₁T₁ + C₂T₂
Working partner    →  deduct salary/commission FIRST, split the rest
```

### Mixtures

```
Add only ONE component  →  anchor on the component that DOESN'T change
Replace part of mixture →  new milk fraction = old fraction × (1 − x/Total)
Mix equal volumes of ratios p:q and r:s
    → milk fraction = ½ [ p/(p+q) + r/(r+s) ]
```

### Ratio ↔ percentage

```
5:4 → 25% more    6:5 → 20% more    3:2 → 50% more
4:5 → 20% less    3:4 → 25% less    2:3 → 33⅓% less
```

---

## 9. Common Mistakes

| # | Mistake | Example | Correction |
|---|---|---|---|
| 1 | **Forming a ratio across units** | 2 hours : 40 min = 1 : 20 | Convert first: 120 : 40 = 3 : 1 |
| 2 | **Splitting by number ratio instead of value ratio** | ₹206 split 5 : 9 : 4 for coins | Multiply counts by coin values first |
| 3 | **Ignoring time in partnership** | Capitals 12,000 : 18,000 ⇒ 2 : 3 | Include months: 12k×12 : 18k×8 = 1 : 1 |
| 4 | **kA = lB = mC read as direct** | 2A = 3B = 4C ⇒ 2 : 3 : 4 | Invert: 1/2 : 1/3 : 1/4 = 6 : 4 : 3 |
| 5 | **Two variables where one suffices** | Setting a, b separately in a 3 : 5 ratio | Use 3x and 5x — halves the algebra |
| 6 | **Adding to only one term** | "Add 9 to each" applied once | Apply to both antecedent and consequent |
| 7 | **"1/n of the rest" read as 1/n of total** | A = ½(B+C) ⇒ A = half the total | A = 1/3 of the total |
| 8 | **Averaging unequal groups** | 20% and 25% ⇒ 22.5% | Weight by 3 : 2 ⇒ 22% |
| 9 | **Commission added after the split** | Split first, then add 15% | Deduct commission first, then split |
| 10 | **Replacement treated as pure removal** | Removing 20 L removes 20 L of milk | It removes milk *in proportion*: (3/4)(20) = 15 L |
| 11 | **Answering the wrong term** | Asked for the second, gave the third | Underline what is asked |
| 12 | **Not reducing before dividing** | Working with 2,40,000 : 3,00,000 : 2,00,000 | Reduce to 12 : 15 : 10 first |

---

## Practice Answer Key

| Q | Ans | Q | Ans | Q | Ans | Q | Ans | Q | Ans |
|---|---|---|---|---|---|---|---|---|---|
| 1 | a | 11 | a | 21 | b | 31 | b | 41 | c |
| 2 | b | 12 | c | 22 | b | 32 | c | 42 | c |
| 3 | b | 13 | c | 23 | c | 33 | b | 43 | c |
| 4 | b | 14 | b | 24 | c | 34 | b | 44 | b |
| 5 | c | 15 | b | 25 | c | 35 | b | 45 | c |
| 6 | c | 16 | b | 26 | a | 36 | b | 46 | c |
| 7 | c | 17 | c | 27 | c | 37 | c | 47 | c |
| 8 | c | 18 | c | 28 | b | 38 | c | 48 | b |
| 9 | b | 19 | b | 29 | b | 39 | c | 49 | c |
| 10 | c | 20 | c | 30 | c | 40 | c | 50 | b |

**Scoring guide:** 45+/50 → strong. 35–44 → solid; drill partnership and mixture-replacement. Below 35 → re-read Sections 2.3, 2.8 and 4.1, then redo the Medium set.

---

**⬅️ Back:** [Topic 2 — Profit, Loss & Discount](02-profit-loss-discount.md) · **➡️ Next:** [Topic 4 — Averages, Mixtures & Alligation](04-averages-mixtures-alligation.md)
