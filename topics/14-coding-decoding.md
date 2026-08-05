# Topic 14 — Coding–Decoding

### EY Placement Aptitude Handbook · Priority Rank #12 · 🔴 Critical

> **Questions in this file are original, modelled on publicly reported EY test patterns. They are not claimed to be actual previous-year EY questions.**

---

## Contents

1. [Why This Topic Matters for EY](#1-why-this-topic-matters-for-ey)
2. [Core Concepts](#2-core-concepts)
3. [Code-Type Bank](#3-code-type-bank)
4. [Shortcuts & Tricks](#4-shortcuts--tricks)
5. [Solved Examples](#5-solved-examples)
6. [Practice Questions (50)](#6-practice-questions)
7. [Detailed Solutions](#7-detailed-solutions)
8. [Quick Revision Sheet](#8-quick-revision-sheet)
9. [Common Mistakes](#9-common-mistakes)

---

## 1. Why This Topic Matters for EY

**Weightage:** 10–12% of the reasoning section — expect **1–2 questions**.

**Why it is high-return:** coding–decoding involves **zero mathematics** and **zero ambiguity**. Once you spot the rule, the answer is mechanical. The entire difficulty lies in identifying the rule quickly, and there are only about eight rules in circulation. Learn those eight and this topic becomes free marks.

**Question styles reported:**

| Style | Example |
|---|---|
| **Letter shift** | "CAT → DBU. Code for DOG?" |
| **Reverse the word** | "TEA → AET. Code for COW?" |
| **Number substitution** | "A=1, B=2… Code for CAB?" |
| **Opposite letters** | "BLACK → YOZXP. Code for WHITE?" |
| **Positional swap** | "SUMMER → RUMMES. Code for WINTER?" |
| **Mixed-language (substitution) code** | "'pit na som' means 'bring me water'…" |
| **Digit-word mapping** | "'5 3 8' means 'good sweet fruit'…" |
| **Rule-based numeric code** | "REASON → 5, BELIEVED → 7. Code for GOVERNMENT?" |

---

## 2. Core Concepts

### 2.1 The alphabet — your only prerequisite

| A | B | C | D | E | F | G | H | I | J | K | L | M |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12 | 13 |

| N | O | P | Q | R | S | T | U | V | W | X | Y | Z |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 14 | 15 | 16 | 17 | 18 | 19 | 20 | 21 | 22 | 23 | 24 | 25 | 26 |

**Anchors (EJOTY):** E = 5 · J = 10 · O = 15 · T = 20 · Y = 25

**Reverse positions (A = 26, Z = 1):** position from the end = **27 − n**

| A↔Z | B↔Y | C↔X | D↔W | E↔V | F↔U | G↔T |
|---|---|---|---|---|---|---|
| H↔S | I↔R | J↔Q | K↔P | L↔O | M↔N | |

> **You cannot do this topic without instant alphabet recall.** If you have to count "A, B, C…" on your fingers, every question costs 40 seconds instead of 10. Spend twenty minutes memorising the table above — it is the highest-leverage memorisation in the reasoning section.

### 2.2 The universal method

```
STEP 1:  Line up the original word and its code, LETTER BY LETTER
STEP 2:  Compute the SHIFT for each letter pair (code position − original position)
STEP 3:  Look at the pattern of shifts:
             all the same           →  constant shift
             +1, +2, +3, …          →  increasing shift
             alternating + and −    →  alternating shift
             27 − n                 →  opposite letters
             none of these          →  positional rearrangement
STEP 4:  Apply the same rule to the target word
STEP 5:  Verify against a second given pair if one exists
```

**Always write the shift row.** Trying to spot the pattern by eye is exactly how candidates misread a +2 shift as a +1.

```
    C   A   T          Original positions:   3   1  20
    ↓   ↓   ↓
    D   B   U          Code positions:       4   2  21
                       ────────────────────────────────
                       SHIFT:               +1  +1  +1     ⇒ constant +1
```

### 2.3 Handling wrap-around

The alphabet is circular for coding purposes:

$$\ldots \to X \to Y \to Z \to A \to B \to \ldots$$

> Z + 1 = **A** · Y + 3 = **B** · A − 1 = **Z** · B − 3 = **Y**

**Rule:** if the computed position exceeds 26, subtract 26. If it drops below 1, add 26.

> B(2) + 25 = 27 → 27 − 26 = 1 = **A**

### 2.4 Positional rearrangement codes

When the code uses **the same letters in a different order**, no shift is involved — only a permutation.

| Type | Example | Rule |
|---|---|---|
| **Full reversal** | TEA → AET | Write the word backwards |
| **First–last swap** | SUMMER → RUMMES | Exchange the outer letters |
| **Adjacent-pair swap** | MOTHER → OMHTRE | Swap letters in pairs: (1,2)(3,4)(5,6) |
| **Half reversal** | SYSTEM → SYSMET | Keep the first half; reverse the second |
| **Rotation** | LOGIC → OGICL | Move the first letter to the end |

**How to tell a rearrangement from a shift:** compare the **letter sets**. If the code uses exactly the same letters as the original, it is a rearrangement. If different letters appear, it is a shift.

### 2.5 Mixed-language (substitution) codes

> *"'pit na som' means 'bring me water'; 'na jo tod' means 'water is life'; 'som tod jo' means 'bring life is'. Which word means 'bring'?"*

**Method — intersect the sentences.**

```
Sentence 1:  pit  na  som     =  bring  me  water
Sentence 2:  na   jo  tod     =  water  is  life
Sentence 3:  som  tod jo      =  bring  life is

1 ∩ 2 :  common code word = "na"   ; common meaning = "water"   ⇒  na = water
1 ∩ 3 :  common code word = "som"  ; common meaning = "bring"   ⇒  som = bring
Remaining in sentence 1: "pit" = "me"
```

> **The technique in one line:** find a code word appearing in exactly two sentences, then find the meaning appearing in exactly those same two sentences. They must correspond.

**When three sentences share a pair of words**, you may only be able to narrow the answer to two possibilities — which is usually all the question requires.

### 2.6 Digit-word codes

Identical logic, with digits instead of nonsense syllables.

> *"'5 3 8' means 'good sweet fruit'; '5 7 2' means 'good tasty juice'; '8 2 9' means 'fresh fruit juice'. Which digit means 'good'?"*

```
Sentences 1 and 2 share the digit 5 and the word "good"  ⇒  5 = good
Sentences 1 and 3 share the digit 8 and the word "fruit" ⇒  8 = fruit
Sentences 2 and 3 share the digit 2 and the word "juice" ⇒  2 = juice
```

By elimination: 3 = sweet, 7 = tasty, 9 = fresh.

**Build a table** rather than tracking it mentally — three sentences generate six deductions and it is easy to lose one.

### 2.7 Rule-based numeric codes

Some codes ignore the letters and encode a **property** of the word.

> *"REASON is coded as 5 and BELIEVED as 7. What is the code for GOVERNMENT?"*

```
REASON      →  6 letters  →  code 5     (letters − 1)
BELIEVED    →  8 letters  →  code 7     (letters − 1)
GOVERNMENT  → 10 letters  →  code 9
```

**Properties commonly encoded:**
- Number of letters (sometimes ±1)
- Number of vowels
- Sum of letter positions
- Position of the first letter

> If in doubt, **count the letters first** — it is by far the most common rule of this type.

---

## 3. Code-Type Bank

| # | Type | Example | Rule |
|---|---|---|---|
| 1 | **Forward shift +1** | CAT → DBU | Each letter advances 1 |
| 2 | **Forward shift +2** | WATER → YCVGT | Each letter advances 2 |
| 3 | **Backward shift −1** | MAN → LZM | Each letter retreats 1 |
| 4 | **Backward shift −2** | TRAIN → RPYGL | Each letter retreats 2 |
| 5 | **Increasing shift** | ABC → BDF | +1, +2, +3, … |
| 6 | **Alternating shift** | ABCD → BAD C-style | +1, −1, +1, −1 |
| 7 | **Opposite letters** | BLACK → YOZXP | Replace *n* with 27 − *n* |
| 8 | **Full reversal** | TEA → AET | Write backwards |
| 9 | **First–last swap** | SUMMER → RUMMES | Exchange outer letters |
| 10 | **Adjacent-pair swap** | MOTHER → OMHTRE | Swap (1,2)(3,4)(5,6) |
| 11 | **Half reversal** | SYSTEM → SYSMET | Reverse the second half |
| 12 | **Number substitution (A=1)** | CAB → 3-1-2 | Positional numbers |
| 13 | **Reverse numbering (A=26)** | CAT → 24-26-7 | 27 − position |
| 14 | **Even numbering (A=2)** | FACE → 12-2-6-10 | 2 × position |
| 15 | **Sum of positions** | CAB → 6 | 3 + 1 + 2 |
| 16 | **Letter count** | REASON → 6 (or 5) | Count the letters |
| 17 | **Substitution language** | "pit na som" | Intersect the sentences |
| 18 | **Digit-word mapping** | "5 3 8" | Intersect the sentences |
| 19 | **Symbol substitution** | Fixed letter→symbol table | Build the table from the pairs |
| 20 | **Conditional/matrix code** | Position-dependent rules | Read the stated conditions |

---

## 4. Shortcuts & Tricks

### 4.1 The shift table — write it every time

```
        W    A    T    E    R
Pos:   23    1   20    5   18
        ↓    ↓    ↓    ↓    ↓
Code:   Y    C    V    G    T
Pos:   25    3   22    7   20
       ───────────────────────
Shift: +2   +2   +2   +2   +2      ⇒  constant +2
```

Thirty seconds spent on this table beats two minutes of squinting at the letters.

### 4.2 Test the three most common rules first

```
1.  +1 shift        (about 30% of all coding questions)
2.  −1 shift        (about 15%)
3.  Reversal        (about 15%)
```

Check these three before anything else — they cover roughly 60% of what appears.

### 4.3 Shift or rearrangement? Compare the letter sets

```
CAT → DBU     letters differ  ⇒  SHIFT
TEA → AET     same letters    ⇒  REARRANGEMENT
```

This single check halves your search space in three seconds.

### 4.4 Spotting the opposite-letter code

The tell-tale sign: **A maps to Z, or the shifts look wildly inconsistent** — some large positive, some large negative.

```
        B    L    A    C    K
Pos:    2   12    1    3   11
Code:   Y    O    Z    X    P
Pos:   25   15   26   24   16
       ─────────────────────────
Sum:   27   27   27   27   27      ⇒  OPPOSITE LETTERS
```

**When the position pairs sum to 27, it is the opposite-letter rule.** Checking the sum is faster than checking the shift.

### 4.5 Mixed-language codes — the intersection grid

Draw a small grid; do not do it in your head.

```
             pit   na   som   jo   tod
Sentence 1:   ✓    ✓     ✓                =  bring, me, water
Sentence 2:        ✓          ✓     ✓     =  water, is, life
Sentence 3:              ✓     ✓     ✓    =  bring, life, is

"na" appears in 1 and 2  →  the shared MEANING is "water"  →  na = water
"som" appears in 1 and 3 →  the shared MEANING is "bring"  →  som = bring
"pit" appears only in 1  →  the leftover meaning is "me"   →  pit = me
```

### 4.6 Handle the wrap-around consciously

```
Forward:   Z + 1 = A     Y + 2 = A     X + 3 = A
Backward:  A − 1 = Z     B − 2 = Z     C − 3 = Z

Arithmetic rule:  if position > 26, subtract 26
                  if position < 1,  add 26
```

Wrap-around appears in roughly one coding question in five, and is a favourite way to make an otherwise easy question discriminate.

### 4.7 Verify against the second pair

Many questions supply **two** coded examples. Use the first to form your hypothesis and the **second to test it**. A rule that fits both is almost certainly correct; a rule that fits only one is wrong.

### 4.8 Sanity checks

```
✓ The code word must have the SAME LENGTH as the original (unless the rule
  is a property code like letter-counting)
✓ A rearrangement code uses EXACTLY the same letters
✓ A constant shift produces the SAME shift for every letter — check all of them
✓ Opposite-letter codes: every position pair sums to 27
✓ In substitution languages, every word must be accounted for
```

---

## 5. Solved Examples

### Example 1 — Constant forward shift

**Q.** If **TEACHER** is coded as **VGCEJGT**, how is **STUDENT** coded?

**Step 1 — Build the shift table.**

| Letter | T | E | A | C | H | E | R |
|---|---|---|---|---|---|---|---|
| Position | 20 | 5 | 1 | 3 | 8 | 5 | 18 |
| Code | V | G | C | E | J | G | T |
| Code position | 22 | 7 | 3 | 5 | 10 | 7 | 20 |
| **Shift** | **+2** | **+2** | **+2** | **+2** | **+2** | **+2** | **+2** |

**Step 2 — The rule is a constant +2 shift.**

**Step 3 — Apply it to STUDENT.**

| Letter | S | T | U | D | E | N | T |
|---|---|---|---|---|---|---|---|
| Position | 19 | 20 | 21 | 4 | 5 | 14 | 20 |
| **+2** | 21 | 22 | 23 | 6 | 7 | 16 | 22 |
| **Code** | **U** | **V** | **W** | **F** | **G** | **P** | **V** |

**Answer: UVWFGPV**

---

### Example 2 — Backward shift with wrap-around

**Q.** If **MOUSE** is coded as **LNTRD**, how is **APPLE** coded?

**Step 1 — Determine the shift.**

| M(13) | O(15) | U(21) | S(19) | E(5) |
|---|---|---|---|---|
| L(12) | N(14) | T(20) | R(18) | D(4) |
| −1 | −1 | −1 | −1 | −1 |

The rule is a constant **−1** shift.

**Step 2 — Apply to APPLE, watching for wrap-around.**

| Letter | A | P | P | L | E |
|---|---|---|---|---|---|
| Position | 1 | 16 | 16 | 12 | 5 |
| −1 | **0 → 26** | 15 | 15 | 11 | 4 |
| **Code** | **Z** | **O** | **O** | **K** | **D** |

**Answer: ZOOKD**

> **The wrap-around on A.** Position 1 − 1 = 0, which is invalid. Add 26 to get 26 = **Z**. Missing this gives an impossible answer and is the single most common slip in shift codes.

---

### Example 3 — Opposite-letter code

**Q.** If **GARDEN** is coded as **TZIWVM**, how is **FLOWER** coded?

**Step 1 — Check the position sums.**

| Letter | G | A | R | D | E | N |
|---|---|---|---|---|---|---|
| Position | 7 | 1 | 18 | 4 | 5 | 14 |
| Code | T | Z | I | W | V | M |
| Code position | 20 | 26 | 9 | 23 | 22 | 13 |
| **Sum** | **27** | **27** | **27** | **27** | **27** | **27** |

Every pair sums to 27 ⇒ the rule is **opposite letters** (A↔Z, B↔Y, …).

**Step 2 — Apply to FLOWER using 27 − n.**

| Letter | F | L | O | W | E | R |
|---|---|---|---|---|---|---|
| Position | 6 | 12 | 15 | 23 | 5 | 18 |
| 27 − n | 21 | 15 | 12 | 4 | 22 | 9 |
| **Code** | **U** | **O** | **L** | **D** | **V** | **I** |

**Answer: UOLDVI**

> **The 27-sum check is the fastest diagnostic in this topic.** If you see A → Z or Z → A anywhere in a coded pair, test the opposite-letter rule immediately.

---

### Example 4 — Positional rearrangement

**Q.** If **CHAMBER** is coded as **REBMAHC**, how is **JOURNAL** coded?

**Step 1 — Compare the letter sets.**
CHAMBER and REBMAHC contain exactly the same letters ⇒ this is a **rearrangement**, not a shift.

**Step 2 — Identify the arrangement.**
```
C  H  A  M  B  E  R
R  E  B  M  A  H  C     ← the word written backwards
```

**Step 3 — Apply to JOURNAL.**
```
J  O  U  R  N  A  L
L  A  N  R  U  O  J
```

**Answer: LANRUOJ**

---

### Example 5 — Adjacent-pair swap

**Q.** If **MOTHER** is coded as **OMHTRE**, how is **FATHER** coded?

**Step 1 — Check the letter sets.** Identical ⇒ a rearrangement.

**Step 2 — Identify the pattern.**
```
Original:   M O | T H | E R
Code:       O M | H T | R E
             ↕     ↕     ↕
Letters are swapped WITHIN each adjacent pair.
```

**Step 3 — Apply to FATHER.**
```
Original:   F A | T H | E R
Swap each:  A F | H T | R E
```

**Answer: AFHTRE**

> **Chunk the word into pairs before swapping.** Trying to do it letter by letter invites off-by-one errors, particularly with six- and eight-letter words.

---

### Example 6 — Number-substitution code

**Q.** In a certain code, **ENGLAND** is written as **1234526** and **FRANCE** is written as **785291**. How is **GREECE** written in that code?

**Step 1 — Build the letter–digit table from ENGLAND.**

| Letter | E | N | G | L | A | N | D |
|---|---|---|---|---|---|---|---|
| Digit | 1 | 2 | 3 | 4 | 5 | 2 | 6 |

So: **E=1, N=2, G=3, L=4, A=5, D=6**
*(Note that both N's map to 2 — a consistency check that the table is correct.)*

**Step 2 — Extend the table using FRANCE.**

| Letter | F | R | A | N | C | E |
|---|---|---|---|---|---|---|
| Digit | 7 | 8 | 5 | 2 | 9 | 1 |

The overlapping letters agree: **A=5 ✓, N=2 ✓, E=1 ✓** — the table is consistent.

New entries: **F=7, R=8, C=9**

**Step 3 — Encode GREECE.**

| Letter | G | R | E | E | C | E |
|---|---|---|---|---|---|---|
| Digit | 3 | 8 | 1 | 1 | 9 | 1 |

**Answer: 381191**

> **Always verify the overlap.** If A had mapped to 5 in one word and 6 in another, your letter alignment would be wrong and you would need to re-count.

---

### Example 7 — Mixed-language substitution code

**Q.** In a certain code language:
- '**tem sur nik**' means '**apples are red**'
- '**sur pol dam**' means '**red roses bloom**'
- '**nik dam gor**' means '**are bloom now**'

Which word means '**red**'?

**Step 1 — Set out the sentences.**

```
S1:  tem  sur  nik     =  apples, are, red
S2:  sur  pol  dam     =  red, roses, bloom
S3:  nik  dam  gor     =  are, bloom, now
```

**Step 2 — Intersect S1 and S2.**
- Shared code word: **sur**
- Shared meaning: **red**
$$\implies \textbf{sur} = \textbf{red}$$

**Step 3 — Verify with the other intersections.**
- S1 ∩ S3: shared word **nik**, shared meaning **are** ⇒ nik = are ✓
- S2 ∩ S3: shared word **dam**, shared meaning **bloom** ⇒ dam = bloom ✓

**Step 4 — Fill in by elimination.**
- S1 leftover: **tem** = apples
- S2 leftover: **pol** = roses
- S3 leftover: **gor** = now

**Complete dictionary:**

| Code | Meaning |
|---|---|
| tem | apples |
| sur | **red** |
| nik | are |
| pol | roses |
| dam | bloom |
| gor | now |

**Answer: sur**

---

### Example 8 — Rule-based numeric code

**Q.** In a certain code, **REASON** is written as **5** and **BELIEVED** is written as **7**. How is **GOVERNMENT** written?

**Step 1 — The code is a single digit, so it cannot be a letter-by-letter substitution.**
Look for a **property** of the word.

**Step 2 — Count the letters.**

| Word | Letters | Code |
|---|---|---|
| REASON | 6 | 5 |
| BELIEVED | 8 | 7 |

**Step 3 — Identify the relationship.**
$$\text{Code} = \text{Number of letters} - 1$$

**Step 4 — Apply.**
GOVERNMENT has **10** letters:
$$10 - 1 = \mathbf{9}$$

**Answer: 9**

> **When a code is a single number, check these in order:**
> 1. Letter count (possibly ±1) — by far the most common
> 2. Number of vowels
> 3. Sum of letter positions
> 4. Position of the first or last letter

---

## 6. Practice Questions

**Instructions:** 50 questions. Easy (1–20), Medium (21–40), Hard (41–50).
Target: **30 seconds per question**. Full solutions in [Section 7](#7-detailed-solutions).

### 🟢 EASY (Questions 1–20)

**Q1.** If CAT is coded as DBU, how is DOG coded?
(a) EPG  (b) EPH  (c) EOH  (d) DPH

**Q2.** If BOOK is coded as CPPL, how is PEN coded?
(a) QEO  (b) QFO  (c) QFN  (d) PFO

**Q3.** If MAN is coded as LZM, how is BOY coded?
(a) ANX  (b) ANY  (c) BNX  (d) AOX

**Q4.** If A = 1, B = 2, C = 3 and so on, what is the code for CAB?
(a) 123  (b) 213  (c) 312  (d) 321

**Q5.** If RED is coded as 18-5-4, how is BLUE coded?
(a) 2-12-21-5  (b) 2-11-21-5  (c) 2-12-20-5  (d) 3-12-21-5

**Q6.** If TEA is written as AET, how is COW written?
(a) WCO  (b) OWC  (c) WOC  (d) COW

**Q7.** If SUN is coded as TVO, how is MOON coded?
(a) NPPM  (b) NPPO  (c) NOPO  (d) NPOO

**Q8.** In a certain code, DELHI is written as CDKGH. How is MUMBAI written?
(a) LTLAZH  (b) LTMAZH  (c) LTLBZH  (d) LSLAZH

**Q9.** If FAN is coded as GBO, what is the code for CAR?
(a) DBR  (b) DBS  (c) CBS  (d) DAS

**Q10.** If GO is coded as HP, what is the code for IN?
(a) JN  (b) JO  (c) IO  (d) KO

**Q11.** If BAT = 2-1-20, then CAT = ?
(a) 2-1-20  (b) 3-1-19  (c) 3-1-20  (d) 3-2-20

**Q12.** If LAMP is coded as MBNQ, how is DESK coded?
(a) EFTK  (b) EFTL  (c) EETL  (d) DFTL

**Q13.** If TIGER is written as REGIT, how is LION written?
(a) NOLI  (b) NIOL  (c) NOIL  (d) OLIN

**Q14.** If PLAY is coded as QMBZ, how is WORK coded?
(a) XPSK  (b) XPSL  (c) XOSL  (d) XPRL

**Q15.** If ROSE is coded as 1234, how is SORE coded?
(a) 3214  (b) 3124  (c) 3241  (d) 2314

**Q16.** If CAP is coded as 3-1-16, how is MAP coded?
(a) 12-1-16  (b) 13-1-16  (c) 13-2-16  (d) 13-1-15

**Q17.** If HAT is coded as IBU, how is BAT coded?
(a) CBT  (b) CAU  (c) CBU  (d) BBU

**Q18.** If DOG is coded as 4-15-7, what is the code for CAT?
(a) 3-1-19  (b) 3-1-20  (c) 3-2-20  (d) 4-1-20

**Q19.** If SIT is coded as TJU, how is RUN coded?
(a) SVN  (b) SVO  (c) SUO  (d) TVO

**Q20.** If NAME is coded as EMAN, how is FACE coded?
(a) ECAF  (b) EACF  (c) CEAF  (d) ECFA

---

### 🟡 MEDIUM (Questions 21–40)

**Q21.** If TEACHER is coded as VGCEJGT, how is STUDENT coded?
(a) UVWFGPV  (b) UVWFGPU  (c) TVWFGPV  (d) UVXFGPV

**Q22.** In a certain code, WATER is written as YCVGT. How is FIRE written?
(a) HKTG  (b) HKSG  (c) GKTG  (d) HJTG

**Q23.** If MOTHER is coded as OMHTRE, how is FATHER coded?
(a) AFHTRE  (b) AFTHER  (c) AFHTER  (d) FAHTRE

**Q24.** If 5 * 3 = 16 and 7 * 4 = 22, then 9 * 5 = ?
(a) 24  (b) 26  (c) 28  (d) 30

**Q25.** If A = 2, B = 4, C = 6 and so on, what is the code for FACE?
(a) 12-2-6-10  (b) 6-1-3-5  (c) 12-2-3-10  (d) 12-1-6-10

**Q26.** If ENGLAND is written as 1234526 and FRANCE is written as 785291, how is GREECE written?
(a) 381191  (b) 381911  (c) 318191  (d) 381891

**Q27.** If FRIEND is coded as HTKGPF, how is CANDLE coded?
(a) ECPFNG  (b) ECPFMG  (c) DCPFNG  (d) ECQFNG

**Q28.** In a certain code, PAINT is written as TNIAP. How is EXCEL written?
(a) LECEX  (b) LECXE  (c) LCEXE  (d) LEXCE

**Q29.** If '123' means 'hot filtered coffee', '356' means 'very hot day', and '589' means 'day and night', which digit stands for 'day'?
(a) 3  (b) 5  (c) 6  (d) 8

**Q30.** If '247' means 'spread the news', '203' means 'tell the truth', and '765' means 'news is bad', which digit means 'news'?
(a) 2  (b) 4  (c) 7  (d) 6

**Q31.** If REASON is coded as 5 and BELIEVED as 7, what is the code for GOVERNMENT?
(a) 8  (b) 9  (c) 10  (d) 11

**Q32.** If COMPUTER is coded as RETUPMOC, how is MACHINE coded?
(a) ENIHCAM  (b) EHINCAM  (c) ENIHACM  (d) MACHINE

**Q33.** If A = 26, B = 25, C = 24 and so on, what is the code for CAT?
(a) 24-26-7  (b) 24-26-6  (c) 23-26-7  (d) 24-25-7

**Q34.** If GARDEN is coded as TZIWVM, how is FLOWER coded?
(a) UOLDVI  (b) UOLDIV  (c) ULODVI  (d) UOLCVI

**Q35.** If MANGO is written as NBOHP, how is APPLE written?
(a) BQQMF  (b) BQQLF  (c) BPQMF  (d) BQPMF

**Q36.** If SUMMER is coded as RUMMES, how is WINTER coded?
(a) RINTEW  (b) RENTIW  (c) WINTER  (d) RITNEW

**Q37.** In a code, 2 = B, 4 = D and 6 = F. What does 20 represent?
(a) R  (b) S  (c) T  (d) U

**Q38.** If FLOWER is coded as 6-12-15-23-5-18, what is the code for ROSE?
(a) 18-15-18-5  (b) 18-15-19-5  (c) 17-15-19-5  (d) 18-14-19-5

**Q39.** If CHAIR is coded as DIBJS, what is the code for TABLE?
(a) UBCMF  (b) UBCLF  (c) UACMF  (d) UBDMF

**Q40.** In a certain code, TRAIN is written as SQZHM. How is BUS written?
(a) ATR  (b) ATS  (c) AUR  (d) BTR

---

### 🔴 HARD (Questions 41–50)

**Q41.** In a certain code language, 'pit na som' means 'bring me water', 'na jo tod' means 'water is life', and 'som tod jo' means 'bring life is'. Which word means 'bring'?
(a) pit  (b) na  (c) som  (d) tod

**Q42.** If A = 1, B = 2 and so on, and a word's code is the **sum** of its letter values, what is the code for CAB?
(a) 5  (b) 6  (c) 7  (d) 312

**Q43.** In a code, DOCTOR is written as FQEVQT. How is NURSE written?
(a) PWTUG  (b) PWTUF  (c) PVTUG  (d) OWTUG

**Q44.** If PAPER is coded as OZODQ, how is PENCIL coded?
(a) ODMBHK  (b) ODMBHL  (c) OEMBHK  (d) ODNBHK

**Q45.** If BLACK is coded as YOZXP, how is WHITE coded?
(a) DSRGV  (b) DSRGU  (c) DTRGV  (d) DSQGV

**Q46.** '5 3 8' means 'good sweet fruit', '5 7 2' means 'good tasty juice', and '8 2 9' means 'fresh fruit juice'. Which number means 'good'?
(a) 3  (b) 5  (c) 8  (d) 2

**Q47.** Using the code in Q46, which number means 'fruit'?
(a) 3  (b) 5  (c) 8  (d) 9

**Q48.** If SYSTEM is coded as SYSMET, how is FLIGHT coded?
(a) FLITHG  (b) FLIGHT  (c) FLIHTG  (d) LFITHG

**Q49.** In a certain code, HEALTH is written as GDZKSG. How is DOCTOR written?
(a) CNBSNQ  (b) CNBSNR  (c) CNCSNQ  (d) DNBSNQ

**Q50.** If SPARK is coded as TQBSL and FLAME is coded as GMBNF, what is the code for BLAZE?
(a) CMBAF  (b) CMBZF  (c) CLBAF  (d) CMCAF

---

## 7. Detailed Solutions

### 🟢 EASY — Solutions 1–20

---

**Q1. CAT → DBU. Code for DOG? → (b) EPH**

**Step 1 — Find the shift.**

| C(3) | A(1) | T(20) |
|---|---|---|
| D(4) | B(2) | U(21) |
| +1 | +1 | +1 |

Constant **+1** shift.

**Step 2 — Apply to DOG.**
$$D(4) \to E(5), \quad O(15) \to P(16), \quad G(7) \to H(8)$$

**Answer: (b) EPH**

---

**Q2. BOOK → CPPL. Code for PEN? → (b) QFO**

**Shift:** B→C, O→P, O→P, K→L ⇒ constant **+1**

**Apply:** P(16)→Q(17), E(5)→F(6), N(14)→O(15)

**Answer: (b) QFO**

---

**Q3. MAN → LZM. Code for BOY? → (a) ANX**

**Step 1 — Find the shift.**

| M(13) | A(1) | N(14) |
|---|---|---|
| L(12) | Z(26) | M(13) |
| −1 | **−1 (wrapped)** | −1 |

Note A(1) − 1 = 0 → wraps to 26 = **Z** ✓ Constant **−1** shift.

**Step 2 — Apply to BOY.**
$$B(2) \to A(1), \quad O(15) \to N(14), \quad Y(25) \to X(24)$$

**Answer: (a) ANX**

---

**Q4. A=1, B=2, … Code for CAB? → (c) 312**

$$C = 3, \quad A = 1, \quad B = 2 \implies \mathbf{312}$$

**Answer: (c) 312**

---

**Q5. RED = 18-5-4. Code for BLUE? → (a) 2-12-21-5**

**Confirm the rule:** R = 18 ✓, E = 5 ✓, D = 4 ✓ — straight positional numbering.

**Apply:** B = 2, L = 12, U = 21, E = 5

**Answer: (a) 2-12-21-5**

---

**Q6. TEA → AET. Code for COW? → (c) WOC**

**Step 1 — Check the letter sets.** TEA and AET use the same letters ⇒ rearrangement.

**Step 2 — Identify it.** AET is TEA written backwards.

**Step 3 — Apply.** COW reversed = **WOC**

**Answer: (c) WOC**

---

**Q7. SUN → TVO. Code for MOON? → (b) NPPO**

**Shift:** S→T, U→V, N→O ⇒ **+1**

**Apply:** M(13)→N(14), O(15)→P(16), O(15)→P(16), N(14)→O(15)

**Answer: (b) NPPO**

---

**Q8. DELHI → CDKGH. Code for MUMBAI? → (a) LTLAZH**

**Step 1 — Find the shift.**

| D(4) | E(5) | L(12) | H(8) | I(9) |
|---|---|---|---|---|
| C(3) | D(4) | K(11) | G(7) | H(8) |
| −1 | −1 | −1 | −1 | −1 |

**Step 2 — Apply to MUMBAI.**

| M(13) | U(21) | M(13) | B(2) | A(1) | I(9) |
|---|---|---|---|---|---|
| L(12) | T(20) | L(12) | A(1) | **Z(26)** | H(8) |

*(A wraps to Z.)*

**Answer: (a) LTLAZH**

---

**Q9. FAN → GBO. Code for CAR? → (b) DBS**

**Shift:** F→G, A→B, N→O ⇒ **+1**

**Apply:** C(3)→D(4), A(1)→B(2), R(18)→S(19)

**Answer: (b) DBS**

---

**Q10. GO → HP. Code for IN? → (b) JO**

**Shift:** G→H, O→P ⇒ **+1**

**Apply:** I(9)→J(10), N(14)→O(15)

**Answer: (b) JO**

---

**Q11. BAT = 2-1-20. Code for CAT? → (c) 3-1-20**

Straight positional numbering: C = 3, A = 1, T = 20

**Answer: (c) 3-1-20**

---

**Q12. LAMP → MBNQ. Code for DESK? → (b) EFTL**

**Shift:** L→M, A→B, M→N, P→Q ⇒ **+1**

**Apply:** D(4)→E(5), E(5)→F(6), S(19)→T(20), K(11)→L(12)

**Answer: (b) EFTL**

---

**Q13. TIGER → REGIT. Code for LION? → (c) NOIL**

**Step 1 — Same letters ⇒ rearrangement.** REGIT is TIGER reversed.

**Step 2 — Apply.** LION reversed = **NOIL**

**Answer: (c) NOIL**

---

**Q14. PLAY → QMBZ. Code for WORK? → (b) XPSL**

**Shift:** P→Q, L→M, A→B, Y→Z ⇒ **+1**

**Apply:** W(23)→X(24), O(15)→P(16), R(18)→S(19), K(11)→L(12)

**Answer: (b) XPSL**

---

**Q15. ROSE = 1234. Code for SORE? → (a) 3214**

**Step 1 — Build the table.**

| R | O | S | E |
|---|---|---|---|
| 1 | 2 | 3 | 4 |

**Step 2 — Encode SORE.**

| S | O | R | E |
|---|---|---|---|
| 3 | 2 | 1 | 4 |

**Answer: (a) 3214**

---

**Q16. CAP = 3-1-16. Code for MAP? → (b) 13-1-16**

Positional numbering: M = 13, A = 1, P = 16

**Answer: (b) 13-1-16**

---

**Q17. HAT → IBU. Code for BAT? → (c) CBU**

**Shift:** H→I, A→B, T→U ⇒ **+1**

**Apply:** B(2)→C(3), A(1)→B(2), T(20)→U(21)

**Answer: (c) CBU**

---

**Q18. DOG = 4-15-7. Code for CAT? → (b) 3-1-20**

Positional numbering: C = 3, A = 1, T = 20

**Answer: (b) 3-1-20**

---

**Q19. SIT → TJU. Code for RUN? → (b) SVO**

**Shift:** S→T, I→J, T→U ⇒ **+1**

**Apply:** R(18)→S(19), U(21)→V(22), N(14)→O(15)

**Answer: (b) SVO**

---

**Q20. NAME → EMAN. Code for FACE? → (a) ECAF**

**Step 1 — Same letters ⇒ rearrangement.** EMAN is NAME reversed.

**Step 2 — Apply.** FACE reversed = **ECAF**

**Answer: (a) ECAF**

---

### 🟡 MEDIUM — Solutions 21–40

---

**Q21. TEACHER → VGCEJGT. Code for STUDENT? → (a) UVWFGPV**

**Step 1 — Build the shift table.**

| T(20) | E(5) | A(1) | C(3) | H(8) | E(5) | R(18) |
|---|---|---|---|---|---|---|
| V(22) | G(7) | C(3) | E(5) | J(10) | G(7) | T(20) |
| +2 | +2 | +2 | +2 | +2 | +2 | +2 |

Constant **+2** shift.

**Step 2 — Apply to STUDENT.**

| S(19) | T(20) | U(21) | D(4) | E(5) | N(14) | T(20) |
|---|---|---|---|---|---|---|
| U(21) | V(22) | W(23) | F(6) | G(7) | P(16) | V(22) |

**Answer: (a) UVWFGPV**

---

**Q22. WATER → YCVGT. Code for FIRE? → (a) HKTG**

**Shift:** W(23)→Y(25), A(1)→C(3), T(20)→V(22), E(5)→G(7), R(18)→T(20) ⇒ **+2**

**Apply:** F(6)→H(8), I(9)→K(11), R(18)→T(20), E(5)→G(7)

**Answer: (a) HKTG**

---

**Q23. MOTHER → OMHTRE. Code for FATHER? → (a) AFHTRE**

**Step 1 — Same letters ⇒ rearrangement.**

**Step 2 — Identify the pattern.**
```
M O | T H | E R
O M | H T | R E     ← letters swapped WITHIN each adjacent pair
```

**Step 3 — Apply to FATHER.**
```
F A | T H | E R
A F | H T | R E
```

**Answer: (a) AFHTRE**

---

**Q24. 5 * 3 = 16 and 7 * 4 = 22. Find 9 * 5. → (c) 28**

**Step 1 — Test a relationship involving the sum.**
$$5 + 3 = 8, \quad 8 \times 2 = 16 \checkmark$$
$$7 + 4 = 11, \quad 11 \times 2 = 22 \checkmark$$

**Step 2 — The rule is 2(a + b).**

**Step 3 — Apply.**
$$2(9 + 5) = 2 \times 14 = \mathbf{28}$$

**Answer: (c) 28**

---

**Q25. A = 2, B = 4, C = 6, … Code for FACE? → (a) 12-2-6-10**

**Step 1 — Identify the rule.** Each letter's code is **twice** its alphabet position.

**Step 2 — Apply.**

| Letter | F | A | C | E |
|---|---|---|---|---|
| Position | 6 | 1 | 3 | 5 |
| **× 2** | **12** | **2** | **6** | **10** |

**Answer: (a) 12-2-6-10**

---

**Q26. ENGLAND = 1234526, FRANCE = 785291. Code for GREECE? → (a) 381191**

**Step 1 — Build the table from ENGLAND.**

| E | N | G | L | A | N | D |
|---|---|---|---|---|---|---|
| 1 | 2 | 3 | 4 | 5 | 2 | 6 |

⇒ **E=1, N=2, G=3, L=4, A=5, D=6**
*(Both N's map to 2 — a good consistency check.)*

**Step 2 — Extend using FRANCE.**

| F | R | A | N | C | E |
|---|---|---|---|---|---|
| 7 | 8 | 5 | 2 | 9 | 1 |

Overlaps agree: A=5 ✓, N=2 ✓, E=1 ✓
New: **F=7, R=8, C=9**

**Step 3 — Encode GREECE.**

| G | R | E | E | C | E |
|---|---|---|---|---|---|
| 3 | 8 | 1 | 1 | 9 | 1 |

**Answer: (a) 381191**

---

**Q27. FRIEND → HTKGPF. Code for CANDLE? → (a) ECPFNG**

**Shift:** F(6)→H(8), R(18)→T(20), I(9)→K(11), E(5)→G(7), N(14)→P(16), D(4)→F(6) ⇒ **+2**

**Apply to CANDLE:**

| C(3) | A(1) | N(14) | D(4) | L(12) | E(5) |
|---|---|---|---|---|---|
| E(5) | C(3) | P(16) | F(6) | N(14) | G(7) |

**Answer: (a) ECPFNG**

---

**Q28. PAINT → TNIAP. Code for EXCEL? → (b) LECXE**

**Step 1 — Same letters ⇒ rearrangement.** TNIAP is PAINT reversed.

**Step 2 — Apply.**
```
E X C E L
L E C X E     ← reversed
```

**Answer: (b) LECXE**

---

**Q29. Which digit stands for 'day'? → (b) 5**

**Step 1 — Set out the sentences.**
```
S1:  1 2 3  =  hot, filtered, coffee
S2:  3 5 6  =  very, hot, day
S3:  5 8 9  =  day, and, night
```

**Step 2 — Intersect S2 and S3.**
- Shared digit: **5**
- Shared meaning: **day**

$$\implies 5 = \textbf{day}$$

**Cross-check with S1 ∩ S2:** shared digit **3**, shared meaning **hot** ⇒ 3 = hot ✓ (consistent)

**Answer: (b) 5**

---

**Q30. Which digit means 'news'? → (c) 7**

**Step 1 — Set out the sentences.**
```
S1:  2 4 7  =  spread, the, news
S2:  2 0 3  =  tell, the, truth
S3:  7 6 5  =  news, is, bad
```

**Step 2 — Intersect S1 and S3.**
- Shared digit: **7**
- Shared meaning: **news**

$$\implies 7 = \textbf{news}$$

**Cross-check with S1 ∩ S2:** shared digit **2**, shared meaning **the** ⇒ 2 = the ✓

**Answer: (c) 7**

---

**Q31. REASON → 5, BELIEVED → 7. Code for GOVERNMENT? → (b) 9**

**Step 1 — The code is a single digit ⇒ it encodes a property, not the letters.**

**Step 2 — Count the letters.**

| Word | Letters | Code |
|---|---|---|
| REASON | 6 | 5 |
| BELIEVED | 8 | 7 |

**Step 3 — The rule is: letters − 1.**

**Step 4 — Apply.**
GOVERNMENT has **10** letters ⇒ code = **9**

**Answer: (b) 9**

---

**Q32. COMPUTER → RETUPMOC. Code for MACHINE? → (a) ENIHCAM**

**Step 1 — Same letters ⇒ rearrangement.** RETUPMOC is COMPUTER reversed.

**Step 2 — Apply.**
```
M A C H I N E
E N I H C A M     ← reversed
```

**Answer: (a) ENIHCAM**

---

**Q33. A = 26, B = 25, … Code for CAT? → (a) 24-26-7**

**Step 1 — Identify the rule.** This is reverse numbering: code = **27 − position**.

**Step 2 — Apply.**

| Letter | C | A | T |
|---|---|---|---|
| Position | 3 | 1 | 20 |
| 27 − n | **24** | **26** | **7** |

**Answer: (a) 24-26-7**

---

**Q34. GARDEN → TZIWVM. Code for FLOWER? → (a) UOLDVI**

**Step 1 — Test the 27-sum.**

| G(7) | A(1) | R(18) | D(4) | E(5) | N(14) |
|---|---|---|---|---|---|
| T(20) | Z(26) | I(9) | W(23) | V(22) | M(13) |
| **27** | **27** | **27** | **27** | **27** | **27** |

Every pair sums to 27 ⇒ **opposite-letter code**.

**Step 2 — Apply 27 − n to FLOWER.**

| Letter | F | L | O | W | E | R |
|---|---|---|---|---|---|---|
| Position | 6 | 12 | 15 | 23 | 5 | 18 |
| 27 − n | 21 | 15 | 12 | 4 | 22 | 9 |
| **Code** | **U** | **O** | **L** | **D** | **V** | **I** |

**Answer: (a) UOLDVI**

---

**Q35. MANGO → NBOHP. Code for APPLE? → (a) BQQMF**

**Shift:** M→N, A→B, N→O, G→H, O→P ⇒ **+1**

**Apply:**

| A(1) | P(16) | P(16) | L(12) | E(5) |
|---|---|---|---|---|
| B(2) | Q(17) | Q(17) | M(13) | F(6) |

**Answer: (a) BQQMF**

---

**Q36. SUMMER → RUMMES. Code for WINTER? → (a) RINTEW**

**Step 1 — Same letters ⇒ rearrangement.**

**Step 2 — Identify the pattern.**
```
S U M M E R
R U M M E S
↑         ↑
first and last letters SWAPPED; the middle is unchanged
```

**Step 3 — Apply to WINTER.**
```
W I N T E R    →    R I N T E W
```

**Answer: (a) RINTEW**

---

**Q37. 2 = B, 4 = D, 6 = F. What is 20? → (c) T**

**Rule:** the number is the alphabet position.

$$20 = \textbf{T}$$

*(T is one of the EJOTY anchors.)*

**Answer: (c) T**

---

**Q38. FLOWER = 6-12-15-23-5-18. Code for ROSE? → (b) 18-15-19-5**

**Confirm the rule:** F=6 ✓, L=12 ✓, O=15 ✓, W=23 ✓, E=5 ✓, R=18 ✓ — positional numbering.

**Apply:** R = 18, O = 15, S = 19, E = 5

**Answer: (b) 18-15-19-5**

---

**Q39. CHAIR → DIBJS. Code for TABLE? → (a) UBCMF**

**Shift:** C→D, H→I, A→B, I→J, R→S ⇒ **+1**

**Apply:**

| T(20) | A(1) | B(2) | L(12) | E(5) |
|---|---|---|---|---|
| U(21) | B(2) | C(3) | M(13) | F(6) |

**Answer: (a) UBCMF**

---

**Q40. TRAIN → SQZHM. Code for BUS? → (a) ATR**

**Step 1 — Find the shift.**

| T(20) | R(18) | A(1) | I(9) | N(14) |
|---|---|---|---|---|
| S(19) | Q(17) | **Z(26)** | H(8) | M(13) |
| −1 | −1 | −1 (wrapped) | −1 | −1 |

**Step 2 — Apply to BUS.**
$$B(2) \to A(1), \quad U(21) \to T(20), \quad S(19) \to R(18)$$

**Answer: (a) ATR**

---

### 🔴 HARD — Solutions 41–50

---

**Q41. Which word means 'bring'? → (c) som**

**Step 1 — Set out the three sentences.**
```
S1:  pit  na   som     =  bring, me, water
S2:  na   jo   tod     =  water, is, life
S3:  som  tod  jo      =  bring, life, is
```

**Step 2 — Intersect S1 and S3.**
- Shared code word: **som** (the only word in both)
- Shared meaning: **bring** (the only meaning in both)

$$\implies \textbf{som} = \textbf{bring}$$

**Step 3 — Verify with the other intersections.**
- S1 ∩ S2: shared word **na**, shared meaning **water** ⇒ na = water ✓
- S2 ∩ S3: shared words **jo, tod**; shared meanings **is, life**
  *(These two cannot be separated from the data given — but the question does not require it.)*

**Step 4 — Complete by elimination.**
S1 leftover: **pit = me**

**Verification table:**

| Code | Meaning |
|---|---|
| pit | me |
| na | water |
| **som** | **bring** |
| jo / tod | is / life (indeterminate pair) |

**Answer: (c) som**

> **Note on indeterminacy.** Not every substitution puzzle resolves every word. Here 'jo' and 'tod' appear together in both S2 and S3, so nothing distinguishes them. A well-set question asks only about the words that *can* be determined.

---

**Q42. A=1, B=2, …; code = sum of letter values. Code for CAB? → (b) 6**

**Step 1 — Find each letter's value.**
$$C = 3, \quad A = 1, \quad B = 2$$

**Step 2 — Sum them.**
$$3 + 1 + 2 = \mathbf{6}$$

> **Trap:** answering 312 (option d) — that is the *concatenation* code. Read whether the question asks for the digits written together or for their **sum**.

**Answer: (b) 6**

---

**Q43. DOCTOR → FQEVQT. Code for NURSE? → (a) PWTUG**

**Step 1 — Find the shift.**

| D(4) | O(15) | C(3) | T(20) | O(15) | R(18) |
|---|---|---|---|---|---|
| F(6) | Q(17) | E(5) | V(22) | Q(17) | T(20) |
| +2 | +2 | +2 | +2 | +2 | +2 |

**Step 2 — Apply to NURSE.**

| N(14) | U(21) | R(18) | S(19) | E(5) |
|---|---|---|---|---|
| P(16) | W(23) | T(20) | U(21) | G(7) |

**Answer: (a) PWTUG**

---

**Q44. PAPER → OZODQ. Code for PENCIL? → (a) ODMBHK**

**Step 1 — Find the shift.**

| P(16) | A(1) | P(16) | E(5) | R(18) |
|---|---|---|---|---|
| O(15) | **Z(26)** | O(15) | D(4) | Q(17) |
| −1 | −1 (wrapped) | −1 | −1 | −1 |

**Step 2 — Apply to PENCIL.**

| P(16) | E(5) | N(14) | C(3) | I(9) | L(12) |
|---|---|---|---|---|---|
| O(15) | D(4) | M(13) | B(2) | H(8) | K(11) |

**Answer: (a) ODMBHK**

---

**Q45. BLACK → YOZXP. Code for WHITE? → (a) DSRGV**

**Step 1 — Test the 27-sum.**

| B(2) | L(12) | A(1) | C(3) | K(11) |
|---|---|---|---|---|
| Y(25) | O(15) | Z(26) | X(24) | P(16) |
| **27** | **27** | **27** | **27** | **27** |

⇒ **opposite-letter code**.

**Step 2 — Apply 27 − n to WHITE.**

| Letter | W | H | I | T | E |
|---|---|---|---|---|---|
| Position | 23 | 8 | 9 | 20 | 5 |
| 27 − n | 4 | 19 | 18 | 7 | 22 |
| **Code** | **D** | **S** | **R** | **G** | **V** |

**Answer: (a) DSRGV**

> **Diagnostic tip:** the A → Z mapping in BLACK → YOZXP is the giveaway. Whenever you see A paired with Z (or Z with A), test the opposite-letter rule before anything else.

---

**Q46. Which number means 'good'? → (b) 5**

**Step 1 — Set out the sentences.**
```
S1:  5 3 8  =  good, sweet, fruit
S2:  5 7 2  =  good, tasty, juice
S3:  8 2 9  =  fresh, fruit, juice
```

**Step 2 — Intersect S1 and S2.**
- Shared number: **5**
- Shared meaning: **good**

$$\implies 5 = \textbf{good}$$

**Step 3 — Complete the dictionary.**
- S1 ∩ S3: shared **8**, shared **fruit** ⇒ 8 = fruit
- S2 ∩ S3: shared **2**, shared **juice** ⇒ 2 = juice
- By elimination: 3 = sweet, 7 = tasty, 9 = fresh

**Full table:**

| Number | Meaning |
|---|---|
| 2 | juice |
| 3 | sweet |
| **5** | **good** |
| 7 | tasty |
| 8 | fruit |
| 9 | fresh |

**Answer: (b) 5**

---

**Q47. Which number means 'fruit'? → (c) 8**

From the table built in Q46:
- S1 (5 3 8 = good, sweet, fruit) and S3 (8 2 9 = fresh, fruit, juice) share the number **8** and the meaning **fruit**.

$$\implies 8 = \textbf{fruit}$$

**Answer: (c) 8**

---

**Q48. SYSTEM → SYSMET. Code for FLIGHT? → (a) FLITHG**

**Step 1 — Compare letter by letter.**
```
S Y S | T E M
S Y S | M E T
─────   ─────
 same   reversed
```

The first three letters are unchanged; the last three are **reversed** (TEM → MET).

**Step 2 — Apply to FLIGHT.**
```
F L I | G H T
F L I | T H G
```

**Answer: (a) FLITHG**

> **How to spot a half-code:** if the first few letters of the code match the original exactly, the transformation is confined to the remainder. Split the word and analyse each half separately.

---

**Q49. HEALTH → GDZKSG. Code for DOCTOR? → (a) CNBSNQ**

**Step 1 — Find the shift.**

| H(8) | E(5) | A(1) | L(12) | T(20) | H(8) |
|---|---|---|---|---|---|
| G(7) | D(4) | **Z(26)** | K(11) | S(19) | G(7) |
| −1 | −1 | −1 (wrapped) | −1 | −1 | −1 |

**Step 2 — Apply to DOCTOR.**

| D(4) | O(15) | C(3) | T(20) | O(15) | R(18) |
|---|---|---|---|---|---|
| C(3) | N(14) | B(2) | S(19) | N(14) | Q(17) |

**Answer: (a) CNBSNQ**

---

**Q50. SPARK → TQBSL and FLAME → GMBNF. Code for BLAZE? → (a) CMBAF**

**Step 1 — Verify the rule against both given pairs.**

*SPARK:* S→T, P→Q, A→B, R→S, K→L ⇒ all **+1** ✓
*FLAME:* F→G, L→M, A→B, M→N, E→F ⇒ all **+1** ✓

Two independent confirmations of a constant **+1** shift.

**Step 2 — Apply to BLAZE, watching the Z.**

| Letter | B | L | A | Z | E |
|---|---|---|---|---|---|
| Position | 2 | 12 | 1 | **26** | 5 |
| +1 | 3 | 13 | 2 | **27 → 1** | 6 |
| **Code** | **C** | **M** | **B** | **A** | **F** |

**Answer: (a) CMBAF**

> **The Z wrap-around is the entire point of this question.** Z(26) + 1 = 27, which exceeds the alphabet — subtract 26 to get 1 = **A**. Option (b) CMBZF leaves the Z unchanged and is the intended trap.

---

## 8. Quick Revision Sheet

> **One page. Read 48 hours after study, and again the night before the test.**

### The alphabet (non-negotiable)

```
A1  B2  C3  D4  E5  F6  G7  H8  I9  J10 K11 L12 M13
N14 O15 P16 Q17 R18 S19 T20 U21 V22 W23 X24 Y25 Z26

ANCHORS (EJOTY):  E=5  J=10  O=15  T=20  Y=25

OPPOSITE LETTER = 27 − n
  A↔Z  B↔Y  C↔X  D↔W  E↔V  F↔U  G↔T
  H↔S  I↔R  J↔Q  K↔P  L↔O  M↔N
```

### The method

```
1.  Write the ORIGINAL and CODE letter by letter
2.  Compute the SHIFT for each pair
3.  Read the pattern:
        all equal          → constant shift
        +1,+2,+3           → increasing shift
        pairs sum to 27    → OPPOSITE letters
        same letters used  → REARRANGEMENT
        single number      → property code (count the letters first)
4.  Apply to the target
5.  VERIFY against a second given pair if available
```

### The three most common rules (test these first)

```
1.  +1 shift        ~30% of questions
2.  −1 shift        ~15%
3.  Full reversal   ~15%
```

### Rearrangement types

```
Full reversal       TEA → AET
First-last swap     SUMMER → RUMMES
Adjacent-pair swap  MOTHER → OMHTRE     (1,2)(3,4)(5,6)
Half reversal       SYSTEM → SYSMET     (first half kept, second reversed)
Rotation            LOGIC → OGICL       (first letter moves to the end)

DIAGNOSTIC: same letters in code and original ⇒ rearrangement, not a shift
```

### Numeric codes

```
A=1 positional     CAB → 3-1-2
A=26 reverse       CAT → 24-26-7      (27 − n)
A=2 doubled        FACE → 12-2-6-10   (2n)
SUM of positions   CAB → 6
LETTER COUNT       REASON(6) → 5      (letters − 1)
```

### Wrap-around

```
Z + 1 = A       Y + 2 = A       A − 1 = Z       B − 2 = Z

If position > 26  →  subtract 26
If position < 1   →  add 26
```

### Substitution languages (words or digits)

```
Find a code word appearing in exactly TWO sentences.
Find the meaning appearing in exactly THOSE SAME two sentences.
They correspond.

Repeat for all pairs, then fill the rest by elimination.
Build a TABLE — never do this in your head.

Some words may be INDETERMINATE (if two always appear together).
That is normal; the question will not ask about them.
```

### Sanity checks

```
✓ Code length = original length (unless it's a property code)
✓ Rearrangements reuse exactly the same letters
✓ A constant shift must be the same for EVERY letter — verify all
✓ Opposite codes: every position pair sums to 27
✓ Check wrap-around whenever A or Z appears
```

---

## 9. Common Mistakes

| # | Mistake | Example | Correction |
|---|---|---|---|
| 1 | **Shift checked on one letter only** | Assuming +1 from the first pair | Verify the shift on **every** letter |
| 2 | **Wrap-around ignored** | Z + 1 left as Z | Z + 1 = **A** (27 − 26 = 1) |
| 3 | **Shift vs rearrangement confused** | Hunting for a shift in TEA → AET | Same letters ⇒ rearrangement |
| 4 | **Opposite code missed** | Reading 27-sum pairs as random shifts | Test whether the positions sum to 27 |
| 5 | **Sum vs concatenation** | CAB coded as 312 when the sum is asked | Read whether it wants digits or a total |
| 6 | **Alphabet miscounted** | R read as 17 instead of 18 | Use the EJOTY anchors |
| 7 | **Substitution done mentally** | Losing track of six word-pairs | Build a table |
| 8 | **Pair-swap applied letter by letter** | Off-by-one in a six-letter word | Chunk into pairs first |
| 9 | **Half-code treated as whole** | Applying a rule to all six letters | Split and analyse each half |
| 10 | **Property code missed** | Hunting for letter substitution when the code is "5" | A single number ⇒ count the letters |
| 11 | **Second example ignored** | Using only one given pair | The second pair confirms or refutes the rule |
| 12 | **Direction reversed** | Coding when decoding is asked | Read whether you go word→code or code→word |

---

## Practice Answer Key

| Q | Ans | Q | Ans | Q | Ans | Q | Ans | Q | Ans |
|---|---|---|---|---|---|---|---|---|---|
| 1 | b | 11 | c | 21 | a | 31 | b | 41 | c |
| 2 | b | 12 | b | 22 | a | 32 | a | 42 | b |
| 3 | a | 13 | c | 23 | a | 33 | a | 43 | a |
| 4 | c | 14 | b | 24 | c | 34 | a | 44 | a |
| 5 | a | 15 | a | 25 | a | 35 | a | 45 | a |
| 6 | c | 16 | b | 26 | a | 36 | a | 46 | b |
| 7 | b | 17 | c | 27 | a | 37 | c | 47 | c |
| 8 | a | 18 | b | 28 | b | 38 | b | 48 | a |
| 9 | b | 19 | b | 29 | b | 39 | a | 49 | a |
| 10 | b | 20 | a | 30 | c | 40 | a | 50 | a |

**Scoring guide:** 45+/50 → strong. 35–44 → solid; memorise the alphabet table until recall is instant. Below 35 → the bottleneck is almost certainly alphabet recall, not reasoning — fix that first, then redo the set.

---

**⬅️ Back:** [Topic 13 — Number & Letter Series](13-number-letter-series.md) · **➡️ Next:** [Topic 15 — Blood Relations & Direction Sense](15-blood-relations-direction-sense.md)
