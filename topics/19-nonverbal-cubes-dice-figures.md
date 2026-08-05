# Topic 19 — Cubes, Dice & Non-verbal Reasoning

### EY Placement Aptitude Handbook · Priority Rank #22 · 🟡 Medium

> **Questions in this file are original, modelled on publicly reported EY test patterns. They are not claimed to be actual previous-year EY questions.**

---

## Contents

1. [Why This Topic Matters for EY](#1-why-this-topic-matters-for-ey)
2. [Core Concepts — Painted Cubes](#2-core-concepts--part-a-painted-cubes)
3. [Core Concepts — Dice](#3-core-concepts--part-b-dice)
4. [Core Concepts — Figures & Mirrors](#4-core-concepts--part-c-figures-mirrors--water-images)
5. [Shortcuts & Tricks](#5-shortcuts--tricks)
6. [Solved Examples](#6-solved-examples)
7. [Practice Questions (50)](#7-practice-questions)
8. [Detailed Solutions](#8-detailed-solutions)
9. [Quick Revision Sheet](#9-quick-revision-sheet)
10. [Common Mistakes](#10-common-mistakes)

---

## 1. Why This Topic Matters for EY

**Weightage:** 4–6% of the reasoning section — roughly **0–1 questions** in Patterns A and B, but **substantially more** in Pattern C, whose "inductive reasoning" block is built almost entirely from abstract figure sequences.

**Be strategic about this topic.** The painted-cube formulas take fifteen minutes to learn and then never fail you. The dice rules take another ten. Abstract figure series are harder to prepare for on paper, but the transformation vocabulary in Section 4 covers most of what appears.

**Question styles reported:**

| Sub-topic | Typical shape |
|---|---|
| **Painted cubes** | "A cube of side 4 is painted and cut into 64 — how many have 2 faces painted?" |
| **Cubes, partial painting** | "Painted on all faces except the bottom" |
| **Dice — opposite faces** | "Which number is opposite 3?" |
| **Dice — two views** | Two positions shown; deduce the hidden face |
| **Figure series** | Rotation, reflection, element count |
| **Mirror images** | Reflection about a vertical axis |
| **Water images** | Reflection about a horizontal axis |
| **Paper folding / cutting** | Fold, punch, unfold |

---

## 2. Core Concepts — PART A: PAINTED CUBES

### 2.1 The setup

A large cube of side *n* units is painted on **all six faces**, then cut into **n³** unit cubes.

Each small cube lies in exactly one of four categories, determined by its **position**:

```
              CORNER  →  3 painted faces
                EDGE  →  2 painted faces
                FACE  →  1 painted face
            INTERIOR  →  0 painted faces
```

### 2.2 ⭐ The four formulas

$$\boxed{
\begin{aligned}
\text{3 faces painted (corners)} &= 8 \quad \text{(always, for any } n\text{)}\\
\text{2 faces painted (edges)} &= 12(n-2)\\
\text{1 face painted (faces)} &= 6(n-2)^2\\
\text{0 faces painted (interior)} &= (n-2)^3
\end{aligned}}$$

**The verification identity — use it every time:**

$$8 + 12(n-2) + 6(n-2)^2 + (n-2)^3 = n^3$$

**Why each formula holds:**

| Category | Reasoning |
|---|---|
| **Corners** | A cube has exactly **8** corners, regardless of size |
| **Edges** | A cube has **12** edges; each contributes (n − 2) non-corner cubes |
| **Faces** | A cube has **6** faces; each contributes an (n−2) × (n−2) inner square |
| **Interior** | The hidden core is a cube of side (n − 2) |

### 2.3 The reference table

| n | Total n³ | 3 faces | 2 faces | 1 face | 0 faces |
|---|---|---|---|---|---|
| **2** | 8 | 8 | 0 | 0 | 0 |
| **3** | 27 | 8 | 12 | 6 | 1 |
| **4** | 64 | 8 | 24 | 24 | 8 |
| **5** | 125 | 8 | 36 | 54 | 27 |
| **6** | 216 | 8 | 48 | 96 | 64 |
| **7** | 343 | 8 | 60 | 150 | 125 |
| **10** | 1000 | 8 | 96 | 384 | 512 |

> **The n = 2 case.** Every one of the 8 unit cubes is a corner, so all have exactly 3 painted faces and the other three categories are empty. Check that your formulas reproduce this: 12(0) = 0, 6(0)² = 0, (0)³ = 0 ✓

### 2.4 Derived quantities

$$\text{At least one face painted} = n^3 - (n-2)^3$$
$$\text{Surface cubes} = n^3 - (n-2)^3 \quad \text{(the same set)}$$

> Side 5: at least one face painted = 125 − 27 = **98**

### 2.5 Partial painting

When some faces are left unpainted, **stop using the formulas and count by coordinates**.

Set up axes with each coordinate running 1…n:

```
x = 1 or n   →  on a left/right face
y = 1 or n   →  on a front/back face
z = 1        →  on the BOTTOM face
z = n        →  on the TOP face
```

> **Cube of side 4, painted on all faces EXCEPT the bottom. How many unit cubes have no paint?**
>
> A cube is unpainted when it avoids every painted face:
> ```
> x ∈ {2, 3}      (avoids the left and right faces)     →  2 choices
> y ∈ {2, 3}      (avoids the front and back faces)     →  2 choices
> z ∈ {1, 2, 3}   (avoids only the TOP; bottom is safe) →  3 choices
> ```
> $$\text{Count} = 2 \times 2 \times 3 = \mathbf{12}$$

> **Compare with the fully-painted case:** (4 − 2)³ = 8. Leaving the bottom unpainted adds the four central cubes of the bottom layer, giving 12.

### 2.6 Multi-colour cubes

If the six faces are painted in three colours (opposite faces sharing a colour), the categories map directly:

| Painted faces | Colours seen |
|---|---|
| 3 (corner) | **3 colours** (three mutually adjacent faces, all different) |
| 2 (edge) | **2 colours** |
| 1 (face) | **1 colour** |
| 0 (interior) | none |

> Side 4, three colour-pairs: cubes showing exactly 3 colours = the 8 corners.

---

## 3. Core Concepts — PART B: DICE

### 3.1 The standard die

$$\boxed{\text{Opposite faces sum to } 7}$$

| Face | Opposite |
|---|---|
| 1 | **6** |
| 2 | **5** |
| 3 | **4** |

$$\text{Total of all six faces} = 1+2+3+4+5+6 = 21$$

**Consequences worth memorising:**

$$\text{Top} + \text{Bottom} = 7$$
$$\text{Sum of the four side faces} = 21 - 7 = 14 \quad \text{(always, whatever is on top)}$$

### 3.2 Adjacency

Each face is **adjacent to four faces** and **opposite to exactly one**.

```
        If 1 is on top,
        the four visible sides are 2, 3, 4 and 5 (in some order),
        and 6 is hidden at the bottom.
```

> **The deduction rule:** if a number appears **adjacent** to a face in any view, it cannot be opposite that face. Rule out the four adjacents and the fifth number must be the opposite.

### 3.3 The two-view technique

Two positions of the same die are shown; deduce which numbers are opposite.

**Case A — a common number appears in both views.**

```
View 1:  top = 1, front = 2, right = 3
View 2:  top = 1, front = 4, right = 5

The number 1 stays on top in both.
Therefore 2, 3, 4 and 5 are ALL adjacent to 1.
The only remaining number is 6  ⇒  6 is OPPOSITE 1.
```

**Case B — no number repeats between views.**
Combine the adjacency information from both views and eliminate. Every number you observe next to a face is adjacent to it.

**Case C — two numbers repeat in the same positions.**
The die has simply been rotated about the axis through those two faces; the remaining faces have cycled.

### 3.4 Rotations

```
Rotating about a vertical axis  →  top and bottom UNCHANGED; the four sides cycle
Rotating about a horizontal axis →  top, bottom, front, back cycle; left and right unchanged
```

> A die shows 3 on top and 5 in front. It is tipped forward through 90°, so the front face becomes the top.
> ⇒ **5 is now on top**, and the old top (3) has moved to the back.

### 3.5 Corner rule

Three mutually adjacent faces meet at each corner. At the **diagonally opposite corner**, the three faces are their opposites.

> If 1, 2 and 3 meet at one corner, then **6, 5 and 4** meet at the opposite corner.

---

## 4. Core Concepts — PART C: FIGURES, MIRRORS & WATER IMAGES

### 4.1 The transformation vocabulary

Abstract figure series use a small, closed set of transformations. Learn to name them:

| Transformation | What changes |
|---|---|
| **Rotation** | The whole figure turns 45°, 90°, 135° or 180° |
| **Reflection** | The figure flips about a vertical or horizontal axis |
| **Translation** | An element moves position (often around the perimeter) |
| **Addition** | An element is added each step |
| **Deletion** | An element is removed each step |
| **Substitution** | One shape becomes another |
| **Shading alternation** | Filled ↔ unfilled |
| **Count progression** | The number of dots, lines or sides increases by a fixed amount |

### 4.2 Rotation arithmetic

$$\text{Net rotation after } k \text{ steps of } \theta = k\theta \pmod{360°}$$

| Step angle | Returns to start after |
|---|---|
| 45° | 8 steps |
| 90° | 4 steps |
| 120° | 3 steps |
| 180° | 2 steps |

> A triangle rotating 45° clockwise per step returns to its original orientation after **8 steps** (8 × 45 = 360°).

### 4.3 Cyclic position

An element moving around a fixed number of positions returns to its start after that many steps.

> A dot moving one corner clockwise around a square is back at its starting corner after **4 steps**.

**Position after k steps** = (start + k) mod (number of positions)

### 4.4 Mirror images (vertical axis)

A **mirror image** reflects the figure **left ↔ right**. Top and bottom are unchanged.

```
    ORIGINAL          |         MIRROR
        b             |            d
        p             |            q
       PQR            |          ЯQP  (reversed order, each letter flipped)
```

**Letters unchanged by a vertical mirror** (they have vertical symmetry):

$$\textbf{A, H, I, M, O, T, U, V, W, X, Y}$$

**Words unchanged:** MOM, TOOT, WOW, HIM (letter-wise), MAXIMUM, TOMATO

> **Careful:** in a mirror, the *order* of letters also reverses. "MOM" survives because it is a palindrome of vertically-symmetric letters. "HIM" reverses to "MIH" even though each letter is individually symmetric.

### 4.5 Water images (horizontal axis)

A **water image** reflects the figure **top ↔ bottom**. Left and right are unchanged.

```
    ORIGINAL          |       WATER IMAGE
        b             |            p
        d             |            q
        N             |            И-like inversion
```

**Letters unchanged by a water image** (they have horizontal symmetry):

$$\textbf{B, C, D, E, H, I, K, O, X}$$

> **The b/d/p/q family is the classic test:**
> ```
> b  --mirror-->  d          b  --water-->  p
> d  --mirror-->  b          d  --water-->  q
> ```

### 4.6 Paper folding and punching

```
1.  Count the FOLDS
2.  Each fold DOUBLES the number of holes:  holes = 2^(number of folds)
3.  Holes appear SYMMETRICALLY about each fold line
```

> A square sheet folded twice and punched once yields **2² = 4** holes when unfolded, arranged symmetrically about both fold lines.

---

## 5. Shortcuts & Tricks

### 5.1 The painted-cube memory device

```
CORNERS  →  always 8              (a cube has 8 corners, whatever its size)
EDGES    →  12 × (n − 2)          (12 edges, each with n−2 middle cubes)
FACES    →  6 × (n − 2)²          (6 faces, each an (n−2)² inner square)
INTERIOR →  (n − 2)³              (a hidden cube of side n − 2)

Let m = n − 2.  Then:  8 · 12m · 6m² · m³
And these sum to (m + 2)³ = n³  ✓
```

Every formula contains **(n − 2)**. Compute that value first and everything else falls out.

### 5.2 Always run the verification sum

```
n = 5:   8 + 12(3) + 6(9) + 27
       = 8 + 36 + 54 + 27
       = 125 = 5³  ✓
```

Thirty seconds of checking catches every arithmetic slip in this question type.

### 5.3 Dice — the three facts that cover most questions

```
1.  Opposite faces sum to 7
2.  All six faces sum to 21
3.  The four side faces always sum to 14  (21 − 7)
```

### 5.4 The elimination approach for dice

```
Any number seen ADJACENT to a face cannot be OPPOSITE it.
Rule out all four adjacents; the remaining number is the opposite.
```

> If 3 is seen alongside 1, 2, 5 and 6 across several views, the only number left is **4** ⇒ 4 is opposite 3.

### 5.5 The mirror/water letter lists

```
VERTICAL MIRROR leaves unchanged:   A H I M O T U V W X Y
HORIZONTAL (water) leaves unchanged: B C D E H I K O X

Both:  H  I  O  X       ← unchanged either way
```

### 5.6 The figure-series checklist

Work through these in order:

```
□  Does the figure ROTATE?          by how many degrees?
□  Does it REFLECT?                 about which axis?
□  Do ELEMENTS move?                in which direction, how far?
□  Is anything ADDED or REMOVED?    how many per step?
□  Does SHADING alternate?          on what cycle?
□  Does a COUNT progress?           by what increment?
```

Most series combine **exactly two** of these. Identify both and the answer follows.

### 5.7 Sanity checks

```
CUBES
✓ The four categories must sum to n³
✓ Corners are ALWAYS 8
✓ For n = 2, only corners exist
✓ Partial painting ⇒ count by coordinates, not by formula

DICE
✓ Opposite faces sum to 7
✓ The four sides always total 14
✓ A number cannot be both adjacent and opposite to the same face

FIGURES
✓ Rotation totals reduce mod 360°
✓ Mirror flips LEFT–RIGHT; water flips TOP–BOTTOM
✓ Letter order reverses in a mirror image
```

---

## 6. Solved Examples

### Example 1 — The full painted-cube breakdown

**Q.** A cube of side 5 cm is painted red on all its faces and then cut into 125 cubes of side 1 cm. How many small cubes have (a) three faces painted, (b) two faces painted, (c) exactly one face painted, and (d) no face painted?

**Step 1 — Compute n − 2.**
$$n = 5 \implies n - 2 = 3$$

**Step 2 — Apply the four formulas.**

**(a) Three faces painted — the corners:**
$$= 8 \quad \text{(always)}$$

**(b) Two faces painted — the edges:**
$$12(n-2) = 12 \times 3 = 36$$

**(c) One face painted — the face centres:**
$$6(n-2)^2 = 6 \times 9 = 54$$

**(d) No face painted — the interior:**
$$(n-2)^3 = 27$$

**Step 3 — Verify.**
$$8 + 36 + 54 + 27 = 125 = 5^3 \checkmark$$

**Answer: (a) 8 (b) 36 (c) 54 (d) 27**

---

### Example 2 — Partial painting

**Q.** A cube of side 4 cm is painted on all faces except the bottom, then cut into 64 unit cubes. How many unit cubes have no paint on them?

**Step 1 — Recognise that the formulas do not apply.**
The standard formulas assume **all six** faces are painted. With one face unpainted, count by coordinates.

**Step 2 — Set up coordinates.**
Let each of x, y and z run over {1, 2, 3, 4}, with z = 1 at the bottom and z = 4 at the top.

Painted faces: **top** (z = 4), **left/right** (x = 1 or 4), **front/back** (y = 1 or 4).
The **bottom** (z = 1) is unpainted.

**Step 3 — Determine which cubes escape all painted faces.**

| Coordinate | Allowed values | Count |
|---|---|---|
| x | 2, 3 (avoid x = 1, 4) | 2 |
| y | 2, 3 (avoid y = 1, 4) | 2 |
| z | 1, 2, 3 (avoid only z = 4) | **3** |

**Step 4 — Multiply.**
$$2 \times 2 \times 3 = 12$$

**Answer: 12 unit cubes have no paint**

> **Compare with the fully painted case:** (4 − 2)³ = **8**. Leaving the bottom face unpainted frees up the **four central cubes of the bottom layer**, taking the total from 8 to 12.

---

### Example 3 — Dice, opposite faces

**Q.** Two positions of the same die are shown below.

```
   Position 1:  top = 1,  front = 2,  right = 3
   Position 2:  top = 1,  front = 4,  right = 5
```

Which number lies opposite 1?

**Step 1 — Note what the two views share.**
The number **1** occupies the top face in both positions.

**Step 2 — Collect everything adjacent to 1.**
In position 1, the faces 2 and 3 are visible alongside 1 ⇒ both are adjacent to 1.
In position 2, the faces 4 and 5 are visible alongside 1 ⇒ both are adjacent to 1.

$$\text{Adjacent to 1: } \{2, 3, 4, 5\}$$

**Step 3 — Eliminate.**
A die face is adjacent to exactly four faces and opposite to one. Four numbers are accounted for, so the remaining number must be the opposite.

$$\{1,2,3,4,5,6\} \setminus \{1, 2, 3, 4, 5\} = \{6\}$$

**Answer: 6 lies opposite 1**

**Cross-check with the standard rule:** 1 + 6 = 7 ✓

---

### Example 4 — Dice, sum of side faces

**Q.** A standard die rests on a table with 5 on the top face. What is the sum of the numbers on the four vertical (side) faces?

**Step 1 — Find the bottom face.**
$$\text{Bottom} = 7 - 5 = 2$$

**Step 2 — Subtract the top and bottom from the total.**
$$\text{All faces} = 21$$
$$\text{Four sides} = 21 - (5 + 2) = 21 - 7 = 14$$

**Answer: 14**

> **This answer never changes.** Whatever number is on top, the top and bottom always sum to 7, so the four sides always sum to 21 − 7 = **14**. It is worth recognising instantly.

---

### Example 5 — Mirror and water images

**Q.** Find (a) the mirror image and (b) the water image of the letter **d**.

**(a) Mirror image — reflect left ↔ right.**

```
    d   ──vertical mirror──►   b
```

The bowl of the *d* sits on the left of its stem; reflecting left-to-right moves it to the right, producing **b**.

**(b) Water image — reflect top ↔ bottom.**

```
    d   ──horizontal flip──►   q
```

The stem of the *d* rises above the bowl; flipping vertically drops it below, producing **q**.

**Answer: (a) b (b) q**

**The complete family:**

| Letter | Mirror (vertical axis) | Water (horizontal axis) |
|---|---|---|
| b | **d** | **p** |
| d | **b** | **q** |
| p | **q** | **b** |
| q | **p** | **d** |

---

### Example 6 — Figure rotation series

**Q.** A figure rotates 60° clockwise at each step. After how many steps does it first return to its original orientation? What is its net rotation after 10 steps?

**Part 1 — Return to the start.**
$$k \times 60° = 360° \implies k = 6 \text{ steps}$$

**Part 2 — Net rotation after 10 steps.**
$$10 \times 60° = 600°$$
$$600° \bmod 360° = 240°$$

So after 10 steps the figure has effectively turned **240° clockwise** from its starting orientation — equivalently **120° anticlockwise**.

**Answer: it returns after 6 steps; after 10 steps the net rotation is 240° clockwise**

---

### Example 7 — Multi-colour cube

**Q.** A cube is painted red on two opposite faces, green on two opposite faces and blue on the remaining two faces. It is then cut into 64 equal smaller cubes. How many small cubes show exactly three colours, and how many show exactly one colour?

**Step 1 — Relate colours to painted faces.**
Since opposite faces share a colour, any **three mutually adjacent faces** carry three *different* colours.

| Position | Painted faces | Colours shown |
|---|---|---|
| Corner | 3 | **3** |
| Edge | 2 | **2** |
| Face centre | 1 | **1** |
| Interior | 0 | 0 |

**Step 2 — Apply the formulas with n = 4.**

**Exactly three colours** = corner cubes:
$$= 8$$

**Exactly one colour** = face-centre cubes:
$$6(n-2)^2 = 6 \times 4 = 24$$

**Step 3 — Verify the full breakdown.**
$$8 \; (\text{3 colours}) + 24 \; (\text{2 colours}) + 24 \; (\text{1 colour}) + 8 \; (\text{none}) = 64 \checkmark$$

**Answer: 8 cubes show three colours; 24 show exactly one colour**

> **Why "three mutually adjacent faces must be different colours":** each colour occupies an *opposite pair*, and no two faces meeting at a corner are opposite one another. So the three faces at a corner belong to three different pairs.

---

### Example 8 — Paper folding

**Q.** A square sheet of paper is folded in half, then folded in half again, and a single hole is punched through all layers. How many holes appear when the sheet is unfolded, and how are they arranged?

**Step 1 — Count the layers.**
$$\text{Fold 1} \to 2 \text{ layers} \qquad \text{Fold 2} \to 4 \text{ layers}$$

**Step 2 — Apply the doubling rule.**
$$\text{Holes} = 2^{\text{number of folds}} = 2^2 = 4$$

**Step 3 — Determine the arrangement.**
The holes appear **symmetrically about both fold lines** — one in each quadrant of the sheet, all at the same relative position within its quadrant.

```
    ┌─────────┬─────────┐
    │    ●    │    ●    │
    ├─────────┼─────────┤     ← fold line 1
    │    ●    │    ●    │
    └─────────┴─────────┘
              ↑
         fold line 2
```

**Answer: 4 holes, one in each quadrant, symmetric about both fold lines**

---

## 7. Practice Questions

**Instructions:** Q1–20 Painted cubes · Q21–35 Dice · Q36–50 Figures, mirrors and water images.
Full solutions in [Section 8](#8-detailed-solutions).

---

### 🟢 PAINTED CUBES (Questions 1–20)

**Q1.** A cube of side 4 cm is painted on all faces and cut into cubes of side 1 cm. How many small cubes are obtained?
(a) 16  (b) 32  (c) 48  (d) 64

**Q2.** Using the data of Q1, how many small cubes have three faces painted?
(a) 4  (b) 6  (c) 8  (d) 12

**Q3.** Using the data of Q1, how many small cubes have exactly two faces painted?
(a) 12  (b) 16  (c) 24  (d) 36

**Q4.** Using the data of Q1, how many small cubes have exactly one face painted?
(a) 12  (b) 16  (c) 24  (d) 36

**Q5.** Using the data of Q1, how many small cubes have no face painted?
(a) 4  (b) 6  (c) 8  (d) 12

**Q6.** Using the data of Q1, what is the sum of the four categories (3-face, 2-face, 1-face, 0-face)?
(a) 56  (b) 60  (c) 64  (d) 72

**Q7.** A cube of side 5 cm is painted on all faces and cut into cubes of side 1 cm. How many small cubes are obtained?
(a) 25  (b) 75  (c) 100  (d) 125

**Q8.** Using the data of Q7, how many small cubes have three faces painted?
(a) 6  (b) 8  (c) 12  (d) 24

**Q9.** Using the data of Q7, how many small cubes have exactly two faces painted?
(a) 24  (b) 30  (c) 36  (d) 48

**Q10.** Using the data of Q7, how many small cubes have exactly one face painted?
(a) 36  (b) 45  (c) 54  (d) 60

**Q11.** Using the data of Q7, how many small cubes have no face painted?
(a) 8  (b) 18  (c) 27  (d) 36

**Q12.** A cube of side 3 cm is painted on all faces and cut into cubes of side 1 cm. How many small cubes have no face painted?
(a) 0  (b) 1  (c) 3  (d) 6

**Q13.** Using the data of Q12, how many small cubes have exactly two faces painted?
(a) 6  (b) 8  (c) 12  (d) 24

**Q14.** A cube of side 6 cm is painted on all faces and cut into cubes of side 1 cm. How many small cubes have exactly one face painted?
(a) 54  (b) 64  (c) 96  (d) 144

**Q15.** Using the data of Q14, how many small cubes have no face painted?
(a) 27  (b) 48  (c) 64  (d) 96

**Q16.** A cube is painted red on two opposite faces, green on two opposite faces and blue on the remaining two, then cut into 64 equal cubes. How many small cubes have exactly three colours on them?
(a) 4  (b) 8  (c) 12  (d) 24

**Q17.** Using the data of Q16, how many small cubes have exactly one colour on them?
(a) 8  (b) 16  (c) 24  (d) 36

**Q18.** A cube of side 4 cm is painted on all faces **except the bottom**, then cut into 64 unit cubes. How many unit cubes have no paint on them?
(a) 8  (b) 10  (c) 12  (d) 16

**Q19.** A cube of side 4 cm is cut into 64 unit cubes. How many of these lie on the surface of the large cube?
(a) 48  (b) 52  (c) 56  (d) 60

**Q20.** A cube of side 5 cm is painted on all faces and cut into 125 unit cubes. How many have at least one face painted?
(a) 88  (b) 94  (c) 98  (d) 108

---

### 🟡 DICE (Questions 21–35)

**Q21.** On a standard die, which number lies opposite 1?
(a) 2  (b) 4  (c) 5  (d) 6

**Q22.** On a standard die, which number lies opposite 2?
(a) 3  (b) 4  (c) 5  (d) 6

**Q23.** On a standard die, which number lies opposite 3?
(a) 2  (b) 4  (c) 5  (d) 6

**Q24.** A standard die shows 4 on its top face. What is on the bottom face?
(a) 1  (b) 2  (c) 3  (d) 5

**Q25.** What is the sum of the numbers on two opposite faces of a standard die?
(a) 5  (b) 6  (c) 7  (d) 8

**Q26.** A standard die has 1 on top and 2 facing north. Which number is on the bottom?
(a) 3  (b) 4  (c) 5  (d) 6

**Q27.** Two positions of a die are shown. In the first, 1 is on top with 2 and 3 visible on the sides. In the second, 1 is on top with 4 and 5 visible on the sides. Which number is opposite 1?
(a) 2  (b) 3  (c) 5  (d) 6

**Q28.** In a die, the number 3 is found to be adjacent to 1, 2, 5 and 6. Which number is opposite 3?
(a) 1  (b) 2  (c) 4  (d) 5

**Q29.** On a standard die, the faces showing 1, 2 and 3 meet at one corner. Which three faces meet at the diagonally opposite corner?
(a) 1, 2, 3  (b) 2, 3, 4  (c) 4, 5, 6  (d) 3, 4, 5

**Q30.** A standard die has 5 on its top face. What is the sum of the numbers on the four side faces?
(a) 12  (b) 14  (c) 16  (d) 18

**Q31.** What is the sum of the numbers on all six faces of a standard die?
(a) 18  (b) 20  (c) 21  (d) 24

**Q32.** A standard die shows 6 on top and 4 at the front. What number is at the back?
(a) 1  (b) 2  (c) 3  (d) 5

**Q33.** In a standard die, 1 is adjacent to 2, 3, 4 and 5. Which number is opposite 2?
(a) 3  (b) 4  (c) 5  (d) 6

**Q34.** A die shows 3 on top and 5 at the front. It is tipped forward through 90° so that the front face becomes the top. Which number is now on top?
(a) 2  (b) 3  (c) 4  (d) 5

**Q35.** Two standard dice are placed side by side showing 5 and 3 on their top faces. What is the sum of the numbers on their bottom faces?
(a) 4  (b) 6  (c) 8  (d) 10

---

### 🔴 FIGURES, MIRRORS & WATER IMAGES (Questions 36–50)

**Q36.** A square figure rotates 90° clockwise at each step. After 4 steps, its orientation is:
(a) Rotated 90°  (b) Rotated 180°  (c) Rotated 270°  (d) The same as the start

**Q37.** In a figure series, the number of dots increases by 2 at each step: 2, 4, 6, ? What comes next?
(a) 7  (b) 8  (c) 10  (d) 12

**Q38.** A figure contains 3 lines, then 4, then 5. How many lines does the next figure contain?
(a) 5  (b) 6  (c) 7  (d) 8

**Q39.** An arrow points north, then east, then south. In which direction does it point next?
(a) North  (b) East  (c) South  (d) West

**Q40.** A shape alternates between shaded and unshaded at each step. If figure 1 is shaded, what is figure 5?
(a) Shaded  (b) Unshaded  (c) Half-shaded  (d) Cannot be determined

**Q41.** A triangle rotates 45° clockwise at each step. After 8 steps, its orientation is:
(a) Rotated 45°  (b) Rotated 180°  (c) Rotated 270°  (d) The same as the start

**Q42.** A series of figures shows a triangle, a square and a pentagon. What is the next figure?
(a) Circle  (b) Hexagon  (c) Octagon  (d) Rectangle

**Q43.** A dot moves one corner clockwise around a square at each step. After 4 steps, the dot is at:
(a) The adjacent corner  (b) The opposite corner  (c) The starting corner  (d) The centre

**Q44.** A figure loses one line at each step: 6, 5, 4, ? How many lines does the next figure have?
(a) 2  (b) 3  (c) 4  (d) 5

**Q45.** A pattern rotates 180° at each step. After 3 steps from the start, its orientation is:
(a) The same as the start  (b) Rotated 90°  (c) Rotated 180°  (d) Rotated 270°

**Q46.** What is the mirror image (reflection about a vertical axis) of the letter **b**?
(a) b  (b) d  (c) p  (d) q

**Q47.** What is the water image (reflection about a horizontal axis) of the letter **b**?
(a) b  (b) d  (c) p  (d) q

**Q48.** What is the mirror image of the word **MOM**?
(a) MOM  (b) WOW  (c) NON  (d) MON

**Q49.** Which of the following letters looks unchanged in a vertical mirror?
(a) F  (b) H  (c) J  (d) R

**Q50.** A figure begins with 4 dots and gains 3 dots at each step. How many dots does it have after 4 steps?
(a) 12  (b) 14  (c) 16  (d) 18

---

## 8. Detailed Solutions

### 🟢 PAINTED CUBES — Solutions 1–20

---

**Q1. Cube of side 4 cut into 1 cm cubes. Total? → (d) 64**

$$n^3 = 4^3 = 64$$

**Answer: (d) 64**

---

**Q2. Three faces painted (n = 4)? → (c) 8**

**Formula used:** corners = **8**, always.

A cube has exactly 8 corners regardless of its size, and only corner cubes touch three painted faces.

**Answer: (c) 8**

---

**Q3. Exactly two faces painted (n = 4)? → (c) 24**

**Formula used:** 12(n − 2)

$$12(4-2) = 12 \times 2 = 24$$

*(A cube has 12 edges; each contributes 2 non-corner cubes.)*

**Answer: (c) 24**

---

**Q4. Exactly one face painted (n = 4)? → (c) 24**

**Formula used:** 6(n − 2)²

$$6(4-2)^2 = 6 \times 4 = 24$$

*(Each of the 6 faces has a 2 × 2 inner square.)*

**Answer: (c) 24**

---

**Q5. No face painted (n = 4)? → (c) 8**

**Formula used:** (n − 2)³

$$(4-2)^3 = 2^3 = 8$$

*(The hidden core is a 2 × 2 × 2 cube.)*

**Answer: (c) 8**

---

**Q6. Sum of the four categories? → (c) 64**

$$8 + 24 + 24 + 8 = 64 = 4^3 \checkmark$$

The four categories are mutually exclusive and exhaustive, so they must total n³.

> **Run this check on every painted-cube question.** It takes ten seconds and catches every arithmetic error.

**Answer: (c) 64**

---

**Q7. Cube of side 5 cut into 1 cm cubes. Total? → (d) 125**

$$5^3 = 125$$

**Answer: (d) 125**

---

**Q8. Three faces painted (n = 5)? → (b) 8**

Corners = **8**, always.

**Answer: (b) 8**

---

**Q9. Exactly two faces painted (n = 5)? → (c) 36**

$$12(5-2) = 12 \times 3 = 36$$

**Answer: (c) 36**

---

**Q10. Exactly one face painted (n = 5)? → (c) 54**

$$6(5-2)^2 = 6 \times 9 = 54$$

**Answer: (c) 54**

---

**Q11. No face painted (n = 5)? → (c) 27**

$$(5-2)^3 = 27$$

**Verification of the whole set:** 8 + 36 + 54 + 27 = 125 ✓

**Answer: (c) 27**

---

**Q12. No face painted (n = 3)? → (b) 1**

$$(3-2)^3 = 1^3 = 1$$

Only the single cube at the very centre is completely hidden.

**Answer: (b) 1**

---

**Q13. Exactly two faces painted (n = 3)? → (c) 12**

$$12(3-2) = 12 \times 1 = 12$$

**Full breakdown for n = 3:** 8 corners + 12 edges + 6 face centres + 1 interior = **27** ✓

**Answer: (c) 12**

---

**Q14. Exactly one face painted (n = 6)? → (c) 96**

$$6(6-2)^2 = 6 \times 16 = 96$$

**Answer: (c) 96**

---

**Q15. No face painted (n = 6)? → (c) 64**

$$(6-2)^3 = 4^3 = 64$$

**Verification:** 8 + 12(4) + 6(16) + 64 = 8 + 48 + 96 + 64 = **216** = 6³ ✓

**Answer: (c) 64**

---

**Q16. Exactly three colours (three colour-pairs, 64 cubes)? → (b) 8**

**Step 1 — Relate colours to painted faces.**
Since each colour occupies an **opposite pair** of faces, and no two faces meeting at a corner are opposite one another, the three faces at any corner carry **three different colours**.

**Step 2 — Count the corner cubes.**
$$= 8$$

**Answer: (b) 8**

---

**Q17. Exactly one colour? → (c) 24**

A cube showing exactly one colour is one with exactly **one painted face** — a face-centre cube.

$$6(n-2)^2 = 6(4-2)^2 = 24$$

**Full colour breakdown for n = 4:**

| Colours shown | Position | Count |
|---|---|---|
| 3 | Corner | 8 |
| 2 | Edge | 24 |
| 1 | Face centre | **24** |
| 0 | Interior | 8 |
| | **Total** | **64** ✓ |

**Answer: (c) 24**

---

**Q18. Side 4, painted on all faces except the bottom. Unpainted cubes? → (c) 12**

**Step 1 — The standard formulas do not apply**, because one face is unpainted. Count by coordinates instead.

**Step 2 — Set up axes.**
Let x, y, z each run over {1, 2, 3, 4}, with **z = 1 the bottom** and **z = 4 the top**.

Painted: top (z = 4), left/right (x = 1 or 4), front/back (y = 1 or 4).
Unpainted: **bottom** (z = 1).

**Step 3 — Identify cubes touching no painted face.**

| Coordinate | Must avoid | Allowed values | Count |
|---|---|---|---|
| x | 1 and 4 | 2, 3 | 2 |
| y | 1 and 4 | 2, 3 | 2 |
| z | 4 only | 1, 2, 3 | **3** |

**Step 4 — Multiply.**
$$2 \times 2 \times 3 = 12$$

**Answer: (c) 12**

> **Where the extra 4 comes from.** With all six faces painted the answer would be (4 − 2)³ = 8. Leaving the bottom unpainted adds the **four central cubes of the bottom layer** (x, y ∈ {2,3}, z = 1), giving 12.

---

**Q19. Side 4 — how many unit cubes lie on the surface? → (c) 56**

**Method — total minus interior.**

$$\text{Surface cubes} = n^3 - (n-2)^3 = 64 - 8 = 56$$

**Cross-check by category:** 8 (corner) + 24 (edge) + 24 (face) = **56** ✓
*(Every cube with at least one painted face is on the surface.)*

**Answer: (c) 56**

---

**Q20. Side 5 — how many have at least one face painted? → (c) 98**

$$n^3 - (n-2)^3 = 125 - 27 = 98$$

**Cross-check:** 8 + 36 + 54 = **98** ✓

**Answer: (c) 98**

---

### 🟡 DICE — Solutions 21–35

---

**Q21. Opposite 1? → (d) 6**

**Rule:** opposite faces sum to 7.
$$7 - 1 = 6$$

**Answer: (d) 6**

---

**Q22. Opposite 2? → (c) 5**

$$7 - 2 = 5$$

**Answer: (c) 5**

---

**Q23. Opposite 3? → (b) 4**

$$7 - 3 = 4$$

**Answer: (b) 4**

---

**Q24. Top shows 4. Bottom? → (c) 3**

$$7 - 4 = 3$$

**Answer: (c) 3**

---

**Q25. Sum of two opposite faces? → (c) 7**

The defining property of a standard die: **1↔6, 2↔5, 3↔4**, each pair summing to **7**.

**Answer: (c) 7**

---

**Q26. 1 on top, 2 facing north. Bottom? → (d) 6**

The bottom is determined solely by the top:
$$7 - 1 = 6$$

> The orientation of the die (which number faces north) is **irrelevant** to this question — a deliberate distractor.

**Answer: (d) 6**

---

**Q27. Two views, 1 on top with 2, 3 then 4, 5 visible. Opposite 1? → (d) 6**

**Step 1 — Collect the adjacencies.**
- View 1: faces 2 and 3 appear beside 1 ⇒ both adjacent to 1
- View 2: faces 4 and 5 appear beside 1 ⇒ both adjacent to 1

$$\text{Adjacent to 1} = \{2, 3, 4, 5\}$$

**Step 2 — Eliminate.**
Each face has exactly four adjacent faces and one opposite. All four adjacents are identified, so the remaining number is the opposite:

$$\{1,2,3,4,5,6\} \setminus \{1,2,3,4,5\} = \{\mathbf{6}\}$$

**Cross-check:** 1 + 6 = 7 ✓

**Answer: (d) 6**

---

**Q28. 3 is adjacent to 1, 2, 5, 6. Opposite 3? → (c) 4**

Four adjacents are given; the only number left is **4**.

**Cross-check:** 3 + 4 = 7 ✓

**Answer: (c) 4**

---

**Q29. Faces 1, 2, 3 meet at a corner. What meets at the opposite corner? → (c) 4, 5, 6**

**Rule:** at the diagonally opposite corner, each face is replaced by its **opposite**.

$$1 \to 6, \qquad 2 \to 5, \qquad 3 \to 4$$

$$\implies \{6, 5, 4\}$$

**Answer: (c) 4, 5, 6**

---

**Q30. 5 on top. Sum of the four side faces? → (b) 14**

**Step 1 — Total of all faces.**
$$1+2+3+4+5+6 = 21$$

**Step 2 — Top and bottom.**
$$\text{Bottom} = 7 - 5 = 2 \implies \text{Top} + \text{Bottom} = 7$$

**Step 3 — The four sides.**
$$21 - 7 = 14$$

> **This answer is independent of the top face.** Since top + bottom is always 7, the four sides always total **14**.

**Answer: (b) 14**

---

**Q31. Sum of all six faces? → (c) 21**

$$1+2+3+4+5+6 = 21$$

**Answer: (c) 21**

---

**Q32. 6 on top, 4 at the front. What is at the back? → (c) 3**

Front and back are opposite faces:
$$7 - 4 = 3$$

> The top face (6) is irrelevant here — front and back form their own opposite pair.

**Answer: (c) 3**

---

**Q33. 1 is adjacent to 2, 3, 4 and 5. Opposite 2? → (c) 5**

**Step 1 — Deduce what is opposite 1.**
All four adjacents of 1 are given ⇒ the opposite of 1 is **6**.

**Step 2 — Apply the sum rule to 2.**
$$7 - 2 = 5$$

**Consistency check:** 2 is adjacent to 1, so 2 cannot be opposite 1 ✓ And the pairs 1↔6, 2↔5, 3↔4 are mutually consistent ✓

**Answer: (c) 5**

---

**Q34. 3 on top, 5 at the front; tipped forward 90°. New top? → (d) 5**

**The rotation:** tipping forward through 90° about a horizontal left–right axis moves each face one position:

```
    FRONT  →  TOP
    TOP    →  BACK
    BACK   →  BOTTOM
    BOTTOM →  FRONT
```

The face that was at the front (**5**) is now on top.

**Answer: (d) 5**

> **The left and right faces are unaffected** by a forward tip — only the top, front, bottom and back cycle.

---

**Q35. Two dice show 5 and 3 on top. Sum of the bottoms? → (b) 6**

$$\text{Bottom}_1 = 7 - 5 = 2$$
$$\text{Bottom}_2 = 7 - 3 = 4$$
$$\text{Sum} = 2 + 4 = 6$$

**⚡ Shortcut:** for *k* dice, the tops and bottoms together total 7k. Here 7 × 2 = 14, and the tops total 8, so the bottoms total 14 − 8 = **6** ✓

**Answer: (b) 6**

---

### 🔴 FIGURES, MIRRORS & WATER IMAGES — Solutions 36–50

---

**Q36. Square rotating 90° clockwise; orientation after 4 steps? → (d) The same as the start**

$$4 \times 90° = 360° \equiv 0° \pmod{360°}$$

A full revolution returns the figure to its original orientation.

**Answer: (d) The same as the start**

---

**Q37. Dots: 2, 4, 6, ? → (b) 8**

The count increases by **2** at each step:
$$6 + 2 = 8$$

**Answer: (b) 8**

---

**Q38. Lines: 3, 4, 5, ? → (b) 6**

The count increases by **1** at each step:
$$5 + 1 = 6$$

**Answer: (b) 6**

---

**Q39. Arrow: north, east, south, ? → (d) West**

The arrow rotates **90° clockwise** at each step:
$$\text{N} \to \text{E} \to \text{S} \to \textbf{W}$$

**Answer: (d) West**

---

**Q40. Shading alternates; figure 1 is shaded. Figure 5? → (a) Shaded**

| Figure | 1 | 2 | 3 | 4 | 5 |
|---|---|---|---|---|---|
| State | Shaded | Unshaded | Shaded | Unshaded | **Shaded** |

**Rule:** odd-numbered figures are shaded, even-numbered are unshaded. Figure 5 is odd ⇒ **shaded**.

**Answer: (a) Shaded**

---

**Q41. Triangle rotating 45° clockwise; after 8 steps? → (d) The same as the start**

$$8 \times 45° = 360° \equiv 0° \pmod{360°}$$

**Answer: (d) The same as the start**

---

**Q42. Triangle, square, pentagon, ? → (b) Hexagon**

The number of sides increases by 1 at each step:
$$3 \to 4 \to 5 \to \textbf{6 (hexagon)}$$

**Answer: (b) Hexagon**

---

**Q43. Dot moving one corner clockwise around a square; after 4 steps? → (c) The starting corner**

A square has **4** corners, and the dot advances one corner per step:
$$4 \text{ steps} = 1 \text{ complete circuit}$$

**Answer: (c) The starting corner**

---

**Q44. Lines: 6, 5, 4, ? → (b) 3**

The count decreases by **1** at each step:
$$4 - 1 = 3$$

**Answer: (b) 3**

---

**Q45. Pattern rotating 180° per step; after 3 steps? → (c) Rotated 180°**

$$3 \times 180° = 540°$$
$$540° \bmod 360° = 180°$$

After an odd number of 180° turns, the figure is **inverted** relative to the start.

> **The parity rule:** an even number of 180° rotations returns the figure to its original orientation; an odd number leaves it inverted.

**Answer: (c) Rotated 180°**

---

**Q46. Mirror image of "b"? → (b) d**

A mirror reflects **left ↔ right**. The bowl of the *b* sits to the right of its stem; reflecting moves it to the left, producing **d**.

```
    b  ──vertical mirror──►  d
```

**Answer: (b) d**

---

**Q47. Water image of "b"? → (c) p**

A water image reflects **top ↔ bottom**. The stem of the *b* rises above its bowl; flipping vertically drops the stem below, producing **p**.

```
    b  ──horizontal flip──►  p
```

**Answer: (c) p**

> **The complete family:**
> | Letter | Mirror | Water |
> |---|---|---|
> | b | d | p |
> | d | b | q |
> | p | q | b |
> | q | p | d |

---

**Q48. Mirror image of "MOM"? → (a) MOM**

**Step 1 — Reverse the letter order.**
$$\text{MOM} \to \text{MOM} \quad (\text{it is a palindrome})$$

**Step 2 — Reflect each individual letter.**
Both **M** and **O** have vertical symmetry, so each is unchanged in a mirror.

$$\implies \text{The mirror image is } \textbf{MOM}$$

**Answer: (a) MOM**

> **Two conditions must both hold** for a word to survive a mirror: it must be a palindrome **and** every letter must be vertically symmetric. "HIM" fails the first (it reverses to MIH); "BOB" fails the second (B is not vertically symmetric).

---

**Q49. Which letter is unchanged in a vertical mirror? → (b) H**

**The vertically symmetric letters:**
$$\textbf{A, H, I, M, O, T, U, V, W, X, Y}$$

| Option | Vertically symmetric? |
|---|---|
| F | ✗ |
| **H** | **✓** |
| J | ✗ |
| R | ✗ |

**Answer: (b) H**

---

**Q50. Start with 4 dots, gain 3 per step; after 4 steps? → (c) 16**

**Step 1 — Track the count.**

| Step | Dots |
|---|---|
| Start (0) | 4 |
| 1 | 7 |
| 2 | 10 |
| 3 | 13 |
| 4 | **16** |

**Formula:**
$$4 + (4 \times 3) = 4 + 12 = 16$$

**Answer: (c) 16**

---

## 9. Quick Revision Sheet

> **One page. Read 48 hours after study, and again the night before the test.**

### ⭐ PAINTED CUBES — the four formulas

```
Cube of side n, painted on ALL faces, cut into n³ unit cubes.
Let m = n − 2.

    3 faces (corners)   =  8                ← ALWAYS 8
    2 faces (edges)     =  12m
    1 face  (faces)     =  6m²
    0 faces (interior)  =  m³

    CHECK:  8 + 12m + 6m² + m³ = n³

At least one face painted  =  n³ − m³   (also the SURFACE cubes)
```

**Reference table**

```
  n    Total   3-face   2-face   1-face   0-face
  2      8       8        0        0        0
  3     27       8       12        6        1
  4     64       8       24       24        8
  5    125       8       36       54       27
  6    216       8       48       96       64
```

**Partial painting** — abandon the formulas; count by coordinates.

```
Painted on all faces EXCEPT the bottom, n = 4:
    x ∈ {2,3}     2 choices
    y ∈ {2,3}     2 choices
    z ∈ {1,2,3}   3 choices  (bottom is safe)
                  ──────────
    Unpainted = 2 × 2 × 3 = 12
```

**Multi-colour** (three opposite pairs)

```
3 colours = corners = 8
2 colours = edges   = 12m
1 colour  = faces   = 6m²
```

### DICE

```
⭐ OPPOSITE FACES SUM TO 7      1↔6   2↔5   3↔4

All six faces total            21
Top + Bottom                    7
Four side faces                14   ← always, whatever is on top
For k dice: tops + bottoms  =  7k

ADJACENCY: each face touches 4 others and is opposite exactly 1.
    Any number seen NEXT TO a face is ADJACENT to it.
    Rule out all four adjacents → the fifth is the opposite.

CORNER RULE: if 1, 2, 3 meet at a corner,
             then 6, 5, 4 meet at the opposite corner.

ROTATIONS
    Tip forward 90°:  FRONT→TOP→BACK→BOTTOM→FRONT
                      (left and right unchanged)
    Spin about vertical: top and bottom fixed; the four sides cycle
```

### FIGURES

```
ROTATION ARITHMETIC
    Net after k steps of θ  =  kθ mod 360°
    45° → returns after 8 steps      90° → 4 steps
    120° → 3 steps                   180° → 2 steps

CYCLIC POSITION
    An element on p positions returns to start after p steps

TRANSFORMATION CHECKLIST
    □ rotation?  □ reflection?  □ element movement?
    □ addition / deletion?  □ shading alternation?  □ count progression?
    (most series combine exactly TWO)
```

### MIRRORS AND WATER IMAGES

```
MIRROR  =  reflect LEFT ↔ RIGHT   (vertical axis)
WATER   =  reflect TOP ↔ BOTTOM   (horizontal axis)

           Mirror   Water
    b   →    d        p
    d   →    b        q
    p   →    q        b
    q   →    p        d

UNCHANGED BY A VERTICAL MIRROR:   A H I M O T U V W X Y
UNCHANGED BY A WATER IMAGE:       B C D E H I K O X
UNCHANGED BY EITHER:              H  I  O  X

WORDS: a word survives a mirror only if it is a PALINDROME
       AND every letter is vertically symmetric.
       MOM ✓   TOOT ✓   HIM ✗ (reverses to MIH)
```

### PAPER FOLDING

```
Holes after punching = 2^(number of folds)
Holes appear SYMMETRICALLY about every fold line

2 folds, 1 punch  →  4 holes, one per quadrant
3 folds, 1 punch  →  8 holes
```

---

## 10. Common Mistakes

| # | Mistake | Example | Correction |
|---|---|---|---|
| 1 | **Corner count varied with n** | "n = 5 ⇒ more corners" | Corners are **always 8** |
| 2 | **(n − 1) used instead of (n − 2)** | 12(n − 1) for edges | Both end cubes of an edge are corners ⇒ (n − 2) |
| 3 | **Verification sum skipped** | Accepting an unchecked answer | The four categories must total n³ |
| 4 | **Formulas used with partial painting** | (n − 2)³ when a face is unpainted | Count by coordinates instead |
| 5 | **"At least one face" confused with "exactly one"** | 6(n−2)² for "at least one" | At least one = n³ − (n−2)³ |
| 6 | **Opposite-face rule forgotten** | Guessing what is opposite 3 | Opposite = 7 − face |
| 7 | **Adjacent number taken as opposite** | 2 seen beside 1 ⇒ 2 opposite 1 | Adjacent ⇒ **not** opposite |
| 8 | **Irrelevant orientation used** | Using the north-facing number to find the bottom | Bottom depends only on the top |
| 9 | **Side-face sum recomputed each time** | Adding four numbers | It is **always 14** |
| 10 | **Rotation not reduced mod 360°** | 540° left as-is | 540 mod 360 = 180° |
| 11 | **Mirror and water confused** | b → p called the mirror image | Mirror flips L–R (b → d); water flips T–B (b → p) |
| 12 | **Letter order not reversed in a mirror** | HIM → HIM | The order reverses: HIM → MIH |

---

## Practice Answer Key

| Q | Ans | Q | Ans | Q | Ans | Q | Ans | Q | Ans |
|---|---|---|---|---|---|---|---|---|---|
| 1 | d | 11 | c | 21 | d | 31 | c | 41 | d |
| 2 | c | 12 | b | 22 | c | 32 | c | 42 | b |
| 3 | c | 13 | c | 23 | b | 33 | c | 43 | c |
| 4 | c | 14 | c | 24 | c | 34 | d | 44 | b |
| 5 | c | 15 | c | 25 | c | 35 | b | 45 | c |
| 6 | c | 16 | b | 26 | d | 36 | d | 46 | b |
| 7 | d | 17 | c | 27 | d | 37 | b | 47 | c |
| 8 | b | 18 | c | 28 | c | 38 | b | 48 | a |
| 9 | c | 19 | c | 29 | c | 39 | d | 49 | b |
| 10 | c | 20 | c | 30 | b | 40 | a | 50 | c |

**Scoring guide:** 45+/50 → strong. 35–44 → solid; memorise the four cube formulas and the b/d/p/q table. Below 35 → these are pure-recall sub-topics. Write the cube formulas and the dice rules from memory, then redo the set — near-perfect scores are achievable here.

---

**⬅️ Back:** [Topic 18 — Data Sufficiency & Critical Reasoning](18-data-sufficiency-critical-reasoning.md) · **➡️ Next:** [Topic 20 — Verbal Ability](20-verbal-ability.md)
