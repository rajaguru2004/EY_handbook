# Topic 4 — Averages, Mixtures & Alligation

### EY Placement Aptitude Handbook · Priority Rank #11 · 🟠 High

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

**Weightage:** 6–8% of the quantitative section — typically **1 question**, sometimes embedded in a DI set.

**Why it earns its place in your prep:** the **alligation rule** is one of the highest-leverage shortcuts in all of aptitude. Problems that take 90 seconds algebraically collapse to 15 seconds with a cross-diagram. That time saving compounds across an entire section.

**Question styles reported:**

| Style | Typical shape |
|---|---|
| Simple average | "Average of 5 numbers is 27; one is excluded…" |
| Average with an inclusion/exclusion | "Teacher's age included, average rises by 1" |
| Replacement of a member | "New person replaces one weighing 65 kg" |
| Combined/weighted average | "30 results averaging 20 and 20 results averaging 30" |
| Alligation — price mixing | "In what ratio must ₹15 and ₹20 rice be mixed for ₹18?" |
| Alligation — concentration | "Two vessels with milk:water 5:2 and 3:4" |
| Repeated replacement | "8 L drawn and replaced by water, three times" |
| Average speed | "40 km/h out, 60 km/h back" |

**Prerequisite:** [Topic 3 — Ratio & Proportion](03-ratio-proportion-partnership.md). Alligation *is* a ratio technique.

---

## 2. Core Concepts

### 2.1 The average

$$\text{Average} = \frac{\text{Sum of all observations}}{\text{Number of observations}}$$

Rearranged — and this is the form you will actually use:

$$\boxed{\text{Sum} = \text{Average} \times \text{Count}}$$

**Almost every average problem is solved by converting averages into sums, manipulating the sums, and converting back.** Train yourself to write the sum on the first line.

### 2.2 Properties of the average

| Property | Effect on the average |
|---|---|
| Add *k* to every observation | Average increases by *k* |
| Subtract *k* from every observation | Average decreases by *k* |
| Multiply every observation by *k* | Average is multiplied by *k* |
| Divide every observation by *k* | Average is divided by *k* |

The average always lies **between the smallest and largest** observation. Use this as a sanity check.

### 2.3 Averages of standard sequences

| Sequence | Average |
|---|---|
| First *n* natural numbers (1…n) | $\dfrac{n+1}{2}$ |
| First *n* even numbers (2, 4, …, 2n) | $n + 1$ |
| First *n* odd numbers (1, 3, …, 2n−1) | $n$ |
| First *n* multiples of *k* | $\dfrac{k(n+1)}{2}$ |
| Any set of consecutive numbers | $\dfrac{\text{first} + \text{last}}{2}$ = the middle term |
| Squares of first *n* naturals | $\dfrac{(n+1)(2n+1)}{6}$ |
| Cubes of first *n* naturals | $\dfrac{n(n+1)^2}{4}$ |

> **The consecutive-numbers rule is worth memorising:** for any arithmetic progression, the average equals the middle term (odd count) or the mean of the two middle terms (even count). It also equals (first + last)/2.

### 2.4 The four standard average manoeuvres

These four cover the vast majority of average questions.

**(a) Inclusion — a new member joins**

$$\text{New person's value} = \text{New average} + n \times (\text{change in average})$$

More reliably, just work with sums:

> 20 students average 16. Adding the teacher raises the average to 17.
> Old sum = 20 × 16 = 320. New sum = 21 × 17 = 357.
> **Teacher's age = 357 − 320 = 37.**

**(b) Exclusion — a member leaves**

> 5 numbers average 27. Removing one leaves an average of 25.
> Old sum = 135. New sum = 4 × 25 = 100.
> **Excluded number = 135 − 100 = 35.**

**(c) Replacement — one member swaps for another**

$$\text{New value} = \text{Old value} + n \times (\text{change in average})$$

> 8 people; a newcomer replaces someone weighing 65 kg and the average rises 2.5 kg.
> **New weight = 65 + 8 × 2.5 = 85 kg.**

The logic: the total must rise by 8 × 2.5 = 20 kg, and the only change is the swap.

**(d) Correction of a misread value**

$$\text{Change in average} = \frac{\text{Correct value} - \text{Wrong value}}{n}$$

> 50 students average 62; a mark of 78 was recorded as 128.
> The total was overstated by 50, so the average was overstated by 50/50 = 1.
> **Correct average = 61.**

### 2.5 Weighted average

When groups of different sizes are combined:

$$\text{Weighted average} = \frac{n_1 A_1 + n_2 A_2 + \cdots}{n_1 + n_2 + \cdots}$$

> 30 results averaging 20, and 20 results averaging 30:
> $$\frac{30(20) + 20(30)}{50} = \frac{600 + 600}{50} = 24$$

> **Note it is 24, not 25.** The simple mean of 20 and 30 is 25, but the larger group pulls the answer toward its own average. Never average averages without weighting.

### 2.6 Average speed

$$\text{Average speed} = \frac{\text{Total distance}}{\text{Total time}}$$

**Never** the arithmetic mean of the speeds.

**Special case — equal distances at speeds *u* and *v* (the harmonic mean):**

$$\boxed{\text{Average speed} = \frac{2uv}{u+v}}$$

> Out at 40 km/h, back at 60 km/h:
> $$\frac{2 \times 40 \times 60}{100} = \frac{4800}{100} = 48 \text{ km/h}$$
> (Not 50 — you spend more time at the slower speed.)

**For three equal distances at u, v, w:**
$$\text{Average speed} = \frac{3uvw}{uv + vw + wu}$$

**For equal *times* (not distances) the arithmetic mean IS correct:**
$$\text{Average speed} = \frac{u+v}{2}$$

### 2.7 The Alligation Rule

**The single most valuable shortcut in this topic.**

When two ingredients of values *c* (cheaper) and *d* (dearer) are mixed to produce a mean value *m*:

$$\boxed{\frac{\text{Quantity of cheaper}}{\text{Quantity of dearer}} = \frac{d - m}{m - c}}$$

**The cross diagram:**

```
        Cheaper (c)              Dearer (d)
             \                      /
              \                    /
               \                  /
                 Mean price (m)
               /                  \
              /                    \
         (d − m)                 (m − c)
             │                       │
    Quantity of CHEAPER  :  Quantity of DEARER
```

**Read it as: each quantity gets the difference on the OPPOSITE side.**

**Worked example:** Rice at ₹15/kg and ₹20/kg mixed to give ₹18/kg.

```
        15                    20
          \                  /
              \          /
                  18
              /          \
        (20−18)=2      (18−15)=3
        
   Cheaper : Dearer  =  2 : 3
```

**Verify:** 2 kg at ₹15 = ₹30; 3 kg at ₹20 = ₹60. Total ₹90 for 5 kg ⇒ ₹18/kg ✓

**Why it works:** the mixture's total value must equal the sum of the parts.
$$c \cdot x + d \cdot y = m(x+y) \implies x(m - c) = y(d - m) \implies \frac{x}{y} = \frac{d-m}{m-c} \;∎$$

**Alligation applies to ANY quantity that averages linearly:** price, concentration, percentage, speed (over equal times), marks, age, profit rate — anything.

### 2.8 Alligation with water (free ingredient)

Water is treated as having a value of **₹0**.

> *"In what ratio must water be mixed with milk costing ₹32/L to make the mixture worth ₹28/L?"*

```
      Water (0)              Milk (32)
            \                   /
                \           /
                    28
                /           \
         (32−28)=4        (28−0)=28
         
    Water : Milk = 4 : 28 = 1 : 7
```

### 2.9 Alligation for profit through dilution

> *"Milk costing ₹36/L is diluted with water and sold at ₹36/L for a 20% profit. Find the water : milk ratio."*

**Key step:** if the mixture sells at ₹36 with 20% profit, the mixture's **cost** must be:
$$\frac{36}{1.20} = ₹30 \text{ per litre}$$

Now alligate water (₹0) against milk (₹36) with mean ₹30:
$$\text{Water} : \text{Milk} = (36-30) : (30-0) = 6 : 30 = \mathbf{1 : 5}$$

**Shortcut for this specific pattern:**
$$\boxed{\frac{\text{Water}}{\text{Milk}} = \frac{\text{Profit\%}}{100}}$$
20% profit ⇒ water : milk = 20 : 100 = 1 : 5 ✓

### 2.10 Repeated replacement (the removal formula)

A vessel holds *A* units of pure liquid. *B* units are removed and replaced by water. This is repeated *n* times.

$$\boxed{\text{Liquid remaining} = A\left(1 - \frac{B}{A}\right)^n = A\left(\frac{A-B}{A}\right)^n}$$

> 60 L of milk; 6 L drawn and replaced by water, three times:
> $$60 \times \left(\frac{54}{60}\right)^3 = 60 \times (0.9)^3 = 60 \times 0.729 = 43.74 \text{ L}$$

**Note:** the total volume always returns to *A* after each replacement, so water remaining = A − (liquid remaining).

### 2.11 Single replacement (drawn off and replaced once)

When *x* units of a **mixture** are drawn off and replaced by one pure component, the *other* component's fraction shrinks by the factor (1 − x/Total):

$$\text{New fraction of removed-component} = \text{Old fraction} \times \left(1 - \frac{x}{\text{Total}}\right)$$

This is the fastest route through "replace part of a mixture" questions — see Solved Example 8.

---

## 3. Formula Bank

| # | Concept | Formula |
|---|---|---|
| 1 | Average | $\dfrac{\text{Sum}}{\text{Count}}$ |
| 2 | Sum | $\text{Average} \times \text{Count}$ |
| 3 | Average of first *n* naturals | $\dfrac{n+1}{2}$ |
| 4 | Average of first *n* even numbers | $n+1$ |
| 5 | Average of first *n* odd numbers | $n$ |
| 6 | Average of consecutive numbers | $\dfrac{\text{first}+\text{last}}{2}$ |
| 7 | Average of first *n* multiples of *k* | $\dfrac{k(n+1)}{2}$ |
| 8 | New member's value (inclusion) | $\text{New sum} - \text{Old sum}$ |
| 9 | Excluded value | $\text{Old sum} - \text{New sum}$ |
| 10 | Replacement | $\text{New} = \text{Old} + n \times \Delta\text{Average}$ |
| 11 | Misread correction | $\Delta\text{Average} = \dfrac{\text{Correct} - \text{Wrong}}{n}$ |
| 12 | Weighted average | $\dfrac{n_1A_1 + n_2A_2}{n_1+n_2}$ |
| 13 | Average speed (general) | $\dfrac{\text{Total distance}}{\text{Total time}}$ |
| 14 | Average speed, equal distances | $\dfrac{2uv}{u+v}$ |
| 15 | Average speed, 3 equal distances | $\dfrac{3uvw}{uv+vw+wu}$ |
| 16 | Average speed, equal times | $\dfrac{u+v}{2}$ |
| 17 | **Alligation** | $\dfrac{Q_{\text{cheaper}}}{Q_{\text{dearer}}} = \dfrac{d-m}{m-c}$ |
| 18 | Repeated replacement (*n* times) | $A\left(\dfrac{A-B}{A}\right)^n$ |
| 19 | Single replacement of *x* from total *T* | New fraction $=$ Old fraction $\times \left(1 - \dfrac{x}{T}\right)$ |
| 20 | Dilution for profit *p*% at cost price | $\dfrac{\text{Water}}{\text{Pure}} = \dfrac{p}{100}$ |
| 21 | *n* observations, middle term of AP | Average = middle term |
| 22 | Average of squares of first *n* naturals | $\dfrac{(n+1)(2n+1)}{6}$ |

---

## 4. Shortcuts & Tricks

### 4.1 The deviation method (mental averaging)

Pick a convenient **assumed average**, compute the deviations, average the deviations, and add back.

> **Average of 246, 251, 249, 254, 250**
>
> Assume 250. Deviations: −4, +1, −1, +4, 0. Sum = 0.
> Average deviation = 0/5 = 0.
> **Average = 250 + 0 = 250**

> **Average of 82, 87, 91, 78, 92**
>
> Assume 85. Deviations: −3, +2, +6, −7, +7. Sum = +5.
> Average deviation = 5/5 = 1.
> **Average = 85 + 1 = 86**

This turns four-digit addition into single-digit addition.

### 4.2 The alligation cross — drill it until it's automatic

```
Step 1: Write the two extreme values, left and right.
Step 2: Write the mean value in the middle.
Step 3: Subtract diagonally (always big − small, so both results are positive).
Step 4: The result under EACH extreme is the quantity of THE OTHER one.
```

**Instant results to recognise:**

| Values | Mean | Ratio (cheaper : dearer) |
|---|---|---|
| 60, 80 | 70 | 1 : 1 |
| 15, 20 | 18 | 2 : 3 |
| 15, 20 | 16.50 | 7 : 3 |
| 0 (water), 32 | 28 | 1 : 7 |
| 0 (water), 36 | 30 | 1 : 5 |
| 200, 300 | 260 | 2 : 3 |

### 4.3 Alligation on concentrations, not just prices

Convert both mixtures to a **single common measure** — usually the *fraction of milk* — then alligate.

> Vessel A: milk : water = 5 : 2 ⇒ milk fraction = **5/7**
> Vessel B: milk : water = 3 : 4 ⇒ milk fraction = **3/7**
> Target: 1 : 1 ⇒ milk fraction = **1/2**

```
      3/7                 5/7
         \               /
             \       /
                1/2
             /       \
     (5/7 − 1/2)   (1/2 − 3/7)
      = 3/14         = 1/14

   Quantity of B : Quantity of A = 3 : 1
   → so A : B = 1 : 3
```

**Always write down which quantity you have computed.** Reversing the ratio is the single most common alligation error.

### 4.4 The replacement shortcut

$$\text{New value} = \text{Old value} + (\text{count}) \times (\text{change in average})$$

Memorise the sign convention: if the average **rises**, the newcomer is **heavier/older/higher**; if it falls, lower.

> "Average of 8 rises by 2.5 when a 65 kg person is replaced"
> ⇒ New = 65 + (8 × 2.5) = **85 kg**

> "Average of 10 falls by 1.5 when a 70 kg person is replaced"
> ⇒ New = 70 − (10 × 1.5) = **55 kg**

### 4.5 Overlapping-groups formula

When two overlapping sub-groups cover the whole set with one shared member:

$$\text{Shared value} = (\text{sum of group 1}) + (\text{sum of group 2}) - (\text{total sum})$$

> 11 numbers average 50; first 6 average 49; last 6 average 52. Find the 6th.
> $$6(49) + 6(52) - 11(50) = 294 + 312 - 550 = \mathbf{56}$$

The 6th number is counted in *both* groups, so it appears twice in the sum of groups and once in the total — the difference isolates it.

### 4.6 Repeated-replacement powers

Memorise these so you don't compute cubes under time pressure:

| Fraction retained | Squared | Cubed |
|---|---|---|
| 0.9 (10% removed) | 0.81 | 0.729 |
| 0.8 (20% removed) | 0.64 | 0.512 |
| 0.75 (25% removed) | 0.5625 | 0.4219 |
| 0.5 (50% removed) | 0.25 | 0.125 |

### 4.7 Sanity checks

```
✓ The average always lies BETWEEN the min and max observation
✓ Weighted average lies closer to the LARGER group's average
✓ Average speed (equal distances) is always LESS than the arithmetic mean of speeds
✓ Alligation ratio: the ingredient nearer the mean has the LARGER quantity
✓ After replacement, total volume is UNCHANGED
```

> **The alligation intuition check:** if the mean is close to the dearer value, you need *more* of the dearer ingredient. Mean 18 between 15 and 20 is nearer 20, so the ratio 2 : 3 correctly gives more of the ₹20 rice.

---

## 5. Solved Examples

### Example 1 — Basic average with an exclusion

**Q.** The average of 7 numbers is 45. If one number is removed, the average of the remaining 6 becomes 42. Find the number removed.

**Step 1 — Convert averages into sums.**
$$\text{Original sum} = 7 \times 45 = 315$$
$$\text{New sum} = 6 \times 42 = 252$$

**Step 2 — The difference is the removed number.**
$$315 - 252 = 63$$

**Answer: 63**

**Sanity check:** 63 is above the original average of 45, so removing it should *lower* the average — and it did (45 → 42) ✓

---

### Example 2 — Inclusion raising the average

**Q.** The average age of 24 students in a class is 15 years. When the class teacher's age is included, the average rises to 16 years. Find the teacher's age.

**Step 1 — Sums before and after.**
$$\text{Students' total} = 24 \times 15 = 360$$
$$\text{New total (25 people)} = 25 \times 16 = 400$$

**Step 2 — Teacher's age.**
$$400 - 360 = 40 \text{ years}$$

**Answer: 40 years**

**⚡ Shortcut reasoning:** the teacher must "be" the new average (16) *plus* enough to lift each of the 24 students by 1 year:
$$16 + 24 \times 1 = 40 \checkmark$$

---

### Example 3 — Replacement

**Q.** The average weight of 10 people increases by 1.8 kg when a new person replaces one weighing 53 kg. Find the weight of the new person.

**Step 1 — Compute the total change in weight.**
The average rose by 1.8 kg across 10 people:
$$\text{Total increase} = 10 \times 1.8 = 18 \text{ kg}$$

**Step 2 — Attribute the change to the swap.**
The only change is the substitution, so:
$$\text{New person's weight} = 53 + 18 = 71 \text{ kg}$$

**Answer: 71 kg**

**Formula form:** New = Old + n × ΔAverage = 53 + 10(1.8) = 71 ✓

---

### Example 4 — Weighted average

**Q.** In a company, the average salary of 12 managers is ₹80,000 and the average salary of 48 executives is ₹35,000. Find the average salary of all 60 employees.

**Step 1 — Compute the two group totals.**
$$\text{Managers} = 12 \times 80{,}000 = ₹9{,}60{,}000$$
$$\text{Executives} = 48 \times 35{,}000 = ₹16{,}80{,}000$$

**Step 2 — Grand total.**
$$9{,}60{,}000 + 16{,}80{,}000 = ₹26{,}40{,}000$$

**Step 3 — Divide by the headcount.**
$$\frac{26{,}40{,}000}{60} = ₹44{,}000$$

**Answer: ₹44,000**

**Alligation cross-check:**
```
     35,000              80,000
          \              /
              44,000
          /              \
      36,000            9,000
      
  Executives : Managers = 36,000 : 9,000 = 4 : 1
```
And indeed 48 : 12 = 4 : 1 ✓ — the alligation ratio matches the actual group sizes, confirming ₹44,000.

> Note the answer is much closer to ₹35,000 than to ₹80,000, because executives outnumber managers 4 : 1.

---

### Example 5 — Alligation for price mixing

**Q.** In what ratio must a shopkeeper mix pulses costing ₹24/kg and ₹40/kg so that the mixture is worth ₹30/kg?

**Step 1 — Set up the alligation cross.**

```
        24                    40
          \                  /
              \          /
                  30
              /          \
        (40 − 30)      (30 − 24)
           = 10            = 6
```

**Step 2 — Read the ratio (each quantity takes the opposite difference).**
$$\text{Cheaper} : \text{Dearer} = 10 : 6 = 5 : 3$$

**Verification:** take 5 kg and 3 kg.
$$\text{Cost} = 5(24) + 3(40) = 120 + 120 = ₹240 \text{ for } 8 \text{ kg}$$
$$\frac{240}{8} = ₹30/\text{kg} \checkmark$$

**Answer: 5 : 3**

**Sanity check:** the mean ₹30 is closer to ₹24 than to ₹40, so we need *more* of the cheaper variety — and 5 > 3 ✓

---

### Example 6 — Alligation on concentrations

**Q.** Two vessels contain milk and water in the ratios 5 : 2 and 3 : 5 respectively. In what ratio must the contents be mixed to obtain a mixture that is 50% milk?

**Step 1 — Convert both to milk fractions.**
$$\text{Vessel A: } \frac{5}{5+2} = \frac{5}{7} \qquad \text{Vessel B: } \frac{3}{3+5} = \frac{3}{8}$$
$$\text{Target} = \frac{1}{2}$$

**Step 2 — Alligate.**

```
      3/8                   5/7
         \                 /
             \         /
                 1/2
             /         \
     (5/7 − 1/2)    (1/2 − 3/8)
```

**Step 3 — Compute the two differences.**
$$\frac{5}{7} - \frac{1}{2} = \frac{10 - 7}{14} = \frac{3}{14}$$
$$\frac{1}{2} - \frac{3}{8} = \frac{4 - 3}{8} = \frac{1}{8}$$

**Step 4 — Form the ratio (B : A, since each takes the opposite difference).**
$$B : A = \frac{3}{14} : \frac{1}{8}$$

Multiply both by LCM(14, 8) = 56:
$$B : A = 12 : 7 \implies A : B = 7 : 12$$

**Verification:** take 7 units of A and 12 units of B.
$$\text{Milk} = 7 \times \frac{5}{7} + 12 \times \frac{3}{8} = 5 + 4.5 = 9.5$$
$$\text{Total} = 19 \implies \text{milk fraction} = \frac{9.5}{19} = \frac{1}{2} \checkmark$$

**Answer: A : B = 7 : 12**

> **The most common error here:** writing the answer as 12 : 7. Always label which side of the cross you are reading. The quantity of A takes the difference computed on **B's** side.

---

### Example 7 — Repeated replacement

**Q.** A vessel contains 80 litres of pure milk. 16 litres is drawn out and replaced with water. This process is repeated twice more. Find the quantity of milk left.

**Step 1 — Apply the repeated-replacement formula.**
$$\text{Milk left} = A\left(\frac{A - B}{A}\right)^n$$
with A = 80, B = 16, n = 3.

**Step 2 — Compute the retention fraction.**
$$\frac{80 - 16}{80} = \frac{64}{80} = \frac{4}{5} = 0.8$$

**Step 3 — Raise to the power n.**
$$(0.8)^3 = 0.512$$

**Step 4 — Multiply.**
$$80 \times 0.512 = 40.96 \text{ litres}$$

**Answer: 40.96 litres of milk (and 80 − 40.96 = 39.04 litres of water)**

**Step-by-step verification:**

| Operation | Milk | Water | Total |
|---|---|---|---|
| Start | 80 | 0 | 80 |
| After 1st replacement | 80 × 0.8 = 64 | 16 | 80 |
| After 2nd replacement | 64 × 0.8 = 51.2 | 28.8 | 80 |
| After 3rd replacement | 51.2 × 0.8 = 40.96 | 39.04 | 80 |

> **Why the fraction is 0.8 each time:** removing 16 L of a *uniformly mixed* 80 L removes 20% of whatever is present. The milk therefore retains 80% of its previous amount on every cycle.

---

### Example 8 — Replacing mixture with a pure component

**Q.** A 50-litre mixture contains milk and water in the ratio 3 : 2. How much of the mixture must be drawn off and replaced by pure milk so that the resulting ratio is 4 : 1?

**Step 1 — Find the current quantities.**
Total parts = 5 ⇒ one part = 10 L
$$\text{Milk} = 30 \text{ L}, \qquad \text{Water} = 20 \text{ L}$$

**Step 2 — Identify what stays constant.**
Removing *x* litres of mixture and adding *x* litres of pure milk keeps the **total at 50 L**. Water is only removed, never added — so track the water.

**Step 3 — Water after the operation.**
Drawing off *x* litres removes water in proportion (water is 2/5 of the mixture):
$$\text{Water removed} = \frac{2}{5}x$$
$$\text{Water remaining} = 20 - \frac{2}{5}x$$

**Step 4 — Set the target.**
For a final ratio of 4 : 1 in 50 L, water must be 1/5 of the total:
$$\text{Target water} = \frac{50}{5} = 10 \text{ L}$$

**Step 5 — Solve.**
$$20 - \frac{2}{5}x = 10$$
$$\frac{2}{5}x = 10$$
$$x = 25 \text{ L}$$

**Verification:**
- Draw off 25 L of the mixture ⇒ removes 15 L milk and 10 L water
- Remaining: 15 L milk + 10 L water = 25 L
- Add 25 L pure milk ⇒ 40 L milk + 10 L water = 50 L
- Ratio = 40 : 10 = **4 : 1** ✓

**⚡ Fraction shortcut:** the water fraction must fall from 2/5 to 1/5 — a halving. Since the fraction is multiplied by (1 − x/50):
$$\frac{2}{5}\left(1 - \frac{x}{50}\right) = \frac{1}{5} \implies 1 - \frac{x}{50} = \frac{1}{2} \implies x = 25 \checkmark$$

**Answer: 25 litres**

---

## 6. Practice Questions

**Instructions:** 50 questions. Easy (1–20), Medium (21–40), Hard (41–50).
Target times: Easy 30 s · Medium 60 s · Hard 90 s.
Full solutions in [Section 7](#7-detailed-solutions).

### 🟢 EASY (Questions 1–20)

**Q1.** Find the average of 5, 10, 15, 20 and 25.
(a) 12  (b) 15  (c) 18  (d) 20

**Q2.** Find the average of the first 10 natural numbers.
(a) 5  (b) 5.5  (c) 6  (d) 6.5

**Q3.** The average of 4 numbers is 20. Find their sum.
(a) 60  (b) 70  (c) 80  (d) 90

**Q4.** The average of 3 numbers is 24. If two of them are 20 and 26, find the third.
(a) 22  (b) 24  (c) 26  (d) 28

**Q5.** Find the average of the first 5 even numbers.
(a) 5  (b) 6  (c) 7  (d) 8

**Q6.** The average of 10 numbers is 15. If each number is multiplied by 2, find the new average.
(a) 15  (b) 20  (c) 25  (d) 30

**Q7.** The average weight of 4 people is 60 kg. A fifth person weighing 70 kg joins them. Find the new average.
(a) 61 kg  (b) 62 kg  (c) 63 kg  (d) 65 kg

**Q8.** The average of 6 numbers is 8. If the number 10 is removed, find the average of the remaining numbers.
(a) 7.2  (b) 7.4  (c) 7.6  (d) 7.8

**Q9.** The average of 20, 30, 40 and *x* is 35. Find *x*.
(a) 40  (b) 45  (c) 50  (d) 55

**Q10.** Find the average of the first 20 odd numbers.
(a) 19  (b) 20  (c) 21  (d) 40

**Q11.** A student scores 80, 75, 90, 85 and 70 in five subjects. Find the average.
(a) 78  (b) 79  (c) 80  (d) 82

**Q12.** The average age of 30 students is 12 years. Find the total age.
(a) 300 years  (b) 340 years  (c) 360 years  (d) 380 years

**Q13.** The average of 8 numbers is 25. If 5 is added to each number, find the new average.
(a) 25  (b) 28  (c) 30  (d) 33

**Q14.** In what ratio must tea costing ₹60/kg be mixed with tea costing ₹80/kg to obtain a mixture worth ₹70/kg?
(a) 1 : 1  (b) 1 : 2  (c) 2 : 1  (d) 2 : 3

**Q15.** Find the average of 2, 4, 6, 8, 10 and 12.
(a) 6  (b) 7  (c) 8  (d) 9

**Q16.** Find the average of the first 10 multiples of 3.
(a) 15  (b) 16  (c) 16.5  (d) 17.5

**Q17.** The average temperature over 5 days is 30 °C. Find the total.
(a) 130 °C  (b) 140 °C  (c) 150 °C  (d) 160 °C

**Q18.** The average of 5 numbers is 30. If one number is excluded, the average becomes 28. Find the excluded number.
(a) 32  (b) 35  (c) 38  (d) 40

**Q19.** In what ratio must water be mixed with milk costing ₹32/L to obtain a mixture worth ₹28/L?
(a) 1 : 5  (b) 1 : 6  (c) 1 : 7  (d) 1 : 8

**Q20.** The mean of 3 numbers is 10 and the mean of 2 other numbers is 15. Find the mean of all 5 numbers.
(a) 11  (b) 12  (c) 12.5  (d) 13

---

### 🟡 MEDIUM (Questions 21–40)

**Q21.** The average of 11 numbers is 50. The average of the first 6 is 49 and of the last 6 is 52. Find the 6th number.
(a) 52  (b) 54  (c) 56  (d) 58

**Q22.** The average age of a class of 20 students is 16 years. When the teacher's age is included, the average increases by 1 year. Find the teacher's age.
(a) 35 years  (b) 36 years  (c) 37 years  (d) 38 years

**Q23.** The average weight of 8 people increases by 2.5 kg when a new person replaces one weighing 65 kg. Find the weight of the new person.
(a) 80 kg  (b) 82.5 kg  (c) 85 kg  (d) 87.5 kg

**Q24.** In a 40-litre mixture, milk and water are in the ratio 3 : 1. How much water must be added to make the ratio 3 : 2?
(a) 8 L  (b) 10 L  (c) 12 L  (d) 15 L

**Q25.** In what ratio must rice costing ₹15/kg be mixed with rice costing ₹20/kg so that the mixture is worth ₹18/kg?
(a) 2 : 3  (b) 3 : 2  (c) 1 : 2  (d) 2 : 5

**Q26.** The average of 5 consecutive numbers is 15. Find the largest number.
(a) 16  (b) 17  (c) 18  (d) 19

**Q27.** The average of 30 results is 20 and the average of another 20 results is 30. Find the overall average.
(a) 22  (b) 24  (c) 25  (d) 26

**Q28.** A batsman scores 85 in his 17th innings and thereby increases his batting average by 3. Find his new average.
(a) 34  (b) 35  (c) 37  (d) 38

**Q29.** A container holds 60 litres of milk. 6 litres is removed and replaced by water; this is done twice more. Find the quantity of milk remaining.
(a) 42.00 L  (b) 43.74 L  (c) 44.28 L  (d) 45.60 L

**Q30.** The average of 6 numbers is 30. If the average of the first 4 is 25, find the average of the last 2.
(a) 35  (b) 38  (c) 40  (d) 42

**Q31.** A 20-kg mixture contains milk and water in the ratio 3 : 2. How much milk must be added to make the ratio 4 : 1?
(a) 15 kg  (b) 18 kg  (c) 20 kg  (d) 24 kg

**Q32.** The average marks of 50 students is 62. It is later found that one student's mark of 78 was recorded as 128. Find the correct average.
(a) 60  (b) 61  (c) 61.5  (d) 63

**Q33.** In what ratio must a grocer mix pulses costing ₹15/kg and ₹20/kg to obtain a mixture worth ₹16.50/kg?
(a) 3 : 7  (b) 7 : 3  (c) 2 : 3  (d) 3 : 2

**Q34.** The average salary of all 50 employees in a firm is ₹8,000. The average salary of the 10 officers is ₹15,000. Find the average salary of the remaining 40 employees.
(a) ₹5,750  (b) ₹6,000  (c) ₹6,250  (d) ₹6,500

**Q35.** A vessel contains a mixture of milk and water in the ratio 4 : 1. When 10 litres of the mixture is removed and replaced by water, the ratio becomes 2 : 1. Find the initial quantity of the mixture.
(a) 40 L  (b) 50 L  (c) 60 L  (d) 75 L

**Q36.** The average of 5 numbers is 27. If one number is excluded, the average becomes 25. Find the excluded number.
(a) 30  (b) 32  (c) 35  (d) 37

**Q37.** Two vessels contain milk and water in the ratios 5 : 2 and 3 : 4. In what ratio must they be mixed so that the resulting mixture has milk and water in the ratio 1 : 1?
(a) 1 : 3  (b) 3 : 1  (c) 2 : 3  (d) 3 : 2

**Q38.** The average age of a family of 5 members is 30 years. The youngest member is 6 years old. Find the average age of the family at the time of the youngest member's birth.
(a) 24 years  (b) 26 years  (c) 28 years  (d) 30 years

**Q39.** In what ratio must water be added to milk costing ₹36/L so that, on selling the mixture at ₹36/L, the seller gains 20%?
(a) 1 : 4  (b) 1 : 5  (c) 1 : 6  (d) 2 : 5

**Q40.** The average of 9 observations is 35. The average of the first 5 is 32 and of the last 5 is 39. Find the 5th observation.
(a) 36  (b) 38  (c) 40  (d) 42

---

### 🔴 HARD (Questions 41–50)

**Q41.** A container is full with 40 litres of milk. 8 litres is drawn out and replaced by water; this is repeated twice more. Find the final ratio of milk to water.
(a) 61 : 64  (b) 64 : 61  (c) 32 : 29  (d) 4 : 3

**Q42.** Group A has 20 students with an average weight of 50 kg, Group B has 30 students averaging 60 kg, and Group C has 50 students averaging 40 kg. Find the overall average weight.
(a) 46 kg  (b) 47 kg  (c) 48 kg  (d) 50 kg

**Q43.** A 50-litre mixture contains milk and water in the ratio 3 : 2. How much of the mixture must be replaced by pure milk so that the ratio becomes 4 : 1?
(a) 20 L  (b) 25 L  (c) 30 L  (d) 35 L

**Q44.** The average of 50 numbers is 38. Two numbers, 45 and 55, are discarded. Find the average of the remaining numbers.
(a) 36.5  (b) 37  (c) 37.5  (d) 38.5

**Q45.** A shopkeeper mixes two varieties of tea costing ₹200/kg and ₹300/kg in the ratio 2 : 3 and sells the mixture at ₹312/kg. Find his profit percentage.
(a) 15%  (b) 18%  (c) 20%  (d) 24%

**Q46.** Milk is mixed with water and the mixture is sold at the cost price of pure milk, yielding a 25% profit. Find the ratio of water to milk in the mixture.
(a) 1 : 3  (b) 1 : 4  (c) 1 : 5  (d) 2 : 5

**Q47.** The average age of 8 men increases by 2 years when two women replace two men aged 20 and 24 years. Find the average age of the two women.
(a) 26 years  (b) 28 years  (c) 30 years  (d) 32 years

**Q48.** Three vessels of equal capacity contain milk and water in the ratios 2 : 1, 3 : 2 and 4 : 3. If all three are emptied into a single container, find the ratio of milk to water in the mixture.
(a) 191 : 124  (b) 193 : 122  (c) 197 : 118  (d) 9 : 5

**Q49.** In a 45-litre mixture, the ratio of milk to water is 4 : 1. If 3 litres of water is added, find the percentage of milk in the new mixture.
(a) 70%  (b) 72%  (c) 75%  (d) 78%

**Q50.** A person covers a distance at 40 km/h and returns along the same route at 60 km/h. Find the average speed for the entire journey.
(a) 45 km/h  (b) 48 km/h  (c) 50 km/h  (d) 52 km/h

---

## 7. Detailed Solutions

### 🟢 EASY — Solutions 1–20

---

**Q1. Average of 5, 10, 15, 20, 25. → (b) 15**

**Formula used:** Average = Sum / Count

$$\text{Sum} = 5 + 10 + 15 + 20 + 25 = 75$$
$$\text{Average} = \frac{75}{5} = 15$$

**⚡ Shortcut:** these are consecutive terms of an AP, so the average is the **middle term** = 15 ✓

**Answer: (b) 15**

---

**Q2. Average of the first 10 natural numbers. → (b) 5.5**

**Formula used:** Average of first *n* naturals = (n + 1)/2

$$\frac{10 + 1}{2} = 5.5$$

**Check:** Sum = n(n+1)/2 = 55; 55/10 = 5.5 ✓

**Answer: (b) 5.5**

---

**Q3. Average of 4 numbers is 20. Sum? → (c) 80**

**Formula used:** Sum = Average × Count

$$20 \times 4 = 80$$

**Answer: (c) 80**

---

**Q4. Average of 3 numbers is 24; two are 20 and 26. Third? → (c) 26**

**Step 1 — Total.**
$$3 \times 24 = 72$$

**Step 2 — Subtract the known two.**
$$72 - (20 + 26) = 72 - 46 = 26$$

**Answer: (c) 26**

---

**Q5. Average of the first 5 even numbers. → (b) 6**

The numbers are 2, 4, 6, 8, 10.

**Formula used:** Average of first *n* even numbers = n + 1

$$5 + 1 = 6$$

**Check:** Sum = 30; 30/5 = 6 ✓ (Also the middle term of the AP is 6.)

**Answer: (b) 6**

---

**Q6. Average of 10 numbers is 15; each multiplied by 2. New average? → (d) 30**

**Property used:** multiplying every observation by *k* multiplies the average by *k*.

$$15 \times 2 = 30$$

**Answer: (d) 30**

---

**Q7. 4 people average 60 kg; a fifth weighing 70 kg joins. New average? → (b) 62 kg**

**Step 1 — Original total.**
$$4 \times 60 = 240 \text{ kg}$$

**Step 2 — New total.**
$$240 + 70 = 310 \text{ kg}$$

**Step 3 — New average.**
$$\frac{310}{5} = 62 \text{ kg}$$

**Answer: (b) 62 kg**

---

**Q8. 6 numbers average 8; remove the number 10. New average? → (c) 7.6**

**Step 1 — Original sum.**
$$6 \times 8 = 48$$

**Step 2 — Sum after removal.**
$$48 - 10 = 38 \text{ across } 5 \text{ numbers}$$

**Step 3 — New average.**
$$\frac{38}{5} = 7.6$$

**Sanity check:** 10 is above the average of 8, so removing it should lower the average — and it did ✓

**Answer: (c) 7.6**

---

**Q9. Average of 20, 30, 40 and x is 35. Find x. → (c) 50**

**Step 1 — Required total.**
$$4 \times 35 = 140$$

**Step 2 — Subtract the known values.**
$$x = 140 - (20 + 30 + 40) = 140 - 90 = 50$$

**Answer: (c) 50**

---

**Q10. Average of the first 20 odd numbers. → (b) 20**

**Formula used:** Average of the first *n* odd numbers = *n*

$$= 20$$

**Check:** The numbers run 1, 3, 5, …, 39. Average = (first + last)/2 = (1 + 39)/2 = 20 ✓
(Also: the sum of the first *n* odd numbers is n² = 400, and 400/20 = 20 ✓)

**Answer: (b) 20**

---

**Q11. Marks 80, 75, 90, 85, 70. Average? → (c) 80**

**Deviation method (assume 80):**
$$0, \; -5, \; +10, \; +5, \; -10 \implies \text{sum of deviations} = 0$$
$$\text{Average} = 80 + \frac{0}{5} = 80$$

**Direct check:** Sum = 400; 400/5 = 80 ✓

**Answer: (c) 80**

---

**Q12. 30 students average 12 years. Total? → (c) 360 years**

$$30 \times 12 = 360$$

**Answer: (c) 360 years**

---

**Q13. Average of 8 numbers is 25; add 5 to each. New average? → (c) 30**

**Property used:** adding *k* to every observation adds *k* to the average.

$$25 + 5 = 30$$

**Answer: (c) 30**

---

**Q14. Mix ₹60/kg and ₹80/kg tea for ₹70/kg. Ratio? → (a) 1 : 1**

**Alligation:**
```
        60                    80
          \                  /
                  70
          /                  \
      (80−70)=10         (70−60)=10
```
$$\text{Cheaper} : \text{Dearer} = 10 : 10 = 1 : 1$$

**Intuition:** ₹70 is exactly midway between ₹60 and ₹80, so equal quantities are needed.

**Answer: (a) 1 : 1**

---

**Q15. Average of 2, 4, 6, 8, 10, 12. → (b) 7**

**⚡ Shortcut:** consecutive AP ⇒ average = (first + last)/2 = (2 + 12)/2 = **7**

**Check:** Sum = 42; 42/6 = 7 ✓

**Answer: (b) 7**

---

**Q16. Average of the first 10 multiples of 3. → (c) 16.5**

The numbers are 3, 6, 9, …, 30.

**Formula used:** Average of first *n* multiples of *k* = k(n+1)/2

$$\frac{3 \times 11}{2} = \frac{33}{2} = 16.5$$

**Check:** (first + last)/2 = (3 + 30)/2 = 16.5 ✓

**Answer: (c) 16.5**

---

**Q17. Average temperature 30 °C over 5 days. Total? → (c) 150 °C**

$$5 \times 30 = 150$$

**Answer: (c) 150 °C**

---

**Q18. 5 numbers average 30; excluding one gives 28. Excluded? → (c) 38**

**Step 1 — Sums.**
$$\text{Original} = 5 \times 30 = 150$$
$$\text{Remaining} = 4 \times 28 = 112$$

**Step 2 — Excluded number.**
$$150 - 112 = 38$$

**Answer: (c) 38**

---

**Q19. Water : milk (₹32/L) for a ₹28/L mixture? → (c) 1 : 7**

**Key step:** water costs ₹0.

**Alligation:**
```
     Water (0)              Milk (32)
          \                  /
                  28
          /                  \
      (32−28)=4          (28−0)=28
```
$$\text{Water} : \text{Milk} = 4 : 28 = 1 : 7$$

**Verification:** 1 L water + 7 L milk = 8 L costing 7 × 32 = ₹224.
$$\frac{224}{8} = ₹28/\text{L} \checkmark$$

**Answer: (c) 1 : 7**

---

**Q20. Mean of 3 numbers is 10; mean of 2 others is 15. Mean of all 5? → (b) 12**

**Formula used:** Weighted average

$$\frac{3(10) + 2(15)}{5} = \frac{30 + 30}{5} = \frac{60}{5} = 12$$

> **Trap:** averaging 10 and 15 to get 12.5. The group of 3 carries more weight, pulling the result down to 12.

**Answer: (b) 12**

---

### 🟡 MEDIUM — Solutions 21–40

---

**Q21. 11 numbers average 50; first 6 average 49; last 6 average 52. 6th number? → (c) 56**

**Formula used:** Shared value = (sum of group 1) + (sum of group 2) − (total sum)

**Step 1 — Compute the three sums.**
$$\text{First 6} = 6 \times 49 = 294$$
$$\text{Last 6} = 6 \times 52 = 312$$
$$\text{All 11} = 11 \times 50 = 550$$

**Step 2 — Note the overlap.**
The two groups (positions 1–6 and 6–11) together cover 12 slots for 11 numbers — the **6th number is counted twice**.

**Step 3 — Isolate it.**
$$294 + 312 - 550 = 606 - 550 = 56$$

**Answer: (c) 56**

---

**Q22. 20 students average 16; adding the teacher raises it by 1. Teacher's age? → (c) 37 years**

**Step 1 — Sums before and after.**
$$\text{Students} = 20 \times 16 = 320$$
$$\text{With teacher (21 people, average 17)} = 21 \times 17 = 357$$

**Step 2 — Teacher's age.**
$$357 - 320 = 37 \text{ years}$$

**⚡ Shortcut:** the teacher equals the new average plus the lift given to each student:
$$17 + (20 \times 1) = 37 \checkmark$$

**Answer: (c) 37 years**

---

**Q23. 8 people; average rises 2.5 kg when a 65 kg person is replaced. New weight? → (c) 85 kg**

**Formula used:** New = Old + n × ΔAverage

**Step 1 — Total weight increase.**
$$8 \times 2.5 = 20 \text{ kg}$$

**Step 2 — The only change is the substitution.**
$$\text{New person} = 65 + 20 = 85 \text{ kg}$$

**Answer: (c) 85 kg**

---

**Q24. 40 L mixture, milk : water = 3 : 1. Add water for 3 : 2. → (b) 10 L**

**Step 1 — Current quantities.**
Total parts = 4 ⇒ one part = 10 L
$$\text{Milk} = 30 \text{ L}, \qquad \text{Water} = 10 \text{ L}$$

**Step 2 — Milk is unchanged by adding water.**
Milk stays at **30 L**.

**Step 3 — Water required for a 3 : 2 ratio.**
$$\frac{30}{\text{Water}} = \frac{3}{2} \implies \text{Water} = 20 \text{ L}$$

**Step 4 — Water to add.**
$$20 - 10 = 10 \text{ L}$$

**Verification:** 30 L milk : 20 L water = 3 : 2 ✓ (total 50 L)

**Answer: (b) 10 L**

---

**Q25. Mix ₹15 and ₹20 rice for ₹18/kg. Ratio? → (a) 2 : 3**

**Alligation:**
```
        15                    20
          \                  /
                  18
          /                  \
      (20−18)=2          (18−15)=3
```
$$\text{Cheaper} : \text{Dearer} = 2 : 3$$

**Verification:** 2 kg at ₹15 + 3 kg at ₹20 = ₹30 + ₹60 = ₹90 for 5 kg ⇒ ₹18/kg ✓

**Sanity check:** ₹18 is nearer ₹20, so we need more of the ₹20 variety — and 3 > 2 ✓

**Answer: (a) 2 : 3**

---

**Q26. Average of 5 consecutive numbers is 15. Largest? → (b) 17**

**Key property:** for consecutive numbers, the average is the **middle term**.

**Step 1 — The middle (3rd) number is 15.**
So the sequence is 13, 14, **15**, 16, 17.

**Step 2 — Largest.**
$$= 17$$

**Check:** Sum = 13 + 14 + 15 + 16 + 17 = 75; 75/5 = 15 ✓

**Answer: (b) 17**

---

**Q27. 30 results average 20; 20 results average 30. Overall? → (b) 24**

**Formula used:** Weighted average

$$\frac{30(20) + 20(30)}{30 + 20} = \frac{600 + 600}{50} = \frac{1200}{50} = 24$$

**Alligation cross-check:**
```
        20                    30
          \                  /
                  24
          /                  \
       (30−24)=6          (24−20)=4
       
   Group at 20 : Group at 30 = 6 : 4 = 3 : 2
```
And indeed 30 : 20 = 3 : 2 ✓

> **Trap:** answering 25 (the simple mean). The 30-strong group dominates, so the answer sits below the midpoint.

**Answer: (b) 24**

---

**Q28. Scores 85 in the 17th innings, raising the average by 3. New average? → (c) 37**

**Step 1 — Define the old average.** Let it be *a* (after 16 innings).

**Step 2 — Express the total two ways.**
$$\text{Runs after 17 innings} = 16a + 85$$
$$\text{Also} = 17(a + 3)$$

**Step 3 — Equate and solve.**
$$16a + 85 = 17a + 51$$
$$a = 34$$

**Step 4 — New average.**
$$34 + 3 = 37$$

**Verification:** After 16 innings: 16 × 34 = 544 runs. After the 17th: 544 + 85 = 629 runs.
$$\frac{629}{17} = 37 \checkmark$$

**⚡ Shortcut:** New average = Score − (n − 1) × increase = 85 − 16(3) = 85 − 48 = **37** ✓

**Answer: (c) 37**

---

**Q29. 60 L milk; 6 L replaced by water, three times. Milk left? → (b) 43.74 L**

**Formula used:** Milk left = A(1 − B/A)ⁿ

**Step 1 — Retention fraction per cycle.**
$$\frac{60 - 6}{60} = \frac{54}{60} = 0.9$$

**Step 2 — Three cycles.**
$$(0.9)^3 = 0.729$$

**Step 3 — Multiply.**
$$60 \times 0.729 = 43.74 \text{ L}$$

**Step-by-step verification:**

| After | Milk (L) | Water (L) |
|---|---|---|
| Cycle 1 | 60 × 0.9 = 54.00 | 6.00 |
| Cycle 2 | 54 × 0.9 = 48.60 | 11.40 |
| Cycle 3 | 48.6 × 0.9 = 43.74 | 16.26 |

Total remains 60 L throughout ✓

> **Trap:** answering 60 − 18 = 42 L. After the first cycle the removed 6 L is a *mixture*, not pure milk, so less milk leaves each time.

**Answer: (b) 43.74 L**

---

**Q30. 6 numbers average 30; first 4 average 25. Average of the last 2? → (c) 40**

**Step 1 — Total of all 6.**
$$6 \times 30 = 180$$

**Step 2 — Total of the first 4.**
$$4 \times 25 = 100$$

**Step 3 — Total of the last 2.**
$$180 - 100 = 80$$

**Step 4 — Their average.**
$$\frac{80}{2} = 40$$

**Answer: (c) 40**

---

**Q31. 20 kg, milk : water = 3 : 2. Add milk for 4 : 1. → (c) 20 kg**

**Step 1 — Current quantities.**
Total parts = 5 ⇒ one part = 4 kg
$$\text{Milk} = 12 \text{ kg}, \qquad \text{Water} = 8 \text{ kg}$$

**Step 2 — Adding milk leaves the water unchanged.**
Water stays at **8 kg**.

**Step 3 — Milk needed for a 4 : 1 ratio.**
$$\frac{\text{Milk}}{8} = \frac{4}{1} \implies \text{Milk} = 32 \text{ kg}$$

**Step 4 — Milk to add.**
$$32 - 12 = 20 \text{ kg}$$

**Verification:** 32 kg milk : 8 kg water = 4 : 1 ✓ (total 40 kg)

**Answer: (c) 20 kg**

---

**Q32. 50 students average 62; 78 was recorded as 128. Correct average? → (b) 61**

**Formula used:** ΔAverage = (Correct − Wrong)/n

**Step 1 — Find the error in the total.**
$$78 - 128 = -50$$
The total was **overstated by 50**.

**Step 2 — Convert to an error in the average.**
$$\frac{50}{50} = 1$$

**Step 3 — Correct the average.**
$$62 - 1 = 61$$

**Verification:** Recorded total = 50 × 62 = 3,100. Correct total = 3,100 − 50 = 3,050.
$$\frac{3050}{50} = 61 \checkmark$$

**Answer: (b) 61**

---

**Q33. Mix ₹15 and ₹20 pulses for ₹16.50/kg. Ratio? → (b) 7 : 3**

**Alligation:**
```
        15                    20
          \                  /
                16.50
          /                  \
   (20−16.5)=3.5      (16.5−15)=1.5
```
$$\text{Cheaper} : \text{Dearer} = 3.5 : 1.5 = 35 : 15 = 7 : 3$$

**Verification:** 7 kg at ₹15 + 3 kg at ₹20 = ₹105 + ₹60 = ₹165 for 10 kg ⇒ ₹16.50/kg ✓

**Sanity check:** ₹16.50 is much closer to ₹15, so the cheaper variety dominates — 7 > 3 ✓

**Answer: (b) 7 : 3**

---

**Q34. 50 employees average ₹8,000; 10 officers average ₹15,000. Average of the other 40? → (c) ₹6,250**

**Step 1 — Grand total.**
$$50 \times 8{,}000 = ₹4{,}00{,}000$$

**Step 2 — Officers' total.**
$$10 \times 15{,}000 = ₹1{,}50{,}000$$

**Step 3 — Remaining total.**
$$4{,}00{,}000 - 1{,}50{,}000 = ₹2{,}50{,}000$$

**Step 4 — Average for the 40.**
$$\frac{2{,}50{,}000}{40} = ₹6{,}250$$

**Verification:** (10 × 15,000 + 40 × 6,250)/50 = (1,50,000 + 2,50,000)/50 = ₹8,000 ✓

**Answer: (c) ₹6,250**

---

**Q35. Milk : water = 4 : 1; remove 10 L and replace with water ⇒ 2 : 1. Initial quantity? → (c) 60 L**

**Step 1 — Set up.** Let the total be *T* litres.
$$\text{Milk} = \frac{4T}{5}$$

**Step 2 — Removing 10 L of mixture removes milk in proportion.**
$$\text{Milk removed} = \frac{4}{5} \times 10 = 8 \text{ L}$$
$$\text{Milk remaining} = \frac{4T}{5} - 8$$

**Step 3 — Total stays at T (10 L out, 10 L water in).**
For a final ratio of 2 : 1, milk must be 2/3 of the total:
$$\text{Required milk} = \frac{2T}{3}$$

**Step 4 — Equate and solve.**
$$\frac{4T}{5} - 8 = \frac{2T}{3}$$
$$\frac{4T}{5} - \frac{2T}{3} = 8$$
$$\frac{12T - 10T}{15} = 8$$
$$\frac{2T}{15} = 8 \implies T = 60 \text{ L}$$

**Verification:**
- Start: 60 L with 48 L milk, 12 L water
- Remove 10 L of mixture ⇒ removes 8 L milk, 2 L water ⇒ 40 L milk, 10 L water
- Add 10 L water ⇒ 40 L milk, 20 L water = 60 L
- Ratio = 40 : 20 = **2 : 1** ✓

**Answer: (c) 60 L**

---

**Q36. 5 numbers average 27; excluding one gives 25. Excluded? → (c) 35**

**Step 1 — Sums.**
$$\text{Original} = 5 \times 27 = 135$$
$$\text{Remaining 4} = 4 \times 25 = 100$$

**Step 2 — Excluded number.**
$$135 - 100 = 35$$

**Answer: (c) 35**

---

**Q37. Vessels 5 : 2 and 3 : 4 mixed for 1 : 1. Ratio? → (a) 1 : 3**

**Step 1 — Convert to milk fractions.**
$$\text{Vessel A} = \frac{5}{7}, \qquad \text{Vessel B} = \frac{3}{7}, \qquad \text{Target} = \frac{1}{2}$$

**Step 2 — Alligate.**
```
       3/7                  5/7
          \                /
                1/2
          /                \
   (5/7 − 1/2)        (1/2 − 3/7)
     = 3/14              = 1/14
```

**Step 3 — Read the ratio.** Each quantity takes the *opposite* difference:
$$\text{Quantity of B} : \text{Quantity of A} = \frac{3}{14} : \frac{1}{14} = 3 : 1$$
$$\implies A : B = 1 : 3$$

**Verification:** Take 1 L from A and 3 L from B.
$$\text{Milk} = 1 \times \frac{5}{7} + 3 \times \frac{3}{7} = \frac{5}{7} + \frac{9}{7} = \frac{14}{7} = 2 \text{ L}$$
$$\text{Total} = 4 \text{ L} \implies \text{water} = 2 \text{ L} \implies \text{ratio } 1 : 1 \checkmark$$

> **The classic error:** answering 3 : 1. Label your cross carefully — the quantity of A is determined by the difference on B's side.

**Answer: (a) 1 : 3**

---

**Q38. Family of 5 averages 30; youngest is 6. Average at the youngest's birth? → (d) 30 years**

**Step 1 — Present total age.**
$$5 \times 30 = 150 \text{ years}$$

**Step 2 — Total age of the other 4 members now.**
$$150 - 6 = 144 \text{ years}$$

**Step 3 — Roll back 6 years for those 4 members.**
Six years ago the family had only **4 members**, each 6 years younger:
$$144 - (4 \times 6) = 144 - 24 = 120 \text{ years}$$

**Step 4 — Average at that time.**
$$\frac{120}{4} = 30 \text{ years}$$

**Answer: (d) 30 years**

> **The trap:** subtracting 6 from the present average to get 24. That would be right only if the family size were unchanged — but the youngest did not exist 6 years ago, so the divisor is 4, not 5.

---

**Q39. Water : milk (₹36/L) so that selling at ₹36/L gives 20% profit? → (b) 1 : 5**

**Step 1 — Find the required cost price of the mixture.**
Selling at ₹36 with a 20% profit means:
$$\text{CP of mixture} = \frac{36}{1.20} = ₹30 \text{ per litre}$$

**Step 2 — Alligate water (₹0) against milk (₹36) with mean ₹30.**
```
     Water (0)             Milk (36)
          \                  /
                  30
          /                  \
      (36−30)=6          (30−0)=30
```
$$\text{Water} : \text{Milk} = 6 : 30 = 1 : 5$$

**⚡ Shortcut:** for "sell adulterated goods at cost price of the pure item",
$$\frac{\text{Water}}{\text{Milk}} = \frac{\text{Profit\%}}{100} = \frac{20}{100} = \frac{1}{5} \checkmark$$

**Verification:** 1 L water + 5 L milk = 6 L, costing 5 × 36 = ₹180.
Selling 6 L at ₹36 gives ₹216. Profit = ₹36 on ₹180 = **20%** ✓

**Answer: (b) 1 : 5**

---

**Q40. 9 observations average 35; first 5 average 32; last 5 average 39. 5th observation? → (c) 40**

**Formula used:** Shared value = (group 1 sum) + (group 2 sum) − (total)

**Step 1 — Compute the sums.**
$$\text{First 5} = 5 \times 32 = 160$$
$$\text{Last 5} = 5 \times 39 = 195$$
$$\text{All 9} = 9 \times 35 = 315$$

**Step 2 — The 5th observation lies in both groups.**
Positions 1–5 and 5–9 together cover 10 slots for 9 numbers, so the 5th is double-counted.

**Step 3 — Isolate it.**
$$160 + 195 - 315 = 355 - 315 = 40$$

**Answer: (c) 40**

---

### 🔴 HARD — Solutions 41–50

---

**Q41. 40 L milk; 8 L replaced by water, three times. Final milk : water? → (b) 64 : 61**

**Step 1 — Retention fraction per cycle.**
$$\frac{40 - 8}{40} = \frac{32}{40} = \frac{4}{5} = 0.8$$

**Step 2 — After three cycles.**
$$\text{Milk} = 40 \times (0.8)^3 = 40 \times 0.512 = 20.48 \text{ L}$$

**Step 3 — Water (total is always 40 L).**
$$40 - 20.48 = 19.52 \text{ L}$$

**Step 4 — Form the ratio.**
$$20.48 : 19.52$$

Multiply both by 100 to clear decimals:
$$2048 : 1952$$

Divide by their HCF (32):
$$\frac{2048}{32} : \frac{1952}{32} = 64 : 61$$

**Elegant alternative — work in fifths:**
$$\text{Milk fraction} = \left(\frac{4}{5}\right)^3 = \frac{64}{125}$$
$$\text{Water fraction} = 1 - \frac{64}{125} = \frac{61}{125}$$
$$\text{Ratio} = \mathbf{64 : 61} \checkmark$$

**Step-by-step table:**

| After | Milk (L) | Water (L) |
|---|---|---|
| Cycle 1 | 32.00 | 8.00 |
| Cycle 2 | 25.60 | 14.40 |
| Cycle 3 | 20.48 | 19.52 |

**Answer: (b) 64 : 61**

> **Technique note:** when the removal fraction is a nice fraction (here 1/5 removed, 4/5 retained), work with the fraction rather than the decimal — 64/125 falls out immediately and the ratio needs no simplification.

---

**Q42. Groups: 20 @ 50 kg, 30 @ 60 kg, 50 @ 40 kg. Overall average? → (c) 48 kg**

**Formula used:** Weighted average across three groups

**Step 1 — Compute each group total.**
$$A: 20 \times 50 = 1{,}000 \text{ kg}$$
$$B: 30 \times 60 = 1{,}800 \text{ kg}$$
$$C: 50 \times 40 = 2{,}000 \text{ kg}$$

**Step 2 — Grand total.**
$$1{,}000 + 1{,}800 + 2{,}000 = 4{,}800 \text{ kg}$$

**Step 3 — Total headcount.**
$$20 + 30 + 50 = 100$$

**Step 4 — Overall average.**
$$\frac{4{,}800}{100} = 48 \text{ kg}$$

**Answer: (c) 48 kg**

> **Sanity check:** the answer must lie between 40 and 60. Group C (the largest, at 40 kg) pulls it down; group B (30 people at 60 kg) pulls it up. 48 sits plausibly in between ✓

---

**Q43. 50 L mixture, milk : water = 3 : 2. Replace how much with pure milk for 4 : 1? → (b) 25 L**

**Step 1 — Current quantities.**
One part = 50/5 = 10 L
$$\text{Milk} = 30 \text{ L}, \qquad \text{Water} = 20 \text{ L}$$

**Step 2 — Track the water (it is only removed, never added).**
Drawing off *x* litres of mixture removes water in proportion (water is 2/5 of the mixture):
$$\text{Water removed} = \frac{2}{5}x$$

**Step 3 — Set the target.**
The total stays at 50 L. For a 4 : 1 ratio, water must be 1/5 of 50 = **10 L**.

**Step 4 — Solve.**
$$20 - \frac{2}{5}x = 10$$
$$\frac{2}{5}x = 10$$
$$x = 25 \text{ L}$$

**Verification:**
- Draw off 25 L ⇒ removes 15 L milk and 10 L water
- Left: 15 L milk + 10 L water = 25 L
- Add 25 L pure milk ⇒ 40 L milk + 10 L water = 50 L
- Ratio = **4 : 1** ✓

**⚡ Fraction shortcut:** the water fraction must fall from 2/5 to 1/5 — exactly halved:
$$\frac{2}{5}\left(1 - \frac{x}{50}\right) = \frac{1}{5} \implies 1 - \frac{x}{50} = \frac{1}{2} \implies x = 25 \checkmark$$

**Answer: (b) 25 L**

---

**Q44. 50 numbers average 38; discard 45 and 55. New average? → (c) 37.5**

**Step 1 — Original total.**
$$50 \times 38 = 1{,}900$$

**Step 2 — Remove the two numbers.**
$$1{,}900 - (45 + 55) = 1{,}900 - 100 = 1{,}800$$

**Step 3 — New count.**
$$50 - 2 = 48$$

**Step 4 — New average.**
$$\frac{1{,}800}{48} = 37.5$$

**Sanity check:** both discarded numbers (45 and 55, averaging 50) are above 38, so removing them should *lower* the average — and it did ✓

**Answer: (c) 37.5**

---

**Q45. Mix ₹200 and ₹300 tea in 2 : 3; sell at ₹312/kg. Profit%? → (c) 20%**

**Step 1 — Find the cost price of the mixture per kg (weighted average).**
$$CP = \frac{2(200) + 3(300)}{2 + 3} = \frac{400 + 900}{5} = \frac{1300}{5} = ₹260/\text{kg}$$

**Step 2 — Compute the profit.**
$$\text{Profit} = 312 - 260 = ₹52 \text{ per kg}$$

**Step 3 — Profit percentage (base = CP).**
$$\frac{52}{260} \times 100 = \frac{1}{5} \times 100 = 20\%$$

**Verification with actual quantities:** take 2 kg and 3 kg.
- Cost = 2(200) + 3(300) = ₹1,300 for 5 kg
- Revenue = 5 × 312 = ₹1,560
- Profit = ₹260 on ₹1,300 = **20%** ✓

**Answer: (c) 20%**

---

**Q46. Mixture sold at milk's cost price yields 25% profit. Water : milk? → (b) 1 : 4**

**Step 1 — Set up with variables.**
Let the mixture contain *m* litres of milk and *w* litres of water.
Let the cost of pure milk be ₹*p* per litre.

**Step 2 — Compute cost and revenue.**
$$\text{Cost to the seller} = m \times p \quad \text{(water is free)}$$
$$\text{Revenue} = (m + w) \times p \quad \text{(selling the whole mixture at milk's price)}$$

**Step 3 — Compute the profit.**
$$\text{Profit} = (m+w)p - mp = wp$$

**Step 4 — Express as a percentage of cost.**
$$\text{Profit\%} = \frac{wp}{mp} \times 100 = \frac{w}{m} \times 100$$

**Step 5 — Apply the given 25%.**
$$\frac{w}{m} \times 100 = 25 \implies \frac{w}{m} = \frac{1}{4}$$

**Answer: (b) 1 : 4**

**Numeric verification:** 1 L water + 4 L milk at ₹100/L milk.
- Cost = ₹400 · Revenue = 5 × ₹100 = ₹500 · Profit = ₹100 on ₹400 = **25%** ✓

> **The general result worth memorising:**
> $$\frac{\text{Water}}{\text{Milk}} = \frac{\text{Profit\%}}{100}$$
> 20% ⇒ 1 : 5 · 25% ⇒ 1 : 4 · 50% ⇒ 1 : 2 · 100% ⇒ 1 : 1

---

**Q47. 8 men; average rises 2 years when two women replace men aged 20 and 24. Women's average age? → (c) 30 years**

**Step 1 — Compute the total increase in age.**
The group size stays at 8, and the average rose by 2 years:
$$\text{Total increase} = 8 \times 2 = 16 \text{ years}$$

**Step 2 — Attribute the increase to the swap.**
The two men removed had a combined age of 20 + 24 = **44 years**. The two women must therefore total:
$$44 + 16 = 60 \text{ years}$$

**Step 3 — Their average.**
$$\frac{60}{2} = 30 \text{ years}$$

**Answer: (c) 30 years**

> **Structure of every replacement problem:**
> $$\text{Sum of new members} = \text{Sum of removed members} + n \times \Delta\text{Average}$$
> This holds whether one member or several are replaced, as long as the group size is unchanged.

---

**Q48. Three equal vessels with milk : water = 2:1, 3:2, 4:3. Combined ratio? → (b) 193 : 122**

**Step 1 — Choose a common capacity.**
The ratio parts sum to 3, 5 and 7. Take each vessel's capacity as **LCM(3, 5, 7) = 105 litres** so every quantity is a whole number.

**Step 2 — Break down each vessel.**

| Vessel | Ratio | Milk | Water |
|---|---|---|---|
| I | 2 : 1 | 105 × 2/3 = **70** | 105 × 1/3 = **35** |
| II | 3 : 2 | 105 × 3/5 = **63** | 105 × 2/5 = **42** |
| III | 4 : 3 | 105 × 4/7 = **60** | 105 × 3/7 = **45** |
| **Total** | | **193** | **122** |

**Step 3 — Form the ratio.**
$$\text{Milk} : \text{Water} = 193 : 122$$

**Check:** 193 + 122 = 315 = 3 × 105 ✓ (all the liquid is accounted for)

**Fraction method (equivalent):**
$$\text{Milk fraction} = \frac{1}{3}\left(\frac{2}{3} + \frac{3}{5} + \frac{4}{7}\right) = \frac{1}{3} \times \frac{70 + 63 + 60}{105} = \frac{193}{315}$$
$$\text{Water fraction} = \frac{122}{315} \implies 193 : 122 \checkmark$$

**Answer: (b) 193 : 122**

> **Technique:** for "equal vessels with different ratios", always set the capacity to the LCM of the ratio-sums. It eliminates fractions entirely.

---

**Q49. 45 L, milk : water = 4 : 1; add 3 L water. Percentage of milk? → (c) 75%**

**Step 1 — Current quantities.**
Total parts = 5 ⇒ one part = 9 L
$$\text{Milk} = 36 \text{ L}, \qquad \text{Water} = 9 \text{ L}$$

**Step 2 — After adding 3 L of water.**
$$\text{Milk} = 36 \text{ L (unchanged)}$$
$$\text{Water} = 9 + 3 = 12 \text{ L}$$
$$\text{New total} = 45 + 3 = 48 \text{ L}$$

**Step 3 — Percentage of milk.**
$$\frac{36}{48} \times 100 = \frac{3}{4} \times 100 = 75\%$$

> **Trap:** dividing 36 by the old total of 45 gives 80% — the milk percentage *before* the addition. The denominator must be the new total.

**Answer: (c) 75%**

---

**Q50. 40 km/h out, 60 km/h back. Average speed? → (b) 48 km/h**

**Formula used:** For equal distances, average speed is the **harmonic mean**:
$$\text{Average speed} = \frac{2uv}{u+v}$$

**Step 1 — Substitute.**
$$\frac{2 \times 40 \times 60}{40 + 60} = \frac{4800}{100} = 48 \text{ km/h}$$

**First-principles verification.** Let the one-way distance be 120 km (LCM of 40 and 60).
$$\text{Time out} = \frac{120}{40} = 3 \text{ h}$$
$$\text{Time back} = \frac{120}{60} = 2 \text{ h}$$
$$\text{Total distance} = 240 \text{ km}, \qquad \text{Total time} = 5 \text{ h}$$
$$\text{Average speed} = \frac{240}{5} = 48 \text{ km/h} \checkmark$$

> **Why not 50?** The traveller spends **3 hours** at 40 km/h but only **2 hours** at 60 km/h. More time is spent at the slower speed, so the average is pulled below the arithmetic mean. For equal distances, the average speed is *always* less than (u + v)/2.

**Answer: (b) 48 km/h**

---

## 8. Quick Revision Sheet

> **One page. Read 48 hours after study, and again the night before the test.**

### Averages

```
Average = Sum / Count          →    Sum = Average × Count   ← use this form

Add k to each      →  average + k
Multiply each by k →  average × k
Average always lies between MIN and MAX
```

### Standard sequence averages

```
First n naturals       →  (n+1)/2
First n even numbers   →  n + 1
First n odd numbers    →  n
First n multiples of k →  k(n+1)/2
Consecutive numbers    →  (first + last)/2 = middle term
```

### The four manoeuvres

```
INCLUSION   →  New value  = New sum − Old sum
                          = New average + n × Δaverage
EXCLUSION   →  Removed    = Old sum − New sum
REPLACEMENT →  New value  = Old value + n × Δaverage
CORRECTION  →  Δaverage   = (Correct − Wrong) / n

OVERLAP     →  Shared value = Sum(group1) + Sum(group2) − Total sum
```

### Weighted average

```
(n₁A₁ + n₂A₂) / (n₁ + n₂)      ← never average the averages unweighted
Result always sits CLOSER to the larger group's average
```

### Average speed

```
Equal DISTANCES, speeds u,v    →  2uv/(u+v)        ← harmonic mean
Equal DISTANCES, three speeds  →  3uvw/(uv+vw+wu)
Equal TIMES                    →  (u+v)/2          ← arithmetic mean
General                        →  Total distance / Total time

40 & 60  → 48       30 & 60 → 40       20 & 30 → 24
50 & 30  → 37.5     60 & 40 → 48       80 & 20 → 32
```

### ALLIGATION (the big one)

```
        c (cheaper)            d (dearer)
              \                  /
                    m (mean)
              /                  \
           (d − m)             (m − c)
              │                    │
        Qty of CHEAPER   :   Qty of DEARER

Each quantity takes the difference on the OPPOSITE side.
Works for: price · concentration · % · marks · age · rate — anything linear.
Water = ₹0.
```

**Sanity check:** the ingredient whose value is *closer* to the mean gets the *larger* quantity.

### Mixtures

```
Add ONE component only  →  the OTHER component stays fixed. Anchor on it.

Replace x of a mixture with a pure component:
    new fraction of the removed-component = old fraction × (1 − x/Total)
    (Total is UNCHANGED)

Repeated replacement, n times, B out of A each time:
    Liquid left = A × ((A−B)/A)ⁿ
    0.9³ = 0.729    0.8³ = 0.512    0.75³ = 0.4219    0.5³ = 0.125

Dilution sold at pure price:
    Water/Milk = Profit% / 100
    20% → 1:5    25% → 1:4    50% → 1:2    100% → 1:1

Equal vessels with ratios p:q, r:s, t:u
    → set capacity = LCM of (p+q), (r+s), (t+u)
```

---

## 9. Common Mistakes

| # | Mistake | Example | Correction |
|---|---|---|---|
| 1 | **Averaging averages unweighted** | 30 @ 20 and 20 @ 30 ⇒ 25 | Weight it: (600+600)/50 = 24 |
| 2 | **Arithmetic mean for average speed** | 40 and 60 ⇒ 50 km/h | Harmonic mean: 2(40)(60)/100 = 48 |
| 3 | **Repeated replacement treated linearly** | 3 × 6 L from 60 ⇒ 42 L left | 60 × 0.9³ = 43.74 L |
| 4 | **Alligation ratio reversed** | Reading A's quantity off A's own side | Each quantity takes the **opposite** difference |
| 5 | **Removing pure liquid instead of mixture** | 20 L drawn removes 20 L milk | It removes milk *in proportion* to its fraction |
| 6 | **Old total used after an addition** | 36/45 after adding 3 L water | Use the new total: 36/48 = 75% |
| 7 | **Family-size unchanged over time** | Average 30 six years ago ⇒ 24 | The youngest didn't exist — divide by 4, not 5 |
| 8 | **Overlap double-count ignored** | 6th number = 294 + 312 | Subtract the total: 294 + 312 − 550 = 56 |
| 9 | **Mixing quantities and values** | Splitting cost in the *quantity* ratio | Weight quantities by their unit values first |
| 10 | **Water given a nonzero price** | Alligating water at the milk price | Water = ₹0 |
| 11 | **Wrong base in profit-on-mixture** | Profit ÷ selling price | Profit ÷ **cost of the mixture** |
| 12 | **Replacement sign error** | Average falls ⇒ new member is heavier | Falls ⇒ new member is **lighter**: New = Old − nΔ |

---

## Practice Answer Key

| Q | Ans | Q | Ans | Q | Ans | Q | Ans | Q | Ans |
|---|---|---|---|---|---|---|---|---|---|
| 1 | b | 11 | c | 21 | c | 31 | c | 41 | b |
| 2 | b | 12 | c | 22 | c | 32 | b | 42 | c |
| 3 | c | 13 | c | 23 | c | 33 | b | 43 | b |
| 4 | c | 14 | a | 24 | b | 34 | c | 44 | c |
| 5 | b | 15 | b | 25 | a | 35 | c | 45 | c |
| 6 | d | 16 | c | 26 | b | 36 | c | 46 | b |
| 7 | b | 17 | c | 27 | b | 37 | a | 47 | c |
| 8 | c | 18 | c | 28 | c | 38 | d | 48 | b |
| 9 | c | 19 | c | 29 | b | 39 | b | 49 | c |
| 10 | b | 20 | b | 30 | c | 40 | c | 50 | b |

**Scoring guide:** 45+/50 → strong. 35–44 → solid; drill the alligation cross until the ratio direction is automatic. Below 35 → re-read Sections 2.7–2.11 and redo the Medium set.

---

**⬅️ Back:** [Topic 3 — Ratio, Proportion & Partnership](03-ratio-proportion-partnership.md) · **➡️ Next:** [Topic 5 — Time & Work, Pipes & Cisterns](05-time-and-work.md)
