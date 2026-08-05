# Topic 10 — Permutation, Combination & Probability

### EY Placement Aptitude Handbook · Priority Rank #18 · 🟡 Medium

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

**Weightage:** 5–6% of the quantitative section — roughly **0–1 questions**.

**Be honest about the cost–benefit here.** This is the hardest quant topic per mark, and it appears less often than percentages or time-and-work. If you are on a compressed timetable, cover Sections 2.1–2.6 and 2.10 (the basics plus the complement rule) and move on. If you have time, the full topic is worth having — EY does test it, and a single P&C question can be the difference at the cutoff.

**Question styles reported:**

| Style | Typical shape |
|---|---|
| Direct nPr / nCr | "Find ⁶C₂" |
| Word arrangements | "Arrangements of the letters of SUCCESS" |
| Letters with a restriction | "…so that all vowels come together" |
| Committee selection | "Committee of 5 with exactly 3 men" |
| Circular arrangement | "6 people around a round table" |
| Dice and coins | "Two dice — probability the sum is 7" |
| Cards | "Probability of drawing a king or a heart" |
| Balls from a bag | "Two drawn — probability both are red" |
| "At least one" | "At least one red ball" |
| Geometry counting | "Triangles from 8 points" |

---

## 2. Core Concepts

### 2.1 The two fundamental counting principles

**Multiplication rule (AND):** if a task has stage 1 with *m* outcomes **and** stage 2 with *n* outcomes, the total is *m* × *n*.

> A shirt (4 choices) **and** a tie (3 choices) ⇒ 4 × 3 = **12** outfits.

**Addition rule (OR):** if a task can be done in *m* ways **or** in *n* ways (mutually exclusive), the total is *m* + *n*.

> Travel by bus (4 routes) **or** by train (3 routes) ⇒ 4 + 3 = **7** ways.

> **The word test:** "AND" ⇒ multiply. "OR" ⇒ add. This single rule resolves most set-up confusion.

### 2.2 Factorials

$$n! = n \times (n-1) \times (n-2) \times \cdots \times 2 \times 1$$

$$\boxed{0! = 1} \qquad 1! = 1$$

| n | n! | n | n! |
|---|---|---|---|
| 0 | 1 | 5 | 120 |
| 1 | 1 | 6 | 720 |
| 2 | 2 | 7 | 5,040 |
| 3 | 6 | 8 | 40,320 |
| 4 | 24 | 10 | 3,628,800 |

**Memorise up to 8!.** Beyond that, cancel rather than compute.

### 2.3 ⭐ Permutation vs Combination — the decision

This is the single most important distinction in the topic.

| | **Permutation** | **Combination** |
|---|---|---|
| **Question** | Does ORDER matter? | Order does NOT matter |
| **Notation** | ⁿP_r | ⁿC_r |
| **Formula** | $\dfrac{n!}{(n-r)!}$ | $\dfrac{n!}{r!(n-r)!}$ |
| **Keywords** | arrange, order, rank, seat, password, code, president/secretary | select, choose, committee, team, group, handshake, draw |

**The relationship:**
$$\boxed{^nP_r = \; ^nC_r \times r!}$$

A permutation is "choose *r*, then arrange those *r*".

**Illustration with 3 letters A, B, C choosing 2:**
- **Combinations (order irrelevant):** AB, AC, BC ⇒ ³C₂ = **3**
- **Permutations (order matters):** AB, BA, AC, CA, BC, CB ⇒ ³P₂ = **6** = 3 × 2!

> **The reliable test:** ask *"if I swap two chosen items, is it a different outcome?"*
> - Choosing a president and a secretary: swapping them changes the outcome ⇒ **permutation**
> - Choosing two committee members: swapping them changes nothing ⇒ **combination**

### 2.4 Key properties of ⁿC_r

$$^nC_0 = \; ^nC_n = 1 \qquad ^nC_1 = n \qquad ^nC_r = \; ^nC_{n-r}$$

$$^nC_r + \;^nC_{r-1} = \;^{n+1}C_r \qquad \text{(Pascal's rule)}$$

**The symmetry ⁿC_r = ⁿC_{n−r} is a genuine time-saver:**
> ²⁰C₁₈ = ²⁰C₂ = (20 × 19)/2 = **190** — far easier than the direct expansion.

**Fast evaluation of ⁿC_r:** write *r* factors on top counting down from *n*, and *r*! below.
$$^{10}C_3 = \frac{10 \times 9 \times 8}{3 \times 2 \times 1} = 120$$
$$^{8}C_2 = \frac{8 \times 7}{2} = 28$$

### 2.5 Arrangements with repetition

**All positions independently filled (repetition allowed):**
$$\text{Number of ways} = n^r$$

> 3-letter codes from 5 letters, repetition allowed: 5³ = **125**

**Arranging *n* objects where some are identical:**

$$\boxed{\frac{n!}{p! \times q! \times r! \times \cdots}}$$

where *p*, *q*, *r* are the counts of each repeated object.

> **BOOK** — 4 letters with O repeated twice: 4!/2! = **12**
> **SUCCESS** — 7 letters with S×3, C×2: 7!/(3! × 2!) = 5,040/12 = **420**

### 2.6 Circular arrangements

Fixing one person removes the rotational duplication.

$$\boxed{\text{Circular arrangements of } n \text{ objects} = (n-1)!}$$

If clockwise and anticlockwise are considered **the same** (e.g. a necklace of beads):
$$\frac{(n-1)!}{2}$$

> 6 people around a round table: (6 − 1)! = 5! = **120**

### 2.7 The "together" and "never together" techniques

**Together (block/glue method):**
Treat the group that must stay together as a **single unit**, arrange everything, then arrange *within* the unit.

> 5 boys and 3 girls in a row, all girls together:
> Units = 5 boys + 1 girl-block = **6 units** ⇒ 6! ways
> Girls within the block ⇒ 3! ways
> Total = 6! × 3! = 720 × 6 = **4,320**

**Never together (complement method):**
$$\text{Never together} = \text{Total arrangements} - \text{Arrangements with them together}$$

> Letters of ARRANGE with the two R's never adjacent:
> Total = 7!/(2!2!) = 1,260 · R's together = 6!/2! = 360
> Never together = 1,260 − 360 = **900**

**Alternative for "no two together" — the gap method:**
Arrange the unrestricted items first, then place the restricted ones in the gaps between them.

> Arrange 4 boys (4! ways), creating 5 gaps: `_B_B_B_B_`
> Place 3 girls in 5 gaps: ⁵P₃ ways
> Total = 4! × ⁵P₃ = 24 × 60 = **1,440**

### 2.8 Probability basics

$$\boxed{P(E) = \frac{\text{Number of favourable outcomes}}{\text{Total number of possible outcomes}}}$$

$$0 \le P(E) \le 1 \qquad P(\text{certain}) = 1 \qquad P(\text{impossible}) = 0$$

$$\boxed{P(\text{not } E) = 1 - P(E)}$$

**Standard sample spaces:**

| Experiment | Total outcomes |
|---|---|
| One coin | 2 |
| Two coins | 4 |
| Three coins | 8 (= 2³) |
| *n* coins | 2ⁿ |
| One die | 6 |
| Two dice | 36 |
| Deck of cards | 52 |

**Deck of cards structure (know this cold):**

```
52 cards
├── 26 RED    :  13 Hearts ♥  +  13 Diamonds ♦
└── 26 BLACK  :  13 Spades ♠  +  13 Clubs ♣

Each suit (13 cards):  A, 2, 3, 4, 5, 6, 7, 8, 9, 10, J, Q, K

FACE CARDS  =  J, Q, K  →  3 per suit  →  12 total
ACES        =  4        (one per suit)
```

### 2.9 Addition and multiplication in probability

**Addition rule (OR):**
$$P(A \cup B) = P(A) + P(B) - P(A \cap B)$$

For **mutually exclusive** events (they cannot both happen), P(A ∩ B) = 0:
$$P(A \cup B) = P(A) + P(B)$$

> P(King **or** Heart) = 4/52 + 13/52 − 1/52 = **16/52 = 4/13**
> *(The King of Hearts is in both sets, so it must be subtracted once.)*

**Multiplication rule (AND):**
$$P(A \cap B) = P(A) \times P(B \mid A)$$

For **independent** events, P(B | A) = P(B):
$$P(A \cap B) = P(A) \times P(B)$$

> Two aces drawn **without replacement**:
> $$\frac{4}{52} \times \frac{3}{51} = \frac{12}{2652} = \frac{1}{221}$$
> The second fraction changes because one ace and one card are already gone.

> **With replacement ⇒ independent** (probabilities unchanged).
> **Without replacement ⇒ dependent** (both numerator and denominator shrink).

### 2.10 ⭐ The complement rule — the highest-value shortcut

Whenever a question says **"at least one"**, compute the complement.

$$\boxed{P(\text{at least one}) = 1 - P(\text{none})}$$

> Three coins — P(at least one head):
> P(no head) = P(all tails) = 1/8
> P(at least one head) = 1 − 1/8 = **7/8**
>
> *(The direct route would require summing the cases for exactly 1, 2 and 3 heads: 3/8 + 3/8 + 1/8 — three times the work.)*

The same logic applies to counting problems:
> Selections of 3 balls from 5 red and 4 green with **at least one red**:
> Total = ⁹C₃ = 84 · All green = ⁴C₃ = 4 · **At least one red = 80**

### 2.11 Geometry counting

For *n* points with **no three collinear**:

| Object | Count |
|---|---|
| Straight lines | ⁿC₂ |
| Triangles | ⁿC₃ |
| Quadrilaterals | ⁿC₄ |

For a **polygon with n sides**:
$$\text{Number of diagonals} = \; ^nC_2 - n = \frac{n(n-3)}{2}$$

> Hexagon: 6 × 3/2 = **9 diagonals**

**Handshake problem:** *n* people all shaking hands once each ⇒ ⁿC₂ handshakes.

---

## 3. Formula Bank

| # | Concept | Formula |
|---|---|---|
| 1 | Factorial | $n! = n(n-1)\cdots 1$; $0! = 1$ |
| 2 | Permutation | $^nP_r = \dfrac{n!}{(n-r)!}$ |
| 3 | Combination | $^nC_r = \dfrac{n!}{r!(n-r)!}$ |
| 4 | Relation | $^nP_r = \;^nC_r \times r!$ |
| 5 | Symmetry | $^nC_r = \;^nC_{n-r}$ |
| 6 | Pascal's rule | $^nC_r + \;^nC_{r-1} = \;^{n+1}C_r$ |
| 7 | Special values | $^nC_0 = \;^nC_n = 1$; $^nC_1 = n$ |
| 8 | Arrangements with repetition allowed | $n^r$ |
| 9 | Arrangements with identical items | $\dfrac{n!}{p!\,q!\,r!\cdots}$ |
| 10 | Circular arrangement | $(n-1)!$ |
| 11 | Circular, reflections identical | $\dfrac{(n-1)!}{2}$ |
| 12 | *k* items always together | $(n-k+1)! \times k!$ |
| 13 | Never together | Total − Together |
| 14 | Gap method (no two together) | $m! \times \;^{m+1}P_k$ |
| 15 | Probability | $P(E) = \dfrac{\text{Favourable}}{\text{Total}}$ |
| 16 | Complement | $P(\text{not } E) = 1 - P(E)$ |
| 17 | At least one | $1 - P(\text{none})$ |
| 18 | Addition rule | $P(A\cup B) = P(A)+P(B)-P(A\cap B)$ |
| 19 | Multiplication (independent) | $P(A)\times P(B)$ |
| 20 | Multiplication (dependent) | $P(A)\times P(B\mid A)$ |
| 21 | Diagonals of an *n*-gon | $\dfrac{n(n-3)}{2}$ |
| 22 | Triangles from *n* points | $^nC_3$ (no three collinear) |

---

## 4. Shortcuts & Tricks

### 4.1 The order test (do this first, every time)

```
Ask:  "If I swap two of the selected items, is the outcome DIFFERENT?"

    YES  →  order matters   →  PERMUTATION  (ⁿPᵣ)
    NO   →  order irrelevant →  COMBINATION  (ⁿCᵣ)
```

| Scenario | Type |
|---|---|
| Seating people in a row | Permutation |
| Choosing a committee | Combination |
| Assigning distinct roles (captain, vice-captain) | Permutation |
| Picking a team of 5 | Combination |
| Forming a password / number | Permutation |
| Handshakes / lines through points | Combination |
| Distributing distinct prizes | Permutation |
| Selecting balls from a bag | Combination |

### 4.2 Fast ⁿC_r evaluation

Write **r factors descending from n** on top, and **r!** below.

$$^{10}C_3 = \frac{10 \cdot 9 \cdot 8}{3 \cdot 2 \cdot 1} = 120 \qquad ^{12}C_2 = \frac{12 \cdot 11}{2} = 66 \qquad ^{9}C_4 = \frac{9 \cdot 8 \cdot 7 \cdot 6}{24} = 126$$

**Values worth knowing on sight:**

| ⁿC₂ | | ⁿC₃ | |
|---|---|---|---|
| ⁵C₂ = 10 | ⁸C₂ = 28 | ⁵C₃ = 10 | ⁸C₃ = 56 |
| ⁶C₂ = 15 | ⁹C₂ = 36 | ⁶C₃ = 20 | ⁹C₃ = 84 |
| ⁷C₂ = 21 | ¹⁰C₂ = 45 | ⁷C₃ = 35 | ¹⁰C₃ = 120 |

### 4.3 Use the symmetry

$$^nC_r = \;^nC_{n-r}$$

Always compute the version with the **smaller** *r*.

> ¹⁵C₁₃ = ¹⁵C₂ = 105 · ²⁰C₁₇ = ²⁰C₃ = 1,140 · ¹²C₁₀ = ¹²C₂ = 66

### 4.4 The "together" block method

```
1.  Glue the group into ONE unit
2.  Count the units:  n − k + 1
3.  Arrange the units:  (n − k + 1)!
4.  Arrange INSIDE the block:  k!
5.  Multiply
```

> 3 girls together among 8 people: 6! × 3! = 720 × 6 = **4,320**

### 4.5 Complement first, always

```
Question says "at least one"        →  1 − P(none)
Question says "at most one"         →  P(0) + P(1)
Question says "not all"             →  1 − P(all)
Question says "never together"      →  Total − Together
Question says "at least one red"    →  Total − (all non-red)
```

Whenever the "favourable" description has many cases and the "unfavourable" has one, flip it.

### 4.6 The two-dice grid

Memorise the number of ways to make each sum with two dice:

| Sum | 2 | 3 | 4 | 5 | 6 | **7** | 8 | 9 | 10 | 11 | 12 |
|---|---|---|---|---|---|---|---|---|---|---|---|
| Ways | 1 | 2 | 3 | 4 | 5 | **6** | 5 | 4 | 3 | 2 | 1 |

Total = 36. The distribution peaks at 7 and is symmetric.

**Common probabilities:**

| Event | Ways | Probability |
|---|---|---|
| Sum = 7 | 6 | 1/6 |
| Sum = 8 | 5 | 5/36 |
| Sum > 9 (10, 11, 12) | 6 | 1/6 |
| Sum ≤ 4 | 6 | 1/6 |
| Doubles | 6 | 1/6 |
| Product is odd | 9 | 1/4 |
| Product is even | 27 | 3/4 |

### 4.7 Card probabilities on sight

| Event | Probability |
|---|---|
| A specific card | 1/52 |
| An ace | 4/52 = 1/13 |
| A face card (J, Q, K) | 12/52 = 3/13 |
| A heart | 13/52 = 1/4 |
| A red card | 26/52 = 1/2 |
| A king **or** a heart | 16/52 = 4/13 |
| A red face card | 6/52 = 3/26 |

### 4.8 Sanity checks

```
✓ Every probability lies in [0, 1]. If you get 7/6, you have double-counted.
✓ ⁿCᵣ ≤ ⁿPᵣ always (permutations are r! times as many)
✓ Circular arrangements are FEWER than linear: (n−1)! < n!
✓ "Identical items" arrangements are FEWER than n!
✓ Complements must sum to 1
✓ "At least one" answers are usually LARGE (close to 1)
```

---

## 5. Solved Examples

### Example 1 — Permutation or combination?

**Q.** From a group of 10 people, in how many ways can (a) a committee of 3 be formed, and (b) a President, Secretary and Treasurer be chosen?

**Part (a) — Committee.**
Swapping two committee members changes nothing ⇒ **order does not matter** ⇒ combination.

$$^{10}C_3 = \frac{10 \times 9 \times 8}{3 \times 2 \times 1} = \frac{720}{6} = 120$$

**Part (b) — Three distinct offices.**
Swapping two people swaps their roles ⇒ **order matters** ⇒ permutation.

$$^{10}P_3 = 10 \times 9 \times 8 = 720$$

**Answer: (a) 120 (b) 720**

**Relationship check:** 720 = 120 × 3! ✓ — each committee of 3 can be assigned roles in 3! = 6 ways.

---

### Example 2 — Arrangements with repeated letters

**Q.** In how many distinct ways can the letters of the word **MISSISSIPPI** be arranged?

**Step 1 — Count the letters and their repetitions.**
```
M I S S I S S I P P I   →  11 letters
    M  ×1
    I  ×4
    S  ×4
    P  ×2
```

**Step 2 — Apply the formula.**
$$\frac{11!}{1! \times 4! \times 4! \times 2!} = \frac{39{,}916{,}800}{1 \times 24 \times 24 \times 2}$$

**Step 3 — Compute the denominator.**
$$24 \times 24 \times 2 = 1{,}152$$

**Step 4 — Divide.**
$$\frac{39{,}916{,}800}{1{,}152} = 34{,}650$$

**Answer: 34,650**

> **Why divide?** Swapping the four I's among themselves produces the same visible word. Those 4! = 24 rearrangements are indistinguishable, so we divide them out — and likewise for the S's and P's.

---

### Example 3 — The "together" restriction

**Q.** In how many ways can the letters of the word **EQUATION** be arranged so that all the vowels are together?

**Step 1 — Identify the letters.**
EQUATION has 8 distinct letters.
- Vowels: **E, U, A, I, O** (5)
- Consonants: **Q, T, N** (3)

**Step 2 — Glue the vowels into one block.**
Units to arrange: Q, T, N and [EUAIO] = **4 units**
$$4! = 24 \text{ ways}$$

**Step 3 — Arrange the vowels inside the block.**
$$5! = 120 \text{ ways}$$

**Step 4 — Multiply.**
$$24 \times 120 = 2{,}880$$

**Answer: 2,880**

> **The block method in one line:** (units)! × (block size)!. The only judgement required is counting the units correctly — here 3 consonants + 1 block = 4.

---

### Example 4 — The "never together" complement

**Q.** In how many ways can 5 boys and 4 girls be seated in a row so that no two girls sit together?

**Method — the gap technique** (cleaner than the complement for "no two together").

**Step 1 — Seat the boys first.**
$$5! = 120 \text{ ways}$$

**Step 2 — Identify the gaps.**
Five boys create **6 gaps** (including the two ends):
$$\_ \; B \; \_ \; B \; \_ \; B \; \_ \; B \; \_ \; B \; \_$$

**Step 3 — Place the 4 girls into 4 of these 6 gaps.**
Since the girls are distinct and each gap takes at most one girl (guaranteeing no two are adjacent):
$$^6P_4 = 6 \times 5 \times 4 \times 3 = 360 \text{ ways}$$

**Step 4 — Multiply.**
$$120 \times 360 = 43{,}200$$

**Answer: 43,200**

> **Why the gap method beats the complement here:** "no two girls together" is not the same as "not all four together". The complement of "no two adjacent" is messy (it includes cases with exactly one adjacent pair, two pairs, and so on). The gap method sidesteps all of it.

---

### Example 5 — Committee selection with a condition

**Q.** From 7 men and 5 women, in how many ways can a committee of 5 be formed containing exactly 3 men and 2 women?

**Step 1 — Recognise the structure.**
Two independent choices, joined by "AND" ⇒ multiply.

**Step 2 — Choose the men.**
$$^7C_3 = \frac{7 \times 6 \times 5}{3 \times 2 \times 1} = 35$$

**Step 3 — Choose the women.**
$$^5C_2 = \frac{5 \times 4}{2} = 10$$

**Step 4 — Multiply.**
$$35 \times 10 = 350$$

**Answer: 350**

> **Extension — "at least 3 men":** you would sum the cases with 3, 4 and 5 men:
> $$^7C_3 \cdot ^5C_2 + ^7C_4 \cdot ^5C_1 + ^7C_5 \cdot ^5C_0 = 350 + 175 + 21 = 546$$
> Note the **OR** between cases ⇒ addition; the **AND** within each case ⇒ multiplication.

---

### Example 6 — Basic probability with cards

**Q.** A card is drawn at random from a standard deck of 52. Find the probability that it is (a) a face card, (b) a red king, (c) either a spade or an ace.

**(a) A face card**
Face cards are J, Q, K in each of 4 suits: 3 × 4 = 12.
$$P = \frac{12}{52} = \frac{3}{13}$$

**(b) A red king**
Kings of Hearts and Diamonds: 2 cards.
$$P = \frac{2}{52} = \frac{1}{26}$$

**(c) A spade or an ace**
Use the addition rule — the Ace of Spades belongs to both sets.
$$P(S \cup A) = P(S) + P(A) - P(S \cap A) = \frac{13}{52} + \frac{4}{52} - \frac{1}{52} = \frac{16}{52} = \frac{4}{13}$$

**Answer: (a) 3/13 (b) 1/26 (c) 4/13**

> **Direct count for (c):** 13 spades + 3 non-spade aces = 16 cards ✓ Same result, and a useful cross-check.

---

### Example 7 — Drawing without replacement

**Q.** A bag contains 5 red and 7 blue balls. Two balls are drawn at random without replacement. Find the probability that (a) both are red, (b) they are of different colours.

**Method — use combinations (order is irrelevant when drawing a handful).**

**Step 1 — Total number of ways to draw 2 from 12.**
$$^{12}C_2 = \frac{12 \times 11}{2} = 66$$

**(a) Both red**
$$^5C_2 = \frac{5 \times 4}{2} = 10$$
$$P = \frac{10}{66} = \frac{5}{33}$$

**(b) Different colours (one red AND one blue)**
$$^5C_1 \times ^7C_1 = 5 \times 7 = 35$$
$$P = \frac{35}{66}$$

**Verification using the full partition:**
$$P(\text{both red}) + P(\text{both blue}) + P(\text{different}) = \frac{10}{66} + \frac{21}{66} + \frac{35}{66} = \frac{66}{66} = 1 \checkmark$$
*(Both blue: ⁷C₂ = 21.)*

**Answer: (a) 5/33 (b) 35/66**

**Sequential cross-check for (a):**
$$\frac{5}{12} \times \frac{4}{11} = \frac{20}{132} = \frac{5}{33} \checkmark$$

---

### Example 8 — The complement rule

**Q.** Four coins are tossed simultaneously. Find the probability of getting **at least one tail**.

**Step 1 — Recognise the "at least one" signal.**
Direct counting would require the cases of exactly 1, 2, 3 and 4 tails. Use the complement instead.

**Step 2 — Total outcomes.**
$$2^4 = 16$$

**Step 3 — Compute the complement: NO tails (all heads).**
There is exactly **one** such outcome: HHHH.
$$P(\text{no tail}) = \frac{1}{16}$$

**Step 4 — Subtract from 1.**
$$P(\text{at least one tail}) = 1 - \frac{1}{16} = \frac{15}{16}$$

**Answer: 15/16**

**Verification by direct counting:**
$$\frac{^4C_1 + ^4C_2 + ^4C_3 + ^4C_4}{16} = \frac{4 + 6 + 4 + 1}{16} = \frac{15}{16} \checkmark$$

> **Four terms versus one subtraction.** The complement rule is the single biggest time-saver in probability. Train yourself to reach for it the instant you read "at least".

---

## 6. Practice Questions

**Instructions:** 50 questions. Easy (1–20), Medium (21–40), Hard (41–50).
Target times: Easy 30 s · Medium 60 s · Hard 90 s.
Full solutions in [Section 7](#7-detailed-solutions).

### 🟢 EASY (Questions 1–20)

**Q1.** What is the value of 5!?
(a) 24  (b) 60  (c) 120  (d) 720

**Q2.** Find the value of ⁶P₂.
(a) 12  (b) 15  (c) 30  (d) 36

**Q3.** Find the value of ⁶C₂.
(a) 12  (b) 15  (c) 30  (d) 36

**Q4.** In how many ways can 5 people be arranged in a row?
(a) 25  (b) 60  (c) 120  (d) 720

**Q5.** How many 3-letter codes can be formed from 5 distinct letters if repetition is allowed?
(a) 60  (b) 100  (c) 125  (d) 243

**Q6.** In how many ways can 2 items be chosen from 8?
(a) 16  (b) 28  (c) 36  (d) 56

**Q7.** What is the probability of getting a head in a single toss of a fair coin?
(a) 1/4  (b) 1/3  (c) 1/2  (d) 2/3

**Q8.** What is the probability of rolling a 3 on a fair six-sided die?
(a) 1/2  (b) 1/3  (c) 1/6  (d) 3/6

**Q9.** Two fair coins are tossed. What is the probability of getting two heads?
(a) 1/2  (b) 1/3  (c) 1/4  (d) 3/4

**Q10.** What is the value of 0!?
(a) 0  (b) 1  (c) Undefined  (d) Infinity

**Q11.** In how many ways can the letters of the word CAT be arranged?
(a) 3  (b) 6  (c) 9  (d) 27

**Q12.** What is the value of ⁷C₇?
(a) 0  (b) 1  (c) 7  (d) 49

**Q13.** A bag contains 3 red and 5 blue balls. One ball is drawn at random. What is the probability that it is red?
(a) 3/5  (b) 3/8  (c) 5/8  (d) 1/3

**Q14.** How many diagonals does a hexagon have?
(a) 6  (b) 9  (c) 12  (d) 15

**Q15.** In how many ways can a committee of 3 be selected from 6 people?
(a) 18  (b) 20  (c) 60  (d) 120

**Q16.** What is the probability of getting an even number when a fair die is rolled?
(a) 1/3  (b) 1/2  (c) 2/3  (d) 1/6

**Q17.** How many 2-digit numbers can be formed using the digits 1, 2, 3 and 4 without repetition?
(a) 8  (b) 12  (c) 16  (d) 24

**Q18.** What is the value of ⁿC₀?
(a) 0  (b) 1  (c) n  (d) n!

**Q19.** A card is drawn from a standard deck of 52. What is the probability that it is an ace?
(a) 1/52  (b) 1/26  (c) 1/13  (d) 4/13

**Q20.** In how many distinct ways can the letters of the word BOOK be arranged?
(a) 6  (b) 12  (c) 18  (d) 24

---

### 🟡 MEDIUM (Questions 21–40)

**Q21.** In how many distinct ways can the letters of the word SUCCESS be arranged?
(a) 360  (b) 420  (c) 720  (d) 840

**Q22.** In how many ways can 5 boys and 3 girls be seated in a row so that all the girls sit together?
(a) 2,880  (b) 3,600  (c) 4,320  (d) 5,040

**Q23.** From 6 men and 4 women, in how many ways can a committee of 5 be formed with exactly 3 men?
(a) 100  (b) 120  (c) 150  (d) 200

**Q24.** Two dice are thrown together. What is the probability that the sum of the numbers is 7?
(a) 1/12  (b) 1/9  (c) 1/6  (d) 5/36

**Q25.** In how many ways can 4 people be seated around a circular table?
(a) 4  (b) 6  (c) 12  (d) 24

**Q26.** A bag contains 4 red and 6 blue balls. Two balls are drawn at random. What is the probability that both are red?
(a) 1/15  (b) 2/15  (c) 4/15  (d) 2/5

**Q27.** How many 4-digit numbers can be formed using the digits 1, 2, 3, 4 and 5 without repetition?
(a) 60  (b) 100  (c) 120  (d) 625

**Q28.** A card is drawn from a standard deck. What is the probability that it is a king or a heart?
(a) 4/13  (b) 17/52  (c) 1/4  (d) 5/13

**Q29.** In how many ways can the letters of the word MOBILE be arranged so that the vowels occupy only the odd positions?
(a) 18  (b) 24  (c) 36  (d) 48

**Q30.** Three fair coins are tossed. What is the probability of getting exactly two heads?
(a) 1/4  (b) 3/8  (c) 1/2  (d) 5/8

**Q31.** How many triangles can be formed by joining 8 points, no three of which are collinear?
(a) 28  (b) 48  (c) 56  (d) 336

**Q32.** Two dice are thrown. What is the probability that the sum is greater than 9?
(a) 1/12  (b) 1/9  (c) 1/6  (d) 5/36

**Q33.** In how many ways can 3 distinct prizes be awarded to 5 students if a student may receive more than one prize?
(a) 15  (b) 60  (c) 125  (d) 243

**Q34.** From 7 men and 5 women, in how many ways can a committee of 4 be formed containing at least 3 women?
(a) 60  (b) 70  (c) 75  (d) 80

**Q35.** In how many distinct ways can the letters of the word ENGINEERING be arranged?
(a) 1,38,600  (b) 2,77,200  (c) 5,54,400  (d) 11,08,800

**Q36.** A card is drawn at random from a standard deck. What is the probability that it is a face card?
(a) 1/13  (b) 3/13  (c) 4/13  (d) 1/4

**Q37.** In how many ways can 6 people be seated around a round table if two particular people must sit together?
(a) 24  (b) 48  (c) 72  (d) 120

**Q38.** From 5 red and 4 green balls, in how many ways can 3 balls be selected so that at least one is red?
(a) 74  (b) 76  (c) 80  (d) 84

**Q39.** Two cards are drawn one after another from a deck of 52 without replacement. What is the probability that both are aces?
(a) 1/169  (b) 1/221  (c) 1/13  (d) 4/663

**Q40.** In how many ways can 5 different books be distributed among 3 students if each student may receive any number of books?
(a) 15  (b) 120  (c) 125  (d) 243

---

### 🔴 HARD (Questions 41–50)

**Q41.** In how many ways can the letters of the word ARRANGE be arranged so that the two R's never come together?
(a) 360  (b) 720  (c) 900  (d) 1,260

**Q42.** A box contains 5 white, 4 black and 3 red balls. Three balls are drawn at random. What is the probability that all three are of different colours?
(a) 2/11  (b) 3/11  (c) 4/11  (d) 5/11

**Q43.** How many 5-digit numbers can be formed using the digits 0, 1, 2, 3 and 4 without repetition?
(a) 24  (b) 96  (c) 120  (d) 625

**Q44.** In how many ways can 8 people be seated around a round table if 3 particular people must **not** all sit together?
(a) 3,600  (b) 4,320  (c) 4,680  (d) 5,040

**Q45.** Two dice are thrown. What is the probability that the product of the numbers is even?
(a) 1/4  (b) 1/2  (c) 2/3  (d) 3/4

**Q46.** From a group of 10 people, in how many ways can a committee of 5 be formed if two particular people refuse to serve together?
(a) 176  (b) 186  (c) 196  (d) 206

**Q47.** What is the probability that a randomly chosen leap year contains 53 Sundays?
(a) 1/7  (b) 2/7  (c) 3/7  (d) 4/7

**Q48.** A bag contains 6 white and 4 black balls. Two balls are drawn one after another without replacement. What is the probability that both are white?
(a) 1/3  (b) 2/5  (c) 3/8  (d) 9/25

**Q49.** In how many ways can 4 different rings be worn on 3 fingers, if a finger may hold any number of rings and the order on a finger is not considered?
(a) 12  (b) 27  (c) 64  (d) 81

**Q50.** Three unbiased coins are tossed. What is the probability of getting at least one head?
(a) 1/2  (b) 5/8  (c) 3/4  (d) 7/8

---

## 7. Detailed Solutions

### 🟢 EASY — Solutions 1–20

---

**Q1. Value of 5!. → (c) 120**

$$5! = 5 \times 4 \times 3 \times 2 \times 1 = 120$$

**Answer: (c) 120**

---

**Q2. Value of ⁶P₂. → (c) 30**

**Formula used:** ⁿPᵣ = n!/(n−r)!

$$^6P_2 = \frac{6!}{4!} = 6 \times 5 = 30$$

**Shortcut:** ⁿP₂ is simply n(n−1) — write *r* descending factors from *n*.

**Answer: (c) 30**

---

**Q3. Value of ⁶C₂. → (b) 15**

**Formula used:** ⁿCᵣ = n!/[r!(n−r)!]

$$^6C_2 = \frac{6 \times 5}{2 \times 1} = 15$$

**Relationship check:** ⁶P₂ = ⁶C₂ × 2! = 15 × 2 = 30 ✓ (matches Q2)

**Answer: (b) 15**

---

**Q4. Arrangements of 5 people in a row. → (c) 120**

All 5 are arranged, and order matters:
$$5! = 120$$

**Answer: (c) 120**

---

**Q5. 3-letter codes from 5 letters, repetition allowed. → (c) 125**

**Formula used:** nʳ (each of the *r* positions independently takes any of *n* values)

$$5^3 = 125$$

> **Trap:** using ⁵P₃ = 60. That formula forbids repetition; the question explicitly allows it.

**Answer: (c) 125**

---

**Q6. Choose 2 from 8. → (b) 28**

$$^8C_2 = \frac{8 \times 7}{2} = 28$$

**Answer: (b) 28**

---

**Q7. Probability of a head on one toss. → (c) 1/2**

$$P = \frac{1 \text{ favourable (H)}}{2 \text{ total (H, T)}} = \frac{1}{2}$$

**Answer: (c) 1/2**

---

**Q8. Probability of rolling a 3. → (c) 1/6**

$$P = \frac{1}{6}$$

**Answer: (c) 1/6**

---

**Q9. Two coins — probability of two heads. → (c) 1/4**

**Sample space:** HH, HT, TH, TT — **4** outcomes.
Favourable: HH — **1** outcome.

$$P = \frac{1}{4}$$

**Multiplication check:** (1/2) × (1/2) = 1/4 ✓ (independent tosses)

**Answer: (c) 1/4**

---

**Q10. Value of 0!. → (b) 1**

**By definition, 0! = 1.**

> **Why:** it makes ⁿCₙ = n!/(n! × 0!) = 1 work correctly — there is exactly one way to choose all *n* items.

**Answer: (b) 1**

---

**Q11. Arrangements of CAT. → (b) 6**

Three distinct letters:
$$3! = 6$$

*(CAT, CTA, ACT, ATC, TAC, TCA)*

**Answer: (b) 6**

---

**Q12. Value of ⁷C₇. → (b) 1**

$$^nC_n = 1$$

There is exactly one way to select all 7 items from 7.

**Answer: (b) 1**

---

**Q13. 3 red, 5 blue — probability of red. → (b) 3/8**

$$P = \frac{3}{3+5} = \frac{3}{8}$$

**Answer: (b) 3/8**

---

**Q14. Diagonals of a hexagon. → (b) 9**

**Formula used:** n(n−3)/2

$$\frac{6 \times 3}{2} = 9$$

**Alternative derivation:** total lines between 6 vertices = ⁶C₂ = 15; subtract the 6 sides ⇒ 15 − 6 = 9 ✓

**Answer: (b) 9**

---

**Q15. Committee of 3 from 6. → (b) 20**

$$^6C_3 = \frac{6 \times 5 \times 4}{3 \times 2 \times 1} = \frac{120}{6} = 20$$

**Answer: (b) 20**

---

**Q16. Probability of an even number on a die. → (b) 1/2**

Even outcomes: 2, 4, 6 — **3** of 6.
$$P = \frac{3}{6} = \frac{1}{2}$$

**Answer: (b) 1/2**

---

**Q17. 2-digit numbers from 1, 2, 3, 4 without repetition. → (b) 12**

$$\text{Tens digit: 4 choices} \times \text{Units digit: 3 remaining} = 12$$

*(Equivalently ⁴P₂ = 12.)*

**Answer: (b) 12**

---

**Q18. Value of ⁿC₀. → (b) 1**

$$^nC_0 = \frac{n!}{0! \times n!} = 1$$

There is exactly one way to choose nothing — the empty selection.

**Answer: (b) 1**

---

**Q19. Probability of drawing an ace. → (c) 1/13**

$$P = \frac{4}{52} = \frac{1}{13}$$

**Answer: (c) 1/13**

---

**Q20. Arrangements of BOOK. → (b) 12**

**Formula used:** n!/(p! q! …) for repeated letters

BOOK has 4 letters with **O repeated twice**:
$$\frac{4!}{2!} = \frac{24}{2} = 12$$

> **Trap:** answering 24. Swapping the two identical O's produces the same word, so half the arrangements are duplicates.

**Answer: (b) 12**

---

### 🟡 MEDIUM — Solutions 21–40

---

**Q21. Arrangements of SUCCESS. → (b) 420**

**Step 1 — Count the letters.**
```
S U C C E S S   →  7 letters
   S ×3
   C ×2
   U ×1
   E ×1
```

**Step 2 — Apply the formula.**
$$\frac{7!}{3! \times 2!} = \frac{5{,}040}{6 \times 2} = \frac{5{,}040}{12} = 420$$

**Answer: (b) 420**

---

**Q22. 5 boys and 3 girls in a row, all girls together. → (c) 4,320**

**Step 1 — Glue the girls into one block.**
Units to arrange: 5 boys + 1 girl-block = **6 units**
$$6! = 720$$

**Step 2 — Arrange the girls inside the block.**
$$3! = 6$$

**Step 3 — Multiply.**
$$720 \times 6 = 4{,}320$$

**Answer: (c) 4,320**

---

**Q23. Committee of 5 from 6 men and 4 women, exactly 3 men. → (b) 120**

**Step 1 — Determine the composition.**
Exactly 3 men ⇒ the remaining 2 must be women.

**Step 2 — Count each choice.**
$$^6C_3 = \frac{6 \times 5 \times 4}{6} = 20 \qquad ^4C_2 = \frac{4 \times 3}{2} = 6$$

**Step 3 — Multiply (both conditions must hold ⇒ AND).**
$$20 \times 6 = 120$$

**Answer: (b) 120**

---

**Q24. Two dice — probability the sum is 7. → (c) 1/6**

**Step 1 — Total outcomes.**
$$6 \times 6 = 36$$

**Step 2 — Favourable outcomes for a sum of 7.**
$$(1,6), (2,5), (3,4), (4,3), (5,2), (6,1) \implies 6$$

**Step 3 — Probability.**
$$\frac{6}{36} = \frac{1}{6}$$

> **7 is the most likely sum with two dice** — it has more combinations than any other total. Worth remembering.

**Answer: (c) 1/6**

---

**Q25. 4 people around a circular table. → (b) 6**

**Formula used:** (n − 1)!

$$(4-1)! = 3! = 6$$

> **Why (n−1)! and not n!:** rotating everyone one seat clockwise produces the same *relative* arrangement. Fixing one person's position removes those *n* equivalent rotations.

**Answer: (b) 6**

---

**Q26. 4 red, 6 blue; two drawn — probability both red. → (b) 2/15**

**Step 1 — Total ways to draw 2 from 10.**
$$^{10}C_2 = \frac{10 \times 9}{2} = 45$$

**Step 2 — Ways to draw 2 reds from 4.**
$$^4C_2 = \frac{4 \times 3}{2} = 6$$

**Step 3 — Probability.**
$$\frac{6}{45} = \frac{2}{15}$$

**Sequential cross-check:**
$$\frac{4}{10} \times \frac{3}{9} = \frac{12}{90} = \frac{2}{15} \checkmark$$

**Answer: (b) 2/15**

---

**Q27. 4-digit numbers from 1–5 without repetition. → (c) 120**

$$5 \times 4 \times 3 \times 2 = 120$$

*(Equivalently ⁵P₄ = 5!/1! = 120.)*

**Answer: (c) 120**

---

**Q28. Probability of a king or a heart. → (a) 4/13**

**Formula used:** P(A ∪ B) = P(A) + P(B) − P(A ∩ B)

**Step 1 — Count each set.**
- Kings: 4
- Hearts: 13
- **King of Hearts: 1** (counted in both)

**Step 2 — Apply inclusion–exclusion.**
$$\frac{4}{52} + \frac{13}{52} - \frac{1}{52} = \frac{16}{52} = \frac{4}{13}$$

**Direct count:** 13 hearts + 3 non-heart kings = 16 cards ✓

> **Trap:** answering 17/52 by forgetting to subtract the overlap.

**Answer: (a) 4/13**

---

**Q29. MOBILE with vowels in odd positions only. → (c) 36**

**Step 1 — Classify the letters.**
MOBILE = M, O, B, I, L, E (6 distinct letters)
- Vowels: **O, I, E** (3)
- Consonants: **M, B, L** (3)

**Step 2 — Identify the positions.**
Positions 1–6. The odd positions are **1, 3, 5** — exactly 3 slots.
The even positions are **2, 4, 6** — the remaining 3 slots.

**Step 3 — Arrange the vowels in the odd slots.**
$$3! = 6$$

**Step 4 — Arrange the consonants in the even slots.**
$$3! = 6$$

**Step 5 — Multiply.**
$$6 \times 6 = 36$$

**Answer: (c) 36**

---

**Q30. Three coins — exactly two heads. → (b) 3/8**

**Step 1 — Total outcomes.**
$$2^3 = 8$$

**Step 2 — Favourable: choose which 2 of the 3 tosses are heads.**
$$^3C_2 = 3 \quad \text{(HHT, HTH, THH)}$$

**Step 3 — Probability.**
$$\frac{3}{8}$$

**Answer: (b) 3/8**

---

**Q31. Triangles from 8 points, no three collinear. → (c) 56**

**Concept:** any 3 non-collinear points determine exactly one triangle, and the order of selection is irrelevant ⇒ combination.

$$^8C_3 = \frac{8 \times 7 \times 6}{3 \times 2 \times 1} = \frac{336}{6} = 56$$

> **Trap:** answering 336 (that is ⁸P₃) — but triangle ABC is the same as triangle BCA, so order must not be counted.

**Answer: (c) 56**

---

**Q32. Two dice — probability the sum exceeds 9. → (c) 1/6**

**Step 1 — Identify the qualifying sums.** Greater than 9 means 10, 11 or 12.

**Step 2 — Count the ways for each.**

| Sum | Combinations | Count |
|---|---|---|
| 10 | (4,6), (5,5), (6,4) | 3 |
| 11 | (5,6), (6,5) | 2 |
| 12 | (6,6) | 1 |
| | **Total** | **6** |

**Step 3 — Probability.**
$$\frac{6}{36} = \frac{1}{6}$$

> **"Greater than 9" excludes 9 itself.** Including it would add 4 more outcomes and give 10/36 = 5/18.

**Answer: (c) 1/6**

---

**Q33. 3 distinct prizes to 5 students, repeats allowed. → (c) 125**

**Step 1 — Think prize by prize.** Each prize can go to any of the 5 students, independently.

$$5 \times 5 \times 5 = 5^3 = 125$$

> **Trap:** using ⁵P₃ = 60 (which assumes no student wins twice) or ⁵C₃ = 10 (which ignores that the prizes are distinct).

**Answer: (c) 125**

---

**Q34. Committee of 4 from 7 men and 5 women, at least 3 women. → (c) 75**

**Step 1 — Enumerate the qualifying cases.**
"At least 3 women" from a committee of 4 means **3 women** or **4 women**.

**Case A — 3 women and 1 man:**
$$^5C_3 \times ^7C_1 = 10 \times 7 = 70$$

**Case B — 4 women and 0 men:**
$$^5C_4 \times ^7C_0 = 5 \times 1 = 5$$

**Step 2 — Add (the cases are mutually exclusive ⇒ OR).**
$$70 + 5 = 75$$

**Answer: (c) 75**

> **Structure to internalise:** *within* a case, multiply (men AND women). *Between* cases, add (3 women OR 4 women).

---

**Q35. Arrangements of ENGINEERING. → (b) 2,77,200**

**Step 1 — Count the letters.**
```
E N G I N E E R I N G   →  11 letters
   E ×3      (positions 1, 6, 7)
   N ×3
   G ×2
   I ×2
   R ×1
```
Check: 3 + 3 + 2 + 2 + 1 = 11 ✓

**Step 2 — Apply the formula.**
$$\frac{11!}{3! \times 3! \times 2! \times 2!} = \frac{39{,}916{,}800}{6 \times 6 \times 2 \times 2}$$

**Step 3 — Compute the denominator.**
$$6 \times 6 \times 2 \times 2 = 144$$

**Step 4 — Divide.**
$$\frac{39{,}916{,}800}{144} = 277{,}200$$

**Answer: (b) 2,77,200**

---

**Q36. Probability of a face card. → (b) 3/13**

Face cards are J, Q and K in each of 4 suits:
$$3 \times 4 = 12$$
$$P = \frac{12}{52} = \frac{3}{13}$$

> **Note:** the Ace is **not** a face card in the standard convention.

**Answer: (b) 3/13**

---

**Q37. 6 people around a round table, two particular people together. → (b) 48**

**Step 1 — Glue the pair into one unit.**
Units to arrange: 4 individuals + 1 pair-block = **5 units**

**Step 2 — Arrange them in a circle.**
$$(5-1)! = 4! = 24$$

**Step 3 — Arrange the two people within the block.**
$$2! = 2$$

**Step 4 — Multiply.**
$$24 \times 2 = 48$$

**Answer: (b) 48**

---

**Q38. 3 balls from 5 red and 4 green, at least one red. → (c) 80**

**Method — complement.**

**Step 1 — Total ways to choose 3 from 9.**
$$^9C_3 = \frac{9 \times 8 \times 7}{6} = 84$$

**Step 2 — Ways with NO red (all green).**
$$^4C_3 = 4$$

**Step 3 — Subtract.**
$$84 - 4 = 80$$

**Direct-count verification:**

| Composition | Ways |
|---|---|
| 1 red, 2 green | ⁵C₁ × ⁴C₂ = 5 × 6 = 30 |
| 2 red, 1 green | ⁵C₂ × ⁴C₁ = 10 × 4 = 40 |
| 3 red, 0 green | ⁵C₃ = 10 |
| **Total** | **80** ✓ |

> The complement took one line; the direct count took three. Always check whether the complement is shorter.

**Answer: (c) 80**

---

**Q39. Two aces drawn without replacement. → (b) 1/221**

**Method 1 — Sequential probabilities.**
$$P = \frac{4}{52} \times \frac{3}{51} = \frac{12}{2{,}652} = \frac{1}{221}$$

*(After the first ace is drawn, 3 aces remain among 51 cards.)*

**Method 2 — Combinations.**
$$P = \frac{^4C_2}{^{52}C_2} = \frac{6}{1{,}326} = \frac{1}{221} \checkmark$$

> **Trap:** using 4/52 × 4/52 = 1/169 — that would be correct only *with* replacement.

**Answer: (b) 1/221**

---

**Q40. 5 different books among 3 students, any number each. → (d) 243**

**Step 1 — Think book by book.**
Each of the 5 distinct books can go to any of the 3 students, independently.

$$3 \times 3 \times 3 \times 3 \times 3 = 3^5 = 243$$

> **Which base goes on top?** The **objects being distributed** (books) become the exponent; the **destinations** (students) become the base. Getting this backwards gives 5³ = 125.

**Answer: (d) 243**

---

### 🔴 HARD — Solutions 41–50

---

**Q41. ARRANGE with the two R's never together. → (c) 900**

**Method — complement (Total − Together).**

**Step 1 — Count the letters.**
```
A R R A N G E   →  7 letters
   A ×2
   R ×2
   N, G, E ×1 each
```

**Step 2 — Total arrangements (no restriction).**
$$\frac{7!}{2! \times 2!} = \frac{5{,}040}{4} = 1{,}260$$

**Step 3 — Arrangements with the two R's TOGETHER.**
Glue RR into one unit. Now we arrange 6 units: [RR], A, A, N, G, E — still with A repeated twice.
$$\frac{6!}{2!} = \frac{720}{2} = 360$$

*(Note: the two R's are identical, so there is no internal 2! factor for the block.)*

**Step 4 — Subtract.**
$$1{,}260 - 360 = 900$$

**Answer: (c) 900**

> **The subtlety in Step 3:** for a block of *distinct* items you multiply by k!, but for a block of *identical* items you do not — swapping the two R's changes nothing.

---

**Q42. 5 white, 4 black, 3 red; 3 drawn — all different colours. → (b) 3/11**

**Step 1 — Total ways to draw 3 from 12.**
$$^{12}C_3 = \frac{12 \times 11 \times 10}{6} = 220$$

**Step 2 — Favourable: one of each colour.**
$$^5C_1 \times ^4C_1 \times ^3C_1 = 5 \times 4 \times 3 = 60$$

**Step 3 — Probability.**
$$\frac{60}{220} = \frac{3}{11}$$

**Answer: (b) 3/11**

---

**Q43. 5-digit numbers from 0, 1, 2, 3, 4 without repetition. → (b) 96**

**Step 1 — Identify the constraint.**
A 5-digit number cannot begin with **0**.

**Step 2 — Fill the leading position.**
Choices: 1, 2, 3, 4 ⇒ **4 ways**

**Step 3 — Fill the remaining four positions.**
Four digits remain (including 0), all distinct:
$$4! = 24$$

**Step 4 — Multiply.**
$$4 \times 24 = 96$$

**Verification via the complement:** total permutations of 5 digits = 5! = 120; those starting with 0 = 4! = 24; valid = 120 − 24 = **96** ✓

**Answer: (b) 96**

---

**Q44. 8 around a round table; 3 particular people NOT all together. → (b) 4,320**

**Method — complement.**

**Step 1 — Total circular arrangements of 8.**
$$(8-1)! = 7! = 5{,}040$$

**Step 2 — Arrangements with the 3 together.**
Glue them into one block. Units = 5 individuals + 1 block = **6 units**.
$$(6-1)! \times 3! = 5! \times 6 = 120 \times 6 = 720$$

**Step 3 — Subtract.**
$$5{,}040 - 720 = 4{,}320$$

**Answer: (b) 4,320**

> **Read the restriction precisely.** "Must not **all** sit together" forbids only the case where all three are consecutive. It does *not* forbid two of them sitting together — that would be a different, harder problem.

---

**Q45. Two dice — probability the product is even. → (d) 3/4**

**Method — complement.**

**Step 1 — When is a product ODD?**
Only when **both** numbers are odd.

**Step 2 — Compute P(both odd).**
Each die shows an odd number (1, 3, 5) with probability 3/6 = 1/2.
$$P(\text{both odd}) = \frac{1}{2} \times \frac{1}{2} = \frac{1}{4}$$

**Step 3 — Take the complement.**
$$P(\text{product even}) = 1 - \frac{1}{4} = \frac{3}{4}$$

**Direct verification:** odd-odd pairs = 3 × 3 = 9 of 36 outcomes ⇒ even product in 27/36 = 3/4 ✓

> **Key insight:** a product is even if *at least one* factor is even. "At least one" ⇒ reach for the complement.

**Answer: (d) 3/4**

---

**Q46. Committee of 5 from 10; two people refuse to serve together. → (c) 196**

**Method — complement.**

**Step 1 — Total committees with no restriction.**
$$^{10}C_5 = \frac{10 \times 9 \times 8 \times 7 \times 6}{5 \times 4 \times 3 \times 2 \times 1} = \frac{30{,}240}{120} = 252$$

**Step 2 — Committees containing BOTH of the two people.**
If both are in, we must choose the remaining 3 members from the other 8 people:
$$^8C_3 = \frac{8 \times 7 \times 6}{6} = 56$$

**Step 3 — Subtract the forbidden committees.**
$$252 - 56 = 196$$

**Direct-count verification:**

| Case | Ways |
|---|---|
| Neither of the two | ⁸C₅ = 56 |
| Exactly the first one | ⁸C₄ = 70 |
| Exactly the second one | ⁸C₄ = 70 |
| **Total** | **196** ✓ |

**Answer: (c) 196**

---

**Q47. Probability a leap year has 53 Sundays. → (b) 2/7**

**Step 1 — Break the year into weeks.**
A leap year has **366 days**:
$$366 = 52 \times 7 + 2$$

So the year contains 52 complete weeks **plus 2 extra days**.

**Step 2 — Understand what the 52 weeks guarantee.**
Every day of the week already occurs 52 times. A 53rd Sunday requires Sunday to appear among the **2 extra days**.

**Step 3 — Enumerate the possible pairs of extra days.**
The 2 extra days are always **consecutive**:

| # | Extra days | Contains Sunday? |
|---|---|---|
| 1 | Sunday, Monday | ✓ |
| 2 | Monday, Tuesday | ✗ |
| 3 | Tuesday, Wednesday | ✗ |
| 4 | Wednesday, Thursday | ✗ |
| 5 | Thursday, Friday | ✗ |
| 6 | Friday, Saturday | ✗ |
| 7 | Saturday, Sunday | ✓ |

**Step 4 — Compute the probability.**
2 of the 7 equally likely cases contain a Sunday:
$$P = \frac{2}{7}$$

**Answer: (b) 2/7**

> **Compare with an ordinary year:** 365 = 52 × 7 + **1**, so there is only 1 extra day and 7 possibilities ⇒ P(53 Sundays) = **1/7**.

---

**Q48. 6 white, 4 black; two drawn without replacement — both white. → (a) 1/3**

**Method 1 — Sequential.**
$$P = \frac{6}{10} \times \frac{5}{9} = \frac{30}{90} = \frac{1}{3}$$

*(After one white is removed, 5 whites remain among 9 balls.)*

**Method 2 — Combinations.**
$$P = \frac{^6C_2}{^{10}C_2} = \frac{15}{45} = \frac{1}{3} \checkmark$$

> **Trap:** using (6/10)² = 9/25 — correct only *with* replacement. Both the numerator and the denominator must shrink when drawing without replacement.

**Answer: (a) 1/3**

---

**Q49. 4 different rings on 3 fingers. → (d) 81**

**Step 1 — Think ring by ring.**
Each ring independently chooses one of the 3 fingers. Since the order on a finger does not matter, each ring simply picks a destination.

$$3 \times 3 \times 3 \times 3 = 3^4 = 81$$

**Answer: (d) 81**

> **The base-and-exponent rule:** *destinations* form the base, *objects* form the exponent. Four rings, three fingers ⇒ 3⁴, not 4³.

---

**Q50. Three coins — at least one head. → (d) 7/8**

**Method — complement.**

**Step 1 — Total outcomes.**
$$2^3 = 8$$

**Step 2 — Compute P(no head).**
"No head" means all three are tails — exactly **one** outcome (TTT).
$$P(\text{no head}) = \frac{1}{8}$$

**Step 3 — Subtract from 1.**
$$P(\text{at least one head}) = 1 - \frac{1}{8} = \frac{7}{8}$$

**Direct-count verification:**
$$\frac{^3C_1 + ^3C_2 + ^3C_3}{8} = \frac{3 + 3 + 1}{8} = \frac{7}{8} \checkmark$$

**Answer: (d) 7/8**

---

## 8. Quick Revision Sheet

> **One page. Read 48 hours after study, and again the night before the test.**

### The decision

```
"If I swap two selected items, is the result DIFFERENT?"

   YES  →  PERMUTATION  ⁿPᵣ = n!/(n−r)!
   NO   →  COMBINATION  ⁿCᵣ = n!/[r!(n−r)!]

   ⁿPᵣ = ⁿCᵣ × r!

Permutation words: arrange, order, rank, seat, code, password, distinct roles
Combination words: select, choose, committee, team, group, handshake, draw
```

### Counting principles

```
AND  →  MULTIPLY        OR  →  ADD

Repetition allowed              →  nʳ
n objects, some identical       →  n! / (p! q! r! …)
Circular arrangement            →  (n−1)!
Circular, reflections identical →  (n−1)!/2
```

### Restriction techniques

```
k items TOGETHER    →  glue into 1 block
                       (n−k+1)! × k!
                       (NO ×k! if the block items are identical)

NEVER together      →  Total − Together

NO TWO together     →  gap method:
                       arrange m unrestricted (m!), then place k in the
                       (m+1) gaps:  m! × ᵐ⁺¹Pₖ
```

### Fast values

```
0! = 1   1! = 1   2! = 2   3! = 6   4! = 24
5! = 120  6! = 720  7! = 5040  8! = 40320

ⁿC₂ :  5C2=10  6C2=15  7C2=21  8C2=28  9C2=36  10C2=45
ⁿC₃ :  5C3=10  6C3=20  7C3=35  8C3=56  9C3=84  10C3=120

ⁿCᵣ = ⁿC₍ₙ₋ᵣ₎     ← always compute the SMALLER r
ⁿC₀ = ⁿCₙ = 1     ⁿC₁ = n
```

### Probability

```
P(E) = Favourable / Total          0 ≤ P ≤ 1
P(not E) = 1 − P(E)

⭐ P(at least one) = 1 − P(none)      ← reach for this every time

P(A ∪ B) = P(A) + P(B) − P(A ∩ B)
P(A ∩ B) = P(A) × P(B)          [independent / with replacement]
P(A ∩ B) = P(A) × P(B|A)        [dependent / without replacement]
```

### Standard sample spaces

```
n coins  →  2ⁿ            Two dice  →  36           Deck  →  52

TWO DICE — ways to make each sum:
   2:1  3:2  4:3  5:4  6:5  7:6  8:5  9:4  10:3  11:2  12:1
   Sum = 7 → 1/6      Sum > 9 → 1/6      Doubles → 1/6
   Product even → 3/4  Product odd → 1/4

CARDS:  52 = 26 red + 26 black = 4 suits × 13
   Ace → 1/13     Face card (J,Q,K) → 12/52 = 3/13
   Heart → 1/4    King OR heart → 16/52 = 4/13

CALENDAR:  ordinary year → 1 extra day → P(53 of a given day) = 1/7
           leap year     → 2 extra days → P = 2/7
```

### Geometry counting (n points, no 3 collinear)

```
Lines / handshakes  →  ⁿC₂
Triangles           →  ⁿC₃
Quadrilaterals      →  ⁿC₄
Diagonals of n-gon  →  n(n−3)/2   =  ⁿC₂ − n
```

### Sanity checks

```
✓ 0 ≤ P ≤ 1. A value above 1 means double-counting.
✓ ⁿCᵣ ≤ ⁿPᵣ always
✓ (n−1)! < n!  — circular gives fewer than linear
✓ Complements must sum to 1
✓ "At least one" answers are usually close to 1
✓ Distributing objects: OBJECTS are the exponent, DESTINATIONS the base
```

---

## 9. Common Mistakes

| # | Mistake | Example | Correction |
|---|---|---|---|
| 1 | **Permutation used for a selection** | Committee of 3 from 6 ⇒ ⁶P₃ = 120 | Order irrelevant ⇒ ⁶C₃ = 20 |
| 2 | **Combination used for an arrangement** | 3 distinct prizes ⇒ ⁵C₃ | Prizes are distinct ⇒ 5³ = 125 |
| 3 | **Repetition ignored in words** | BOOK ⇒ 4! = 24 | Divide by 2! for the O's ⇒ 12 |
| 4 | **Block internal arrangement forgotten** | 3 girls together ⇒ 6! only | Multiply by 3! ⇒ 6! × 3! |
| 5 | **Block ×k! applied to identical items** | RR block ⇒ ×2! | Identical letters — no internal factor |
| 6 | **Circular treated as linear** | 6 around a table ⇒ 6! | (6−1)! = 120 |
| 7 | **Leading zero allowed** | 5-digit from 0–4 ⇒ 5! = 120 | Exclude leading 0 ⇒ 96 |
| 8 | **Replacement assumed** | Two aces ⇒ (4/52)² | Without replacement: (4/52)(3/51) |
| 9 | **Overlap not subtracted** | King or heart ⇒ 17/52 | Subtract the King of Hearts ⇒ 16/52 |
| 10 | **"At least" done the long way** | Summing 4 cases | 1 − P(none) |
| 11 | **Base and exponent swapped** | 5 books, 3 students ⇒ 5³ | Destinations are the base ⇒ 3⁵ |
| 12 | **"Not all together" read as "none together"** | Forbidding any two adjacent | Only the all-three case is forbidden |
| 13 | **Rates of an "or" added when not exclusive** | P(A)+P(B) with overlap | Use inclusion–exclusion |
| 14 | **Ace counted as a face card** | 16 face cards | Face cards are J, Q, K only ⇒ 12 |

---

## Practice Answer Key

| Q | Ans | Q | Ans | Q | Ans | Q | Ans | Q | Ans |
|---|---|---|---|---|---|---|---|---|---|
| 1 | c | 11 | b | 21 | b | 31 | c | 41 | c |
| 2 | c | 12 | b | 22 | c | 32 | c | 42 | b |
| 3 | b | 13 | b | 23 | b | 33 | c | 43 | b |
| 4 | c | 14 | b | 24 | c | 34 | c | 44 | b |
| 5 | c | 15 | b | 25 | b | 35 | b | 45 | d |
| 6 | b | 16 | b | 26 | b | 36 | b | 46 | c |
| 7 | c | 17 | b | 27 | c | 37 | b | 47 | b |
| 8 | c | 18 | b | 28 | a | 38 | c | 48 | a |
| 9 | c | 19 | c | 29 | c | 39 | b | 49 | d |
| 10 | b | 20 | b | 30 | b | 40 | d | 50 | d |

**Scoring guide:** 40+/50 → strong (this topic is harder than most). 30–39 → solid; drill the order test and the complement rule. Below 30 → focus on Sections 2.3, 2.5 and 2.10 only — they cover the majority of what EY actually asks.

---

**⬅️ Back:** [Topic 9 — Data Interpretation](09-data-interpretation.md) · **➡️ Next:** [Topic 11 — Mensuration & Geometry](11-mensuration-geometry.md)
