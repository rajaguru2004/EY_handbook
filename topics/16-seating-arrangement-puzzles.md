# Topic 16 — Seating Arrangement & Puzzles

### EY Placement Aptitude Handbook · Priority Rank #8 · 🔴 Critical

> **Questions in this file are original, modelled on publicly reported EY test patterns. They are not claimed to be actual previous-year EY questions.**

---

## Contents

1. [Why This Topic Matters for EY](#1-why-this-topic-matters-for-ey)
2. [Core Concepts](#2-core-concepts)
3. [The Solving Framework](#3-the-solving-framework)
4. [Shortcuts & Tricks](#4-shortcuts--tricks)
5. [Solved Examples](#5-solved-examples)
6. [Practice Questions (50, in 10 sets)](#6-practice-questions)
7. [Detailed Solutions](#7-detailed-solutions)
8. [Quick Revision Sheet](#8-quick-revision-sheet)
9. [Common Mistakes](#9-common-mistakes)

---

## 1. Why This Topic Matters for EY

**Weightage:** 12–15% of the reasoning section — the **second-highest** reasoning topic after series.

**Why the weightage is deceptive:** puzzles arrive in **sets**. One arrangement generates 4–5 questions. Crack the arrangement and you bank five marks in ninety seconds; fail to crack it and you lose five. No other topic has this much variance riding on a single deduction.

**The practical consequence:** if a puzzle resists you for **two minutes**, abandon it and come back. Do not let one set consume a quarter of your section time.

**Question styles reported:**

| Style | Typical shape |
|---|---|
| **Linear arrangement** | 6–8 people in a row, all facing one way |
| **Linear, two rows** | Two rows facing each other |
| **Circular** | 6–8 people around a table, facing the centre or outward |
| **Floor / building** | 5–8 people on numbered floors |
| **Box / stack** | Boxes stacked vertically |
| **Scheduling** | Days of the week, months, time slots |
| **Matrix / attribute** | People + sport + city + colour |
| **Ranking / comparison** | "A scored more than B but less than C" |

---

## 2. Core Concepts

### 2.1 The three question types by information density

| Type | Signal | Approach |
|---|---|---|
| **Fully determined** | Every position is fixed by the clues | Solve completely, then answer |
| **Partially determined** | Two or three valid arrangements exist | Find all of them; the questions will still have unique answers |
| **Over-constrained check** | A clue contradicts another | Re-read — you have misinterpreted a direction |

### 2.2 Linear arrangements

```
       LEFT ←─────────────────────────────→ RIGHT

        1     2     3     4     5     6
      ┌───┬───┬───┬───┬───┬───┐
      │   │   │   │   │   │   │        All facing NORTH
      └───┴───┴───┴───┴───┴───┘
```

**Position vocabulary:**

| Phrase | Meaning (in a row of *n*) |
|---|---|
| "Third from the left" | Position 3 |
| "Third from the right" | Position n − 2 |
| "Immediate left of X" | Position of X, minus 1 |
| "Immediate right of X" | Position of X, plus 1 |
| "Second to the left of X" | Position of X, minus 2 |
| "Between A and B" | Strictly between their positions |
| "Extreme end" | Position 1 or position n |

> **"Second to the left" means two positions away — not one.** "Immediate left" means one. This distinction accounts for a large share of all puzzle errors.

**When everyone faces NORTH (the standard case), the reader's left/right matches the sitters' left/right**, so you can work directly with positions 1…n increasing to the right.

### 2.3 The facing-direction rule (critical)

```
FACING NORTH  →  the person's LEFT is toward position 1
                 the person's RIGHT is toward position n
                 (matches the reader's view)

FACING SOUTH  →  EVERYTHING REVERSES
                 the person's LEFT is toward position n
                 the person's RIGHT is toward position 1
```

**Mark the facing direction next to every person on your diagram.** In mixed-facing puzzles this is the single thing that separates a correct solve from a wasted three minutes.

### 2.4 Circular arrangements

```
                        1
                   8         2
                7               3        (positions numbered CLOCKWISE)
                   6         4
                        5
```

**The convention that matters:**

| Everyone faces | Clockwise motion is toward each person's | Anticlockwise is toward |
|---|---|---|
| **The centre** (inward) | **LEFT** | **RIGHT** |
| **Away from the centre** (outward) | **RIGHT** | **LEFT** |

> **Facing the centre — the standard case.** Imagine standing in a circle looking inward. The person clockwise from you is on your **left**. This feels counter-intuitive at first; draw it once and it sticks.

**Opposite seats:** in a circle of *n* people (n even), the person opposite position *p* is at:
$$p + \frac{n}{2} \quad (\text{wrapping around})$$

For 8 people: 1↔5, 2↔6, 3↔7, 4↔8.
For 6 people: 1↔4, 2↔5, 3↔6.

### 2.5 Vertical arrangements (floors and boxes)

```
        Floor 7   ─────────────    ← TOP
        Floor 6   ─────────────
        Floor 5   ─────────────
        Floor 4   ─────────────
        Floor 3   ─────────────
        Floor 2   ─────────────
        Floor 1   ─────────────    ← BOTTOM
```

| Phrase | Meaning |
|---|---|
| "Immediately above X" | X's floor + 1 |
| "Immediately below X" | X's floor − 1 |
| "Two floors above X" | X's floor + 2 |
| "**Only two people** between A and B" | Their floors differ by **3** |
| "Topmost / lowermost" | Floor n / floor 1 |

> **"Two people between A and B" ⇒ |A − B| = 3, not 2.** Two occupied floors sit in the gap, so the positions differ by three. This is the highest-frequency slip in floor puzzles.

### 2.6 Matrix (attribute) puzzles

When people are matched to two or more attributes, **build a grid**:

```
Person │ Sport      │ City
───────┼────────────┼──────────
  P    │ Cricket    │ Bangalore
  Q    │ Football   │ Mumbai
  R    │ Hockey     │ Kolkata
  S    │ Tennis     │ Delhi
  T    │ Badminton  │ Chennai
```

**Method:** fill directly-stated facts first, then use elimination. A clue linking two *attributes* to each other ("the tennis player lives in Delhi") is often more powerful than one naming a person.

---

## 3. The Solving Framework

### 3.1 The seven-step procedure

```
STEP 1:  Identify the SHAPE (row / circle / floors / grid) and the SIZE
STEP 2:  Draw the empty frame with numbered positions
STEP 3:  Note the FACING direction beside every seat
STEP 4:  Rank the clues by DEFINITENESS:
             ★★★  absolute positions   ("C sits third from the left")
             ★★   relative + anchored  ("A is immediately right of C")
             ★     relative only        ("D is not adjacent to E")
             —     negative constraints ("F is not at an end")
STEP 5:  Place the ★★★ clues FIRST, then ★★, then ★
STEP 6:  Use NEGATIVE clues to eliminate, not to place
STEP 7:  VERIFY every clue against the finished diagram before answering
```

**Step 4 is what separates fast solvers from slow ones.** Working the clues in the given order is almost always the wrong order.

### 3.2 Worked demonstration

> Six friends A, B, C, D, E, F sit in a row facing north.
> 1. C sits third from the left.
> 2. A sits to the immediate right of C.
> 3. B sits at one of the extreme ends.
> 4. D sits second to the right of A.
> 5. F sits to the immediate left of C.

**Step 1–3: frame.**
```
    1     2     3     4     5     6      (all facing north)
  ┌───┬───┬───┬───┬───┬───┐
  │   │   │   │   │   │   │
  └───┴───┴───┴───┴───┴───┘
```

**Step 4–5: rank and place.**

| Clue | Rating | Action |
|---|---|---|
| 1. C is third from the left | ★★★ | **C → 3** |
| 2. A is immediately right of C | ★★ | **A → 4** |
| 5. F is immediately left of C | ★★ | **F → 2** |
| 4. D is second to the right of A | ★★ | **D → 6** |
| 3. B is at an extreme end | ★ | Ends are 1 and 6; 6 is D ⇒ **B → 1** |
| — | — | E takes the only seat left ⇒ **E → 5** |

**Final:**
```
    1     2     3     4     5     6
  ┌───┬───┬───┬───┬───┬───┐
  │ B │ F │ C │ A │ E │ D │
  └───┴───┴───┴───┴───┴───┘
```

**Step 7: verify.** C is 3rd from the left ✓ · A is immediately right of C ✓ · B is at an end ✓ · D is second right of A (4 → 6) ✓ · F is immediately left of C ✓

---

## 4. Shortcuts & Tricks

### 4.1 Start where the information is densest

Scan all the clues before writing anything. Find the position mentioned most often, or the one clue that fixes an absolute seat. That is your anchor.

```
"C sits third from the left"     ← ANCHOR. Start here.
"A is to the immediate right of C" ← chains directly off the anchor
"D sits second to the right of A"  ← chains off A
```

Three clues, one chain, four seats filled.

### 4.2 The "between" arithmetic

| Phrase | Position difference |
|---|---|
| "Immediately next to" | 1 |
| "**One** person between" | 2 |
| "**Two** people between" | 3 |
| "**Three** people between" | 4 |
| "*k* people between" | **k + 1** |

**Memorise: gap = number between + 1.**

### 4.3 Circular direction — the two-second check

```
FACING THE CENTRE:
        clockwise  =  toward each person's LEFT
        anticlockwise = toward each person's RIGHT

FACING OUTWARD: reverse both.
```

Write **"IN"** or **"OUT"** in the middle of your circle before placing anyone. It takes one second and prevents the most common circular-puzzle error.

### 4.4 Use negative clues last

A clue like *"F is not adjacent to A"* or *"C is not at an extreme end"* rarely places anyone. Its value is in **eliminating** the last one or two ambiguous options — so save it for the end, when only a few seats remain.

### 4.5 Try both cases when stuck

If a clue admits two placements, branch:

```
Case A: X at position 2  →  follow the consequences
Case B: X at position 5  →  follow the consequences

One branch will contradict a later clue. Discard it.
```

Branching feels slow but is usually faster than staring. Two branches, each pursued for thirty seconds, beats two minutes of hesitation.

### 4.6 Answer the questions in the right order

Once the arrangement is solved, the five questions are trivially answerable. But **read each one carefully**:

```
"Who sits between C and E?"           → strictly between
"Who is second to the left of A?"     → two positions, not one
"How many sit between B and D?"       → a count, not names
"What is E's position from the LEFT?" → check which end
```

The arrangement is the hard part; losing marks on question wording after solving it is the avoidable tragedy of this topic.

### 4.7 Sanity checks

```
✓ Every person is placed exactly once
✓ Every seat is occupied exactly once
✓ EVERY clue is satisfied — walk through them one by one
✓ In circles, check the opposite pairs (1↔5 for 8, 1↔4 for 6)
✓ In floor puzzles, "k between" means a gap of k+1
✓ Facing direction noted for every person in mixed-facing puzzles
```

---

## 5. Solved Examples

### Example 1 — Linear arrangement

**Q.** Seven friends P, Q, R, S, T, U, V sit in a row facing north.
- S sits fourth from the left.
- Q sits at the extreme right.
- Only two people sit between S and P.
- T sits immediately to the left of S.
- R sits second to the right of S.
- U is not adjacent to S.

Find the complete arrangement.

**Step 1 — Frame (7 seats).**
```
    1     2     3     4     5     6     7
```

**Step 2 — Place the ★★★ absolute clues.**
- S is fourth from the left ⇒ **S → 4**
- Q is at the extreme right ⇒ **Q → 7**

**Step 3 — Chain the ★★ clues off S.**
- T is immediately left of S ⇒ **T → 3**
- R is second to the right of S(4) ⇒ **R → 6**

**Step 4 — Apply the "between" clue.**
Only two people between S(4) and P ⇒ the gap is **3** ⇒ P = 1 or P = 7.
Seat 7 is occupied by Q ⇒ **P → 1**

**Step 5 — Use the negative clue last.**
Seats left: 2 and 5, for U and V.
U is not adjacent to S(4) ⇒ U ≠ 3 and U ≠ 5 ⇒ **U → 2**, and **V → 5**

**Final arrangement:**
```
    1     2     3     4     5     6     7
  ┌───┬───┬───┬───┬───┬───┬───┐
  │ P │ U │ T │ S │ V │ R │ Q │
  └───┴───┴───┴───┴───┴───┴───┘
```

**Verification:** S is 4th from the left ✓ · Q at the extreme right ✓ · two people (U, T) between P and S ✓ · T immediately left of S ✓ · R second right of S ✓ · U not adjacent to S ✓

> **Note the clue order.** The puzzle lists "only two people between S and P" third, but it was more efficient to place T and R first — they chain directly off the anchored S. Working clues in the order given would have left you juggling two possibilities for P unnecessarily.

---

### Example 2 — Circular arrangement, facing the centre

**Q.** Six people A, B, C, D, E, F sit around a circular table facing the centre.
- A sits opposite D.
- B sits to the immediate right of A.
- C sits to the immediate left of D.
- E sits second to the left of A.

Find the arrangement.

**Step 1 — Frame and convention.**
```
                    1
               6         2
                   IN
               5         3
                    4
```
Positions run **clockwise**. Facing the centre ⇒ **clockwise = each person's LEFT**, anticlockwise = right.

**Step 2 — Anchor.**
Place **A → 1**. In a circle of 6, opposite means +3 ⇒ **D → 4**.

**Step 3 — Apply the direction clues.**
- B is to the **immediate right** of A(1). Right = anticlockwise ⇒ **B → 6**
- C is to the **immediate left** of D(4). Left = clockwise ⇒ **C → 5**
- E is **second to the left** of A(1). Left = clockwise, two places ⇒ **E → 3**

**Step 4 — Fill the last seat.**
Only position 2 remains ⇒ **F → 2**

**Final arrangement (clockwise):**
```
                    A(1)
              B(6)        F(2)
                    IN
              C(5)        E(3)
                    D(4)
```

**Verification:** A opposite D (1 ↔ 4) ✓ · B immediately anticlockwise of A ✓ · C immediately clockwise of D ✓ · E two clockwise from A ✓

---

### Example 3 — Floor puzzle

**Q.** Seven people P, Q, R, S, T, U, V live on seven floors of a building, floor 1 being the lowest.
- P lives on floor 4.
- Q lives immediately above P.
- Only two people live between Q and R.
- S lives on the topmost floor.
- T lives immediately below R.
- U lives below V.

Find the arrangement.

**Step 1 — Frame.**
```
  Floor 7  ______
  Floor 6  ______
  Floor 5  ______
  Floor 4  ______
  Floor 3  ______
  Floor 2  ______
  Floor 1  ______
```

**Step 2 — Absolute placements.**
- **P → 4** · **S → 7**

**Step 3 — Chain from P.**
- Q immediately above P ⇒ **Q → 5**

**Step 4 — Apply the "between" clue.**
Two people between Q(5) and R ⇒ gap of **3** ⇒ R = 2 or R = 8.
Floor 8 does not exist ⇒ **R → 2**

**Step 5 — Chain from R.**
- T immediately below R(2) ⇒ **T → 1**

**Step 6 — Place the remainder.**
Floors left: **3** and **6**, for U and V.
U lives below V ⇒ **U → 3**, **V → 6**

**Final arrangement:**
```
  Floor 7   S
  Floor 6   V
  Floor 5   Q
  Floor 4   P
  Floor 3   U
  Floor 2   R
  Floor 1   T
```

**Verification:** P on 4 ✓ · Q immediately above P ✓ · two people (U, P) between R(2) and Q(5) ✓ · S on top ✓ · T immediately below R ✓ · U(3) below V(6) ✓

> **Step 4 is the crux.** "Only two people between" means the floors differ by **three**, not two. Reading it as two would put R at 3 or 7 and the puzzle would not close.

---

### Example 4 — Matrix puzzle

**Q.** Five friends each like a different sport and live in a different city.
- P likes cricket.
- The tennis player lives in Delhi.
- S lives in Delhi.
- R likes hockey.
- The badminton player lives in Chennai.
- Q lives in Mumbai.
- P lives in Bangalore.
- T does not live in Kolkata.

Determine each person's sport and city.

**Step 1 — Build the grid and enter the direct facts.**

| Person | Sport | City |
|---|---|---|
| P | **Cricket** | **Bangalore** |
| Q | ? | **Mumbai** |
| R | **Hockey** | ? |
| S | ? | **Delhi** |
| T | ? | ? |

**Step 2 — Link the attribute clues.**
The tennis player lives in Delhi, and S lives in Delhi ⇒ **S plays tennis**.

**Step 3 — Narrow the remaining sports.**
Cricket, hockey and tennis are taken ⇒ Q and T have **badminton** and **football**.

**Step 4 — Use the badminton–Chennai link.**
The badminton player lives in **Chennai**. Q lives in **Mumbai**, so Q cannot play badminton.
$$\implies Q \text{ plays } \textbf{football}, \qquad T \text{ plays } \textbf{badminton}$$

And since the badminton player is in Chennai ⇒ **T lives in Chennai** ✓ (consistent with "T does not live in Kolkata")

**Step 5 — Assign the last city.**
Cities used: Bangalore (P), Mumbai (Q), Delhi (S), Chennai (T).
The only one left is **Kolkata** ⇒ **R lives in Kolkata**

**Final grid:**

| Person | Sport | City |
|---|---|---|
| P | Cricket | Bangalore |
| Q | Football | Mumbai |
| R | Hockey | Kolkata |
| S | Tennis | Delhi |
| T | Badminton | Chennai |

**Verification:** every clue checks out, all five sports and all five cities are used exactly once ✓

> **The unlocking move was Step 4** — combining a person-fact (Q is in Mumbai) with an attribute-fact (badminton ⇒ Chennai) to eliminate a possibility. Attribute-to-attribute clues are usually the most powerful in matrix puzzles; look for them first.

---

## 6. Practice Questions

**Instructions:** 50 questions across 10 puzzle sets.
Sets 1–3 Easy · Sets 4–7 Medium · Sets 8–10 Hard.
Solve each arrangement fully before answering its questions.
Full solutions in [Section 7](#7-detailed-solutions).

---

### 🟢 SET 1 — Linear arrangement (Questions 1–5)

**Six friends A, B, C, D, E and F sit in a row facing north.**
- C sits third from the left.
- A sits to the immediate right of C.
- B sits at one of the extreme ends.
- D sits second to the right of A.
- F sits to the immediate left of C.

**Q1.** Who sits at the extreme right?
(a) A  (b) B  (c) D  (d) E

**Q2.** Who sits between C and E?
(a) A  (b) B  (c) D  (d) F

**Q3.** How many people sit between B and D?
(a) 2  (b) 3  (c) 4  (d) 5

**Q4.** Who sits second to the left of A?
(a) B  (b) C  (c) E  (d) F

**Q5.** What is E's position from the left end?
(a) Third  (b) Fourth  (c) Fifth  (d) Sixth

---

### 🟢 SET 2 — Circular arrangement (Questions 6–10)

**Six people P, Q, R, S, T and U sit around a circular table facing the centre.**
- P sits opposite S.
- Q sits to the immediate right of P.
- T sits to the immediate left of S.
- R sits second to the left of P.

**Q6.** Who sits opposite Q?
(a) P  (b) R  (c) T  (d) U

**Q7.** Who sits between S and Q (moving clockwise from S)?
(a) P  (b) R  (c) T  (d) U

**Q8.** Who sits to the immediate left of U?
(a) P  (b) Q  (c) R  (d) S

**Q9.** How many people sit between P and S when moving clockwise from P?
(a) 1  (b) 2  (c) 3  (d) 4

**Q10.** Who sits opposite U?
(a) Q  (b) R  (c) S  (d) T

---

### 🟢 SET 3 — Ranking (Questions 11–15)

**Five students A, B, C, D and E took an examination and all scored different marks.**
- A scored more than B but less than C.
- D scored more than C.
- E scored the least.

**Q11.** Who scored the highest?
(a) A  (b) C  (c) D  (d) E

**Q12.** Who scored the second highest?
(a) A  (b) B  (c) C  (d) D

**Q13.** Who scored the lowest?
(a) A  (b) B  (c) D  (d) E

**Q14.** How many students scored more than A?
(a) 1  (b) 2  (c) 3  (d) 4

**Q15.** Who occupies the middle position in the ranking?
(a) A  (b) B  (c) C  (d) D

---

### 🟡 SET 4 — Floor puzzle (Questions 16–20)

**Seven people P, Q, R, S, T, U and V live on seven different floors of a building. Floor 1 is the lowest and floor 7 the topmost.**
- P lives on floor 4.
- Q lives immediately above P.
- Only two people live between Q and R.
- S lives on the topmost floor.
- T lives immediately below R.
- U lives below V.

**Q16.** Who lives on floor 3?
(a) R  (b) T  (c) U  (d) V

**Q17.** How many people live between R and P?
(a) 1  (b) 2  (c) 3  (d) 4

**Q18.** Who lives immediately above V?
(a) P  (b) Q  (c) S  (d) U

**Q19.** On which floor does T live?
(a) 1  (b) 2  (c) 3  (d) 6

**Q20.** How many people live above Q?
(a) 1  (b) 2  (c) 3  (d) 4

---

### 🟡 SET 5 — Scheduling (Questions 21–25)

**Six people A, B, C, D, E and F attend a seminar on six different days from Monday to Saturday (one person per day).**
- A attends on Wednesday.
- B attends two days after A.
- C attends before A but not on Monday.
- D attends on Monday.
- E attends immediately after B.

**Q21.** Who attends on Thursday?
(a) C  (b) E  (c) F  (d) B

**Q22.** Who attends immediately before A?
(a) B  (b) C  (c) D  (d) F

**Q23.** How many people attend between C and B?
(a) 1  (b) 2  (c) 3  (d) 4

**Q24.** On which day does E attend?
(a) Thursday  (b) Friday  (c) Saturday  (d) Tuesday

**Q25.** Who attends on the last day?
(a) B  (b) E  (c) F  (d) C

---

### 🟡 SET 6 — Eight in a row (Questions 26–30)

**Eight friends A, B, C, D, E, F, G and H sit in a row facing north.**
- D sits third from the left.
- Only two people sit between A and F.
- B sits immediately to the right of D.
- G sits third to the right of B.
- A sits at one of the extreme ends.
- C is not adjacent to D.
- H sits to the left of C.
- E sits at an extreme end.

**Q26.** Who sits immediately to the left of F?
(a) A  (b) B  (c) C  (d) D

**Q27.** How many people sit between H and G?
(a) 2  (b) 3  (c) 4  (d) 5

**Q28.** Who sits at the extreme right?
(a) A  (b) E  (c) G  (d) C

**Q29.** What is C's position from the right end?
(a) Second  (b) Third  (c) Fourth  (d) Fifth

**Q30.** Who sits third to the left of C?
(a) B  (b) D  (c) E  (d) H

---

### 🟡 SET 7 — Box stack (Questions 31–35)

**Six boxes P, Q, R, S, T and U are placed one above another.**
- Box R is immediately above box P.
- Only two boxes are placed between P and Q.
- Box S is at the bottom.
- Box T is immediately above box U.

**Q31.** Which box is at the top?
(a) P  (b) Q  (c) R  (d) T

**Q32.** Which box is immediately below P?
(a) Q  (b) S  (c) T  (d) U

**Q33.** How many boxes are placed between Q and P?
(a) 1  (b) 2  (c) 3  (d) 4

**Q34.** Which box is third from the bottom?
(a) Q  (b) T  (c) U  (d) P

**Q35.** Which box is immediately above S?
(a) P  (b) Q  (c) T  (d) U

---

### 🔴 SET 8 — Circular, eight people (Questions 36–40)

**Eight people A, B, C, D, E, F, G and H sit around a circular table facing the centre.**
- A sits third to the left of B.
- C sits opposite A.
- D sits immediately to the left of B.
- E sits second to the right of C.
- G sits immediately to the right of A.
- H sits immediately to the left of A.

**Q36.** Who sits opposite B?
(a) E  (b) F  (c) G  (d) H

**Q37.** Who sits between C and D?
(a) A  (b) B  (c) E  (d) F

**Q38.** Who sits to the immediate right of E?
(a) A  (b) F  (c) G  (d) H

**Q39.** How many people sit between A and C moving clockwise from A?
(a) 2  (b) 3  (c) 4  (d) 5

**Q40.** Who sits opposite F?
(a) D  (b) E  (c) G  (d) H

---

### 🔴 SET 9 — Floors with attributes (Questions 41–45)

**Five people A, B, C, D and E live on five different floors of a building (floor 1 lowest, floor 5 topmost). Each owns a car of a different colour: red, blue, white, black and green.**
- The person on floor 3 owns the red car.
- A lives above B.
- C owns the blue car and lives on floor 1.
- D lives immediately below the person who owns the white car.
- The person on floor 5 owns the black car.
- E lives on floor 4.

**Q41.** Who lives on floor 5?
(a) A  (b) B  (c) D  (d) E

**Q42.** What colour car does D own?
(a) Red  (b) White  (c) Green  (d) Black

**Q43.** Who owns the white car?
(a) A  (b) B  (c) D  (d) E

**Q44.** On which floor does B live?
(a) 1  (b) 2  (c) 3  (d) 5

**Q45.** Who lives immediately above C?
(a) A  (b) B  (c) D  (d) E

---

### 🔴 SET 10 — Matrix puzzle (Questions 46–50)

**Five friends P, Q, R, S and T each like a different sport and live in a different city.**
- P likes cricket.
- The person who likes tennis lives in Delhi.
- S lives in Delhi.
- R likes hockey.
- The person who likes badminton lives in Chennai.
- Q lives in Mumbai.
- P lives in Bangalore.
- T does not live in Kolkata.

**Q46.** Who likes badminton?
(a) Q  (b) R  (c) S  (d) T

**Q47.** Where does R live?
(a) Mumbai  (b) Chennai  (c) Kolkata  (d) Delhi

**Q48.** Which sport does Q like?
(a) Tennis  (b) Football  (c) Badminton  (d) Hockey

**Q49.** Who lives in Delhi?
(a) P  (b) Q  (c) R  (d) S

**Q50.** Which sport does the person living in Bangalore like?
(a) Cricket  (b) Hockey  (c) Tennis  (d) Football

---

## 7. Detailed Solutions

### 🟢 SET 1 — Solutions 1–5

**Building the arrangement.**

**Step 1 — Frame (6 seats, all facing north).**
```
    1     2     3     4     5     6
```

**Step 2 — Rank and apply the clues.**

| Order | Clue | Deduction |
|---|---|---|
| 1 | C sits third from the left | **C → 3** |
| 2 | A is immediately right of C | **A → 4** |
| 3 | F is immediately left of C | **F → 2** |
| 4 | D is second to the right of A(4) | **D → 6** |
| 5 | B is at an extreme end | Ends are 1 and 6; 6 = D ⇒ **B → 1** |
| 6 | (remaining) | **E → 5** |

**Final arrangement:**
```
    1     2     3     4     5     6
  ┌───┬───┬───┬───┬───┬───┐
  │ B │ F │ C │ A │ E │ D │
  └───┴───┴───┴───┴───┴───┘
```

**Verification:** C is 3rd from the left ✓ · A immediately right of C ✓ · B at an end ✓ · D second right of A ✓ · F immediately left of C ✓

---

**Q1. Extreme right? → (c) D**
Position 6 holds **D**.

**Answer: (c) D**

---

**Q2. Between C and E? → (a) A**
C is at 3, E at 5. The seat strictly between is position 4 = **A**.

**Answer: (a) A**

---

**Q3. People between B and D? → (c) 4**
B is at 1, D at 6. The seats between are 2, 3, 4 and 5 ⇒ F, C, A, E = **4 people**.

*(Gap = 6 − 1 − 1 = 4.)*

**Answer: (c) 4**

---

**Q4. Second to the left of A? → (d) F**
A is at 4. Two positions to the left ⇒ position 2 = **F**.

> **Not "immediate left".** Immediate left of A would be C at position 3.

**Answer: (d) F**

---

**Q5. E's position from the left? → (c) Fifth**
E occupies position **5**.

**Answer: (c) Fifth**

---

### 🟢 SET 2 — Solutions 6–10

**Building the arrangement.**

**Step 1 — Frame and convention.**
Six seats numbered **clockwise**. Everyone faces the **centre**, so:
$$\text{clockwise} = \text{each person's LEFT} \qquad \text{anticlockwise} = \text{RIGHT}$$

**Step 2 — Apply the clues.**

| Order | Clue | Deduction |
|---|---|---|
| 1 | Anchor | **P → 1** |
| 2 | P sits opposite S | Opposite of 1 in a 6-circle is 4 ⇒ **S → 4** |
| 3 | Q is immediate **right** of P | Right = anticlockwise ⇒ **Q → 6** |
| 4 | T is immediate **left** of S(4) | Left = clockwise ⇒ **T → 5** |
| 5 | R is second to the **left** of P(1) | Two clockwise ⇒ **R → 3** |
| 6 | (remaining) | **U → 2** |

**Final arrangement (clockwise):**
```
                   P(1)
             Q(6)        U(2)
                   IN
             T(5)        R(3)
                   S(4)
```

**Verification:** P opposite S (1↔4) ✓ · Q immediately anticlockwise of P ✓ · T immediately clockwise of S ✓ · R two clockwise from P ✓

---

**Q6. Opposite Q? → (b) R**
Q is at 6. Opposite = 6 + 3 = 9 → 9 − 6 = **3** = **R**.

**Answer: (b) R**

---

**Q7. Between S and Q (clockwise from S)? → (c) T**
Moving clockwise from S(4): position 5, then 6 (Q). The single seat between is 5 = **T**.

**Answer: (c) T**

---

**Q8. Immediate left of U? → (c) R**
U is at 2. Left = **clockwise** ⇒ position 3 = **R**.

> **The direction trap.** Facing the centre, "left" moves clockwise. Reading it as anticlockwise would give P — a planted distractor.

**Answer: (c) R**

---

**Q9. People between P and S, clockwise from P? → (b) 2**
From P(1) clockwise to S(4): positions 2 and 3 ⇒ U and R = **2 people**.

**Answer: (b) 2**

---

**Q10. Opposite U? → (d) T**
U is at 2. Opposite = 2 + 3 = **5** = **T**.

**Answer: (d) T**

---

### 🟢 SET 3 — Solutions 11–15

**Building the ranking.**

**Step 1 — Translate each clue into an inequality.**
```
A > B          and          C > A          ⇒   C > A > B
D > C                                      ⇒   D > C > A > B
E is the least                             ⇒   D > C > A > B > E
```

**Final ranking (highest to lowest):**
```
    1st   2nd   3rd   4th   5th
     D  >  C  >  A  >  B  >  E
```

---

**Q11. Highest scorer? → (c) D**

**Answer: (c) D**

---

**Q12. Second highest? → (c) C**

**Answer: (c) C**

---

**Q13. Lowest scorer? → (d) E**

**Answer: (d) E**

---

**Q14. How many scored more than A? → (b) 2**
A is 3rd. Above A are **D and C** = 2 students.

**Answer: (b) 2**

---

**Q15. Middle of the ranking? → (a) A**
With five students, the middle is the **3rd** position = **A**.

**Answer: (a) A**

---

### 🟡 SET 4 — Solutions 16–20

**Building the arrangement.**

| Order | Clue | Deduction |
|---|---|---|
| 1 | P lives on floor 4 | **P → 4** |
| 2 | S lives on the topmost floor | **S → 7** |
| 3 | Q immediately above P | **Q → 5** |
| 4 | Two people between Q(5) and R | Gap = **3** ⇒ R = 2 or 8; floor 8 doesn't exist ⇒ **R → 2** |
| 5 | T immediately below R(2) | **T → 1** |
| 6 | U lives below V | Floors left are 3 and 6 ⇒ **U → 3**, **V → 6** |

**Final arrangement:**
```
  Floor 7   S
  Floor 6   V
  Floor 5   Q
  Floor 4   P
  Floor 3   U
  Floor 2   R
  Floor 1   T
```

**Verification:** P on 4 ✓ · Q immediately above P ✓ · two people (U, P) between R and Q ✓ · S topmost ✓ · T immediately below R ✓ · U below V ✓

---

**Q16. Who lives on floor 3? → (c) U**

**Answer: (c) U**

---

**Q17. People between R and P? → (a) 1**
R is on floor 2, P on floor 4. The only floor between is **3** ⇒ **1 person** (U).

**Answer: (a) 1**

---

**Q18. Immediately above V? → (c) S**
V is on floor 6, so floor 7 = **S**.

**Answer: (c) S**

---

**Q19. T's floor? → (a) 1**

**Answer: (a) 1**

---

**Q20. People above Q? → (b) 2**
Q is on floor 5. Above are floors 6 (V) and 7 (S) ⇒ **2 people**.

**Answer: (b) 2**

---

### 🟡 SET 5 — Solutions 21–25

**Building the schedule.**

| Order | Clue | Deduction |
|---|---|---|
| 1 | A attends on Wednesday | **A → Wed** |
| 2 | B attends two days after A | Wed + 2 = **B → Fri** |
| 3 | E attends immediately after B | **E → Sat** |
| 4 | D attends on Monday | **D → Mon** |
| 5 | C attends before Wed but not Monday | Only Tuesday remains ⇒ **C → Tue** |
| 6 | (remaining) | **F → Thu** |

**Final schedule:**

| Day | Person |
|---|---|
| Monday | D |
| Tuesday | C |
| Wednesday | A |
| Thursday | F |
| Friday | B |
| Saturday | E |

---

**Q21. Who attends on Thursday? → (c) F**

**Answer: (c) F**

---

**Q22. Immediately before A? → (b) C**
A is on Wednesday; the previous day, Tuesday, belongs to **C**.

**Answer: (b) C**

---

**Q23. People between C and B? → (b) 2**
C is on Tuesday, B on Friday. Between them are **Wednesday (A) and Thursday (F)** = 2 people.

**Answer: (b) 2**

---

**Q24. E's day? → (c) Saturday**

**Answer: (c) Saturday**

---

**Q25. Who attends on the last day? → (b) E**
The last day is Saturday ⇒ **E**.

**Answer: (b) E**

---

### 🟡 SET 6 — Solutions 26–30

**Building the arrangement.**

**Step 1 — Frame (8 seats, facing north).**
```
    1     2     3     4     5     6     7     8
```

**Step 2 — Apply the clues in order of definiteness.**

| Order | Clue | Deduction |
|---|---|---|
| 1 | D sits third from the left | **D → 3** |
| 2 | B is immediately right of D | **B → 4** |
| 3 | G is third to the right of B(4) | **G → 7** |
| 4 | A is at an extreme end | Ends are 1 and 8 |
| 5 | Only two people between A and F | Gap = **3** |

Testing A = 1: F would be at 4, but that is B ⇒ **rejected**.
Testing A = 8: F would be at 5 ⇒ **A → 8, F → 5** ✓

| Order | Clue | Deduction |
|---|---|---|
| 6 | E sits at an extreme end | Seat 8 is A ⇒ **E → 1** |
| 7 | C is not adjacent to D(3) | C ≠ 2, 4. Seats left are 2 and 6 ⇒ **C → 6** |
| 8 | H sits to the left of C(6) | The only seat left is 2 ⇒ **H → 2** ✓ (2 < 6) |

**Final arrangement:**
```
    1     2     3     4     5     6     7     8
  ┌───┬───┬───┬───┬───┬───┬───┬───┐
  │ E │ H │ D │ B │ F │ C │ G │ A │
  └───┴───┴───┴───┴───┴───┴───┴───┘
```

**Verification:** D 3rd from left ✓ · two people (B, ...) — check: between A(8) and F(5) are seats 6 and 7 = C and G = **2 people** ✓ · B immediately right of D ✓ · G third right of B ✓ · A at an end ✓ · C(6) not adjacent to D(3) ✓ · H(2) left of C(6) ✓ · E at an end ✓

---

**Q26. Immediately left of F? → (b) B**
F is at 5, so seat 4 = **B**.

**Answer: (b) B**

---

**Q27. People between H and G? → (c) 4**
H is at 2, G at 7. Seats between: 3, 4, 5, 6 ⇒ D, B, F, C = **4 people**.

*(Gap = 7 − 2 − 1 = 4.)*

**Answer: (c) 4**

---

**Q28. Extreme right? → (a) A**
Seat 8 holds **A**.

**Answer: (a) A**

---

**Q29. C's position from the right? → (b) Third**
C is at seat 6 in a row of 8:
$$8 - 6 + 1 = 3 \implies \textbf{third from the right}$$

**Answer: (b) Third**

---

**Q30. Third to the left of C? → (b) D**
C is at 6. Three positions to the left ⇒ seat **3** = **D**.

**Answer: (b) D**

---

### 🟡 SET 7 — Solutions 31–35

**Building the stack.**

**Step 1 — Frame (6 levels, 1 at the bottom).**

**Step 2 — Apply the fixed clue.**
S is at the bottom ⇒ **S → 1**

**Step 3 — Work through the constraints systematically.**
The remaining constraints are:
- R = P + 1 (R immediately above P)
- |P − Q| = 3 (two boxes between them)
- T = U + 1 (T immediately above U)

Positions 2–6 are available for P, Q, R, T and U.

**Test each possible P:**

| P | R = P+1 | Q = P±3 | Remaining two positions | Consecutive for T/U? |
|---|---|---|---|---|
| 2 | 3 | 5 | 4, 6 | ✗ not consecutive |
| 3 | 4 | 6 | 2, 5 | ✗ not consecutive |
| 4 | 5 | 7 (invalid) or 1 (= S) | — | ✗ |
| **5** | **6** | **2** | **3, 4** | **✓ consecutive** |

**Step 4 — Resolve T and U.**
With positions 3 and 4 left and T immediately above U:
$$U \to 3, \qquad T \to 4$$

**Final stack:**
```
  Position 6   R    ← top
  Position 5   P
  Position 4   T
  Position 3   U
  Position 2   Q
  Position 1   S    ← bottom
```

**Verification:** R immediately above P ✓ · two boxes (U, T) between Q(2) and P(5) ✓ · S at the bottom ✓ · T immediately above U ✓

---

**Q31. Box at the top? → (c) R**

**Answer: (c) R**

---

**Q32. Immediately below P? → (c) T**
P is at position 5, so position 4 = **T**.

**Answer: (c) T**

---

**Q33. Boxes between Q and P? → (b) 2**
Q is at 2, P at 5. Between them are positions 3 and 4 ⇒ U and T = **2 boxes**.

**Answer: (b) 2**

---

**Q34. Third from the bottom? → (c) U**
Counting up: 1 = S, 2 = Q, 3 = **U**.

**Answer: (c) U**

---

**Q35. Immediately above S? → (b) Q**
S is at the bottom (1), so position 2 = **Q**.

**Answer: (b) Q**

---

### 🔴 SET 8 — Solutions 36–40

**Building the arrangement.**

**Step 1 — Frame and convention.**
Eight seats numbered **clockwise**. Everyone faces the **centre**:
$$\text{clockwise} = \text{LEFT} \qquad \text{anticlockwise} = \text{RIGHT}$$
Opposite pairs in an 8-circle: 1↔5, 2↔6, 3↔7, 4↔8.

**Step 2 — Apply the clues.**

| Order | Clue | Deduction |
|---|---|---|
| 1 | Anchor | **A → 1** |
| 2 | C sits opposite A | **C → 5** |
| 3 | A is third to the **left** of B | Left = clockwise, so moving 3 clockwise from B reaches A ⇒ B = 1 − 3 = −2 → **B → 6** |
| 4 | D is immediately **left** of B(6) | Left = clockwise ⇒ **D → 7** |
| 5 | E is second to the **right** of C(5) | Right = anticlockwise, two places ⇒ **E → 3** |
| 6 | G is immediately **right** of A(1) | Anticlockwise ⇒ **G → 8** |
| 7 | H is immediately **left** of A(1) | Clockwise ⇒ **H → 2** |
| 8 | (remaining) | **F → 4** |

**Final arrangement (clockwise):**
```
                    A(1)
              G(8)        H(2)
          D(7)      IN        E(3)
              B(6)        F(4)
                    C(5)
```

**Verification:** C opposite A (1↔5) ✓ · three clockwise from B(6): 7, 8, 1 = A ✓ · D immediately clockwise of B ✓ · E two anticlockwise from C(5): 4, 3 ✓ · G immediately anticlockwise of A ✓ · H immediately clockwise of A ✓

---

**Q36. Opposite B? → (d) H**
B is at 6. Opposite of 6 is **2** = **H**.

**Answer: (d) H**

---

**Q37. Between C and D? → (b) B**
C is at 5, D at 7. The seat between is **6** = **B**.

**Answer: (b) B**

---

**Q38. Immediate right of E? → (b) F**
E is at 3. Right = **anticlockwise** ⇒ position 4 = **F**.

**Answer: (b) F**

---

**Q39. People between A and C, clockwise from A? → (b) 3**
From A(1) clockwise to C(5): positions 2, 3, 4 ⇒ H, E, F = **3 people**.

**Answer: (b) 3**

---

**Q40. Opposite F? → (c) G**
The opposite pairs in an 8-circle are 1↔5, 2↔6, 3↔7, **4↔8**.
F is at position 4, so the person opposite sits at position **8** = **G**.

**Answer: (c) G**

---

### 🔴 SET 9 — Solutions 41–45

**Building the arrangement.**

**Step 1 — Place the direct facts.**

| Floor | Person | Car |
|---|---|---|
| 5 | ? | **Black** |
| 4 | **E** | ? |
| 3 | ? | **Red** |
| 2 | ? | ? |
| 1 | **C** | **Blue** |

**Step 2 — Deduce the remaining colours.**
Colours used: black (floor 5), red (floor 3), blue (floor 1).
Floors 2 and 4 must carry **white** and **green** in some order.

**Step 3 — Apply the D-and-white clue.**
"D lives immediately below the person who owns the white car."

- If white were on floor 2, D would be on floor 1 — but that is C ⇒ **rejected**
- Therefore white is on **floor 4**, and **D lives on floor 3**

So **E (floor 4) owns the white car**, and floor 2 carries the remaining colour, **green**.

**Step 4 — Place A and B.**
Floors left: **2** and **5**, for A and B.
A lives above B ⇒ **B → 2**, **A → 5**

**Final arrangement:**

| Floor | Person | Car |
|---|---|---|
| 5 | **A** | Black |
| 4 | **E** | White |
| 3 | **D** | Red |
| 2 | **B** | Green |
| 1 | **C** | Blue |

**Verification:** floor 3 has red ✓ · A(5) above B(2) ✓ · C on floor 1 with blue ✓ · D(3) immediately below the white owner E(4) ✓ · floor 5 has black ✓ · E on floor 4 ✓

---

**Q41. Who lives on floor 5? → (a) A**

**Answer: (a) A**

---

**Q42. D's car colour? → (a) Red**
D lives on floor 3, which carries the **red** car.

**Answer: (a) Red**

---

**Q43. Who owns the white car? → (d) E**
White is on floor 4, occupied by **E**.

**Answer: (d) E**

---

**Q44. B's floor? → (b) 2**

**Answer: (b) 2**

---

**Q45. Immediately above C? → (b) B**
C is on floor 1, so floor 2 = **B**.

**Answer: (b) B**

---

### 🔴 SET 10 — Solutions 46–50

**Building the grid.**

**Step 1 — Enter the direct facts.**

| Person | Sport | City |
|---|---|---|
| P | **Cricket** | **Bangalore** |
| Q | ? | **Mumbai** |
| R | **Hockey** | ? |
| S | ? | **Delhi** |
| T | ? | ? |

**Step 2 — Link tennis to Delhi.**
The tennis player lives in Delhi, and S lives in Delhi ⇒ **S plays tennis**.

**Step 3 — Narrow Q and T.**
Cricket, hockey and tennis are assigned ⇒ Q and T must have **badminton** and **football**.

**Step 4 — Use the badminton–Chennai link.**
The badminton player lives in **Chennai**. Q lives in **Mumbai** ⇒ Q cannot play badminton.
$$\implies \textbf{Q plays football}, \qquad \textbf{T plays badminton}$$
And therefore **T lives in Chennai** ✓ *(consistent with "T does not live in Kolkata")*

**Step 5 — Assign the last city.**
Cities used: Bangalore (P), Mumbai (Q), Delhi (S), Chennai (T).
Only **Kolkata** remains ⇒ **R lives in Kolkata**

**Final grid:**

| Person | Sport | City |
|---|---|---|
| P | Cricket | Bangalore |
| Q | Football | Mumbai |
| R | Hockey | Kolkata |
| S | Tennis | Delhi |
| T | Badminton | Chennai |

---

**Q46. Who likes badminton? → (d) T**

**Answer: (d) T**

---

**Q47. Where does R live? → (c) Kolkata**

**Answer: (c) Kolkata**

---

**Q48. Q's sport? → (b) Football**

**Answer: (b) Football**

---

**Q49. Who lives in Delhi? → (d) S**

**Answer: (d) S**

---

**Q50. Sport of the Bangalore resident? → (a) Cricket**
P lives in Bangalore and plays **cricket**.

**Answer: (a) Cricket**

---

## 8. Quick Revision Sheet

> **One page. Read 48 hours after study, and again the night before the test.**

### The seven-step framework

```
1.  Identify the SHAPE and SIZE
2.  Draw the frame with numbered positions
3.  Mark the FACING direction beside every seat
4.  RANK the clues:
        ★★★ absolute position     ("third from the left")
        ★★  relative + anchored   ("immediately right of C")
        ★   relative only         ("between X and Y")
        —   negative              ("not adjacent to D")
5.  Place ★★★ first, then ★★, then ★
6.  Use NEGATIVE clues to eliminate at the end
7.  VERIFY every clue on the finished diagram
```

### Position vocabulary

```
"Third from the left"       →  position 3
"Third from the right"      →  position n − 2
"Immediate left of X"       →  X − 1
"Second to the left of X"   →  X − 2      ← TWO places, not one
"k people between A and B"  →  |A − B| = k + 1

Position from the right = n − (position from the left) + 1
```

### ⭐ Circular convention

```
FACING THE CENTRE (standard)
    clockwise      =  each person's LEFT
    anticlockwise  =  each person's RIGHT

FACING OUTWARD
    reverse both

OPPOSITE SEATS
    6 people:  1↔4  2↔5  3↔6
    8 people:  1↔5  2↔6  3↔7  4↔8
    n people:  p ↔ p + n/2  (wrap around)

Write "IN" or "OUT" in the middle of your circle BEFORE placing anyone.
```

### Linear facing rule

```
FACING NORTH  →  person's left = toward position 1   (matches the reader)
FACING SOUTH  →  EVERYTHING REVERSES

In mixed-facing rows, write N or S beside every single person.
```

### Floors and boxes

```
Floor n = TOP        Floor 1 = BOTTOM

"Immediately above X"   →  X + 1
"Immediately below X"   →  X − 1
"k people between"      →  gap of k + 1

Test candidate placements systematically — a table of cases
beats guesswork when two constraints interact.
```

### Matrix puzzles

```
Build a GRID with one row per person and one column per attribute.

Fill DIRECT facts first.
Then use ATTRIBUTE-TO-ATTRIBUTE clues ("the tennis player lives in Delhi")
    — these are usually the most powerful.
Finish by ELIMINATION.
```

### Timing discipline

```
Puzzle resisting after 2 MINUTES?  →  flag it and move on.
A 5-question set is worth 5 marks — but so are five easy questions
elsewhere, and those take 2 minutes total.
```

### Sanity checks

```
✓ Every person placed exactly once; every seat filled exactly once
✓ EVERY clue re-checked against the final diagram
✓ Circular: verify the opposite pairs
✓ Floors: "k between" = gap of k+1
✓ Facing direction noted wherever it varies
```

---

## 9. Common Mistakes

| # | Mistake | Example | Correction |
|---|---|---|---|
| 1 | **"Second to the left" read as "immediate left"** | Placing D at A − 1 | Second = **two** positions away |
| 2 | **"k between" gap miscounted** | Two between ⇒ gap of 2 | Gap = **k + 1** = 3 |
| 3 | **Circular direction inverted** | Facing centre, left = anticlockwise | Facing centre, left = **clockwise** |
| 4 | **Facing direction ignored** | Same left/right for all in a mixed row | Mark N or S beside each person |
| 5 | **Clues worked in the given order** | Starting with a vague clue | Rank by definiteness first |
| 6 | **Negative clues used to place** | "Not adjacent to D" ⇒ placing someone | Use them to **eliminate**, at the end |
| 7 | **No verification pass** | Answering from a half-checked diagram | Walk through every clue at the end |
| 8 | **Branching avoided** | Staring at an ambiguous clue | Try both cases; one will contradict |
| 9 | **Opposite seat miscomputed** | Opposite of 4 in an 8-circle given as 7 | 4 + 4 = **8** |
| 10 | **Question wording misread after solving** | Naming a person when a count was asked | Re-read each question |
| 11 | **Position from the wrong end** | Giving 6th when 3rd-from-right was asked | n − p + 1 |
| 12 | **Time sunk on one puzzle** | Five minutes on a single set | Two-minute rule: flag and move on |

---

## Practice Answer Key

| Q | Ans | Q | Ans | Q | Ans | Q | Ans | Q | Ans |
|---|---|---|---|---|---|---|---|---|---|
| 1 | c | 11 | c | 21 | c | 31 | c | 41 | a |
| 2 | a | 12 | c | 22 | b | 32 | c | 42 | a |
| 3 | c | 13 | d | 23 | b | 33 | b | 43 | d |
| 4 | d | 14 | b | 24 | c | 34 | c | 44 | b |
| 5 | c | 15 | a | 25 | b | 35 | b | 45 | b |
| 6 | b | 16 | c | 26 | b | 36 | d | 46 | d |
| 7 | c | 17 | a | 27 | c | 37 | b | 47 | c |
| 8 | c | 18 | c | 28 | a | 38 | b | 48 | b |
| 9 | b | 19 | a | 29 | b | 39 | b | 49 | d |
| 10 | d | 20 | b | 30 | b | 40 | c | 50 | a |

**Scoring guide:** 40+/50 → strong (puzzles are all-or-nothing per set, so scores cluster). 30–39 → solid; drill the circular-direction convention and the "k between" arithmetic. Below 30 → work through the ten sets again slowly, **writing out the full arrangement each time**. Speed comes only after the method is automatic.

---

**⬅️ Back:** [Topic 15 — Blood Relations & Direction Sense](15-blood-relations-direction-sense.md) · **➡️ Next:** [Topic 17 — Syllogisms & Venn Diagrams](17-syllogisms-venn-diagrams.md)
