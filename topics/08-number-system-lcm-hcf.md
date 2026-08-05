# Topic 8 — Number System, LCM & HCF

### EY Placement Aptitude Handbook · Priority Rank #13 · 🟠 High

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

**Weightage:** 5–7% of the quantitative section — typically **1 question**.

**Why it earns study time beyond its raw weightage:** number-system fluency (divisibility rules, unit digits, factor counting) makes you *faster* everywhere else. Divisibility rules speed up fraction simplification in DI. Unit-digit logic lets you eliminate three options in five seconds. LCM underpins the entire Time & Work method.

**Question styles reported:**

| Style | Typical shape |
|---|---|
| Direct LCM / HCF | "Find the LCM of 12, 15 and 20" |
| HCF × LCM = product | "HCF 12, LCM 336, one number 84 — find the other" |
| "Same remainder" HCF | "Greatest number dividing 43, 91, 183 with the same remainder" |
| "Common remainder" LCM | "Least number leaving remainder 3 when divided by 6, 7, 8" |
| Unit digit of a power | "Unit digit of 7¹⁰⁵" |
| Remainder of a large power | "Remainder when 2³¹ is divided by 5" |
| Number of factors | "How many factors does 360 have?" |
| Trailing zeros in a factorial | "Number of zeros at the end of 100!" |
| Divisibility rules | "5A2 is divisible by 3 — find A" |
| Successive division | "Divided by 3, 4, 7 leaves 2, 1, 4" |

---

## 2. Core Concepts

### 2.1 Classification of numbers

```
                        REAL NUMBERS
                             │
              ┌──────────────┴──────────────┐
          RATIONAL                      IRRATIONAL
      (p/q, q ≠ 0)                  (√2, π, e, …)
              │
      ┌───────┴────────┐
   INTEGERS        FRACTIONS
      │
  ┌───┴────┬─────────┐
NEGATIVE  ZERO   POSITIVE (Natural)
                     │
              ┌──────┴──────┐
           PRIME        COMPOSITE   (and 1, which is neither)
```

| Type | Definition | Examples |
|---|---|---|
| **Natural** | Counting numbers | 1, 2, 3, … |
| **Whole** | Naturals plus zero | 0, 1, 2, … |
| **Integer** | Whole numbers and their negatives | …, −2, −1, 0, 1, 2, … |
| **Prime** | Exactly two factors (1 and itself) | 2, 3, 5, 7, 11, 13, … |
| **Composite** | More than two factors | 4, 6, 8, 9, 10, … |
| **Co-prime** | HCF of the pair is 1 | (8, 15), (9, 16) |

> **Two facts examiners exploit:**
> - **1 is neither prime nor composite** (it has only one factor).
> - **2 is the only even prime.**

**Primes up to 50 (memorise):**
```
2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47
```
There are **15** primes below 50 and **25** below 100.

**Testing primality:** a number *n* is prime if it is divisible by no prime ≤ √n.
> Is 143 prime? √143 ≈ 12. Test 2, 3, 5, 7, 11: **143 = 11 × 13** ⇒ not prime.

### 2.2 Divisibility rules

| Divisor | Rule |
|---|---|
| **2** | Last digit is even |
| **3** | **Digit sum** divisible by 3 |
| **4** | Last **two** digits form a number divisible by 4 |
| **5** | Last digit is 0 or 5 |
| **6** | Divisible by both 2 and 3 |
| **7** | Double the last digit, subtract from the rest; repeat |
| **8** | Last **three** digits divisible by 8 |
| **9** | **Digit sum** divisible by 9 |
| **10** | Last digit is 0 |
| **11** | (Sum of odd-place digits) − (sum of even-place digits) is 0 or a multiple of 11 |
| **12** | Divisible by both 3 and 4 |
| **25** | Last two digits are 00, 25, 50 or 75 |

**Worked examples:**

> **Is 4,832 divisible by 8?** Last three digits: 832. 832 ÷ 8 = 104 ✓ **Yes**

> **Is 91,839 divisible by 11?**
> Digits from the right: 9(odd), 3(even), 8(odd), 1(even), 9(odd)
> Odd places: 9 + 8 + 9 = 26; Even places: 3 + 1 = 4
> 26 − 4 = 22, a multiple of 11 ⇒ **Yes**

> **Is 1,073 divisible by 7?**
> 107 − (2 × 3) = 107 − 6 = 101. 101 is not divisible by 7 ⇒ **No**

### 2.3 HCF and LCM

**HCF (Highest Common Factor / GCD):** the largest number that divides all the given numbers.

**LCM (Lowest Common Multiple):** the smallest number divisible by all the given numbers.

**Method 1 — Prime factorisation:**
```
        24 = 2³ × 3
        36 = 2² × 3²

  HCF = product of the LOWEST powers of COMMON primes = 2² × 3 = 12
  LCM = product of the HIGHEST powers of ALL primes   = 2³ × 3² = 72
```

**Method 2 — Division (Euclid's algorithm) for HCF of two numbers:**
```
HCF(1071, 462):
    1071 = 2 × 462 + 147
     462 = 3 × 147 + 21
     147 = 7 × 21  + 0     →  HCF = 21
```

**The master identity (two numbers only):**

$$\boxed{\text{HCF} \times \text{LCM} = \text{Product of the two numbers}}$$

> HCF = 12, LCM = 336, one number = 84.
> Other number = (12 × 336)/84 = 4,032/84 = **48**

> **This identity holds only for TWO numbers.** For three or more it fails: HCF(2,3,4) × LCM(2,3,4) = 1 × 12 = 12, but 2 × 3 × 4 = 24.

**HCF and LCM of fractions:**

$$\text{HCF of fractions} = \frac{\text{HCF of numerators}}{\text{LCM of denominators}}$$

$$\text{LCM of fractions} = \frac{\text{LCM of numerators}}{\text{HCF of denominators}}$$

> HCF of 3/4 and 5/6 = HCF(3,5)/LCM(4,6) = **1/12**
> LCM of 2/3, 4/9, 8/27 = LCM(2,4,8)/HCF(3,9,27) = **8/3**

### 2.4 ⭐ The two remainder patterns (learn to tell them apart)

These two families look similar and are constantly confused. The distinction is simple:

| Pattern | Signal | Tool |
|---|---|---|
| **Type A — SAME remainder given** | "leaves remainder 3 in each case" | **LCM** |
| **Type B — same but UNKNOWN remainder** | "leaves the same remainder" (value not stated) | **HCF of differences** |

---

**Type A — LCM-based.** *"Least number which when divided by 6, 7 and 8 leaves remainder 3."*

$$N = \text{LCM}(6,7,8) \times k + 3 = 168k + 3$$

Smallest: **171**.

**Variant — different remainders with a constant deficit.** *"Divided by 5, 6, 7 leaves 3, 4, 5."*
Notice 5 − 3 = 2, 6 − 4 = 2, 7 − 5 = 2 — a **common deficit of 2**.
$$N = \text{LCM}(5,6,7) \times k - 2 = 210k - 2$$
Smallest: **208**.

---

**Type B — HCF of differences.** *"Greatest number that divides 43, 91 and 183 leaving the same remainder."*

Since all three leave the same remainder *r*, the divisor must divide every **difference**:

$$91 - 43 = 48, \qquad 183 - 91 = 92, \qquad 183 - 43 = 140$$
$$\text{HCF}(48, 92, 140) = 4$$

**Answer: 4.** *(Check: 43 = 4(10) + 3, 91 = 4(22) + 3, 183 = 4(45) + 3 — remainder 3 each time ✓)*

**Variant — different stated remainders.** *"Greatest number dividing 400, 435, 541 leaving remainders 9, 10, 14."*
Subtract each remainder first, then take the HCF:
$$\text{HCF}(391, 425, 527) = 17$$

### 2.5 Unit digits (cyclicity)

The last digit of a power repeats in a short cycle.

| Base ends in | Cycle | Length |
|---|---|---|
| **0** | 0 | 1 |
| **1** | 1 | 1 |
| **2** | 2, 4, 8, 6 | 4 |
| **3** | 3, 9, 7, 1 | 4 |
| **4** | 4, 6 | 2 |
| **5** | 5 | 1 |
| **6** | 6 | 1 |
| **7** | 7, 9, 3, 1 | 4 |
| **8** | 8, 4, 2, 6 | 4 |
| **9** | 9, 1 | 2 |

**Procedure for base ending in 2, 3, 7 or 8 (cycle length 4):**
```
1.  Divide the EXPONENT by 4
2.  Remainder 1 → 1st element   Remainder 2 → 2nd element
    Remainder 3 → 3rd element   Remainder 0 → 4th (LAST) element
```

> **Unit digit of 7¹⁰⁵:** 105 ÷ 4 leaves remainder 1 ⇒ 1st element of (7, 9, 3, 1) ⇒ **7**
> **Unit digit of 2⁴⁰:** 40 ÷ 4 leaves remainder 0 ⇒ 4th element of (2, 4, 8, 6) ⇒ **6**
> **Unit digit of 8²³:** 23 ÷ 4 leaves remainder 3 ⇒ 3rd element of (8, 4, 2, 6) ⇒ **2**

**Digits 0, 1, 5 and 6 always end in themselves** — 6⁵⁰ ends in 6, 5¹⁰⁰ ends in 5.

### 2.6 Number of factors, sum of factors

If $N = p^a \times q^b \times r^c$ (prime factorisation), then:

| Quantity | Formula |
|---|---|
| **Number of factors** | $(a+1)(b+1)(c+1)$ |
| **Sum of factors** | $\dfrac{p^{a+1}-1}{p-1} \times \dfrac{q^{b+1}-1}{q-1} \times \cdots$ |
| **Number of perfect-square factors** | Count only **even** exponents: $\left(\lfloor\frac{a}{2}\rfloor+1\right)\left(\lfloor\frac{b}{2}\rfloor+1\right)\cdots$ |
| **Product of all factors** | $N^{(\text{number of factors})/2}$ |

> **360 = 2³ × 3² × 5¹** ⇒ number of factors = 4 × 3 × 2 = **24**

> **Sum of factors of 60 = 2² × 3 × 5:**
> $$(1+2+4)(1+3)(1+5) = 7 \times 4 \times 6 = 168$$

### 2.7 Trailing zeros in a factorial

A trailing zero comes from a factor of 10 = 2 × 5. In any factorial there are always more 2s than 5s, so **count the 5s**.

$$\boxed{\text{Zeros in } n! = \left\lfloor\frac{n}{5}\right\rfloor + \left\lfloor\frac{n}{25}\right\rfloor + \left\lfloor\frac{n}{125}\right\rfloor + \cdots}$$

> **Zeros in 100!** = ⌊100/5⌋ + ⌊100/25⌋ + ⌊100/125⌋ = 20 + 4 + 0 = **24**
> **Zeros in 25!** = 5 + 1 = **6**

### 2.8 Standard summation formulas

| Series | Sum |
|---|---|
| First *n* natural numbers | $\dfrac{n(n+1)}{2}$ |
| First *n* odd numbers | $n^2$ |
| First *n* even numbers | $n(n+1)$ |
| Squares of first *n* naturals | $\dfrac{n(n+1)(2n+1)}{6}$ |
| Cubes of first *n* naturals | $\left[\dfrac{n(n+1)}{2}\right]^2$ |

### 2.9 Useful factorisation identities

$$a^n - b^n \text{ is divisible by } (a - b) \text{ for all } n$$
$$a^n - b^n \text{ is divisible by } (a + b) \text{ for even } n$$
$$\boxed{a^n + b^n \text{ is divisible by } (a + b) \text{ for ODD } n}$$

> **Is 15²³ + 23²³ divisible by 19?**
> 15 + 23 = 38 = 2 × 19, and 23 is odd ⇒ divisible by 38, hence by **19**. Remainder = 0.

### 2.10 Successive division

> *"A number, when successively divided by 3, 4 and 7, leaves remainders 2, 1 and 4."*

"Successively" means the **quotient** of each division is fed into the next. Work **backwards** from the last division:

```
Let the final quotient be 0 (smallest case).
    Third division:  b = 7(0) + 4  =  4
    Second division: a = 4(4) + 1  = 17
    First division:  N = 3(17) + 2 = 53
```

**Check:** 53 ÷ 3 = 17 remainder **2** ✓ · 17 ÷ 4 = 4 remainder **1** ✓ · 4 ÷ 7 = 0 remainder **4** ✓

---

## 3. Formula Bank

| # | Concept | Formula |
|---|---|---|
| 1 | HCF × LCM (two numbers) | $= a \times b$ |
| 2 | HCF of fractions | $\dfrac{\text{HCF of numerators}}{\text{LCM of denominators}}$ |
| 3 | LCM of fractions | $\dfrac{\text{LCM of numerators}}{\text{HCF of denominators}}$ |
| 4 | Same remainder *r* given | $N = \text{LCM} \times k + r$ |
| 5 | Common deficit *d* | $N = \text{LCM} \times k - d$ |
| 6 | Same unknown remainder | HCF of the pairwise **differences** |
| 7 | Different stated remainders | HCF of (number − its remainder) |
| 8 | Number of factors of $p^aq^br^c$ | $(a+1)(b+1)(c+1)$ |
| 9 | Sum of factors | $\prod \dfrac{p^{a+1}-1}{p-1}$ |
| 10 | Perfect-square factors | $\prod\left(\lfloor\tfrac{a}{2}\rfloor + 1\right)$ |
| 11 | Product of all factors | $N^{d(N)/2}$ |
| 12 | Trailing zeros in *n*! | $\sum \left\lfloor \dfrac{n}{5^i} \right\rfloor$ |
| 13 | Sum of first *n* naturals | $\dfrac{n(n+1)}{2}$ |
| 14 | Sum of first *n* odd numbers | $n^2$ |
| 15 | Sum of first *n* even numbers | $n(n+1)$ |
| 16 | Sum of squares | $\dfrac{n(n+1)(2n+1)}{6}$ |
| 17 | Sum of cubes | $\left[\dfrac{n(n+1)}{2}\right]^2$ |
| 18 | Count of multiples of *k* in [a, b] | $\left\lfloor\dfrac{b}{k}\right\rfloor - \left\lfloor\dfrac{a-1}{k}\right\rfloor$ |
| 19 | $a^n + b^n$ divisible by $(a+b)$ | when *n* is **odd** |
| 20 | $a^n - b^n$ divisible by $(a-b)$ | for all *n* |
| 21 | Dividend | $= \text{Divisor} \times \text{Quotient} + \text{Remainder}$ |
| 22 | Remainder when divisor is a factor | $r_{\text{small}} = r_{\text{large}} \bmod \text{small divisor}$ |

---

## 4. Shortcuts & Tricks

### 4.1 The divisibility toolkit (drill these)

```
2  →  last digit even
3  →  digit sum ÷ 3
4  →  last TWO digits ÷ 4
5  →  ends in 0 or 5
6  →  passes 2 AND 3
8  →  last THREE digits ÷ 8
9  →  digit sum ÷ 9
11 →  alternating digit sum is 0 or ÷ 11
```

Digit-sum rules (3 and 9) and alternating-sum (11) are the ones that pay off most often.

### 4.2 The remainder-type decision tree

```
Does the question STATE the remainder value?
    │
    ├─ YES, and it's the SAME for all divisors
    │      → N = LCM × k + r
    │
    ├─ YES, different remainders but CONSTANT DEFICIT (divisor − remainder equal)
    │      → N = LCM × k − d
    │
    └─ NO, it just says "the same remainder"
           → HCF of the pairwise DIFFERENCES
```

Getting this classification right is 90% of the battle on remainder questions.

### 4.3 Unit digit in four seconds

```
1.  Look at the base's LAST DIGIT only
2.  If it's 0, 1, 5 or 6  →  answer is that digit. Done.
3.  If it's 4 or 9        →  cycle length 2. Even exponent → 6 (for 4) or 1 (for 9).
                                             Odd exponent → 4 or 9.
4.  Otherwise (2,3,7,8)   →  divide the EXPONENT by 4, use the remainder
                             (remainder 0 means take the LAST element)
```

**Quick reference:**

| Power | Unit digit |
|---|---|
| 2⁴ᵏ, 3⁴ᵏ, 7⁴ᵏ | 6, 1, 1 |
| 4^even, 4^odd | 6, 4 |
| 9^even, 9^odd | 1, 9 |
| Anything ending in 5 or 6 | 5 or 6 |

### 4.4 Remainder of a big power

Compute the **cycle of remainders**, not the number itself.

> **Remainder of 3⁴⁰ ÷ 7:**
```
3¹ ≡ 3     3² ≡ 2     3³ ≡ 6
3⁴ ≡ 4     3⁵ ≡ 5     3⁶ ≡ 1   ← cycle length 6
40 ÷ 6 leaves remainder 4  →  3⁴⁰ ≡ 3⁴ ≡ 4
```

**For divisor 5 or 10, use the unit digit instead** — it is faster:
> 2³¹: unit digit is 8 (31 mod 4 = 3) ⇒ 8 mod 5 = **3**

### 4.5 The divisor-of-a-divisor shortcut

> *"A number divided by 342 leaves remainder 47. Find the remainder when divided by 19."*

Since **342 = 19 × 18**, the divisor 19 divides 342 exactly. So:
$$N = 342k + 47 \implies N \bmod 19 = 47 \bmod 19 = 47 - 38 = \mathbf{9}$$

**Rule:** if the smaller divisor is a factor of the larger, just reduce the *remainder* modulo the smaller divisor.

### 4.6 Counting multiples in a range

$$\text{Count of multiples of } k \text{ from } a \text{ to } b = \left\lfloor\frac{b}{k}\right\rfloor - \left\lfloor\frac{a-1}{k}\right\rfloor$$

> Multiples of 7 between 100 and 300:
> ⌊300/7⌋ − ⌊99/7⌋ = 42 − 14 = **28**

Or, equivalently: first multiple 105 (= 7 × 15), last 294 (= 7 × 42) ⇒ 42 − 15 + 1 = 28 ✓

### 4.7 The "sum of two numbers with given HCF" pattern

> *"Sum = 528, HCF = 33. How many such pairs?"*

Write the numbers as 33*a* and 33*b* with **a and b co-prime**:
$$33(a + b) = 528 \implies a + b = 16$$

Now count co-prime pairs summing to 16:
$$(1,15), (3,13), (5,11), (7,9)$$
*(Pairs like (2,14), (4,12), (6,10), (8,8) share a factor with each other, so they are excluded.)*

**Answer: 4 pairs.**

### 4.8 Squares and cubes worth knowing

| n | n² | n³ | | n | n² |
|---|---|---|---|---|---|
| 11 | 121 | 1331 | | 16 | 256 |
| 12 | 144 | 1728 | | 17 | 289 |
| 13 | 169 | 2197 | | 18 | 324 |
| 14 | 196 | 2744 | | 19 | 361 |
| 15 | 225 | 3375 | | 25 | 625 |

Recognising 1,331 = 11³, 1,728 = 12³ and 9,261 = 21³ saves real time (they also appear constantly in compound-interest questions).

---

## 5. Solved Examples

### Example 1 — HCF and LCM by factorisation

**Q.** Find the HCF and LCM of 72, 108 and 180.

**Step 1 — Factorise each number.**
$$72 = 2^3 \times 3^2$$
$$108 = 2^2 \times 3^3$$
$$180 = 2^2 \times 3^2 \times 5$$

**Step 2 — HCF: lowest power of each COMMON prime.**
Common primes: 2 and 3.
- Lowest power of 2: 2²
- Lowest power of 3: 3²
$$\text{HCF} = 2^2 \times 3^2 = 36$$

**Step 3 — LCM: highest power of EVERY prime present.**
- Highest power of 2: 2³
- Highest power of 3: 3³
- Highest power of 5: 5¹
$$\text{LCM} = 2^3 \times 3^3 \times 5 = 8 \times 27 \times 5 = 1{,}080$$

**Answer: HCF = 36, LCM = 1,080**

> **Memory aid:** **H**CF takes the **L**owest; **L**CM takes the **H**ighest. (The letters swap — a useful reminder that the two rules are opposites.)

---

### Example 2 — The HCF × LCM identity

**Q.** The HCF of two numbers is 15 and their LCM is 300. If one number is 60, find the other.

**Step 1 — Apply the identity.**
$$\text{HCF} \times \text{LCM} = a \times b$$
$$15 \times 300 = 60 \times b$$

**Step 2 — Solve.**
$$b = \frac{4{,}500}{60} = 75$$

**Verification:**
- HCF(60, 75): 60 = 2² × 3 × 5, 75 = 3 × 5² ⇒ HCF = 15 ✓
- LCM(60, 75) = 2² × 3 × 5² = 300 ✓

**Answer: 75**

---

### Example 3 — Type A remainder (LCM-based)

**Q.** Find the least number which, when divided by 8, 12 and 20, leaves a remainder of 5 in each case.

**Step 1 — Recognise the type.** The remainder is **stated and identical** ⇒ LCM method.

**Step 2 — Compute the LCM.**
$$8 = 2^3, \quad 12 = 2^2 \times 3, \quad 20 = 2^2 \times 5$$
$$\text{LCM} = 2^3 \times 3 \times 5 = 120$$

**Step 3 — Add the remainder.**
$$N = 120k + 5$$

**Step 4 — Take the smallest positive case (k = 1).**
$$N = 125$$

**Verification:**
- 125 ÷ 8 = 15 remainder 5 ✓
- 125 ÷ 12 = 10 remainder 5 ✓
- 125 ÷ 20 = 6 remainder 5 ✓

**Answer: 125**

> **Note on k:** k = 0 gives N = 5, which technically leaves remainder 5 when divided by 8, 12 and 20 — but questions of this type intend a number *greater* than all the divisors. Take k = 1 unless the question says otherwise.

---

### Example 4 — Type B remainder (HCF of differences)

**Q.** Find the greatest number that divides 258, 323 and 388, leaving the same remainder in each case.

**Step 1 — Recognise the type.** The remainder is the **same but unstated** ⇒ HCF of differences.

**Step 2 — Compute the pairwise differences.**
$$323 - 258 = 65$$
$$388 - 323 = 65$$
$$388 - 258 = 130$$

**Step 3 — Take the HCF.**
$$\text{HCF}(65, 65, 130) = 65$$

**Verification:**
- 258 = 65 × 3 + 63
- 323 = 65 × 4 + 63
- 388 = 65 × 5 + 63

Remainder is **63** in every case ✓

**Answer: 65**

> **Why differences work:** if N = dq₁ + r and M = dq₂ + r, then M − N = d(q₂ − q₁) — the remainder cancels out, so *d* must divide the difference exactly.

---

### Example 5 — Unit digit of a large power

**Q.** Find the unit digit of 13⁴⁷.

**Step 1 — Only the last digit of the base matters.**
The base ends in **3**.

**Step 2 — Recall the cycle for 3.**
$$3^1 = 3, \quad 3^2 = 9, \quad 3^3 = 27 \to 7, \quad 3^4 = 81 \to 1$$
Cycle: **(3, 9, 7, 1)**, length 4.

**Step 3 — Reduce the exponent modulo 4.**
$$47 \div 4 = 11 \text{ remainder } 3$$

**Step 4 — Take the 3rd element of the cycle.**
$$\text{Unit digit} = 7$$

**Answer: 7**

> **Remainder 0 means the LAST element**, not the first. For example 3⁴⁰: 40 mod 4 = 0 ⇒ take the 4th element ⇒ unit digit **1**.

---

### Example 6 — Number of factors and their sum

**Q.** How many factors does 720 have? Also find the sum of all its factors.

**Step 1 — Prime factorisation.**
$$720 = 16 \times 45 = 2^4 \times 3^2 \times 5^1$$

**Step 2 — Number of factors.**
$$(4+1)(2+1)(1+1) = 5 \times 3 \times 2 = 30$$

**Step 3 — Sum of factors.**
$$\left(\frac{2^5-1}{2-1}\right)\left(\frac{3^3-1}{3-1}\right)\left(\frac{5^2-1}{5-1}\right)$$
$$= \left(\frac{31}{1}\right)\left(\frac{26}{2}\right)\left(\frac{24}{4}\right) = 31 \times 13 \times 6 = 2{,}418$$

**Alternative form of the sum** (often easier mentally):
$$(1+2+4+8+16)(1+3+9)(1+5) = 31 \times 13 \times 6 = 2{,}418$$

**Answer: 30 factors; sum = 2,418**

---

### Example 7 — Trailing zeros in a factorial

**Q.** How many zeros are there at the end of 50!?

**Step 1 — Understand the source of trailing zeros.**
Each trailing zero requires a factor of 10 = 2 × 5. Factorials always contain far more 2s than 5s, so the number of zeros equals the **number of 5s**.

**Step 2 — Count the powers of 5.**
$$\left\lfloor\frac{50}{5}\right\rfloor = 10 \quad \text{(multiples of 5)}$$
$$\left\lfloor\frac{50}{25}\right\rfloor = 2 \quad \text{(multiples of 25, which contribute a SECOND 5 each)}$$
$$\left\lfloor\frac{50}{125}\right\rfloor = 0$$

**Step 3 — Sum.**
$$10 + 2 + 0 = 12$$

**Answer: 12 zeros**

> **Why the second term is needed:** 25 = 5², 50 = 2 × 5². These numbers each supply *two* fives, not one — the ⌊n/25⌋ term catches the extra one.

---

### Example 8 — Successive division

**Q.** A number, when successively divided by 4, 5 and 6, leaves remainders 1, 2 and 3 respectively. Find the smallest such number.

**Step 1 — Understand "successively".**
The **quotient** of each division becomes the dividend of the next:
```
N  ÷ 4  →  quotient a, remainder 1
a  ÷ 5  →  quotient b, remainder 2
b  ÷ 6  →  quotient c, remainder 3
```

**Step 2 — Work backwards, taking the final quotient as 0 (for the smallest N).**

$$c = 0 \implies b = 6(0) + 3 = 3$$
$$a = 5(3) + 2 = 17$$
$$N = 4(17) + 1 = 69$$

**Verification:**
- 69 ÷ 4 = 17 remainder **1** ✓
- 17 ÷ 5 = 3 remainder **2** ✓
- 3 ÷ 6 = 0 remainder **3** ✓

**Answer: 69**

> **Do not confuse this with ordinary division.** "Successively divided" chains the quotients; "divided by 4, 5 and 6" (without "successively") means each divides the *original* number, which is an LCM problem instead.

---

## 6. Practice Questions

**Instructions:** 50 questions. Easy (1–20), Medium (21–40), Hard (41–50).
Target times: Easy 30 s · Medium 60 s · Hard 90 s.
Full solutions in [Section 7](#7-detailed-solutions).

### 🟢 EASY (Questions 1–20)

**Q1.** Find the HCF of 24 and 36.
(a) 6  (b) 8  (c) 12  (d) 18

**Q2.** Find the LCM of 12 and 18.
(a) 24  (b) 36  (c) 48  (d) 72

**Q3.** Find the HCF of 48 and 60.
(a) 6  (b) 8  (c) 12  (d) 24

**Q4.** Find the LCM of 8, 12 and 16.
(a) 24  (b) 36  (c) 48  (d) 96

**Q5.** The product of two numbers is 144 and their HCF is 6. Find their LCM.
(a) 18  (b) 20  (c) 24  (d) 36

**Q6.** What is the unit digit of 7⁴?
(a) 1  (b) 3  (c) 7  (d) 9

**Q7.** Find the smallest number exactly divisible by 12, 15 and 20.
(a) 40  (b) 50  (c) 60  (d) 120

**Q8.** Which of the following is true of 143?
(a) It is prime  (b) It is 11 × 13  (c) It is 7 × 21  (d) It is 3 × 47

**Q9.** Find the sum of the first 20 natural numbers.
(a) 190  (b) 200  (c) 210  (d) 220

**Q10.** Find the remainder when 17 is divided by 5.
(a) 1  (b) 2  (c) 3  (d) 4

**Q11.** Find the HCF of 18 and 24.
(a) 3  (b) 6  (c) 9  (d) 12

**Q12.** How many prime numbers are there between 1 and 20?
(a) 6  (b) 7  (c) 8  (d) 9

**Q13.** Find the LCM of 6 and 9.
(a) 12  (b) 18  (c) 24  (d) 54

**Q14.** Find the unit digit of 2¹⁰.
(a) 2  (b) 4  (c) 6  (d) 8

**Q15.** What is the largest three-digit number divisible by 7?
(a) 987  (b) 991  (c) 994  (d) 997

**Q16.** Find the sum of the squares of the first 10 natural numbers.
(a) 285  (b) 355  (c) 385  (d) 405

**Q17.** Find the HCF of the fractions 3/4 and 5/6.
(a) 1/2  (b) 1/6  (c) 1/12  (d) 1/24

**Q18.** Which of the following is divisible by 9?
(a) 234  (b) 235  (c) 236  (d) 237

**Q19.** The three-digit number 5A2 is divisible by 3. Find the least possible value of A.
(a) 0  (b) 1  (c) 2  (d) 3

**Q20.** Find the LCM of 15 and 25.
(a) 45  (b) 60  (c) 75  (d) 150

---

### 🟡 MEDIUM (Questions 21–40)

**Q21.** Find the greatest number that divides 43, 91 and 183, leaving the same remainder in each case.
(a) 4  (b) 7  (c) 9  (d) 13

**Q22.** Find the least number which, when divided by 5, 6, 7 and 8, leaves a remainder of 3, but which is exactly divisible by 9.
(a) 1,043  (b) 1,443  (c) 1,683  (d) 2,523

**Q23.** Find the unit digit of 7¹⁰⁵.
(a) 1  (b) 3  (c) 7  (d) 9

**Q24.** The HCF and LCM of two numbers are 12 and 336 respectively. If one number is 84, find the other.
(a) 36  (b) 42  (c) 48  (d) 56

**Q25.** Find the least number which, when divided by 6, 7 and 8, leaves a remainder of 3 in each case.
(a) 165  (b) 168  (c) 171  (d) 175

**Q26.** Find the remainder when 2³¹ is divided by 5.
(a) 1  (b) 2  (c) 3  (d) 4

**Q27.** How many numbers between 100 and 300 are divisible by 7?
(a) 26  (b) 27  (c) 28  (d) 29

**Q28.** Find the greatest four-digit number divisible by 15, 25 and 40.
(a) 9,000  (b) 9,600  (c) 9,750  (d) 9,900

**Q29.** When a number is divided by 296, the remainder is 75. What is the remainder when the same number is divided by 37?
(a) 1  (b) 2  (c) 8  (d) 11

**Q30.** How many factors does 360 have?
(a) 18  (b) 20  (c) 24  (d) 30

**Q31.** Find the sum of all the factors of 60.
(a) 144  (b) 156  (c) 168  (d) 180

**Q32.** What is the smallest number that must be added to 1,056 to make it exactly divisible by 23?
(a) 1  (b) 2  (c) 3  (d) 21

**Q33.** Find the LCM of the fractions 2/3, 4/9 and 8/27.
(a) 2/27  (b) 8/27  (c) 8/3  (d) 16/3

**Q34.** How many zeros are there at the end of 25!?
(a) 4  (b) 5  (c) 6  (d) 7

**Q35.** The sum of two numbers is 528 and their HCF is 33. How many such pairs of numbers are possible?
(a) 2  (b) 3  (c) 4  (d) 6

**Q36.** Find the remainder when 3⁴⁰ is divided by 7.
(a) 1  (b) 2  (c) 4  (d) 6

**Q37.** Find the HCF of 1.08, 0.36 and 0.9.
(a) 0.03  (b) 0.09  (c) 0.18  (d) 0.36

**Q38.** A number, when divided by 342, leaves a remainder of 47. What is the remainder when the same number is divided by 19?
(a) 5  (b) 7  (c) 9  (d) 11

**Q39.** Find the largest number that divides 62, 132 and 237, leaving the same remainder in each case.
(a) 25  (b) 30  (c) 35  (d) 40

**Q40.** Find the unit digit of 3⁴⁵ × 7³².
(a) 1  (b) 3  (c) 7  (d) 9

---

### 🔴 HARD (Questions 41–50)

**Q41.** Find the least number which, when divided by 12, 15, 20 and 54, leaves a remainder of 8 in each case.
(a) 428  (b) 488  (c) 548  (d) 638

**Q42.** How many zeros are there at the end of 100!?
(a) 20  (b) 22  (c) 24  (d) 25

**Q43.** Find the remainder when 7¹⁰⁰ is divided by 100.
(a) 1  (b) 7  (c) 43  (d) 49

**Q44.** The HCF of two numbers is 11 and their LCM is 693. If one number is 77, find the other.
(a) 88  (b) 99  (c) 121  (d) 143

**Q45.** Find the smallest number which, when increased by 5, becomes exactly divisible by 24, 32, 36 and 54.
(a) 859  (b) 869  (c) 1,723  (d) 1,733

**Q46.** How many factors of 1,080 are perfect squares?
(a) 3  (b) 4  (c) 6  (d) 8

**Q47.** Find the remainder when 15²³ + 23²³ is divided by 19.
(a) 0  (b) 1  (c) 9  (d) 18

**Q48.** Find the largest number that divides 1,305, 4,665 and 6,905, leaving the same remainder in each case.
(a) 1,020  (b) 1,120  (c) 1,220  (d) 1,320

**Q49.** A number, when successively divided by 3, 4 and 7, leaves remainders 2, 1 and 4 respectively. Find the smallest such number.
(a) 43  (b) 53  (c) 63  (d) 73

**Q50.** Find the sum of the first 25 odd natural numbers and the sum of the first 25 even natural numbers.
(a) 600 and 625  (b) 625 and 650  (c) 650 and 675  (d) 625 and 675

---

## 7. Detailed Solutions

### 🟢 EASY — Solutions 1–20

---

**Q1. HCF of 24 and 36. → (c) 12**

**Method — prime factorisation.**
$$24 = 2^3 \times 3, \qquad 36 = 2^2 \times 3^2$$

**HCF = lowest power of each common prime:**
$$2^2 \times 3^1 = 12$$

**Answer: (c) 12**

---

**Q2. LCM of 12 and 18. → (b) 36**

$$12 = 2^2 \times 3, \qquad 18 = 2 \times 3^2$$

**LCM = highest power of every prime:**
$$2^2 \times 3^2 = 36$$

**Identity check:** HCF(12,18) = 6, and 6 × 36 = 216 = 12 × 18 ✓

**Answer: (b) 36**

---

**Q3. HCF of 48 and 60. → (c) 12**

$$48 = 2^4 \times 3, \qquad 60 = 2^2 \times 3 \times 5$$
$$\text{HCF} = 2^2 \times 3 = 12$$

**Answer: (c) 12**

---

**Q4. LCM of 8, 12, 16. → (c) 48**

$$8 = 2^3, \qquad 12 = 2^2 \times 3, \qquad 16 = 2^4$$
$$\text{LCM} = 2^4 \times 3 = 48$$

**Check:** 48 ÷ 8 = 6 ✓, 48 ÷ 12 = 4 ✓, 48 ÷ 16 = 3 ✓

**Answer: (c) 48**

---

**Q5. Product 144, HCF 6. LCM? → (c) 24**

**Formula used:** HCF × LCM = product of the numbers

$$6 \times \text{LCM} = 144 \implies \text{LCM} = 24$$

*(The numbers would be 6 and 24, or 12 and 12 — but the LCM is determined regardless.)*

**Answer: (c) 24**

---

**Q6. Unit digit of 7⁴. → (a) 1**

**Cycle for 7:** 7, 9, 3, 1 (length 4)

$$7^4 = 2401 \implies \text{unit digit} = 1$$

**Answer: (a) 1**

---

**Q7. Smallest number divisible by 12, 15 and 20. → (c) 60**

This is the LCM.
$$12 = 2^2 \times 3, \quad 15 = 3 \times 5, \quad 20 = 2^2 \times 5$$
$$\text{LCM} = 2^2 \times 3 \times 5 = 60$$

**Answer: (c) 60**

---

**Q8. What is true of 143? → (b) It is 11 × 13**

**Test for primality.** √143 ≈ 11.96, so test primes up to 11: 2, 3, 5, 7, 11.
- Not even ⇒ not divisible by 2
- Digit sum 1+4+3 = 8 ⇒ not divisible by 3
- Doesn't end in 0 or 5 ⇒ not divisible by 5
- 143 ÷ 7 = 20.43 ⇒ no
- **143 ÷ 11 = 13** ✓

$$143 = 11 \times 13 \implies \text{composite}$$

**Answer: (b) It is 11 × 13**

---

**Q9. Sum of the first 20 natural numbers. → (c) 210**

**Formula used:** n(n+1)/2

$$\frac{20 \times 21}{2} = 210$$

**Answer: (c) 210**

---

**Q10. Remainder when 17 ÷ 5. → (b) 2**

$$17 = 5 \times 3 + 2$$

**Answer: (b) 2**

---

**Q11. HCF of 18 and 24. → (b) 6**

$$18 = 2 \times 3^2, \qquad 24 = 2^3 \times 3$$
$$\text{HCF} = 2 \times 3 = 6$$

**Answer: (b) 6**

---

**Q12. Primes between 1 and 20. → (c) 8**

$$2, \; 3, \; 5, \; 7, \; 11, \; 13, \; 17, \; 19$$

That is **8** primes.

> **Note:** 1 is *not* prime — it has only one factor. Including it would give the wrong answer of 9.

**Answer: (c) 8**

---

**Q13. LCM of 6 and 9. → (b) 18**

$$6 = 2 \times 3, \qquad 9 = 3^2$$
$$\text{LCM} = 2 \times 3^2 = 18$$

**Answer: (b) 18**

---

**Q14. Unit digit of 2¹⁰. → (b) 4**

**Cycle for 2:** 2, 4, 8, 6 (length 4)

$$10 \div 4 = 2 \text{ remainder } 2$$

Take the **2nd** element of the cycle:
$$\text{Unit digit} = 4$$

**Check:** 2¹⁰ = 1,024 ✓

**Answer: (b) 4**

---

**Q15. Largest three-digit number divisible by 7. → (c) 994**

$$\frac{999}{7} = 142.71 \implies \text{take } 142$$
$$7 \times 142 = 994$$

**Check:** 994 + 7 = 1,001 (four digits) ⇒ 994 is the largest ✓

**Answer: (c) 994**

---

**Q16. Sum of squares of the first 10 naturals. → (c) 385**

**Formula used:** n(n+1)(2n+1)/6

$$\frac{10 \times 11 \times 21}{6} = \frac{2310}{6} = 385$$

**Answer: (c) 385**

---

**Q17. HCF of 3/4 and 5/6. → (c) 1/12**

**Formula used:** HCF of fractions = HCF(numerators) / LCM(denominators)

$$= \frac{\text{HCF}(3,5)}{\text{LCM}(4,6)} = \frac{1}{12}$$

**Answer: (c) 1/12**

---

**Q18. Which is divisible by 9? → (a) 234**

**Rule:** digit sum must be divisible by 9.

| Number | Digit sum | ÷ 9? |
|---|---|---|
| 234 | 9 | ✓ |
| 235 | 10 | ✗ |
| 236 | 11 | ✗ |
| 237 | 12 | ✗ |

**Check:** 234 = 9 × 26 ✓

**Answer: (a) 234**

---

**Q19. 5A2 divisible by 3. Least A? → (c) 2**

**Rule:** digit sum divisible by 3.

$$5 + A + 2 = 7 + A$$

We need 7 + A to be a multiple of 3:
- A = 0 ⇒ 7 ✗
- A = 1 ⇒ 8 ✗
- **A = 2 ⇒ 9 ✓**

**Check:** 522 = 3 × 174 ✓

**Answer: (c) 2**

---

**Q20. LCM of 15 and 25. → (c) 75**

$$15 = 3 \times 5, \qquad 25 = 5^2$$
$$\text{LCM} = 3 \times 5^2 = 75$$

**Answer: (c) 75**

---

### 🟡 MEDIUM — Solutions 21–40

---

**Q21. Greatest number dividing 43, 91, 183 with the same remainder. → (a) 4**

**Type B: same but unstated remainder ⇒ HCF of differences.**

**Step 1 — Compute the pairwise differences.**
$$91 - 43 = 48$$
$$183 - 91 = 92$$
$$183 - 43 = 140$$

**Step 2 — Find the HCF.**
$$48 = 2^4 \times 3$$
$$92 = 2^2 \times 23$$
$$140 = 2^2 \times 5 \times 7$$
$$\text{HCF} = 2^2 = 4$$

**Verification:**
- 43 = 4 × 10 + **3**
- 91 = 4 × 22 + **3**
- 183 = 4 × 45 + **3**

Same remainder of 3 throughout ✓

**Answer: (a) 4**

---

**Q22. Least number leaving remainder 3 when divided by 5, 6, 7, 8, but divisible by 9. → (c) 1,683**

**Step 1 — Handle the "remainder 3" condition (Type A).**
$$\text{LCM}(5,6,7,8) = 840$$
$$N = 840k + 3$$

**Step 2 — Impose the divisibility-by-9 condition.**
$$840k + 3 \equiv 0 \pmod 9$$

**Step 3 — Reduce 840 modulo 9.**
Digit sum of 840 = 8 + 4 + 0 = 12 ⇒ 12 mod 9 = **3**.
$$3k + 3 \equiv 0 \pmod 9$$
$$3(k+1) \equiv 0 \pmod 9 \implies k + 1 \equiv 0 \pmod 3$$

**Step 4 — Find the smallest valid k.**
$$k = 2 \quad (\text{since } 2 + 1 = 3 \text{ is divisible by } 3)$$

**Step 5 — Compute N.**
$$N = 840(2) + 3 = 1{,}683$$

**Verification:**
- 1,683 ÷ 5 = 336 r 3 ✓ · ÷ 6 = 280 r 3 ✓ · ÷ 7 = 240 r 3 ✓ · ÷ 8 = 210 r 3 ✓
- 1,683 ÷ 9 = 187 exactly ✓ (digit sum 1+6+8+3 = 18, divisible by 9)

**Answer: (c) 1,683**

---

**Q23. Unit digit of 7¹⁰⁵. → (c) 7**

**Step 1 — Cycle for 7:** 7, 9, 3, 1 (length 4)

**Step 2 — Reduce the exponent modulo 4.**
$$105 \div 4 = 26 \text{ remainder } 1$$

**Step 3 — Take the 1st element.**
$$\text{Unit digit} = 7$$

**Answer: (c) 7**

---

**Q24. HCF 12, LCM 336, one number 84. Other? → (c) 48**

**Formula used:** HCF × LCM = a × b

$$12 \times 336 = 84 \times b$$
$$b = \frac{4{,}032}{84} = 48$$

**Verification:**
- 84 = 2² × 3 × 7, 48 = 2⁴ × 3
- HCF = 2² × 3 = 12 ✓
- LCM = 2⁴ × 3 × 7 = 336 ✓

**Answer: (c) 48**

---

**Q25. Least number leaving remainder 3 when divided by 6, 7, 8. → (c) 171**

**Type A: stated identical remainder ⇒ LCM + r.**

**Step 1 — Compute the LCM.**
$$6 = 2 \times 3, \quad 7 = 7, \quad 8 = 2^3$$
$$\text{LCM} = 2^3 \times 3 \times 7 = 168$$

**Step 2 — Add the remainder.**
$$N = 168 + 3 = 171$$

**Verification:** 171 ÷ 6 = 28 r 3 ✓ · ÷ 7 = 24 r 3 ✓ · ÷ 8 = 21 r 3 ✓

**Answer: (c) 171**

---

**Q26. Remainder when 2³¹ ÷ 5. → (c) 3**

**Step 1 — Use the unit digit (fastest route for divisor 5).**
Cycle for 2: 2, 4, 8, 6.
$$31 \div 4 = 7 \text{ remainder } 3 \implies \text{3rd element} = 8$$

**Step 2 — The remainder mod 5 depends only on the last digit.**
$$8 \bmod 5 = 3$$

**Cross-check with a remainder cycle:**
$$2^1 \equiv 2, \; 2^2 \equiv 4, \; 2^3 \equiv 3, \; 2^4 \equiv 1 \pmod 5 \quad \text{(cycle length 4)}$$
$$31 \bmod 4 = 3 \implies 2^{31} \equiv 2^3 \equiv 3 \pmod 5 \checkmark$$

**Answer: (c) 3**

---

**Q27. Numbers between 100 and 300 divisible by 7. → (c) 28**

**Step 1 — Find the first multiple ≥ 100.**
$$7 \times 15 = 105$$

**Step 2 — Find the last multiple ≤ 300.**
$$7 \times 42 = 294$$

**Step 3 — Count the multiples from the 15th to the 42nd.**
$$42 - 15 + 1 = 28$$

**Formula check:**
$$\left\lfloor\frac{300}{7}\right\rfloor - \left\lfloor\frac{99}{7}\right\rfloor = 42 - 14 = 28 \checkmark$$

**Answer: (c) 28**

---

**Q28. Greatest four-digit number divisible by 15, 25 and 40. → (b) 9,600**

**Step 1 — Compute the LCM.**
$$15 = 3 \times 5, \quad 25 = 5^2, \quad 40 = 2^3 \times 5$$
$$\text{LCM} = 2^3 \times 3 \times 5^2 = 600$$

**Step 2 — Find the largest multiple of 600 below 10,000.**
$$\frac{9{,}999}{600} = 16.66 \implies \text{take } 16$$
$$600 \times 16 = 9{,}600$$

**Verification:** 9,600 ÷ 15 = 640 ✓ · ÷ 25 = 384 ✓ · ÷ 40 = 240 ✓
And 600 × 17 = 10,200 — five digits ⇒ 9,600 is the largest ✓

**Answer: (b) 9,600**

---

**Q29. Divided by 296 leaves 75. Remainder when divided by 37? → (a) 1**

**Step 1 — Check whether 37 divides 296.**
$$296 = 37 \times 8 \checkmark$$

**Step 2 — Express the number.**
$$N = 296k + 75$$

Since 296k is a multiple of 37, it contributes nothing to the remainder.

**Step 3 — Reduce the remainder modulo 37.**
$$75 \bmod 37 = 75 - 74 = 1$$

**Answer: (a) 1**

> **The shortcut:** whenever the smaller divisor is a factor of the larger, simply reduce the *given remainder* modulo the smaller divisor.

---

**Q30. Number of factors of 360. → (c) 24**

**Step 1 — Prime factorisation.**
$$360 = 8 \times 45 = 2^3 \times 3^2 \times 5^1$$

**Step 2 — Apply the formula (a+1)(b+1)(c+1).**
$$(3+1)(2+1)(1+1) = 4 \times 3 \times 2 = 24$$

**Answer: (c) 24**

---

**Q31. Sum of all factors of 60. → (c) 168**

**Step 1 — Prime factorisation.**
$$60 = 2^2 \times 3 \times 5$$

**Step 2 — Apply the sum-of-factors formula.**
$$(1 + 2 + 4)(1 + 3)(1 + 5) = 7 \times 4 \times 6 = 168$$

**Verification by listing:** 1 + 2 + 3 + 4 + 5 + 6 + 10 + 12 + 15 + 20 + 30 + 60
$$= 168 \checkmark$$
*(60 has (2+1)(1+1)(1+1) = 12 factors — all listed above.)*

**Answer: (c) 168**

---

**Q32. Smallest number to add to 1,056 for divisibility by 23. → (b) 2**

**Step 1 — Divide.**
$$\frac{1056}{23} = 45 \text{ remainder } 21$$
*(Since 23 × 45 = 1,035 and 1,056 − 1,035 = 21.)*

**Step 2 — Compute what is needed to reach the next multiple.**
$$23 - 21 = 2$$

**Verification:** 1,056 + 2 = 1,058 = 23 × 46 ✓

**Answer: (b) 2**

---

**Q33. LCM of 2/3, 4/9, 8/27. → (c) 8/3**

**Formula used:** LCM of fractions = LCM(numerators) / HCF(denominators)

$$= \frac{\text{LCM}(2, 4, 8)}{\text{HCF}(3, 9, 27)} = \frac{8}{3}$$

**Verification:** 8/3 divided by each fraction should give a whole number:
$$\frac{8/3}{2/3} = 4 \checkmark \qquad \frac{8/3}{4/9} = 6 \checkmark \qquad \frac{8/3}{8/27} = 9 \checkmark$$

**Answer: (c) 8/3**

---

**Q34. Zeros at the end of 25!. → (c) 6**

**Formula used:** count the factors of 5.

$$\left\lfloor\frac{25}{5}\right\rfloor + \left\lfloor\frac{25}{25}\right\rfloor = 5 + 1 = 6$$

**Explanation of the two terms:**
- Five multiples of 5 (5, 10, 15, 20, 25) each contribute at least one 5
- 25 = 5² contributes a **second** 5, caught by the ⌊25/25⌋ term

**Answer: (c) 6**

---

**Q35. Sum 528, HCF 33. Number of possible pairs? → (c) 4**

**Step 1 — Express the numbers using the HCF.**
Let the numbers be 33*a* and 33*b*, where **a and b are co-prime**.

**Step 2 — Use the sum condition.**
$$33(a + b) = 528 \implies a + b = 16$$

**Step 3 — List the co-prime pairs summing to 16.**

| Pair (a, b) | HCF | Valid? |
|---|---|---|
| (1, 15) | 1 | ✓ |
| (2, 14) | 2 | ✗ |
| (3, 13) | 1 | ✓ |
| (4, 12) | 4 | ✗ |
| (5, 11) | 1 | ✓ |
| (6, 10) | 2 | ✗ |
| (7, 9) | 1 | ✓ |
| (8, 8) | 8 | ✗ |

**Step 4 — Count.**
Four valid pairs: **(33, 495), (99, 429), (165, 363), (231, 297)**

**Answer: (c) 4**

> **Why co-primality is required:** if a and b shared a factor *k*, the actual HCF would be 33k, not 33.

---

**Q36. Remainder when 3⁴⁰ ÷ 7. → (c) 4**

**Step 1 — Build the remainder cycle of powers of 3 modulo 7.**

| Power | Value | mod 7 |
|---|---|---|
| 3¹ | 3 | 3 |
| 3² | 9 | 2 |
| 3³ | 27 | 6 |
| 3⁴ | 81 | 4 |
| 3⁵ | 243 | 5 |
| 3⁶ | 729 | **1** ← cycle closes |

Cycle length = **6**.

**Step 2 — Reduce the exponent modulo 6.**
$$40 \div 6 = 6 \text{ remainder } 4$$

**Step 3 — Read off the 4th entry.**
$$3^{40} \equiv 3^4 \equiv 4 \pmod 7$$

**Answer: (c) 4**

---

**Q37. HCF of 1.08, 0.36 and 0.9. → (c) 0.18**

**Step 1 — Convert to whole numbers with a common number of decimal places.**
$$1.08 \to 108, \qquad 0.36 \to 36, \qquad 0.90 \to 90$$
*(All expressed in hundredths.)*

**Step 2 — Find the HCF of the integers.**
$$108 = 2^2 \times 3^3, \qquad 36 = 2^2 \times 3^2, \qquad 90 = 2 \times 3^2 \times 5$$
$$\text{HCF} = 2 \times 3^2 = 18$$

**Step 3 — Convert back (divide by 100).**
$$\text{HCF} = 0.18$$

**Verification:** 1.08/0.18 = 6 ✓ · 0.36/0.18 = 2 ✓ · 0.9/0.18 = 5 ✓

**Answer: (c) 0.18**

---

**Q38. Divided by 342 leaves 47. Remainder when divided by 19? → (c) 9**

**Step 1 — Check the factor relationship.**
$$342 = 19 \times 18 \checkmark$$

**Step 2 — Express the number.**
$$N = 342k + 47$$

342k is a multiple of 19, so only the remainder matters.

**Step 3 — Reduce 47 modulo 19.**
$$47 - 38 = 9$$

**Answer: (c) 9**

---

**Q39. Largest number dividing 62, 132, 237 with the same remainder. → (c) 35**

**Type B ⇒ HCF of differences.**

**Step 1 — Compute the differences.**
$$132 - 62 = 70$$
$$237 - 132 = 105$$
$$237 - 62 = 175$$

**Step 2 — HCF.**
$$70 = 2 \times 5 \times 7$$
$$105 = 3 \times 5 \times 7$$
$$175 = 5^2 \times 7$$
$$\text{HCF} = 5 \times 7 = 35$$

**Verification:**
- 62 = 35 × 1 + **27**
- 132 = 35 × 3 + **27**
- 237 = 35 × 6 + **27** ✓

**Answer: (c) 35**

---

**Q40. Unit digit of 3⁴⁵ × 7³². → (b) 3**

**Step 1 — Unit digit of 3⁴⁵.**
Cycle for 3: 3, 9, 7, 1.
$$45 \div 4 = 11 \text{ remainder } 1 \implies \text{1st element} = 3$$

**Step 2 — Unit digit of 7³².**
Cycle for 7: 7, 9, 3, 1.
$$32 \div 4 = 8 \text{ remainder } 0 \implies \text{4th (last) element} = 1$$

**Step 3 — Multiply the unit digits.**
$$3 \times 1 = 3$$

**Answer: (b) 3**

> **The key subtlety:** a remainder of **0** means take the **last** element of the cycle, not the first.

---

### 🔴 HARD — Solutions 41–50

---

**Q41. Least number leaving remainder 8 when divided by 12, 15, 20, 54. → (c) 548**

**Type A ⇒ LCM + r.**

**Step 1 — Factorise each divisor.**
$$12 = 2^2 \times 3$$
$$15 = 3 \times 5$$
$$20 = 2^2 \times 5$$
$$54 = 2 \times 3^3$$

**Step 2 — Compute the LCM (highest power of each prime).**
- Highest power of 2: 2²
- Highest power of 3: 3³
- Highest power of 5: 5¹

$$\text{LCM} = 4 \times 27 \times 5 = 540$$

**Step 3 — Add the remainder.**
$$N = 540 + 8 = 548$$

**Verification:**
- 548 ÷ 12 = 45 remainder 8 ✓
- 548 ÷ 15 = 36 remainder 8 ✓
- 548 ÷ 20 = 27 remainder 8 ✓
- 548 ÷ 54 = 10 remainder 8 ✓

**Answer: (c) 548**

---

**Q42. Zeros at the end of 100!. → (c) 24**

**Formula used:** $\sum \lfloor n/5^i \rfloor$

$$\left\lfloor\frac{100}{5}\right\rfloor = 20$$
$$\left\lfloor\frac{100}{25}\right\rfloor = 4$$
$$\left\lfloor\frac{100}{125}\right\rfloor = 0$$

$$\text{Total} = 20 + 4 + 0 = 24$$

**Interpretation of the terms:**
- 20 multiples of 5 each supply at least one factor of 5
- 4 multiples of 25 (25, 50, 75, 100) each supply a **second** 5

**Answer: (c) 24**

> **Common error:** answering 20 by stopping after the first term. Every multiple of 25 contributes an extra 5 that the first term misses.

---

**Q43. Remainder when 7¹⁰⁰ ÷ 100. → (a) 1**

**Step 1 — Build the cycle of the last two digits of powers of 7.**

| Power | Value | Last two digits |
|---|---|---|
| 7¹ | 7 | 07 |
| 7² | 49 | 49 |
| 7³ | 343 | 43 |
| 7⁴ | 2,401 | **01** ← cycle closes |

Cycle length = **4**.

**Step 2 — Reduce the exponent modulo 4.**
$$100 \div 4 = 25 \text{ remainder } 0$$

A remainder of 0 means we land on the **last** element of the cycle, i.e. 7⁴ ≡ 01.

**Step 3 — Conclude.**
$$7^{100} = (7^4)^{25} \equiv 1^{25} \equiv 1 \pmod{100}$$

**Answer: (a) 1**

> **General principle:** to find a remainder modulo *m* for a huge power, build the cycle of remainders. Here 7⁴ ≡ 1 (mod 100) makes every exponent that is a multiple of 4 collapse to 1.

---

**Q44. HCF 11, LCM 693, one number 77. Other? → (b) 99**

**Formula used:** HCF × LCM = a × b

$$11 \times 693 = 77 \times b$$
$$b = \frac{7{,}623}{77} = 99$$

**Verification:**
- 77 = 7 × 11, 99 = 3² × 11
- HCF = 11 ✓
- LCM = 3² × 7 × 11 = 693 ✓

**Answer: (b) 99**

---

**Q45. Smallest number which, when increased by 5, is divisible by 24, 32, 36 and 54. → (a) 859**

**Step 1 — Factorise the divisors.**
$$24 = 2^3 \times 3$$
$$32 = 2^5$$
$$36 = 2^2 \times 3^2$$
$$54 = 2 \times 3^3$$

**Step 2 — Compute the LCM.**
- Highest power of 2: 2⁵ = 32
- Highest power of 3: 3³ = 27

$$\text{LCM} = 32 \times 27 = 864$$

**Step 3 — Reverse the "+5".**
The number *plus 5* equals 864, so:
$$N = 864 - 5 = 859$$

**Verification:** 859 + 5 = 864.
- 864 ÷ 24 = 36 ✓ · ÷ 32 = 27 ✓ · ÷ 36 = 24 ✓ · ÷ 54 = 16 ✓

**Answer: (a) 859**

> **Read the direction carefully.** "Increased by 5 becomes divisible" ⇒ subtract 5 from the LCM. "Decreased by 5 becomes divisible" would mean adding 5.

---

**Q46. Factors of 1,080 that are perfect squares. → (b) 4**

**Step 1 — Prime factorisation.**
$$1{,}080 = 8 \times 135 = 2^3 \times 3^3 \times 5^1$$

**Step 2 — Understand the condition.**
A factor is a perfect square only if **every exponent in it is even**.

**Step 3 — Count the even-exponent choices for each prime.**

| Prime | Available exponents | Even choices | Count |
|---|---|---|---|
| 2 | 0, 1, 2, 3 | 0, 2 | 2 |
| 3 | 0, 1, 2, 3 | 0, 2 | 2 |
| 5 | 0, 1 | 0 | 1 |

**Step 4 — Multiply.**
$$2 \times 2 \times 1 = 4$$

**The four square factors, listed explicitly:**
$$2^0 3^0 = 1, \qquad 2^2 3^0 = 4, \qquad 2^0 3^2 = 9, \qquad 2^2 3^2 = 36$$

**Answer: (b) 4**

---

**Q47. Remainder when 15²³ + 23²³ ÷ 19. → (a) 0**

**Step 1 — Recall the identity.**
$$a^n + b^n \text{ is divisible by } (a + b) \text{ whenever } n \text{ is ODD}$$

**Step 2 — Check the conditions.**
$$a = 15, \quad b = 23, \quad n = 23 \; (\text{odd}) \checkmark$$
$$a + b = 15 + 23 = 38$$

**Step 3 — Conclude.**
So 15²³ + 23²³ is divisible by **38**. Since 38 = 2 × 19, it is also divisible by **19**.

$$\text{Remainder} = 0$$

**Answer: (a) 0**

> **Why the identity holds:** $a^n + b^n = (a+b)(a^{n-1} - a^{n-2}b + \cdots + b^{n-1})$ when *n* is odd. The alternating signs only close up correctly for odd exponents — for even *n* the factorisation fails (e.g. 2² + 3² = 13 is not divisible by 5).

---

**Q48. Largest number dividing 1,305, 4,665 and 6,905 with the same remainder. → (b) 1,120**

**Type B ⇒ HCF of differences.**

**Step 1 — Compute the pairwise differences.**
$$4{,}665 - 1{,}305 = 3{,}360$$
$$6{,}905 - 4{,}665 = 2{,}240$$
$$6{,}905 - 1{,}305 = 5{,}600$$

**Step 2 — Factorise each difference.**
$$3{,}360 = 2^5 \times 3 \times 5 \times 7$$
$$2{,}240 = 2^6 \times 5 \times 7$$
$$5{,}600 = 2^5 \times 5^2 \times 7$$

**Step 3 — Take the lowest power of each common prime.**
- 2: lowest power is 2⁵ = 32
- 5: lowest power is 5¹ = 5
- 7: lowest power is 7¹ = 7
- 3 does not appear in all three ⇒ excluded

$$\text{HCF} = 32 \times 5 \times 7 = 1{,}120$$

**Verification:**
- 1,305 = 1,120 × 1 + **185**
- 4,665 = 1,120 × 4 + **185**
- 6,905 = 1,120 × 6 + **185** ✓

**Answer: (b) 1,120**

---

**Q49. Successively divided by 3, 4, 7 leaving 2, 1, 4. Smallest number? → (b) 53**

**Step 1 — Understand "successively divided".**
Each division's **quotient** becomes the next dividend:
```
N ÷ 3  →  quotient a, remainder 2
a ÷ 4  →  quotient b, remainder 1
b ÷ 7  →  quotient c, remainder 4
```

**Step 2 — Work backwards, setting the final quotient to 0 for the smallest N.**

$$c = 0 \implies b = 7(0) + 4 = 4$$
$$a = 4(4) + 1 = 17$$
$$N = 3(17) + 2 = 53$$

**Verification:**
| Division | Quotient | Remainder |
|---|---|---|
| 53 ÷ 3 | 17 | **2** ✓ |
| 17 ÷ 4 | 4 | **1** ✓ |
| 4 ÷ 7 | 0 | **4** ✓ |

**Answer: (b) 53**

> **Do not treat this as an LCM problem.** "Successively divided" chains the quotients. If the question had said "when divided by 3, 4 and 7" (each dividing the *original* number), it would be an entirely different — and in this case unsolvable — problem.

---

**Q50. Sum of the first 25 odd numbers and the first 25 even numbers. → (b) 625 and 650**

**Step 1 — Sum of the first *n* odd numbers.**
$$\text{Formula: } n^2$$
$$25^2 = 625$$
*(The series is 1 + 3 + 5 + … + 49.)*

**Step 2 — Sum of the first *n* even numbers.**
$$\text{Formula: } n(n+1)$$
$$25 \times 26 = 650$$
*(The series is 2 + 4 + 6 + … + 50.)*

**Cross-check.** Together they are the first 50 natural numbers:
$$625 + 650 = 1{,}275 = \frac{50 \times 51}{2} \checkmark$$

Also note the even sum exceeds the odd sum by exactly 25 — one extra unit for each of the 25 pairs ✓

**Answer: (b) 625 and 650**

---

## 8. Quick Revision Sheet

> **One page. Read 48 hours after study, and again the night before the test.**

### Divisibility rules

```
2  → last digit even              8  → last THREE digits ÷ 8
3  → digit sum ÷ 3                9  → digit sum ÷ 9
4  → last TWO digits ÷ 4         10  → ends in 0
5  → ends in 0 or 5              11  → alternating digit sum ÷ 11 (or 0)
6  → passes 2 AND 3              25  → last two digits: 00/25/50/75
7  → double last digit, subtract from the rest; repeat
```

### HCF & LCM

```
HCF = product of LOWEST powers of COMMON primes
LCM = product of HIGHEST powers of ALL primes

HCF × LCM = a × b        ← TWO numbers only

HCF of fractions = HCF(numerators) / LCM(denominators)
LCM of fractions = LCM(numerators) / HCF(denominators)
```

### ⭐ Remainder decision tree

```
Remainder VALUE is stated, same for all divisors
     →  N = LCM × k + r

Different remainders, CONSTANT DEFICIT (divisor − remainder equal)
     →  N = LCM × k − d

Remainder is the same but UNSTATED
     →  HCF of the pairwise DIFFERENCES

Different STATED remainders, "greatest divisor"
     →  HCF of (number − its remainder)

Divisor is a FACTOR of a bigger divisor
     →  new remainder = old remainder MOD smaller divisor
```

### Unit digits (cyclicity)

```
0,1,5,6  →  always end in themselves
4        →  even exp → 6;  odd exp → 4
9        →  even exp → 1;  odd exp → 9
2        →  2,4,8,6      3  →  3,9,7,1
7        →  7,9,3,1      8  →  8,4,2,6

Exponent mod 4:  1→1st  2→2nd  3→3rd  0→LAST (4th)
```

### Factors

```
N = pᵃ qᵇ rᶜ

Number of factors        =  (a+1)(b+1)(c+1)
Sum of factors           =  (1+p+…+pᵃ)(1+q+…+qᵇ)…
Perfect-square factors   =  (⌊a/2⌋+1)(⌊b/2⌋+1)…
Product of all factors   =  N^(d(N)/2)

360 = 2³·3²·5  →  24 factors
60  = 2²·3·5   →  12 factors, sum 168
```

### Factorials

```
Trailing zeros in n!  =  ⌊n/5⌋ + ⌊n/25⌋ + ⌊n/125⌋ + …

    25!  → 5 + 1  = 6
    50!  → 10 + 2 = 12
   100!  → 20 + 4 = 24
```

### Series sums

```
1+2+…+n        =  n(n+1)/2
1+3+5+…        =  n²          (first n odd numbers)
2+4+6+…        =  n(n+1)      (first n even numbers)
1²+2²+…+n²     =  n(n+1)(2n+1)/6
1³+2³+…+n³     =  [n(n+1)/2]²
```

### Divisibility identities

```
aⁿ − bⁿ  divisible by (a − b)   for ALL n
aⁿ − bⁿ  divisible by (a + b)   for EVEN n
aⁿ + bⁿ  divisible by (a + b)   for ODD n
```

### Facts to have ready

```
Primes < 50 : 2 3 5 7 11 13 17 19 23 29 31 37 41 43 47   (15 of them)
Primes < 100: 25 of them
1 is NEITHER prime NOR composite.  2 is the ONLY even prime.

Squares:  11²=121  12²=144  13²=169  14²=196  15²=225
          16²=256  17²=289  18²=324  19²=361  25²=625
Cubes:    11³=1331  12³=1728  13³=2197  21³=9261

Count of multiples of k in [a,b] = ⌊b/k⌋ − ⌊(a−1)/k⌋
```

---

## 9. Common Mistakes

| # | Mistake | Example | Correction |
|---|---|---|---|
| 1 | **HCF/LCM rules swapped** | HCF takes highest powers | HCF = **lowest**; LCM = **highest** |
| 2 | **HCF × LCM used for 3 numbers** | HCF(2,3,4) × LCM = 2×3×4 | The identity holds for **two** numbers only |
| 3 | **Remainder type misidentified** | Using LCM when the remainder is unstated | Unstated ⇒ HCF of differences |
| 4 | **Cycle remainder 0 read as 1st element** | 7³² ⇒ unit digit 7 | Remainder 0 ⇒ **last** element ⇒ 1 |
| 5 | **1 counted as prime** | 9 primes below 20 | 1 is not prime ⇒ 8 primes |
| 6 | **Trailing zeros: only ⌊n/5⌋** | 100! ⇒ 20 zeros | Add ⌊n/25⌋: 20 + 4 = 24 |
| 7 | **Fraction HCF/LCM formulas swapped** | HCF = LCM(num)/HCF(den) | HCF = HCF(num)/LCM(den) |
| 8 | **"Successively divided" as ordinary division** | Treating it as an LCM problem | Chain the quotients backwards |
| 9 | **"Increased by 5" direction reversed** | LCM + 5 | If +5 makes it divisible, N = LCM − 5 |
| 10 | **Co-primality forgotten in HCF-sum pairs** | Counting (2,14) as valid | a and b must be co-prime |
| 11 | **Decimal HCF without scaling** | HCF of 1.08 and 0.36 directly | Scale to integers first, then rescale |
| 12 | **aⁿ + bⁿ identity applied to even n** | 2² + 3² divisible by 5 | Only valid for **odd** n |

---

## Practice Answer Key

| Q | Ans | Q | Ans | Q | Ans | Q | Ans | Q | Ans |
|---|---|---|---|---|---|---|---|---|---|
| 1 | c | 11 | b | 21 | a | 31 | c | 41 | c |
| 2 | b | 12 | c | 22 | c | 32 | b | 42 | c |
| 3 | c | 13 | b | 23 | c | 33 | c | 43 | a |
| 4 | c | 14 | b | 24 | c | 34 | c | 44 | b |
| 5 | c | 15 | c | 25 | c | 35 | c | 45 | a |
| 6 | a | 16 | c | 26 | c | 36 | c | 46 | b |
| 7 | c | 17 | c | 27 | c | 37 | c | 47 | a |
| 8 | b | 18 | a | 28 | b | 38 | c | 48 | b |
| 9 | c | 19 | c | 29 | a | 39 | c | 49 | b |
| 10 | b | 20 | c | 30 | c | 40 | b | 50 | b |

**Scoring guide:** 45+/50 → strong. 35–44 → solid; drill the remainder decision tree and unit-digit cycles. Below 35 → re-read Sections 2.4 and 2.5, then redo the Medium set.

---

**⬅️ Back:** [Topic 7 — Simple & Compound Interest](07-simple-compound-interest.md) · **➡️ Next:** [Topic 9 — Data Interpretation](09-data-interpretation.md)
