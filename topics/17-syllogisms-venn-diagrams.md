# Topic 17 — Syllogisms & Venn Diagrams

### EY Placement Aptitude Handbook · Priority Rank #17 · 🟠 High

> **Questions in this file are original, modelled on publicly reported EY test patterns. They are not claimed to be actual previous-year EY questions.**

---

## Contents

1. [Why This Topic Matters for EY](#1-why-this-topic-matters-for-ey)
2. [Core Concepts](#2-core-concepts)
3. [The Rule Bank](#3-the-rule-bank)
4. [Shortcuts & Tricks](#4-shortcuts--tricks)
5. [Solved Examples](#5-solved-examples)
6. [Practice Questions (50)](#6-practice-questions)
7. [Detailed Solutions](#7-detailed-solutions)
8. [Quick Revision Sheet](#8-quick-revision-sheet)
9. [Common Mistakes](#9-common-mistakes)

---

## 1. Why This Topic Matters for EY

**Weightage:** Syllogisms 7–9% · Venn-diagram set problems 4–6% of the reasoning section. Together: **1–2 questions**.

**Why this topic is worth prioritising:** syllogisms are **fully deterministic**. Unlike puzzles, there is no searching and no ambiguity — a fixed set of rules produces a fixed answer every time. Once you internalise the eight rules in Section 3, you will never get one wrong. Very few topics offer that guarantee.

**Question styles reported:**

| Style | Format |
|---|---|
| **Two-statement syllogism** | 2 statements + 2 conclusions |
| **Three-statement syllogism** | 3 statements + 2 conclusions |
| **Possibility conclusions** | "Some A being C is a possibility" |
| **Venn set problems** | "In a class of 60, 35 play cricket…" |
| **Three-set inclusion–exclusion** | Maths / Physics / Chemistry overlaps |

**The standard answer options:**

```
(a)  Only conclusion I follows
(b)  Only conclusion II follows
(c)  Either I or II follows
(d)  Neither I nor II follows
(e)  Both I and II follow
```

---

## 2. Core Concepts

### 2.1 The four statement types

Every syllogism statement is one of exactly four forms:

| Type | Form | Name | Venn representation |
|---|---|---|---|
| **A** | **All** A are B | Universal affirmative | A entirely inside B |
| **E** | **No** A is B | Universal negative | A and B disjoint |
| **I** | **Some** A are B | Particular affirmative | A and B overlap |
| **O** | **Some** A are not B | Particular negative | Part of A lies outside B |

```
   ALL A are B              NO A is B
   ┌─────────────┐          ┌─────┐  ┌─────┐
   │      B      │          │  A  │  │  B  │
   │   ┌─────┐   │          └─────┘  └─────┘
   │   │  A  │   │           (disjoint)
   │   └─────┘   │
   └─────────────┘

   SOME A are B            SOME A are not B
   ┌────┬────┬────┐        ┌────┬────┬────┐
   │ A  │ ∩  │ B  │        │ A  │ ∩  │ B  │
   └────┴────┴────┘        └────┴────┴────┘
        (overlap)          (the A-only region is non-empty)
```

### 2.2 ⭐ The golden rule of syllogisms

$$\boxed{\textbf{A conclusion follows ONLY if it is true in EVERY possible diagram}}$$

If you can draw **even one** valid Venn diagram in which the conclusion fails, the conclusion does **not** follow.

**This is the entire topic.** Every rule below is a consequence of it.

> **Do not use real-world knowledge.** If a statement says "All birds are fish", accept it. Syllogisms test *formal* validity, not truth. Bringing in what you know about birds is the fastest route to a wrong answer.

### 2.3 The conversion rules

Some statements can be validly reversed; others cannot.

| Original | Valid conversion? | Result |
|---|---|---|
| **All A are B** | ⚠️ Partial only | **Some B are A** ✓ (not "All B are A") |
| **No A is B** | ✅ Full | **No B is A** ✓ |
| **Some A are B** | ✅ Full | **Some B are A** ✓ |
| **Some A are not B** | ❌ Never | Nothing follows |

> **"All A are B" does NOT give "All B are A".** It gives only "**Some** B are A". This single asymmetry generates more wrong answers than any other rule in the topic.

### 2.4 The eight combination rules

Given two statements sharing a common term, what follows?

| Statement 1 | Statement 2 | Conclusion |
|---|---|---|
| All A are B | All B are C | **All A are C** ✓ |
| All A are B | No B is C | **No A is C** ✓ |
| Some A are B | All B are C | **Some A are C** ✓ |
| Some A are B | No B is C | **Some A are not C** ✓ |
| All A are B | Some B are C | ❌ **No conclusion** |
| Some A are B | Some B are C | ❌ **No conclusion** |
| No A is B | No B is C | ❌ **No conclusion** |
| Some A are not B | Anything | ❌ **No conclusion** |

**Three master principles that generate all of the above:**

```
1.  Two PARTICULAR statements ("some") ⇒ NO conclusion
2.  Two NEGATIVE statements ("no" / "some…not") ⇒ NO conclusion
3.  The conclusion inherits the WEAKER quality:
        one particular premise  ⇒  particular conclusion
        one negative premise    ⇒  negative conclusion
```

### 2.5 ⭐ The "Either–Or" case (complementary pairs)

Sometimes **neither** conclusion follows individually, yet **one of them must be true**. The answer is then **"Either I or II follows"**.

**This happens only when the two conclusions form a complementary pair:**

| Pair | Complementary? |
|---|---|
| "Some A are B" and "No A is B" | ✅ Yes |
| "All A are B" and "Some A are not B" | ✅ Yes |
| "Some A are B" and "Some A are not B" | ❌ No (both can be true) |
| "All A are B" and "No A is B" | ❌ No (both can be false) |

**The three-part test:**

```
1.  Does conclusion I follow on its own?      NO
2.  Does conclusion II follow on its own?     NO
3.  Do I and II have the SAME subject and predicate,
    and are they logical opposites?            YES
        ⇒ ANSWER: "Either I or II follows"
```

**Worked instance:**
> Statements: Some books are pens. Some pens are pencils.
> Conclusions: I. Some books are pencils. II. No book is a pencil.
>
> Two particular premises ⇒ neither conclusion follows individually.
> But "Some books are pencils" and "No book is a pencil" are exact opposites — one of them *must* be true.
> **Answer: Either I or II follows.**

### 2.6 Possibility conclusions

A conclusion phrased *"Some A being B is a possibility"* follows if the situation is **not ruled out** by the statements.

```
"…is a possibility" FOLLOWS   ⇔  the statements do NOT forbid it
"…is a possibility" FAILS     ⇔  the statements make it IMPOSSIBLE
```

> Statements: All A are B. Some B are C.
> Conclusion: "Some A being C is a possibility." — **Follows**, because nothing prevents the A-region from overlapping C.

> Statements: All A are B. No B is C.
> Conclusion: "Some A being C is a possibility." — **Does not follow**, because A lies inside B and B is disjoint from C, so A can never touch C.

### 2.7 Venn diagrams for set counting

A separate but related question type: numerical set problems.

**Two sets:**

$$n(A \cup B) = n(A) + n(B) - n(A \cap B)$$
$$\text{Only A} = n(A) - n(A \cap B)$$
$$\text{Neither} = \text{Total} - n(A \cup B)$$

```
        ┌──────────────────────────────────┐
        │  TOTAL                           │
        │    ┌─────────┬─────────┐         │
        │    │  Only   │  Only   │         │
        │    │    A    │∩│  B    │         │
        │    └─────────┴─────────┘         │
        │                     NEITHER      │
        └──────────────────────────────────┘
```

**Three sets — inclusion–exclusion:**

$$n(A \cup B \cup C) = n(A) + n(B) + n(C) - n(A\cap B) - n(B\cap C) - n(C\cap A) + n(A\cap B\cap C)$$

**Region formulas (three sets):**

| Region | Formula |
|---|---|
| Only A | $n(A) - n(A\cap B) - n(A\cap C) + n(A\cap B\cap C)$ |
| Exactly A and B (not C) | $n(A\cap B) - n(A\cap B\cap C)$ |
| All three | $n(A\cap B\cap C)$ |
| None | Total $- \; n(A\cup B\cup C)$ |

> **Watch the "+ all three" term in the Only-A formula.** Subtracting both pairwise overlaps removes the triple region twice, so it must be added back once.

---

## 3. The Rule Bank

| # | Rule | Result |
|---|---|---|
| 1 | All A are B + All B are C | All A are C |
| 2 | All A are B + No B is C | No A is C |
| 3 | Some A are B + All B are C | Some A are C |
| 4 | Some A are B + No B is C | Some A are not C |
| 5 | No A is B + All C are B | No A is C |
| 6 | All A are B + Some B are C | **No conclusion** |
| 7 | Some A are B + Some B are C | **No conclusion** |
| 8 | No A is B + No B is C | **No conclusion** |
| 9 | Some A are not B + anything | **No conclusion** |
| 10 | Conversion: All A are B | ⇒ **Some** B are A |
| 11 | Conversion: No A is B | ⇒ No B is A |
| 12 | Conversion: Some A are B | ⇒ Some B are A |
| 13 | Conversion: Some A are not B | ⇒ **nothing** |
| 14 | Two particulars | **No conclusion** |
| 15 | Two negatives | **No conclusion** |
| 16 | Conclusion quality | Follows the **weaker** premise |
| 17 | Complementary pair, neither follows alone | **Either–Or** |
| 18 | Possibility conclusion | Follows unless **forbidden** |
| 19 | Two-set union | $n(A)+n(B)-n(A\cap B)$ |
| 20 | Three-set union | $\sum n - \sum n(\text{pairs}) + n(\text{triple})$ |
| 21 | Only A (two sets) | $n(A) - n(A\cap B)$ |
| 22 | Only A (three sets) | $n(A) - n(A\cap B) - n(A\cap C) + n(A\cap B\cap C)$ |

---

## 4. Shortcuts & Tricks

### 4.1 The instant-elimination checklist

Before drawing anything, scan the two statements:

```
□  Both contain "some"?          →  NO conclusion (check Either–Or)
□  Both are negative?            →  NO conclusion
□  One is "Some…are not"?        →  NO conclusion from it
□  Is there a common term?       →  if not, NO conclusion
```

This resolves a large fraction of questions in five seconds.

### 4.2 The chain test

Valid syllogisms form a **chain** through the common term:

```
All A → All B → All C          ⇒  All A are C          ✓
Some A → All B → All C         ⇒  Some A are C         ✓
All A → No B ✗ C               ⇒  No A is C            ✓

All A → Some B (broken chain)  ⇒  NOTHING              ✗
Some A → Some B (broken)       ⇒  NOTHING              ✗
```

**The chain breaks whenever the SECOND statement is particular ("some").** A "some" premise cannot carry a universal conclusion forward.

### 4.3 Test conclusions by drawing the counter-case

To disprove a conclusion, draw the *least favourable* diagram.

> Statements: All cars are vehicles. Some vehicles are buses.
> Conclusion: Some cars are buses.
>
> **Draw the counter-case:** put the bus circle overlapping vehicles but entirely **outside** cars.
```
   ┌────────── VEHICLES ──────────┐
   │  ┌──────┐          ┌──────┐  │
   │  │ CARS │          │      │──┼── BUSES
   │  └──────┘          └──────┘  │
   └──────────────────────────────┘
```
> A valid diagram exists in which no car is a bus ⇒ the conclusion **does not follow**.

**One counter-diagram is enough.** You do not need to enumerate all cases.

### 4.4 The reliable conversions

Even when the main chain yields nothing, a **conversion** of one statement may be a valid conclusion.

| Statement given | Conclusion that always follows |
|---|---|
| Some vehicles are buses | **Some buses are vehicles** ✓ |
| No bird is a fish | **No fish is a bird** ✓ |
| All teachers are graduates | **Some graduates are teachers** ✓ |

> Many questions include one conclusion that is merely a conversion of a premise. Spotting it is free marks — it always follows.

### 4.5 The Either–Or detector

```
Neither conclusion follows individually?
    ↓
Do they share the SAME subject and predicate?
    ↓
Are they logical OPPOSITES?
    ↓
    YES  →  "Either I or II follows"
    NO   →  "Neither follows"

COMPLEMENTARY PAIRS:
    Some A are B      ↔  No A is B
    All A are B       ↔  Some A are not B
```

### 4.6 The negative-existence conclusions

These follow more often than candidates expect:

> **No A is B, and All B are C** ⇒ **Some C are not A** ✓
> *(The B's are inside C and outside A, so part of C lies outside A.)*

> **All A are B, and No B is C** ⇒ **Some C are not A** ✓ (and **No A is C** ✓)

**The assumption:** standard syllogism convention treats every named set as **non-empty**. That is what licenses "some C are not A" from "no A is B, all B are C".

### 4.7 Venn counting — the two working formulas

```
TWO SETS
    At least one  =  n(A) + n(B) − n(A∩B)
    Neither       =  Total − (at least one)
    Only A        =  n(A) − n(A∩B)
    Both (from neither) = n(A) + n(B) − [Total − Neither]

THREE SETS
    Union   =  ΣSingles − ΣPairs + Triple
    Only A  =  n(A) − n(A∩B) − n(A∩C) + n(A∩B∩C)
```

### 4.8 Sanity checks

```
✓ "All A are B" NEVER gives "All B are A"
✓ Two "some" statements NEVER give a definite conclusion
✓ Two negatives NEVER give a conclusion
✓ Either–Or requires the conclusions to be exact opposites
✓ A "possibility" conclusion follows unless it is IMPOSSIBLE
✓ Venn: the sum of all regions must equal the total
✓ No region can be negative — if one is, re-read the data
```

---

## 5. Solved Examples

### Example 1 — The basic chain

**Q.** Statements: All roses are flowers. All flowers are plants.
Conclusions: I. All roses are plants. II. Some plants are roses.

**Step 1 — Draw the diagram.**
```
   ┌──────────── PLANTS ────────────┐
   │  ┌──────── FLOWERS ────────┐   │
   │  │     ┌── ROSES ──┐       │   │
   │  │     └───────────┘       │   │
   │  └─────────────────────────┘   │
   └────────────────────────────────┘
```

**Step 2 — Test conclusion I.**
Roses ⊂ Flowers ⊂ Plants ⇒ every rose is a plant.
$$\text{I \textbf{follows}} \checkmark$$

**Step 3 — Test conclusion II.**
"All roses are plants" converts partially to "**Some** plants are roses" — a valid conversion (roses exist and are inside plants).
$$\text{II \textbf{follows}} \checkmark$$

**Answer: (e) Both I and II follow**

> **Note what would NOT follow:** "All plants are roses". Conversion of a universal affirmative yields only a *particular*.

---

### Example 2 — The broken chain

**Q.** Statements: All pens are books. Some books are papers.
Conclusions: I. Some pens are papers. II. All books are pens.

**Step 1 — Check the chain.**
The second statement is **particular** ("some books"), so the chain from pens through books to papers is broken.

**Step 2 — Draw a counter-diagram for conclusion I.**
```
   ┌────────── BOOKS ──────────┐
   │  ┌──────┐                 │
   │  │ PENS │        ┌────────┼───── PAPERS
   │  └──────┘        └────────┼
   └───────────────────────────┘
```
The papers overlap the books in a region entirely outside pens.
$$\text{I does \textbf{not} follow} ✗$$

**Step 3 — Test conclusion II.**
"All pens are books" gives only "**Some** books are pens", never "All books are pens".
$$\text{II does \textbf{not} follow} ✗$$

**Step 4 — Check for a complementary pair.**
I ("Some pens are papers") and II ("All books are pens") have different subjects and predicates ⇒ **not complementary**, so the Either–Or case does not apply.

**Answer: (d) Neither I nor II follows**

---

### Example 3 — Some + All (valid chain)

**Q.** Statements: Some men are doctors. All doctors are educated.
Conclusions: I. Some men are educated. II. All men are educated.

**Step 1 — Check the chain.**
The second statement is **universal**, so the chain holds:
$$\text{Some men} \to \text{doctors} \to \text{all educated}$$

**Step 2 — Test conclusion I.**
Those men who are doctors must be educated (since all doctors are).
$$\text{I \textbf{follows}} \checkmark$$

**Step 3 — Test conclusion II.**
Only *some* men are doctors. The remaining men are unconstrained.
```
   ┌──────── EDUCATED ────────┐
   │   ┌── DOCTORS ──┐        │
   │   │      ┌──────┼────────┼──── MEN
   │   └──────┴──────┘        │
   └──────────────────────────┘
        ↑ part of MEN lies outside EDUCATED
```
$$\text{II does \textbf{not} follow} ✗$$

**Answer: (a) Only conclusion I follows**

> **The quality rule at work:** one particular premise ⇒ the conclusion can only be **particular**. "All men are educated" is universal and therefore impossible from this pair.

---

### Example 4 — The Either–Or case

**Q.** Statements: Some fruits are sweet. Some sweet things are costly.
Conclusions: I. Some fruits are costly. II. No fruit is costly.

**Step 1 — Apply the instant check.**
Both statements are **particular** ⇒ no definite conclusion follows.

**Step 2 — Confirm that neither conclusion follows individually.**

*Counter-diagram for I* — the costly things overlap sweet but avoid fruits entirely:
```
   FRUITS ──┬── SWEET ──┬── COSTLY
            └───────────┘
   (no overlap between fruits and costly)
```
⇒ I does not follow ✗

*Counter-diagram for II* — the costly things overlap the fruit∩sweet region:
```
   FRUITS ──┬── SWEET
            └── COSTLY overlapping the shared region
```
⇒ II does not follow ✗

**Step 3 — Apply the complementary test.**
```
I :  Some fruits ARE costly
II:  No fruit IS costly

Same subject (fruits), same predicate (costly), exact opposites.
```
One of them **must** be true — either at least one fruit is costly, or none is. There is no third possibility.

**Answer: (c) Either I or II follows**

---

### Example 5 — Universal negative

**Q.** Statements: All apples are fruits. No fruit is a vegetable.
Conclusions: I. No apple is a vegetable. II. Some vegetables are fruits.

**Step 1 — Draw.**
```
   ┌───────── FRUITS ─────────┐        ┌──────────────┐
   │    ┌── APPLES ──┐        │        │  VEGETABLES  │
   │    └────────────┘        │        └──────────────┘
   └──────────────────────────┘         (entirely separate)
```

**Step 2 — Test conclusion I.**
Apples lie inside fruits; fruits are disjoint from vegetables ⇒ apples cannot be vegetables.
$$\text{I \textbf{follows}} \checkmark$$

*(This is Rule 2: All A are B + No B is C ⇒ No A is C.)*

**Step 3 — Test conclusion II.**
"No fruit is a vegetable" directly **contradicts** "Some vegetables are fruits".
$$\text{II does \textbf{not} follow} ✗$$

**Answer: (a) Only conclusion I follows**

---

### Example 6 — Three statements

**Q.** Statements: Some pens are markers. All markers are pencils. No pencil is red.
Conclusions: I. Some pens are not red. II. No marker is red.

**Step 1 — Draw the nested structure.**
```
   ┌──────────── PENCILS ────────────┐      ┌────────┐
   │    ┌──── MARKERS ────┐          │      │  RED   │
   │    │   ┌─────────────┼──────────┼──────┼─ PENS  │
   │    └───┴─────────────┘          │      └────────┘
   └─────────────────────────────────┘   (disjoint from pencils)
```

**Step 2 — Test conclusion I.**
Chain: some pens are markers → all markers are pencils → no pencil is red.
$$\text{Those pens are markers} \to \text{pencils} \to \text{not red}$$
$$\text{I \textbf{follows}} \checkmark$$

*(Rule 4: Some A are B + [B ⊂ C] + No C is D ⇒ Some A are not D.)*

**Step 3 — Test conclusion II.**
All markers are pencils, and no pencil is red ⇒ no marker can be red.
$$\text{II \textbf{follows}} \checkmark$$

*(Rule 2 applied to markers, pencils and red.)*

**Answer: (e) Both I and II follow**

---

### Example 7 — Two-set Venn counting

**Q.** In a group of 200 people, 120 like tea, 90 like coffee, and 30 like neither. How many like both?

**Step 1 — Find how many like at least one.**
$$n(\text{at least one}) = 200 - 30 = 170$$

**Step 2 — Apply the union formula.**
$$n(T \cup C) = n(T) + n(C) - n(T \cap C)$$
$$170 = 120 + 90 - n(T \cap C)$$

**Step 3 — Solve.**
$$n(T \cap C) = 210 - 170 = 40$$

**Step 4 — Verify by filling the regions.**

| Region | Count |
|---|---|
| Only tea | 120 − 40 = **80** |
| Both | **40** |
| Only coffee | 90 − 40 = **50** |
| Neither | **30** |
| **Total** | **200** ✓ |

**Answer: 40 people like both**

---

### Example 8 — Three-set inclusion–exclusion

**Q.** In a class of 80 students, 45 study Mathematics, 40 study Physics and 35 study Chemistry. 20 study both Mathematics and Physics, 15 study both Physics and Chemistry, 18 study both Mathematics and Chemistry, and 10 study all three.
Find (a) how many study at least one subject, (b) how many study none, and (c) how many study only Mathematics.

**(a) At least one — the inclusion–exclusion formula.**

$$n(M \cup P \cup C) = \sum n - \sum n(\text{pairs}) + n(\text{triple})$$
$$= (45 + 40 + 35) - (20 + 15 + 18) + 10$$
$$= 120 - 53 + 10 = 77$$

**(b) None.**
$$80 - 77 = 3$$

**(c) Only Mathematics.**
$$n(M) - n(M\cap P) - n(M\cap C) + n(M\cap P\cap C)$$
$$= 45 - 20 - 18 + 10 = 17$$

**Full region breakdown (worth constructing as a check):**

| Region | Calculation | Count |
|---|---|---|
| Only M | 45 − 20 − 18 + 10 | 17 |
| Only P | 40 − 20 − 15 + 10 | 15 |
| Only C | 35 − 15 − 18 + 10 | 12 |
| M and P only | 20 − 10 | 10 |
| P and C only | 15 − 10 | 5 |
| M and C only | 18 − 10 | 8 |
| All three | — | 10 |
| **Union** | 17+15+12+10+5+8+10 | **77** ✓ |
| None | 80 − 77 | 3 |
| **Total** | | **80** ✓ |

**Answer: (a) 77 (b) 3 (c) 17**

> **Why "+ 10" appears in the Only-M formula.** Subtracting both pairwise overlaps removes the triple-overlap region **twice**, so it must be added back **once** to leave it correctly excluded exactly once.

---

## 6. Practice Questions

**Instructions:** Q1–40 are syllogisms; Q41–49 are Venn set problems; Q50 is a syllogism.

**For all syllogism questions, choose from:**
```
(a)  Only conclusion I follows
(b)  Only conclusion II follows
(c)  Either I or II follows
(d)  Neither I nor II follows
(e)  Both I and II follow
```

**In every syllogism, take the statements to be true even if they contradict common knowledge.**
Full solutions in [Section 7](#7-detailed-solutions).

---

### 🟢 EASY (Questions 1–20)

**Q1.** Statements: All cats are animals. All animals are living things.
Conclusions: I. All cats are living things. II. Some living things are cats.

**Q2.** Statements: All pens are books. Some books are papers.
Conclusions: I. Some pens are papers. II. All books are pens.

**Q3.** Statements: No dog is a cat. All cats are pets.
Conclusions: I. Some pets are not dogs. II. No dog is a pet.

**Q4.** Statements: All flowers are red. All red things are bright.
Conclusions: I. All flowers are bright. II. Some bright things are flowers.

**Q5.** Statements: Some men are doctors. All doctors are educated.
Conclusions: I. Some men are educated. II. All men are educated.

**Q6.** Statements: All birds fly. Some birds are parrots.
Conclusions: I. Some parrots fly. II. All parrots fly.

**Q7.** Statements: All A are B. No B is C.
Conclusions: I. No A is C. II. Some C are not A.

**Q8.** Statements: Some books are pens. Some pens are pencils.
Conclusions: I. Some books are pencils. II. No book is a pencil.

**Q9.** Statements: All roses are flowers. Some flowers fade quickly.
Conclusions: I. Some roses fade quickly. II. All flowers are roses.

**Q10.** Statements: All squares are rectangles. All rectangles are quadrilaterals.
Conclusions: I. All squares are quadrilaterals. II. Some quadrilaterals are squares.

**Q11.** Statements: No student is lazy. Some lazy people are rich.
Conclusions: I. Some rich people are not students. II. No rich person is a student.

**Q12.** Statements: All apples are fruits. No fruit is a vegetable.
Conclusions: I. No apple is a vegetable. II. Some vegetables are fruits.

**Q13.** Statements: Some pens are red. All red things are bright.
Conclusions: I. Some pens are bright. II. All pens are bright.

**Q14.** Statements: All cars are vehicles. Some vehicles are buses.
Conclusions: I. Some cars are buses. II. Some buses are vehicles.

**Q15.** Statements: All teachers are graduates. Some graduates are rich.
Conclusions: I. Some teachers are rich. II. Some rich people are graduates.

**Q16.** Statements: No bird is a fish. All fish swim.
Conclusions: I. Some swimmers are not birds. II. All swimmers are fish.

**Q17.** Statements: All metals conduct electricity. Copper is a metal.
Conclusions: I. Copper conducts electricity. II. All conductors are metals.

**Q18.** Statements: Some chairs are tables. All tables are wooden.
Conclusions: I. Some chairs are wooden. II. All chairs are wooden.

**Q19.** Statements: All boys are students. No student is a teacher.
Conclusions: I. No boy is a teacher. II. Some students are boys.

**Q20.** Statements: Some fruits are sweet. Some sweet things are costly.
Conclusions: I. Some fruits are costly. II. No fruit is costly.

---

### 🟡 MEDIUM (Questions 21–40)

**Q21.** Statements: All pens are pencils. Some pencils are erasers. All erasers are sharpeners.
Conclusions: I. Some pencils are sharpeners. II. Some pens are sharpeners.

**Q22.** Statements: All dogs are animals. All animals are mammals. No mammal is a bird.
Conclusions: I. No dog is a bird. II. Some mammals are dogs.

**Q23.** Statements: Some A are B. No B is C. All C are D.
Conclusions: I. Some A are not C. II. Some D are not B.

**Q24.** Statements: All papers are books. All books are novels. Some novels are magazines.
Conclusions: I. Some papers are magazines. II. Some books are magazines.

**Q25.** Statements: No table is a chair. Some chairs are stools. All stools are wooden.
Conclusions: I. Some wooden things are not tables. II. Some stools are not tables.

**Q26.** Statements: All singers are dancers. Some dancers are actors.
Conclusions: I. Some singers are actors. II. Some actors are dancers.

**Q27.** Statements: Some pens are markers. All markers are pencils. No pencil is red.
Conclusions: I. Some pens are not red. II. No marker is red.

**Q28.** Statements: All lions are wild. Some wild animals are tame.
Conclusions: I. Some lions are tame. II. Some tame animals are wild.

**Q29.** Statements: Some X are Y. All Y are Z. Some Z are W.
Conclusions: I. Some X are Z. II. Some X are W.

**Q30.** Statements: No P is Q. All Q are R.
Conclusions: I. Some R are not P. II. All R are Q.

**Q31.** Statements: All students are hardworking. All hardworking people are successful. Some successful people are rich.
Conclusions: I. All students are successful. II. Some students are rich.

**Q32.** Statements: Some birds are crows. All crows are black. No black thing is white.
Conclusions: I. Some birds are not white. II. Some crows are not white.

**Q33.** Statements: All boxes are cartons. Some cartons are packets.
Conclusions: I. Some boxes are packets. II. Some packets are cartons.

**Q34.** Statements: Some cups are plates. Some plates are bowls. Some bowls are glasses.
Conclusions: I. Some cups are bowls. II. Some plates are glasses.

**Q35.** Statements: All keys are locks. No lock is a door.
Conclusions: I. No key is a door. II. Some locks are keys.

**Q36.** Statements: All engineers are graduates. Some graduates are doctors. All doctors are professionals.
Conclusions: I. Some graduates are professionals. II. Some engineers are professionals.

**Q37.** Statements: Some ropes are threads. No thread is a wire.
Conclusions: I. Some ropes are not wires. II. All ropes are wires.

**Q38.** Statements: All fruits are tasty. Some tasty things are costly. All costly things are rare.
Conclusions: I. Some tasty things are rare. II. Some fruits are rare.

**Q39.** Statements: No cat is a rat. All rats are rodents.
Conclusions: I. Some rodents are not cats. II. No rodent is a cat.

**Q40.** Statements: Some pens are blue. Some blue things are ink.
Conclusions: I. Some pens are ink. II. Some ink is pens.

---

### 🔴 HARD — Venn set problems (Questions 41–49) and syllogism (Q50)

**Q41.** In a class of 60 students, 35 play cricket, 30 play football and 15 play both. How many play neither game?
(a) 5  (b) 10  (c) 15  (d) 20

**Q42.** In a survey of 100 people, 60 read newspaper A, 45 read newspaper B and 25 read both. How many read at least one newspaper?
(a) 75  (b) 80  (c) 85  (d) 105

**Q43.** Using the data of Q42, how many read only newspaper A?
(a) 25  (b) 30  (c) 35  (d) 40

**Q44.** In a group of 200 people, 120 like tea, 90 like coffee and 30 like neither. How many like both?
(a) 30  (b) 40  (c) 50  (d) 60

**Q45.** In a class of 80 students, 45 study Mathematics, 40 study Physics and 35 study Chemistry. 20 study Mathematics and Physics, 15 study Physics and Chemistry, 18 study Mathematics and Chemistry, and 10 study all three. How many study at least one subject?
(a) 70  (b) 74  (c) 77  (d) 80

**Q46.** Using the data of Q45, how many students study none of the three subjects?
(a) 3  (b) 5  (c) 6  (d) 10

**Q47.** Using the data of Q45, how many students study only Mathematics?
(a) 7  (b) 12  (c) 15  (d) 17

**Q48.** In a group of 150 people, 90 speak Hindi, 70 speak English and 40 speak both. How many speak only English?
(a) 20  (b) 30  (c) 40  (d) 50

**Q49.** Using the data of Q48, how many speak neither Hindi nor English?
(a) 20  (b) 30  (c) 40  (d) 50

**Q50.** Statements: All A are B. Some B are C. No C is D. All D are E.
Conclusions: I. Some B are not D. II. Some E are not C.

---

## 7. Detailed Solutions

### 🟢 EASY — Solutions 1–20

---

**Q1. All cats are animals; all animals are living. → (e) Both follow**

**Diagram:**
```
   ┌──────── LIVING ────────┐
   │  ┌──── ANIMALS ────┐   │
   │  │   ┌─ CATS ─┐    │   │
   │  │   └────────┘    │   │
   │  └─────────────────┘   │
   └────────────────────────┘
```

**I. All cats are living things** — Rule 1 (All + All chain) ⇒ **follows** ✓

**II. Some living things are cats** — the partial conversion of "All cats are living things" ⇒ **follows** ✓

**Answer: (e) Both I and II follow**

---

**Q2. All pens are books; some books are papers. → (d) Neither follows**

**I. Some pens are papers** — the second premise is particular, so the chain breaks.

*Counter-diagram:* place papers overlapping books but entirely outside pens ⇒ **does not follow** ✗

**II. All books are pens** — "All pens are books" gives only "**Some** books are pens", never the full converse ⇒ **does not follow** ✗

**Complementary check:** different subjects and predicates ⇒ not an Either–Or pair.

**Answer: (d) Neither I nor II follows**

---

**Q3. No dog is a cat; all cats are pets. → (a) Only I**

**Diagram:**
```
   ┌────── PETS ──────┐
   │   ┌── CATS ──┐   │        ┌──────┐
   │   └──────────┘   │        │ DOGS │
   └──────────────────┘        └──────┘
```

**I. Some pets are not dogs** — cats are pets, and no cat is a dog, so those pets are not dogs ⇒ **follows** ✓

**II. No dog is a pet** — nothing prevents dogs from also being pets (the dog circle could overlap the pets circle outside the cats region) ⇒ **does not follow** ✗

**Answer: (a) Only conclusion I follows**

---

**Q4. All flowers are red; all red are bright. → (e) Both follow**

**I. All flowers are bright** — Rule 1 chain ⇒ **follows** ✓

**II. Some bright things are flowers** — partial conversion ⇒ **follows** ✓

**Answer: (e) Both I and II follow**

---

**Q5. Some men are doctors; all doctors are educated. → (a) Only I**

**I. Some men are educated** — Rule 3 (Some + All) ⇒ **follows** ✓

**II. All men are educated** — only *some* men are doctors; the rest are unconstrained ⇒ **does not follow** ✗

> **The quality rule:** a particular premise cannot yield a universal conclusion.

**Answer: (a) Only conclusion I follows**

---

**Q6. All birds fly; some birds are parrots. → (a) Only I**

**I. Some parrots fly** — those parrots that are birds must fly (all birds fly). Since "some birds are parrots" guarantees such parrots exist ⇒ **follows** ✓

**II. All parrots fly** — the statements do not say that *all* parrots are birds; some parrots could lie outside the bird circle ⇒ **does not follow** ✗

> **Ignore real-world knowledge.** You know all parrots are birds, but the *statements* do not say so — and formal validity is what is being tested.

**Answer: (a) Only conclusion I follows**

---

**Q7. All A are B; no B is C. → (e) Both follow**

**Diagram:**
```
   ┌──── B ────┐        ┌─────┐
   │  ┌─ A ─┐  │        │  C  │
   │  └─────┘  │        └─────┘
   └───────────┘
```

**I. No A is C** — Rule 2 (All + No) ⇒ **follows** ✓

**II. Some C are not A** — since no A is C, every member of C lies outside A. Taking C as non-empty ⇒ **follows** ✓

**Answer: (e) Both I and II follow**

---

**Q8. Some books are pens; some pens are pencils. → (c) Either I or II**

**Step 1 — Two particular premises ⇒ no definite conclusion.**

**I. Some books are pencils** — a counter-diagram with no overlap exists ⇒ ✗
**II. No book is a pencil** — a counter-diagram with an overlap exists ⇒ ✗

**Step 2 — Complementary test.**
```
I :  Some books ARE pencils
II:  NO book IS a pencil
```
Same subject, same predicate, exact opposites ⇒ one must be true.

**Answer: (c) Either I or II follows**

---

**Q9. All roses are flowers; some flowers fade quickly. → (d) Neither**

**I. Some roses fade quickly** — the second premise is particular, so the chain breaks. The fading flowers could all lie outside roses ⇒ ✗

**II. All flowers are roses** — invalid full conversion ⇒ ✗

**Complementary check:** different subjects ⇒ not a pair.

**Answer: (d) Neither I nor II follows**

---

**Q10. All squares are rectangles; all rectangles are quadrilaterals. → (e) Both follow**

**I. All squares are quadrilaterals** — Rule 1 chain ⇒ **follows** ✓
**II. Some quadrilaterals are squares** — partial conversion ⇒ **follows** ✓

**Answer: (e) Both I and II follow**

---

**Q11. No student is lazy; some lazy people are rich. → (a) Only I**

**I. Some rich people are not students** — those lazy people who are rich cannot be students (no student is lazy) ⇒ **follows** ✓

**II. No rich person is a student** — other rich people, who are not lazy, could well be students ⇒ **does not follow** ✗

**Answer: (a) Only conclusion I follows**

---

**Q12. All apples are fruits; no fruit is a vegetable. → (a) Only I**

**I. No apple is a vegetable** — Rule 2 ⇒ **follows** ✓
**II. Some vegetables are fruits** — directly contradicts the second premise ⇒ ✗

**Answer: (a) Only conclusion I follows**

---

**Q13. Some pens are red; all red things are bright. → (a) Only I**

**I. Some pens are bright** — Rule 3 (Some + All) ⇒ **follows** ✓
**II. All pens are bright** — only some pens are red ⇒ ✗

**Answer: (a) Only conclusion I follows**

---

**Q14. All cars are vehicles; some vehicles are buses. → (b) Only II**

**I. Some cars are buses** — the chain breaks at the particular second premise.

*Counter-diagram:*
```
   ┌───────── VEHICLES ─────────┐
   │  ┌──────┐        ┌─────────┼──── BUSES
   │  │ CARS │        └─────────┼
   │  └──────┘                  │
   └────────────────────────────┘
```
⇒ **does not follow** ✗

**II. Some buses are vehicles** — the valid conversion of "Some vehicles are buses" ⇒ **follows** ✓

**Answer: (b) Only conclusion II follows**

---

**Q15. All teachers are graduates; some graduates are rich. → (b) Only II**

**I. Some teachers are rich** — broken chain (particular second premise) ⇒ ✗
**II. Some rich people are graduates** — conversion of "Some graduates are rich" ⇒ **follows** ✓

**Answer: (b) Only conclusion II follows**

---

**Q16. No bird is a fish; all fish swim. → (a) Only I**

**I. Some swimmers are not birds** — fish swim and no fish is a bird, so those swimmers are not birds ⇒ **follows** ✓
**II. All swimmers are fish** — other creatures could swim ⇒ ✗

**Answer: (a) Only conclusion I follows**

---

**Q17. All metals conduct; copper is a metal. → (a) Only I**

**I. Copper conducts electricity** — copper ⊂ metals ⊂ conductors ⇒ **follows** ✓
**II. All conductors are metals** — invalid full conversion; non-metals could conduct ⇒ ✗

**Answer: (a) Only conclusion I follows**

---

**Q18. Some chairs are tables; all tables are wooden. → (a) Only I**

**I. Some chairs are wooden** — Rule 3 ⇒ **follows** ✓
**II. All chairs are wooden** — only some chairs are tables ⇒ ✗

**Answer: (a) Only conclusion I follows**

---

**Q19. All boys are students; no student is a teacher. → (e) Both follow**

**I. No boy is a teacher** — Rule 2 ⇒ **follows** ✓
**II. Some students are boys** — partial conversion of "All boys are students" ⇒ **follows** ✓

**Answer: (e) Both I and II follow**

---

**Q20. Some fruits are sweet; some sweet things are costly. → (c) Either I or II**

**Step 1 — Two particulars ⇒ nothing definite follows.**

**Step 2 — Neither conclusion holds alone** (counter-diagrams exist for both).

**Step 3 — Complementary pair:**
```
I :  Some fruits ARE costly
II:  NO fruit IS costly
```
Exact opposites ⇒ **Either–Or**.

**Answer: (c) Either I or II follows**

---

### 🟡 MEDIUM — Solutions 21–40

---

**Q21. All pens are pencils; some pencils are erasers; all erasers are sharpeners. → (a) Only I**

**I. Some pencils are sharpeners** — chain: some pencils are erasers → all erasers are sharpeners (Rule 3) ⇒ **follows** ✓

**II. Some pens are sharpeners** — pens are inside pencils, but the eraser-overlap region of pencils need not touch pens.

*Counter-diagram:*
```
   ┌────────── PENCILS ──────────┐
   │  ┌──────┐      ┌────────────┼── ERASERS ⊂ SHARPENERS
   │  │ PENS │      └────────────┼
   │  └──────┘                   │
   └─────────────────────────────┘
```
⇒ **does not follow** ✗

**Answer: (a) Only conclusion I follows**

---

**Q22. All dogs are animals; all animals are mammals; no mammal is a bird. → (e) Both follow**

**I. No dog is a bird** — dogs ⊂ animals ⊂ mammals, and mammals are disjoint from birds ⇒ **follows** ✓
**II. Some mammals are dogs** — partial conversion (dogs ⊂ mammals) ⇒ **follows** ✓

**Answer: (e) Both I and II follow**

---

**Q23. Some A are B; no B is C; all C are D. → (e) Both follow**

**I. Some A are not C** — the A's that are B cannot be C (since no B is C) ⇒ **follows** ✓

**II. Some D are not B** — all C are D, and no C is B (the converse of "no B is C"), so those D-members that are C lie outside B. Taking C as non-empty ⇒ **follows** ✓

**Diagram:**
```
        ┌── A ──┬── B ──┐         ┌────── D ──────┐
        └───────┴───────┘         │   ┌── C ──┐   │
                                  │   └───────┘   │
        (B and C disjoint)        └───────────────┘
```

**Answer: (e) Both I and II follow**

---

**Q24. All papers are books; all books are novels; some novels are magazines. → (d) Neither**

**I. Some papers are magazines** — the chain reaches novels universally, but the third premise is particular. The magazine overlap could sit entirely in the novels-outside-books region ⇒ ✗

**II. Some books are magazines** — same reasoning ⇒ ✗

**Complementary check:** the two conclusions have different subjects ⇒ not an Either–Or pair.

**Answer: (d) Neither I nor II follows**

---

**Q25. No table is a chair; some chairs are stools; all stools are wooden. → (e) Both follow**

**Step 1 — Trace the chain.**
Some chairs are stools. Those chairs are not tables (no table is a chair). Therefore **those stools are not tables**.

**II. Some stools are not tables** ⇒ **follows** ✓

**Step 2 — Extend to wooden.**
All stools are wooden, so those non-table stools are wooden.

**I. Some wooden things are not tables** ⇒ **follows** ✓

**Answer: (e) Both I and II follow**

---

**Q26. All singers are dancers; some dancers are actors. → (b) Only II**

**I. Some singers are actors** — broken chain (particular second premise) ⇒ ✗
**II. Some actors are dancers** — conversion of "Some dancers are actors" ⇒ **follows** ✓

**Answer: (b) Only conclusion II follows**

---

**Q27. Some pens are markers; all markers are pencils; no pencil is red. → (e) Both follow**

**I. Some pens are not red** — those pens are markers → pencils → not red ⇒ **follows** ✓
**II. No marker is red** — markers ⊂ pencils, and no pencil is red ⇒ **follows** ✓

**Answer: (e) Both I and II follow**

---

**Q28. All lions are wild; some wild animals are tame. → (b) Only II**

**I. Some lions are tame** — broken chain ⇒ ✗
**II. Some tame animals are wild** — conversion of "Some wild are tame" ⇒ **follows** ✓

**Answer: (b) Only conclusion II follows**

---

**Q29. Some X are Y; all Y are Z; some Z are W. → (a) Only I**

**I. Some X are Z** — Rule 3 (Some X are Y + All Y are Z) ⇒ **follows** ✓
**II. Some X are W** — the third premise is particular; the W-overlap need not touch X ⇒ ✗

**Answer: (a) Only conclusion I follows**

---

**Q30. No P is Q; all Q are R. → (a) Only I**

**I. Some R are not P** — Q ⊂ R and no Q is P, so the Q-part of R lies outside P ⇒ **follows** ✓
**II. All R are Q** — invalid full conversion ⇒ ✗

**Answer: (a) Only conclusion I follows**

---

**Q31. All students are hardworking; all hardworking are successful; some successful are rich. → (a) Only I**

**I. All students are successful** — Rule 1 chain through hardworking ⇒ **follows** ✓
**II. Some students are rich** — the third premise is particular; the rich region of "successful" need not include students ⇒ ✗

**Answer: (a) Only conclusion I follows**

---

**Q32. Some birds are crows; all crows are black; no black thing is white. → (e) Both follow**

**I. Some birds are not white** — those birds are crows → black → not white ⇒ **follows** ✓
**II. Some crows are not white** — all crows are black and no black thing is white, so **no** crow is white; hence certainly *some* crows are not white ⇒ **follows** ✓

> **A universal implies its particular.** "No crow is white" is stronger than "some crows are not white", so the weaker statement also holds (given that crows exist).

**Answer: (e) Both I and II follow**

---

**Q33. All boxes are cartons; some cartons are packets. → (b) Only II**

**I. Some boxes are packets** — broken chain ⇒ ✗
**II. Some packets are cartons** — conversion ⇒ **follows** ✓

**Answer: (b) Only conclusion II follows**

---

**Q34. Some cups are plates; some plates are bowls; some bowls are glasses. → (d) Neither**

All three premises are **particular** ⇒ no definite conclusion.

**I. Some cups are bowls** ✗ · **II. Some plates are glasses** ✗

**Complementary check:** different subjects and predicates ⇒ not a pair.

**Answer: (d) Neither I nor II follows**

---

**Q35. All keys are locks; no lock is a door. → (e) Both follow**

**I. No key is a door** — Rule 2 ⇒ **follows** ✓
**II. Some locks are keys** — partial conversion ⇒ **follows** ✓

**Answer: (e) Both I and II follow**

---

**Q36. All engineers are graduates; some graduates are doctors; all doctors are professionals. → (a) Only I**

**I. Some graduates are professionals** — some graduates are doctors, and all doctors are professionals (Rule 3) ⇒ **follows** ✓
**II. Some engineers are professionals** — the doctor-overlap of graduates need not touch engineers ⇒ ✗

**Answer: (a) Only conclusion I follows**

---

**Q37. Some ropes are threads; no thread is a wire. → (a) Only I**

**I. Some ropes are not wires** — Rule 4 (Some + No) ⇒ **follows** ✓
**II. All ropes are wires** — contradicts I; nothing supports it ⇒ ✗

**Answer: (a) Only conclusion I follows**

---

**Q38. All fruits are tasty; some tasty are costly; all costly are rare. → (a) Only I**

**I. Some tasty things are rare** — some tasty are costly, and all costly are rare (Rule 3) ⇒ **follows** ✓
**II. Some fruits are rare** — the costly region of "tasty" need not overlap fruits ⇒ ✗

**Answer: (a) Only conclusion I follows**

---

**Q39. No cat is a rat; all rats are rodents. → (a) Only I**

**I. Some rodents are not cats** — rats ⊂ rodents and no rat is a cat ⇒ **follows** ✓
**II. No rodent is a cat** — other rodents could be cats (the statements do not forbid it) ⇒ ✗

**Answer: (a) Only conclusion I follows**

---

**Q40. Some pens are blue; some blue are ink. → (d) Neither**

**Step 1 — Two particulars ⇒ nothing definite.**

**I. Some pens are ink** ✗ · **II. Some ink is pens** ✗

**Step 2 — Complementary check.**
I and II are **conversions of each other**, not opposites. Both are false in the same counter-diagram, so they do not exhaust the possibilities.

$$\implies \text{NOT an Either–Or pair}$$

**Answer: (d) Neither I nor II follows**

> **The distinction from Q8 and Q20.** There, the second conclusion was "**No** book is a pencil" — the negation. Here it is "Some ink is pens" — merely the reverse of the first. Reversal is not negation, so the Either–Or rule does not apply.

---

### 🔴 HARD — Solutions 41–50

---

**Q41. 60 students; 35 cricket, 30 football, 15 both. How many play neither? → (b) 10**

**Step 1 — At least one game.**
$$n(C \cup F) = 35 + 30 - 15 = 50$$

**Step 2 — Neither.**
$$60 - 50 = 10$$

**Region check:**

| Region | Count |
|---|---|
| Only cricket | 35 − 15 = 20 |
| Both | 15 |
| Only football | 30 − 15 = 15 |
| Neither | 10 |
| **Total** | **60** ✓ |

**Answer: (b) 10**

---

**Q42. 100 people; 60 read A, 45 read B, 25 both. At least one? → (b) 80**

$$n(A \cup B) = 60 + 45 - 25 = 80$$

**Answer: (b) 80**

---

**Q43. From Q42 — how many read only A? → (c) 35**

$$\text{Only A} = n(A) - n(A \cap B) = 60 - 25 = 35$$

**Full breakdown:** Only A = 35 · Both = 25 · Only B = 20 · Neither = 20 · Total = 100 ✓

**Answer: (c) 35**

---

**Q44. 200 people; 120 tea, 90 coffee, 30 neither. How many like both? → (b) 40**

**Step 1 — At least one.**
$$200 - 30 = 170$$

**Step 2 — Apply the union formula.**
$$170 = 120 + 90 - n(\text{both})$$
$$n(\text{both}) = 210 - 170 = 40$$

**Region check:** Only tea 80 · Both 40 · Only coffee 50 · Neither 30 ⇒ total 200 ✓

**Answer: (b) 40**

---

**Q45. Three subjects — how many study at least one? → (c) 77**

**Formula used:** inclusion–exclusion for three sets.

$$n(M \cup P \cup C) = \sum n - \sum n(\text{pairs}) + n(\text{triple})$$

**Step 1 — Sum the singles.**
$$45 + 40 + 35 = 120$$

**Step 2 — Sum the pairwise overlaps.**
$$20 + 15 + 18 = 53$$

**Step 3 — Combine.**
$$120 - 53 + 10 = 77$$

**Answer: (c) 77**

---

**Q46. From Q45 — how many study none? → (a) 3**

$$80 - 77 = 3$$

**Answer: (a) 3**

---

**Q47. From Q45 — how many study only Mathematics? → (d) 17**

**Formula used:** Only M = n(M) − n(M∩P) − n(M∩C) + n(M∩P∩C)

$$= 45 - 20 - 18 + 10 = 17$$

**Full region table (a valuable check):**

| Region | Calculation | Count |
|---|---|---|
| Only M | 45 − 20 − 18 + 10 | **17** |
| Only P | 40 − 20 − 15 + 10 | 15 |
| Only C | 35 − 15 − 18 + 10 | 12 |
| M and P only | 20 − 10 | 10 |
| P and C only | 15 − 10 | 5 |
| M and C only | 18 − 10 | 8 |
| All three | — | 10 |
| **Union** | | **77** ✓ |
| None | 80 − 77 | 3 |
| **Total** | | **80** ✓ |

> **Why "+ 10"?** Subtracting both pairwise overlaps removes the all-three region twice. Adding it back once leaves it excluded exactly once, as required.

**Answer: (d) 17**

---

**Q48. 150 people; 90 Hindi, 70 English, 40 both. Only English? → (b) 30**

$$\text{Only English} = 70 - 40 = 30$$

**Answer: (b) 30**

---

**Q49. From Q48 — how many speak neither? → (b) 30**

**Step 1 — At least one.**
$$90 + 70 - 40 = 120$$

**Step 2 — Neither.**
$$150 - 120 = 30$$

**Region check:** Only Hindi 50 · Both 40 · Only English 30 · Neither 30 ⇒ total 150 ✓

**Answer: (b) 30**

---

**Q50. All A are B; some B are C; no C is D; all D are E. → (e) Both follow**

**Step 1 — Test conclusion I: "Some B are not D".**
Some B are C (given). No C is D (given), so those B-members that are C cannot be D.
$$\implies \text{Some B are not D} \quad \textbf{follows} \checkmark$$

**Step 2 — Test conclusion II: "Some E are not C".**
All D are E (given). No C is D, equivalently no D is C. So every member of D lies inside E and outside C.
Taking D as non-empty (standard convention):
$$\implies \text{Some E are not C} \quad \textbf{follows} \checkmark$$

**Diagram:**
```
   ┌───── B ─────┐                ┌────── E ──────┐
   │  ┌─ A ─┐    │                │   ┌── D ──┐   │
   │  └─────┘  ┌─┼──── C          │   └───────┘   │
   └───────────┴─┘                └───────────────┘
                 ↑
        C and D are disjoint, so the D-part of E lies outside C
```

**Answer: (e) Both I and II follow**

---

## 8. Quick Revision Sheet

> **One page. Read 48 hours after study, and again the night before the test.**

### ⭐ The golden rule

```
A conclusion FOLLOWS only if it is true in EVERY possible diagram.
One valid counter-diagram is enough to reject it.

Never use real-world knowledge. Accept the statements as given.
```

### Conversions

```
All A are B      →  SOME B are A     ✓   (never "All B are A")
No A is B        →  No B is A        ✓
Some A are B     →  Some B are A     ✓
Some A are not B →  NOTHING          ✗
```

### The combination rules

```
All A are B  + All B are C   →  All A are C          ✓
All A are B  + No B is C     →  No A is C            ✓
Some A are B + All B are C   →  Some A are C         ✓
Some A are B + No B is C     →  Some A are not C     ✓
No A is B    + All C are B   →  No A is C            ✓

All A are B  + Some B are C  →  NOTHING              ✗
Some + Some                  →  NOTHING              ✗
No + No                      →  NOTHING              ✗
"Some…are not" + anything    →  NOTHING              ✗
```

### The three master principles

```
1.  Two PARTICULARS ("some")  ⇒  no conclusion
2.  Two NEGATIVES             ⇒  no conclusion
3.  The conclusion takes the WEAKER quality:
        one particular premise ⇒ particular conclusion
        one negative premise   ⇒ negative conclusion
```

### ⭐ The Either–Or test

```
1.  Does I follow alone?     NO
2.  Does II follow alone?    NO
3.  Same subject & predicate, and exact OPPOSITES?   YES
        ⇒  "Either I or II follows"

COMPLEMENTARY PAIRS
    Some A are B   ↔   No A is B
    All A are B    ↔   Some A are not B

NOT complementary
    Some A are B   vs  Some A are not B     (both can be true)
    Some A are B   vs  Some B are A         (mere conversion)
    All A are B    vs  No A is B            (both can be false)
```

### Possibility conclusions

```
"Some A being B is a possibility"
    FOLLOWS  ⇔  the statements do NOT forbid it
    FAILS    ⇔  the statements make it impossible
```

### Venn set counting

```
TWO SETS
    n(A∪B)   =  n(A) + n(B) − n(A∩B)
    Only A   =  n(A) − n(A∩B)
    Neither  =  Total − n(A∪B)
    Both     =  n(A) + n(B) − [Total − Neither]

THREE SETS
    n(A∪B∪C) = ΣSingles − ΣPairs + Triple

    Only A            =  n(A) − n(A∩B) − n(A∩C) + n(A∩B∩C)
    Exactly A and B   =  n(A∩B) − n(A∩B∩C)
    None              =  Total − n(A∪B∪C)

ALWAYS CHECK: the sum of all regions = the total
```

### Sanity checks

```
✓ "All A are B" never gives "All B are A"
✓ Two "some" statements never give a definite conclusion
✓ Two negatives never give a conclusion
✓ Either–Or requires exact opposites, not mere reversal
✓ A universal implies its particular (No A is B ⇒ Some A are not B)
✓ No Venn region may be negative
```

---

## 9. Common Mistakes

| # | Mistake | Example | Correction |
|---|---|---|---|
| 1 | **Full conversion of "All"** | All pens are books ⇒ all books are pens | Only "**some** books are pens" |
| 2 | **Real-world knowledge used** | "All parrots are birds" assumed | Use only what the statements say |
| 3 | **Chain forced through a "some"** | All A are B + Some B are C ⇒ Some A are C | The chain breaks — nothing follows |
| 4 | **Two particulars given a conclusion** | Some + Some ⇒ Some | Two particulars ⇒ nothing |
| 5 | **Either–Or applied to a reversal** | "Some A are B" and "Some B are A" | Reversal ≠ negation |
| 6 | **Either–Or missed entirely** | Answering "neither" for a true pair | Check for exact opposites |
| 7 | **Universal conclusion from a particular premise** | Some men are doctors ⇒ all men educated | Weaker premise caps the conclusion |
| 8 | **Negative existence conclusions rejected** | "Some R are not P" dismissed | No P is Q + All Q are R ⇒ it follows |
| 9 | **Possibility read as certainty** | Rejecting "is a possibility" | It follows unless forbidden |
| 10 | **Triple overlap not added back** | Only A = n(A) − pairs | Add the triple term back once |
| 11 | **"Neither" region forgotten** | Union taken as the total | Total = Union + Neither |
| 12 | **Only one diagram tested** | Accepting the first drawing | Test the *least favourable* case |

---

## Practice Answer Key

| Q | Ans | Q | Ans | Q | Ans | Q | Ans | Q | Ans |
|---|---|---|---|---|---|---|---|---|---|
| 1 | e | 11 | a | 21 | a | 31 | a | 41 | b |
| 2 | d | 12 | a | 22 | e | 32 | e | 42 | b |
| 3 | a | 13 | a | 23 | e | 33 | b | 43 | c |
| 4 | e | 14 | b | 24 | d | 34 | d | 44 | b |
| 5 | a | 15 | b | 25 | e | 35 | e | 45 | c |
| 6 | a | 16 | a | 26 | b | 36 | a | 46 | a |
| 7 | e | 17 | a | 27 | e | 37 | a | 47 | d |
| 8 | c | 18 | a | 28 | b | 38 | a | 48 | b |
| 9 | d | 19 | e | 29 | a | 39 | a | 49 | b |
| 10 | e | 20 | c | 30 | a | 40 | d | 50 | e |

**Scoring guide:** 45+/50 → strong. 35–44 → solid; drill the conversion rules and the Either–Or test. Below 35 → this topic is entirely rule-based — write out the eight combination rules from memory, then redo the whole set. You should be able to reach near-perfect scores here.

---

**⬅️ Back:** [Topic 16 — Seating Arrangement & Puzzles](16-seating-arrangement-puzzles.md) · **➡️ Next:** [Topic 18 — Data Sufficiency & Critical Reasoning](18-data-sufficiency-critical-reasoning.md)
