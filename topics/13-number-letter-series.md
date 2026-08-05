# Topic 13 — Number & Letter Series

### EY Placement Aptitude Handbook · Priority Rank #6 · 🔴 Critical

> **Questions in this file are original, modelled on publicly reported EY test patterns. They are not claimed to be actual previous-year EY questions.**

---

## Contents

1. [Why This Topic Matters for EY](#1-why-this-topic-matters-for-ey)
2. [Core Concepts](#2-core-concepts)
3. [Pattern Bank](#3-pattern-bank)
4. [Shortcuts & Tricks](#4-shortcuts--tricks)
5. [Solved Examples](#5-solved-examples)
6. [Practice Questions (50)](#6-practice-questions)
7. [Detailed Solutions](#7-detailed-solutions)
8. [Quick Revision Sheet](#8-quick-revision-sheet)
9. [Common Mistakes](#9-common-mistakes)

---

## 1. Why This Topic Matters for EY

**Weightage:** 15–18% of the reasoning section — the **highest-frequency reasoning topic**. Expect 2–3 questions.

**Why it is worth serious drilling:** series questions have no formulas to derive and no diagrams to draw. They are **pure pattern recognition**, which means they respond almost entirely to *exposure*. A candidate who has seen 200 series solves the next one in 10 seconds; a candidate who has seen 20 stares at it for two minutes. In a section where you have 40 seconds per question, that difference decides the section.

**Question styles reported:**

| Style | Example shape |
|---|---|
| **Find the next term** | "2, 6, 12, 20, 30, ?" |
| **Find the missing term** | "3, 8, ?, 24, 35" |
| **Find the wrong term** | "2, 5, 10, 17, 27, 37" — which does not belong? |
| **Letter series** | "A, C, E, G, ?" |
| **Alpha-numeric series** | "A1, C3, E5, ?" |
| **Letter-group series** | "ACE, BDF, CEG, ?" |
| **Two interleaved series** | "8, 24, 12, 36, 18, ?" |

---

## 2. Core Concepts

### 2.1 The universal method

```
STEP 1:  Compute the FIRST DIFFERENCES between consecutive terms
STEP 2:  If they are constant       → arithmetic progression, done
         If they grow steadily      → take SECOND differences
         If they grow fast          → check for a MULTIPLICATIVE pattern
STEP 3:  Check the term against n², n³, n!, 2ⁿ or primes
STEP 4:  If nothing works, split into ALTERNATE terms (two interleaved series)
STEP 5:  Verify your rule on EVERY given term before answering
```

**Step 5 is non-negotiable.** A rule that explains four of five terms is the wrong rule. Series questions frequently offer options that fit a partial pattern.

### 2.2 The difference table

Write the differences underneath the series. This single habit solves most questions instantly.

```
Series:        2     6     12     20     30     ?
1st diff:         4     6      8     10     [12]
2nd diff:            2     2      2      [2]     ← CONSTANT ⇒ quadratic
                                                    Next term = 30 + 12 = 42
```

| What the differences show | What it means |
|---|---|
| Constant 1st difference | Arithmetic progression: aₙ = a + (n−1)d |
| Constant 2nd difference | Quadratic pattern (often n² based) |
| Constant ratio | Geometric progression: aₙ = arⁿ⁻¹ |
| Differences are themselves a known series | Layered pattern (e.g. differences are squares) |

### 2.3 The number families you must recognise on sight

| Family | First terms |
|---|---|
| **Squares** | 1, 4, 9, 16, 25, 36, 49, 64, 81, 100, 121, 144, 169, 196, 225 |
| **Cubes** | 1, 8, 27, 64, 125, 216, 343, 512, 729, 1000 |
| **Primes** | 2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47 |
| **Fibonacci** | 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89 |
| **Factorials** | 1, 2, 6, 24, 120, 720, 5040 |
| **Powers of 2** | 2, 4, 8, 16, 32, 64, 128, 256, 512, 1024 |
| **Powers of 3** | 3, 9, 27, 81, 243, 729 |
| **Triangular numbers** | 1, 3, 6, 10, 15, 21, 28, 36, 45 |
| **2ⁿ − 1** | 1, 3, 7, 15, 31, 63, 127 |
| **n² − 1** | 0, 3, 8, 15, 24, 35, 48, 63, 80, 99 |
| **n² + 1** | 2, 5, 10, 17, 26, 37, 50, 65 |
| **n³ − 1** | 0, 7, 26, 63, 124, 215 |
| **n³ + n²** | 2, 12, 36, 80, 150 |

> **Near-miss recognition is the real skill.** If a series reads 3, 8, 15, 24, 35, you should immediately think "those are 4, 9, 16, 25, 36 minus one" — i.e. **n² − 1**. Train yourself to compare against the squares and cubes automatically.

### 2.4 The alphabet positions (memorise cold)

| A | B | C | D | E | F | G | H | I | J | K | L | M |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12 | 13 |

| N | O | P | Q | R | S | T | U | V | W | X | Y | Z |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 14 | 15 | 16 | 17 | 18 | 19 | 20 | 21 | 22 | 23 | 24 | 25 | 26 |

**The anchors worth memorising:** A=1, **E=5**, **J=10**, **O=15**, **T=20**, **Y=25**, Z=26.
*(Mnemonic: **EJOTY** — every fifth letter.)*

**The reverse (opposite) pairs — used constantly:**

$$\text{Opposite of a letter at position } n = 27 - n$$

| A↔Z | B↔Y | C↔X | D↔W | E↔V | F↔U | G↔T |
|---|---|---|---|---|---|---|
| H↔S | I↔R | J↔Q | K↔P | L↔O | M↔N | |

> **AZ, BY, CX, ?** — each pair is a letter and its opposite ⇒ next is **DW**.

### 2.5 Types of letter series

| Type | Example | Rule |
|---|---|---|
| **Constant skip** | A, C, E, G, ? | +2 each time ⇒ **I** |
| **Increasing skip** | A, B, D, G, ? | +1, +2, +3, +4 ⇒ **K** |
| **Reverse order** | Z, Y, X, W, ? | −1 ⇒ **V** |
| **Reverse skip** | Z, W, T, Q, ? | −3 ⇒ **N** |
| **Opposite pairs** | AZ, BY, CX, ? | letter + its mirror ⇒ **DW** |
| **Letter groups** | ACE, BDF, CEG, ? | each letter +1 ⇒ **DFH** |
| **Alpha-numeric** | A1, C3, E5, ? | letter +2, number +2 ⇒ **G7** |

**Method for letter series: convert to numbers, find the pattern, convert back.**

> A, B, D, G, ? → 1, 2, 4, 7, ?
> Differences: 1, 2, 3, [4] ⇒ next = 7 + 4 = 11 ⇒ **K**

### 2.6 Interleaved (alternating) series

When nothing works on the whole series, split it into odd-position and even-position terms.

> **8, 24, 12, 36, 18, ?**
>
> Odd positions: 8, 12, 18 → differences 4, 6 (growing)
> Even positions: 24, 36 → ×1.5
>
> Better reading — an alternating **operation**:
> ```
> 8  ×3→ 24  ÷2→ 12  ×3→ 36  ÷2→ 18  ×3→ [54]
> ```
> Answer: **54**

**Signals that a series is interleaved:**
- Terms alternate between rising and falling
- Differences alternate in sign
- The series has an obviously "jumpy" feel

### 2.7 The "wrong term" question

> *"Find the term that does not belong: 2, 5, 10, 17, 27, 37, 50"*

```
1.  Establish the rule from the terms that agree with each other
2.  Predict every term from that rule
3.  The mismatch is the answer
```

Here the pattern is **n² + 1**: 2, 5, 10, 17, 26, 37, 50.
The sixth term should be **26**, not 27 ⇒ **27 is the wrong term**.

---

## 3. Pattern Bank

| # | Pattern | Example |
|---|---|---|
| 1 | Add a constant | 2, 5, 8, 11 (+3) |
| 2 | Subtract a constant | 100, 90, 80, 70 (−10) |
| 3 | Multiply by a constant | 3, 6, 12, 24 (×2) |
| 4 | Divide by a constant | 240, 120, 60, 30 (÷2) |
| 5 | Increasing addition | 2, 4, 7, 11, 16 (+2, +3, +4, +5) |
| 6 | Squares | 1, 4, 9, 16, 25 |
| 7 | Cubes | 1, 8, 27, 64, 125 |
| 8 | n² ± 1 | 0, 3, 8, 15, 24 · 2, 5, 10, 17, 26 |
| 9 | n³ ± 1 | 0, 7, 26, 63, 124 · 2, 9, 28, 65 |
| 10 | ×2 + 1 | 3, 7, 15, 31, 63 |
| 11 | ×2 − 1 | 3, 5, 9, 17, 33 |
| 12 | ×3 + 1 | 2, 7, 22, 67 |
| 13 | Fibonacci-type (sum of the previous two) | 1, 1, 2, 3, 5, 8 |
| 14 | Factorials | 1, 2, 6, 24, 120 |
| 15 | Primes | 2, 3, 5, 7, 11, 13 |
| 16 | Triangular numbers | 1, 3, 6, 10, 15 |
| 17 | 2ⁿ − 1 | 1, 3, 7, 15, 31 |
| 18 | Alternating ×a, ÷b | 8, 24, 12, 36, 18 |
| 19 | Alternating +a, −b | 10, 15, 13, 18, 16 |
| 20 | Two interleaved series | 2, 100, 4, 90, 6, 80 |
| 21 | Cumulative sums | 1, 3, 6, 10 (partial sums of 1,2,3,4) |
| 22 | Sum of squares (cumulative) | 1, 5, 14, 30, 55 |
| 23 | nⁿ | 1, 4, 27, 256, 3125 |
| 24 | Multiply by increasing factors | 2, 4, 12, 48, 240 (×2, ×3, ×4, ×5) |
| 25 | Divide by increasing factors | 240, 120, 40, 10, 2 (÷2, ÷3, ÷4, ÷5) |

---

## 4. Shortcuts & Tricks

### 4.1 The 10-second triage

```
Look at the GROWTH RATE first:

    Slow, steady growth      →  addition pattern (take differences)
    Rapid growth             →  multiplication, powers or factorials
    Rises and falls          →  alternating or interleaved
    Terms near perfect squares/cubes → n² or n³ variant
```

This triage narrows the search before you compute anything.

### 4.2 Always write the differences

```
Series:       5     11     23     47     ?

1st diff:        6     12     24    [48]     ← doubling!
                                              Next = 47 + 48 = 95

Cross-check with a multiplicative rule:
    5×2+1 = 11 ✓   11×2+1 = 23 ✓   23×2+1 = 47 ✓   47×2+1 = 95 ✓
```

Two independent routes to the same answer is the strongest possible confirmation.

### 4.3 Compare against squares and cubes reflexively

| Series | Compare with | Rule |
|---|---|---|
| 3, 8, 15, 24, 35 | 4, 9, 16, 25, 36 | n² − 1 |
| 2, 5, 10, 17, 26 | 1, 4, 9, 16, 25 | n² + 1 |
| 0, 7, 26, 63 | 1, 8, 27, 64 | n³ − 1 |
| 2, 9, 28, 65 | 1, 8, 27, 64 | n³ + 1 |
| 2, 8, 18, 32, 50 | 1, 4, 9, 16, 25 | 2n² |
| 3, 12, 27, 48 | 1, 4, 9, 16 | 3n² |

### 4.4 EJOTY — instant letter positions

```
E = 5     J = 10     O = 15     T = 20     Y = 25

Count forwards or backwards from the nearest anchor:
    R  →  just before T(20)?  No — R is 18 (two before T)
    M  →  three after J(10)   →  13
    W  →  two after T(20)... T=20, U=21, V=22, W=23
```

**And for the opposite letter: 27 − position.**
> R is 18 ⇒ opposite is 27 − 18 = 9 ⇒ **I**

### 4.5 Letter series → number series

Always convert. Patterns that are invisible in letters become obvious in numbers.

> **B, E, H, K, ?**
> → 2, 5, 8, 11, [14] (differences of 3)
> → 14 = **N**

> **A, C, F, J, ?**
> → 1, 3, 6, 10, [15] (differences 2, 3, 4, **5**)
> → 15 = **O**

### 4.6 The alternate-split test

If a single rule refuses to fit, immediately split:

```
Series:     2, 100, 4, 90, 6, 80, ?

Odd positions:  2, 4, 6, [8]      ← +2
Even positions: 100, 90, 80       ← −10

The '?' is in position 7 (odd) ⇒ answer = 8
```

**Always check which position the '?' occupies** before reading off the answer.

### 4.7 Verify before you commit

```
□  Does my rule explain the FIRST term?
□  Does it explain EVERY intermediate term?
□  Is my answer among the options?
□  Is there a SECOND rule that also fits? (if so, prefer the simpler one)
```

> **Series questions are the most common source of "plausible but wrong" answers.** The 15 seconds spent verifying against all given terms is the best-spent time in the reasoning section.

---

## 5. Solved Examples

### Example 1 — Second differences

**Q.** Find the next term: 3, 7, 13, 21, 31, ?

**Step 1 — First differences.**
```
Series:      3     7     13     21     31     ?
1st diff:       4     6      8     10     [?]
```

**Step 2 — Second differences.**
```
2nd diff:          2     2      2     [2]
```
The second differences are constant at 2, so the first differences continue in an arithmetic sequence.

**Step 3 — Extend.**
Next first difference = 10 + 2 = **12**
$$\text{Next term} = 31 + 12 = 43$$

**Alternative reading — compare against n² :**
$$n^2 + n + 1: \quad 1+1+1 = 3, \; 4+2+1 = 7, \; 9+3+1 = 13, \; 16+4+1 = 21, \; 25+5+1 = 31$$
For n = 6: 36 + 6 + 1 = **43** ✓

**Answer: 43**

---

### Example 2 — Multiplicative with an offset

**Q.** Find the next term: 4, 9, 19, 39, ?

**Step 1 — Check the differences.**
```
1st diff:  5, 10, 20   ← these are doubling
```
Doubling differences signal a "×2 + constant" rule.

**Step 2 — Test ×2 + 1.**
$$4 \times 2 + 1 = 9 \checkmark$$
$$9 \times 2 + 1 = 19 \checkmark$$
$$19 \times 2 + 1 = 39 \checkmark$$

**Step 3 — Apply.**
$$39 \times 2 + 1 = 79$$

**Answer: 79**

> **The signature of "×2 + c":** the *differences* double. Whenever you see 5, 10, 20, 40 as differences, test a multiplicative rule immediately.

---

### Example 3 — Recognising n² − 1

**Q.** Find the missing term: 3, 8, ?, 24, 35, 48

**Step 1 — Compare against the squares.**
```
Given:    3    8    ?    24    35    48
Squares:  4    9   16    25    36    49
```
Every given term is exactly **one less** than a perfect square.

**Step 2 — Identify the rule.**
$$a_n = (n+1)^2 - 1$$

**Step 3 — Fill the gap.**
The missing term corresponds to 16 − 1 = **15**.

**Verification of the full series:** 3, 8, 15, 24, 35, 48 — differences 5, 7, 9, 11, 13 (consecutive odd numbers, exactly what n² − 1 produces) ✓

**Answer: 15**

---

### Example 4 — Interleaved series

**Q.** Find the next term: 5, 12, 10, 24, 20, 48, ?

**Step 1 — Try a single rule.** The terms rise and fall irregularly — no single rule fits.

**Step 2 — Split by position.**

```
Position:   1    2    3    4    5    6    7
Term:       5   12   10   24   20   48    ?

ODD  positions (1,3,5,7):   5, 10, 20, [?]   ← ×2
EVEN positions (2,4,6):    12, 24, 48        ← ×2
```

**Step 3 — Identify the '?' position.**
The '?' is the **7th** term — an odd position, continuing 5, 10, 20.

**Step 4 — Extend.**
$$20 \times 2 = 40$$

**Answer: 40**

> **Always check the position index.** Answering 96 (continuing the even sub-series) is the classic error here.

---

### Example 5 — Letter series with an increasing skip

**Q.** Find the next term: A, C, F, J, O, ?

**Step 1 — Convert to positions.**
$$A=1, \; C=3, \; F=6, \; J=10, \; O=15$$

**Step 2 — Take the differences.**
$$2, \; 3, \; 4, \; 5 \implies \text{next difference} = 6$$

**Step 3 — Extend and convert back.**
$$15 + 6 = 21 \implies \textbf{U}$$

**Recognition bonus:** 1, 3, 6, 10, 15, 21 are the **triangular numbers**.

**Answer: U**

---

### Example 6 — Letter groups

**Q.** Find the next term: BDF, CEG, DFH, ?

**Step 1 — Convert each group to positions.**
$$\text{BDF} = (2, 4, 6)$$
$$\text{CEG} = (3, 5, 7)$$
$$\text{DFH} = (4, 6, 8)$$

**Step 2 — Identify the pattern.**
Each letter advances by **+1** from the corresponding letter in the previous group. (Within each group, the letters go up by 2.)

**Step 3 — Extend.**
$$(5, 7, 9) = \textbf{EGI}$$

**Answer: EGI**

> **Group-series method:** compare *position by position* across groups (first letter with first letter, second with second), not within a single group. Both patterns usually exist, but the across-groups one determines the next term.

---

### Example 7 — Finding the wrong term

**Q.** One term in this series is incorrect. Identify it: 6, 12, 21, 33, 46, 63

**Step 1 — Take the differences.**
```
Series:     6    12    21    33    46    63
1st diff:      6     9    12    13    17
```

**Step 2 — Look for the intended pattern.**
The first three differences are 6, 9, 12 — increasing by 3. If the pattern continued, the differences would be **6, 9, 12, 15, 18**.

**Step 3 — Build the correct series.**
$$6, \; 12, \; 21, \; 33, \; \mathbf{48}, \; 66$$

**Step 4 — Compare with the given series.**
```
Correct:   6, 12, 21, 33, 48, 66
Given:     6, 12, 21, 33, 46, 63
                              ↑
                        first mismatch
```

The **46** breaks the pattern; it should be 48.

**Answer: 46 is the wrong term (it should be 48)**

> **Method discipline:** establish the rule from the terms that *agree* (here the first four), then predict forwards. Do not try to force a rule that accommodates every term — one of them is deliberately broken.

---

### Example 8 — Alternating operations

**Q.** Find the next term: 10, 30, 15, 45, 22.5, ?

**Step 1 — Examine consecutive ratios.**
$$\frac{30}{10} = 3 \qquad \frac{15}{30} = \frac{1}{2} \qquad \frac{45}{15} = 3 \qquad \frac{22.5}{45} = \frac{1}{2}$$

**Step 2 — Identify the alternating rule.**
$$\times 3, \; \div 2, \; \times 3, \; \div 2, \; \times 3, \ldots$$

**Step 3 — Apply the next operation.**
The last operation was ÷2, so the next is ×3:
$$22.5 \times 3 = 67.5$$

**Answer: 67.5**

**Full verification:**
```
10  ×3→  30  ÷2→  15  ×3→  45  ÷2→  22.5  ×3→  67.5  ✓
```

---

## 6. Practice Questions

**Instructions:** 50 questions. Easy (1–20), Medium (21–40), Hard (41–50).
Target: **30 seconds per question**. Full solutions in [Section 7](#7-detailed-solutions).

### 🟢 EASY (Questions 1–20)

**Q1.** 2, 4, 6, 8, ?
(a) 9  (b) 10  (c) 12  (d) 16

**Q2.** 3, 6, 12, 24, ?
(a) 36  (b) 42  (c) 48  (d) 54

**Q3.** 1, 4, 9, 16, ?
(a) 20  (b) 23  (c) 25  (d) 36

**Q4.** 5, 10, 15, 20, ?
(a) 22  (b) 24  (c) 25  (d) 30

**Q5.** 1, 8, 27, 64, ?
(a) 100  (b) 116  (c) 125  (d) 144

**Q6.** 2, 5, 8, 11, ?
(a) 12  (b) 13  (c) 14  (d) 15

**Q7.** 100, 90, 80, 70, ?
(a) 50  (b) 55  (c) 60  (d) 65

**Q8.** 1, 1, 2, 3, 5, ?
(a) 6  (b) 7  (c) 8  (d) 10

**Q9.** 2, 6, 18, 54, ?
(a) 108  (b) 144  (c) 162  (d) 216

**Q10.** 7, 14, 28, 56, ?
(a) 84  (b) 98  (c) 112  (d) 128

**Q11.** A, C, E, G, ?
(a) H  (b) I  (c) J  (d) K

**Q12.** B, D, F, H, ?
(a) I  (b) J  (c) K  (d) L

**Q13.** Z, Y, X, W, ?
(a) T  (b) U  (c) V  (d) S

**Q14.** A, B, D, G, ?
(a) I  (b) J  (c) K  (d) L

**Q15.** 3, 9, 27, 81, ?
(a) 162  (b) 216  (c) 243  (d) 324

**Q16.** 10, 20, 30, 40, ?
(a) 45  (b) 50  (c) 55  (d) 60

**Q17.** 81, 64, 49, 36, ?
(a) 16  (b) 20  (c) 25  (d) 27

**Q18.** 2, 3, 5, 7, 11, ?
(a) 12  (b) 13  (c) 14  (d) 15

**Q19.** AZ, BY, CX, ?
(a) DV  (b) DW  (c) EW  (d) EV

**Q20.** 1, 3, 6, 10, ?
(a) 13  (b) 14  (c) 15  (d) 16

---

### 🟡 MEDIUM (Questions 21–40)

**Q21.** 4, 9, 19, 39, ?
(a) 59  (b) 69  (c) 79  (d) 89

**Q22.** 2, 6, 12, 20, 30, ?
(a) 40  (b) 42  (c) 44  (d) 46

**Q23.** 5, 11, 23, 47, ?
(a) 85  (b) 89  (c) 95  (d) 99

**Q24.** 120, 99, 80, 63, 48, ?
(a) 33  (b) 35  (c) 37  (d) 39

**Q25.** 1, 4, 27, 256, ?
(a) 625  (b) 1,024  (c) 3,125  (d) 4,096

**Q26.** 3, 7, 15, 31, ?
(a) 47  (b) 55  (c) 63  (d) 71

**Q27.** 2, 12, 36, 80, ?
(a) 120  (b) 130  (c) 150  (d) 180

**Q28.** 6, 11, 21, 36, 56, ?
(a) 76  (b) 81  (c) 86  (d) 91

**Q29.** 1, 2, 6, 24, 120, ?
(a) 240  (b) 480  (c) 600  (d) 720

**Q30.** 8, 24, 12, 36, 18, ?
(a) 36  (b) 48  (c) 54  (d) 72

**Q31.** AC, FH, KM, ?
(a) OQ  (b) PR  (c) QS  (d) NP

**Q32.** 0, 7, 26, 63, ?
(a) 100  (b) 112  (c) 124  (d) 136

**Q33.** 13, 35, 57, 79, ?
(a) 810  (b) 901  (c) 911  (d) 921

**Q34.** 5, 16, 51, 158, ?
(a) 441  (b) 465  (c) 481  (d) 497

**Q35.** 2, 3, 5, 9, 17, ?
(a) 29  (b) 31  (c) 33  (d) 35

**Q36.** B, E, H, K, ?
(a) L  (b) M  (c) N  (d) O

**Q37.** 11, 13, 17, 19, 23, ?
(a) 25  (b) 27  (c) 29  (d) 31

**Q38.** 144, 121, 100, 81, ?
(a) 49  (b) 60  (c) 64  (d) 72

**Q39.** Z, W, T, Q, ?
(a) M  (b) N  (c) O  (d) P

**Q40.** 4, 12, 6, 18, 9, ?
(a) 18  (b) 24  (c) 27  (d) 36

---

### 🔴 HARD (Questions 41–50)

**Q41.** 1, 5, 14, 30, 55, ?
(a) 85  (b) 88  (c) 91  (d) 96

**Q42.** 3, 8, 15, 24, 35, ?
(a) 44  (b) 46  (c) 48  (d) 50

**Q43.** 2, 8, 18, 32, 50, ?
(a) 64  (b) 68  (c) 72  (d) 80

**Q44.** 7, 26, 63, 124, ?
(a) 195  (b) 205  (c) 215  (d) 225

**Q45.** 1, 3, 7, 15, 31, ?
(a) 47  (b) 55  (c) 63  (d) 71

**Q46.** ACE, BDF, CEG, ?
(a) DEF  (b) DFH  (c) EGI  (d) DGH

**Q47.** 240, 120, 40, 10, ?
(a) 1  (b) 2  (c) 4  (d) 5

**Q48.** 6, 12, 21, 33, ?
(a) 45  (b) 46  (c) 48  (d) 51

**Q49.** 1, 2, 5, 26, ?
(a) 156  (b) 456  (c) 677  (d) 782

**Q50.** CMM, EOO, GQQ, ?
(a) HRR  (b) IRR  (c) ISS  (d) JSS

---

## 7. Detailed Solutions

### 🟢 EASY — Solutions 1–20

---

**Q1. 2, 4, 6, 8, ? → (b) 10**

**Pattern:** add 2 each time.
$$2 \xrightarrow{+2} 4 \xrightarrow{+2} 6 \xrightarrow{+2} 8 \xrightarrow{+2} \mathbf{10}$$

*(These are the even numbers.)*

**Answer: (b) 10**

---

**Q2. 3, 6, 12, 24, ? → (c) 48**

**Pattern:** multiply by 2 each time.
$$3 \xrightarrow{\times2} 6 \xrightarrow{\times2} 12 \xrightarrow{\times2} 24 \xrightarrow{\times2} \mathbf{48}$$

**Answer: (c) 48**

---

**Q3. 1, 4, 9, 16, ? → (c) 25**

**Pattern:** perfect squares.
$$1^2, \; 2^2, \; 3^2, \; 4^2, \; \mathbf{5^2 = 25}$$

**Difference check:** 3, 5, 7, [9] — consecutive odd numbers, the signature of squares. 16 + 9 = 25 ✓

**Answer: (c) 25**

---

**Q4. 5, 10, 15, 20, ? → (c) 25**

**Pattern:** add 5 (multiples of 5).
$$20 + 5 = \mathbf{25}$$

**Answer: (c) 25**

---

**Q5. 1, 8, 27, 64, ? → (c) 125**

**Pattern:** perfect cubes.
$$1^3, \; 2^3, \; 3^3, \; 4^3, \; \mathbf{5^3 = 125}$$

**Answer: (c) 125**

---

**Q6. 2, 5, 8, 11, ? → (c) 14**

**Pattern:** add 3.
$$11 + 3 = \mathbf{14}$$

**Answer: (c) 14**

---

**Q7. 100, 90, 80, 70, ? → (c) 60**

**Pattern:** subtract 10.
$$70 - 10 = \mathbf{60}$$

**Answer: (c) 60**

---

**Q8. 1, 1, 2, 3, 5, ? → (c) 8**

**Pattern:** Fibonacci — each term is the sum of the previous two.
$$1 + 1 = 2 \quad 1 + 2 = 3 \quad 2 + 3 = 5 \quad 3 + 5 = \mathbf{8}$$

**Answer: (c) 8**

---

**Q9. 2, 6, 18, 54, ? → (c) 162**

**Pattern:** multiply by 3.
$$54 \times 3 = \mathbf{162}$$

**Answer: (c) 162**

---

**Q10. 7, 14, 28, 56, ? → (c) 112**

**Pattern:** multiply by 2.
$$56 \times 2 = \mathbf{112}$$

**Answer: (c) 112**

---

**Q11. A, C, E, G, ? → (b) I**

**Convert to positions:** 1, 3, 5, 7 — the odd numbers, advancing by 2.

$$7 + 2 = 9 \implies \textbf{I}$$

**Answer: (b) I**

---

**Q12. B, D, F, H, ? → (b) J**

**Positions:** 2, 4, 6, 8 — advancing by 2.

$$8 + 2 = 10 \implies \textbf{J}$$

*(J = 10 is one of the EJOTY anchors.)*

**Answer: (b) J**

---

**Q13. Z, Y, X, W, ? → (c) V**

**Pattern:** the alphabet in reverse, one step at a time.

$$Z(26) \to Y(25) \to X(24) \to W(23) \to \textbf{V}(22)$$

**Answer: (c) V**

---

**Q14. A, B, D, G, ? → (c) K**

**Convert to positions:** 1, 2, 4, 7

**Differences:** 1, 2, 3 ⇒ next difference is **4**

$$7 + 4 = 11 \implies \textbf{K}$$

**Answer: (c) K**

---

**Q15. 3, 9, 27, 81, ? → (c) 243**

**Pattern:** powers of 3 (×3 each time).
$$81 \times 3 = \mathbf{243}$$

**Answer: (c) 243**

---

**Q16. 10, 20, 30, 40, ? → (b) 50**

**Pattern:** add 10.
$$40 + 10 = \mathbf{50}$$

**Answer: (b) 50**

---

**Q17. 81, 64, 49, 36, ? → (c) 25**

**Pattern:** descending perfect squares.
$$9^2, \; 8^2, \; 7^2, \; 6^2, \; \mathbf{5^2 = 25}$$

**Answer: (c) 25**

---

**Q18. 2, 3, 5, 7, 11, ? → (b) 13**

**Pattern:** prime numbers in order.
$$2, \; 3, \; 5, \; 7, \; 11, \; \mathbf{13}$$

> **Trap:** answering 12 or 14 by looking for an arithmetic rule. The differences (1, 2, 2, 4) are irregular — that irregularity is itself the clue that primes are involved.

**Answer: (b) 13**

---

**Q19. AZ, BY, CX, ? → (b) DW**

**Pattern:** each pair consists of a letter and its **opposite** (positions summing to 27).

| Pair | Positions | Sum |
|---|---|---|
| AZ | 1, 26 | 27 |
| BY | 2, 25 | 27 |
| CX | 3, 24 | 27 |
| **DW** | **4, 23** | **27** ✓ |

The first letter advances A → B → C → **D**, and its partner is 27 − 4 = 23 = **W**.

**Answer: (b) DW**

---

**Q20. 1, 3, 6, 10, ? → (c) 15**

**Pattern:** triangular numbers — the differences increase by 1.
```
1  +2→  3  +3→  6  +4→  10  +5→  15
```

*(Equivalently, these are the cumulative sums 1, 1+2, 1+2+3, 1+2+3+4, …)*

**Answer: (c) 15**

---

### 🟡 MEDIUM — Solutions 21–40

---

**Q21. 4, 9, 19, 39, ? → (c) 79**

**Step 1 — Differences.**
$$5, \; 10, \; 20 \quad \text{— these are doubling}$$

Doubling differences signal a multiplicative rule.

**Step 2 — Test ×2 + 1.**
$$4(2)+1 = 9 \checkmark \quad 9(2)+1 = 19 \checkmark \quad 19(2)+1 = 39 \checkmark$$

**Step 3 — Apply.**
$$39 \times 2 + 1 = \mathbf{79}$$

**Answer: (c) 79**

---

**Q22. 2, 6, 12, 20, 30, ? → (b) 42**

**Step 1 — Differences.**
$$4, \; 6, \; 8, \; 10 \implies \text{next} = 12$$

**Step 2 — Extend.**
$$30 + 12 = \mathbf{42}$$

**Pattern recognition:** these are **n(n+1)** — the products 1×2, 2×3, 3×4, 4×5, 5×6, **6×7 = 42** ✓

**Answer: (b) 42**

---

**Q23. 5, 11, 23, 47, ? → (c) 95**

**Step 1 — Differences.**
$$6, \; 12, \; 24 \quad \text{— doubling}$$

**Step 2 — Test ×2 + 1.**
$$5(2)+1 = 11 \checkmark \quad 11(2)+1 = 23 \checkmark \quad 23(2)+1 = 47 \checkmark$$

**Step 3 — Apply.**
$$47 \times 2 + 1 = \mathbf{95}$$

**Cross-check via differences:** the next difference is 48, and 47 + 48 = 95 ✓

**Answer: (c) 95**

---

**Q24. 120, 99, 80, 63, 48, ? → (b) 35**

**Step 1 — Compare against the squares.**
```
Given:    120   99   80   63   48    ?
Squares:  121  100   81   64   49   36
```
Every term is exactly **one less than a perfect square**.

**Step 2 — Identify the sequence of squares.**
$$11^2, \; 10^2, \; 9^2, \; 8^2, \; 7^2, \; \mathbf{6^2}$$

**Step 3 — Apply.**
$$36 - 1 = \mathbf{35}$$

**Difference check:** −21, −19, −17, −15, [−13] ⇒ 48 − 13 = 35 ✓

**Answer: (b) 35**

---

**Q25. 1, 4, 27, 256, ? → (c) 3,125**

**Step 1 — Recognise the pattern.**
$$1^1 = 1, \quad 2^2 = 4, \quad 3^3 = 27, \quad 4^4 = 256$$

The rule is **nⁿ**.

**Step 2 — Apply.**
$$5^5 = 3{,}125$$

**Answer: (c) 3,125**

---

**Q26. 3, 7, 15, 31, ? → (c) 63**

**Step 1 — Test ×2 + 1.**
$$3(2)+1 = 7 \checkmark \quad 7(2)+1 = 15 \checkmark \quad 15(2)+1 = 31 \checkmark$$

**Step 2 — Apply.**
$$31 \times 2 + 1 = \mathbf{63}$$

**Pattern recognition:** these are **2ⁿ − 1** for n = 2, 3, 4, 5, 6: 4−1, 8−1, 16−1, 32−1, **64−1 = 63** ✓

**Answer: (c) 63**

---

**Q27. 2, 12, 36, 80, ? → (c) 150**

**Step 1 — Test against n³ + n².**
$$n=1: \; 1+1 = 2 \checkmark$$
$$n=2: \; 8+4 = 12 \checkmark$$
$$n=3: \; 27+9 = 36 \checkmark$$
$$n=4: \; 64+16 = 80 \checkmark$$

**Step 2 — Apply for n = 5.**
$$125 + 25 = \mathbf{150}$$

**Alternative reading:** the terms are n²(n + 1) — that is, 1(2), 4(3), 9(4), 16(5), **25(6) = 150** ✓

**Answer: (c) 150**

---

**Q28. 6, 11, 21, 36, 56, ? → (b) 81**

**Step 1 — Differences.**
$$5, \; 10, \; 15, \; 20 \quad \text{— increasing by 5}$$

**Step 2 — Next difference.**
$$20 + 5 = 25$$

**Step 3 — Extend.**
$$56 + 25 = \mathbf{81}$$

**Answer: (b) 81**

---

**Q29. 1, 2, 6, 24, 120, ? → (d) 720**

**Step 1 — Examine the ratios.**
$$\frac{2}{1} = 2, \quad \frac{6}{2} = 3, \quad \frac{24}{6} = 4, \quad \frac{120}{24} = 5$$

The multiplier increases by 1 each step.

**Step 2 — Apply.**
$$120 \times 6 = \mathbf{720}$$

**Pattern recognition:** these are the **factorials** 1!, 2!, 3!, 4!, 5!, **6! = 720** ✓

**Answer: (d) 720**

---

**Q30. 8, 24, 12, 36, 18, ? → (c) 54**

**Step 1 — Examine consecutive ratios.**
$$\frac{24}{8} = 3, \quad \frac{12}{24} = \frac{1}{2}, \quad \frac{36}{12} = 3, \quad \frac{18}{36} = \frac{1}{2}$$

**Step 2 — Identify the alternating rule.**
$$\times3, \; \div2, \; \times3, \; \div2, \; \times3 \ldots$$

**Step 3 — The last operation was ÷2, so next is ×3.**
$$18 \times 3 = \mathbf{54}$$

**Full chain:**
```
8  ×3→ 24  ÷2→ 12  ×3→ 36  ÷2→ 18  ×3→ 54 ✓
```

**Answer: (c) 54**

---

**Q31. AC, FH, KM, ? → (b) PR**

**Step 1 — Convert to positions.**
$$\text{AC} = (1, 3) \qquad \text{FH} = (6, 8) \qquad \text{KM} = (11, 13)$$

**Step 2 — Identify two patterns.**
- First letters: 1, 6, 11 ⇒ **+5** each time
- Second letters: 3, 8, 13 ⇒ **+5** each time
- Within each pair, the second letter is 2 ahead of the first

**Step 3 — Extend.**
$$(11 + 5, \; 13 + 5) = (16, 18) = \textbf{PR}$$

**Answer: (b) PR**

---

**Q32. 0, 7, 26, 63, ? → (c) 124**

**Step 1 — Compare against the cubes.**
```
Given:  0    7    26    63     ?
Cubes:  1    8    27    64   125
```
Every term is **one less than a cube**.

**Step 2 — Apply the rule n³ − 1 for n = 5.**
$$125 - 1 = \mathbf{124}$$

**Answer: (c) 124**

---

**Q33. 13, 35, 57, 79, ? → (c) 911**

**Step 1 — Read the terms as PAIRS OF DIGITS rather than as numbers.**
```
13  →  1, 3
35  →  3, 5
57  →  5, 7
79  →  7, 9
```

**Step 2 — Identify the pattern.**
Each term is formed from **two consecutive odd numbers** written side by side.

**Step 3 — Extend.**
The next pair of consecutive odd numbers is **9 and 11**, written together as:
$$\mathbf{911}$$

> **The signal:** the differences here are a constant 22, which would predict 101. But 101 is not among the options, and the digit structure (1-3, 3-5, 5-7, 7-9) is unmistakable. **When arithmetic differences produce an answer not among the options, look at the digits themselves.**

**Answer: (c) 911**

---

**Q34. 5, 16, 51, 158, ? → (c) 481**

**Step 1 — Test a "×3 + something" rule.**
$$5 \times 3 = 15, \quad 16 - 15 = \mathbf{1}$$
$$16 \times 3 = 48, \quad 51 - 48 = \mathbf{3}$$
$$51 \times 3 = 153, \quad 158 - 153 = \mathbf{5}$$

**Step 2 — Identify the added values.**
They are 1, 3, 5 — consecutive odd numbers. The next addend is **7**.

**Step 3 — Apply.**
$$158 \times 3 + 7 = 474 + 7 = \mathbf{481}$$

**Answer: (c) 481**

---

**Q35. 2, 3, 5, 9, 17, ? → (c) 33**

**Step 1 — Differences.**
$$1, \; 2, \; 4, \; 8 \quad \text{— doubling}$$

**Step 2 — Next difference.**
$$8 \times 2 = 16$$

**Step 3 — Extend.**
$$17 + 16 = \mathbf{33}$$

**Alternative rule:** each term is **2 × previous − 1**:
$$2(2)-1 = 3 \checkmark \quad 2(3)-1 = 5 \checkmark \quad 2(5)-1 = 9 \checkmark \quad 2(9)-1 = 17 \checkmark \quad 2(17)-1 = 33 \checkmark$$

**Answer: (c) 33**

---

**Q36. B, E, H, K, ? → (c) N**

**Positions:** 2, 5, 8, 11 ⇒ advancing by **3**

$$11 + 3 = 14 \implies \textbf{N}$$

**Answer: (c) N**

---

**Q37. 11, 13, 17, 19, 23, ? → (c) 29**

**Pattern:** consecutive prime numbers.

$$11, \; 13, \; 17, \; 19, \; 23, \; \mathbf{29}$$

> **Note:** 25 is not prime (5 × 5) and 27 is not prime (3³). The next prime after 23 is 29.

**Answer: (c) 29**

---

**Q38. 144, 121, 100, 81, ? → (c) 64**

**Pattern:** descending perfect squares.
$$12^2, \; 11^2, \; 10^2, \; 9^2, \; \mathbf{8^2 = 64}$$

**Answer: (c) 64**

---

**Q39. Z, W, T, Q, ? → (b) N**

**Convert to positions:** 26, 23, 20, 17 ⇒ decreasing by **3**

$$17 - 3 = 14 \implies \textbf{N}$$

**Answer: (b) N**

---

**Q40. 4, 12, 6, 18, 9, ? → (c) 27**

**Step 1 — Examine the ratios.**
$$\frac{12}{4} = 3, \quad \frac{6}{12} = \frac{1}{2}, \quad \frac{18}{6} = 3, \quad \frac{9}{18} = \frac{1}{2}$$

**Step 2 — The alternating rule is ×3, ÷2.**

**Step 3 — The last operation was ÷2, so next is ×3.**
$$9 \times 3 = \mathbf{27}$$

**Answer: (c) 27**

---

### 🔴 HARD — Solutions 41–50

---

**Q41. 1, 5, 14, 30, 55, ? → (c) 91**

**Step 1 — Differences.**
$$4, \; 9, \; 16, \; 25$$

These are **perfect squares** (2², 3², 4², 5²).

**Step 2 — Next difference.**
$$6^2 = 36$$

**Step 3 — Extend.**
$$55 + 36 = \mathbf{91}$$

**Pattern recognition:** these are the **cumulative sums of squares**:
$$1, \; 1+4, \; 1+4+9, \; 1+4+9+16, \; \ldots$$

**Formula check:** the sum of the first *n* squares is n(n+1)(2n+1)/6. For n = 6:
$$\frac{6 \times 7 \times 13}{6} = 91 \checkmark$$

**Answer: (c) 91**

---

**Q42. 3, 8, 15, 24, 35, ? → (c) 48**

**Step 1 — Compare against the squares.**
```
Given:    3    8   15   24   35    ?
Squares:  4    9   16   25   36   49
```
Every term is **one less than a perfect square**.

**Step 2 — Apply n² − 1 for n = 7.**
$$49 - 1 = \mathbf{48}$$

**Difference check:** 5, 7, 9, 11, [13] — consecutive odd numbers ⇒ 35 + 13 = 48 ✓

**Answer: (c) 48**

---

**Q43. 2, 8, 18, 32, 50, ? → (c) 72**

**Step 1 — Halve each term.**
$$1, \; 4, \; 9, \; 16, \; 25 \quad \text{— perfect squares!}$$

**Step 2 — Identify the rule.**
$$a_n = 2n^2$$

**Step 3 — Apply for n = 6.**
$$2 \times 36 = \mathbf{72}$$

**Difference check:** 6, 10, 14, 18, [22] — an arithmetic sequence with common difference 4 ⇒ 50 + 22 = 72 ✓

**Answer: (c) 72**

---

**Q44. 7, 26, 63, 124, ? → (c) 215**

**Step 1 — Compare against the cubes.**
```
Given:   7    26    63    124     ?
Cubes:   8    27    64    125   216
```
Every term is **one less than a cube**.

**Step 2 — Identify the sequence.**
$$2^3-1, \; 3^3-1, \; 4^3-1, \; 5^3-1, \; \mathbf{6^3-1}$$

**Step 3 — Apply.**
$$216 - 1 = \mathbf{215}$$

**Answer: (c) 215**

---

**Q45. 1, 3, 7, 15, 31, ? → (c) 63**

**Step 1 — Differences.**
$$2, \; 4, \; 8, \; 16 \quad \text{— powers of 2}$$

**Step 2 — Next difference.**
$$32$$

**Step 3 — Extend.**
$$31 + 32 = \mathbf{63}$$

**Pattern recognition:** these are **2ⁿ − 1**:
$$2^1-1 = 1, \; 2^2-1 = 3, \; 2^3-1 = 7, \; 2^4-1 = 15, \; 2^5-1 = 31, \; \mathbf{2^6-1 = 63} \checkmark$$

**Alternative rule:** ×2 + 1 each time ⇒ 31(2) + 1 = 63 ✓

**Answer: (c) 63**

---

**Q46. ACE, BDF, CEG, ? → (b) DFH**

**Step 1 — Convert each group to positions.**
$$\text{ACE} = (1, 3, 5)$$
$$\text{BDF} = (2, 4, 6)$$
$$\text{CEG} = (3, 5, 7)$$

**Step 2 — Identify the across-group pattern.**
Each letter advances by **+1** from the corresponding letter in the previous group.

*(Within each group the letters advance by 2, but that is constant across all groups — it does not determine the next term.)*

**Step 3 — Extend.**
$$(4, 6, 8) = \textbf{DFH}$$

**Answer: (b) DFH**

---

**Q47. 240, 120, 40, 10, ? → (b) 2**

**Step 1 — Examine the divisors.**
$$\frac{240}{120} = 2, \quad \frac{120}{40} = 3, \quad \frac{40}{10} = 4$$

The divisor increases by 1 each step: ÷2, ÷3, ÷4, then **÷5**.

**Step 2 — Apply.**
$$\frac{10}{5} = \mathbf{2}$$

**Full chain:**
```
240  ÷2→ 120  ÷3→ 40  ÷4→ 10  ÷5→ 2 ✓
```

> **Trap:** answering 5 by assuming a constant ÷2. Check the ratio at **every** step — here it changes each time.

**Answer: (b) 2**

---

**Q48. 6, 12, 21, 33, ? → (c) 48**

**Step 1 — Differences.**
$$6, \; 9, \; 12 \quad \text{— increasing by 3}$$

**Step 2 — Next difference.**
$$12 + 3 = 15$$

**Step 3 — Extend.**
$$33 + 15 = \mathbf{48}$$

**Answer: (c) 48**

---

**Q49. 1, 2, 5, 26, ? → (c) 677**

**Step 1 — Look for a relationship between consecutive terms.**
$$1^2 + 1 = 2 \checkmark$$
$$2^2 + 1 = 5 \checkmark$$
$$5^2 + 1 = 26 \checkmark$$

**Step 2 — The rule is: square the previous term and add 1.**

**Step 3 — Apply.**
$$26^2 + 1 = 676 + 1 = \mathbf{677}$$

> **The signal:** explosive growth (1 → 2 → 5 → 26) rules out addition and simple multiplication. When terms grow this fast, test whether each term is a function of the **previous term squared**.

**Answer: (c) 677**

---

**Q50. CMM, EOO, GQQ, ? → (c) ISS**

**Step 1 — Convert to positions.**
$$\text{CMM} = (3, 13, 13)$$
$$\text{EOO} = (5, 15, 15)$$
$$\text{GQQ} = (7, 17, 17)$$

**Step 2 — Identify the pattern.**
- First letters: 3, 5, 7 ⇒ **+2** each time
- Second and third letters (always identical): 13, 15, 17 ⇒ **+2** each time

**Step 3 — Extend.**
$$(9, 19, 19) = (\text{I}, \text{S}, \text{S}) = \textbf{ISS}$$

**Verification:** I = 9 ✓ and S = 19 ✓ (S is one before T = 20)

**Answer: (c) ISS**

---

## 8. Quick Revision Sheet

> **One page. Read 48 hours after study, and again the night before the test.**

### The method

```
1.  Take FIRST DIFFERENCES
2.  Constant?          → arithmetic, done
    Steadily growing?  → take SECOND differences
    Doubling?          → test ×2 + c
    Ratios constant?   → geometric
3.  Compare terms against n², n³, n!, 2ⁿ, primes
4.  Nothing fits?      → SPLIT into alternate terms
5.  VERIFY on every given term before answering
```

### Number families — recognise on sight

```
SQUARES     1  4  9  16  25  36  49  64  81  100 121 144 169 196 225
CUBES       1  8  27  64  125  216  343  512  729  1000
PRIMES      2  3  5  7  11  13  17  19  23  29  31  37  41  43  47
FIBONACCI   1  1  2  3  5  8  13  21  34  55  89
FACTORIAL   1  2  6  24  120  720  5040
2ⁿ          2  4  8  16  32  64  128  256  512
TRIANGULAR  1  3  6  10  15  21  28  36  45

NEAR-MISS FAMILIES — the ones that actually appear:
   n² − 1   →  0  3  8  15  24  35  48  63  80  99
   n² + 1   →  2  5  10  17  26  37  50  65
   n³ − 1   →  0  7  26  63  124  215
   2ⁿ − 1   →  1  3  7  15  31  63  127
   2n²      →  2  8  18  32  50  72
   n(n+1)   →  2  6  12  20  30  42
   n³ + n²  →  2  12  36  80  150
   nⁿ       →  1  4  27  256  3125
```

### Alphabet

```
A1  B2  C3  D4  E5  F6  G7  H8  I9  J10 K11 L12 M13
N14 O15 P16 Q17 R18 S19 T20 U21 V22 W23 X24 Y25 Z26

ANCHORS (EJOTY):  E=5  J=10  O=15  T=20  Y=25
OPPOSITE LETTER:  position 27 − n
   A↔Z  B↔Y  C↔X  D↔W  E↔V  F↔U  G↔T
   H↔S  I↔R  J↔Q  K↔P  L↔O  M↔N
```

### Letter-series method

```
1.  Convert letters to POSITION NUMBERS
2.  Find the numeric pattern
3.  Convert back

Constant skip     A C E G  →  1 3 5 7  →  +2  →  I
Growing skip      A B D G  →  1 2 4 7  →  +1,+2,+3  →  K(11)
Reverse           Z W T Q  →  26 23 20 17  →  −3  →  N(14)
Groups            compare POSITION-BY-POSITION across groups
```

### Special reads

```
DIGIT-BASED    13, 35, 57, 79  →  read as digit PAIRS (1&3, 3&5, …)  →  911
INTERLEAVED    split odd/even positions — CHECK WHICH POSITION '?' OCCUPIES
ALTERNATING    ×3 ÷2 ×3 ÷2 …   or   +5 −2 +5 −2 …
WRONG TERM     build the rule from the AGREEING terms, then predict
```

### Signals

```
Differences doubling            →  ×2 + c
Differences are squares         →  cumulative sums of squares
Differences are odd numbers     →  n² based
Divisor/multiplier changes      →  ÷2 ÷3 ÷4 …  or  ×2 ×3 ×4 …
Explosive growth                →  previous term SQUARED, or factorial
Irregular differences           →  primes
Rises and falls                 →  interleaved / alternating
```

---

## 9. Common Mistakes

| # | Mistake | Example | Correction |
|---|---|---|---|
| 1 | **Rule fitted to only some terms** | Explaining 4 of 5 terms | Verify against **every** term |
| 2 | **Differences not computed** | Guessing from the terms alone | Write the difference row first |
| 3 | **Interleaved series missed** | Forcing one rule on 8, 24, 12, 36 | Split by position |
| 4 | **Wrong position for the '?'** | Continuing the even sub-series | Count the index of the '?' |
| 5 | **Constant ratio assumed** | 240, 120, 40 read as ÷2 throughout | Check every ratio: ÷2, ÷3, ÷4 |
| 6 | **Digit patterns overlooked** | 13, 35, 57 forced into arithmetic | Read the digits as pairs |
| 7 | **Near-miss families missed** | 3, 8, 15, 24 not linked to squares | Always compare with n² and n³ |
| 8 | **Primes mistaken for arithmetic** | 2, 3, 5, 7, 11 ⇒ next 14 | Irregular gaps ⇒ suspect primes |
| 9 | **Letters not converted to numbers** | Guessing at A, B, D, G | Convert: 1, 2, 4, 7 ⇒ +1, +2, +3 |
| 10 | **Within-group pattern used for groups** | ACE ⇒ next is EGI | Compare **across** groups: DFH |
| 11 | **Wrong-term rule built from all terms** | Trying to include the faulty term | Build from the terms that agree |
| 12 | **Alternating operation phase lost** | Applying ÷2 when ×3 was due | Track which operation came last |

---

## Practice Answer Key

| Q | Ans | Q | Ans | Q | Ans | Q | Ans | Q | Ans |
|---|---|---|---|---|---|---|---|---|---|
| 1 | b | 11 | b | 21 | c | 31 | b | 41 | c |
| 2 | c | 12 | b | 22 | b | 32 | c | 42 | c |
| 3 | c | 13 | c | 23 | c | 33 | c | 43 | c |
| 4 | c | 14 | c | 24 | b | 34 | c | 44 | c |
| 5 | c | 15 | c | 25 | c | 35 | c | 45 | c |
| 6 | c | 16 | b | 26 | c | 36 | c | 46 | b |
| 7 | c | 17 | c | 27 | c | 37 | c | 47 | b |
| 8 | c | 18 | b | 28 | b | 38 | c | 48 | c |
| 9 | c | 19 | b | 29 | d | 39 | b | 49 | c |
| 10 | c | 20 | c | 30 | c | 40 | c | 50 | c |

**Scoring guide:** 45+/50 → strong. 35–44 → solid; drill the near-miss families (n²±1, n³±1, 2ⁿ−1) until recognition is instant. Below 35 → this topic responds purely to volume — redo this set, then find 100 more series anywhere and work through them.

---

**⬅️ Back:** [Topic 12 — Ages, Clocks & Calendars](12-ages-clocks-calendars.md) · **➡️ Next:** [Topic 14 — Coding–Decoding](14-coding-decoding.md)
