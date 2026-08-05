# Topic 11 — Mensuration & Geometry

### EY Placement Aptitude Handbook · Priority Rank #20 · 🟡 Medium

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

**Weightage:** 4–5% of the quantitative section — roughly **0–1 questions**.

**Why it is still worth an evening of your time:** this is the most **purely recall-based** topic in the syllabus. There is no interpretation, no trap-heavy wording, no multi-step reasoning — you either know the formula or you don't. A candidate who memorises the twenty formulas in Section 3 will answer any mensuration question in under 30 seconds. That is the best marks-per-minute-of-study ratio anywhere in the handbook.

**Question styles reported:**

| Style | Typical shape |
|---|---|
| Direct area/perimeter | "Area of a circle with radius 7" |
| Direct volume/surface area | "Volume of a cylinder, r = 7, h = 10" |
| Percentage change in dimensions | "Side increased 20% — change in area?" |
| Reverse (find a dimension from an area) | "Area 240, parallel sides 20 and 28 — find the height" |
| Melting and recasting | "Cone melted into spheres — how many?" |
| Paths and borders | "2 m path around a 40 × 30 field" |
| Ratio of similar solids | "Volumes 8 : 27 — ratio of surface areas?" |
| Heron's formula | "Triangle with sides 13, 14, 15" |
| Pythagorean triples | "Legs 6 and 8 — find the hypotenuse" |

---

## 2. Core Concepts

### 2.1 The value of π

For exam purposes:

$$\pi = \frac{22}{7} \approx 3.14$$

> **Use 22/7 whenever the radius is a multiple of 7** — the 7s cancel and the arithmetic becomes exact. Exam-setters choose radii of 7, 14, 21 and 3.5 precisely for this reason. If you see one of those numbers, 22/7 is intended.

### 2.2 Two-dimensional figures

| Figure | Area | Perimeter |
|---|---|---|
| **Square** (side *a*) | $a^2$ | $4a$ |
| **Rectangle** (l × b) | $lb$ | $2(l+b)$ |
| **Triangle** (base *b*, height *h*) | $\tfrac{1}{2}bh$ | $a+b+c$ |
| **Equilateral triangle** (side *a*) | $\tfrac{\sqrt{3}}{4}a^2$ | $3a$ |
| **Parallelogram** | $b \times h$ | $2(a+b)$ |
| **Rhombus** (diagonals *d₁*, *d₂*) | $\tfrac{1}{2}d_1d_2$ | $4a$ |
| **Trapezium** (parallel sides *a*, *b*) | $\tfrac{1}{2}(a+b)h$ | sum of sides |
| **Circle** (radius *r*) | $\pi r^2$ | $2\pi r$ |
| **Semicircle** | $\tfrac{1}{2}\pi r^2$ | $\pi r + 2r$ |
| **Sector** (angle θ°) | $\tfrac{\theta}{360}\pi r^2$ | $\tfrac{\theta}{360}\cdot 2\pi r + 2r$ |
| **Ring / annulus** | $\pi(R^2 - r^2)$ | — |

**Diagonals:**

$$\text{Square: } d = a\sqrt{2} \quad\text{so}\quad \text{Area} = \frac{d^2}{2}$$
$$\text{Rectangle: } d = \sqrt{l^2 + b^2}$$

### 2.3 Heron's formula (triangle from three sides)

When the height is unknown but all three sides are given:

$$s = \frac{a+b+c}{2} \qquad \text{Area} = \sqrt{s(s-a)(s-b)(s-c)}$$

> Triangle with sides 13, 14, 15:
> s = 21 ⇒ Area = √(21 × 8 × 7 × 6) = √7,056 = **84**

### 2.4 Pythagorean triples (memorise — they save real time)

$$a^2 + b^2 = c^2$$

| Triple | Multiples that appear |
|---|---|
| **3, 4, 5** | 6-8-10 · 9-12-15 · 12-16-20 · 15-20-25 · 30-40-50 |
| **5, 12, 13** | 10-24-26 · 15-36-39 |
| **8, 15, 17** | 16-30-34 |
| **7, 24, 25** | — |
| **9, 40, 41** | — |
| **20, 21, 29** | — |

> Legs 6 and 8 ⇒ hypotenuse **10** (the 3-4-5 triple doubled) — no square roots required.

### 2.5 Three-dimensional solids

| Solid | Volume | Curved / Lateral SA | Total SA |
|---|---|---|---|
| **Cube** (edge *a*) | $a^3$ | $4a^2$ | $6a^2$ |
| **Cuboid** (l, b, h) | $lbh$ | $2h(l+b)$ | $2(lb+bh+hl)$ |
| **Cylinder** (r, h) | $\pi r^2 h$ | $2\pi rh$ | $2\pi r(r+h)$ |
| **Cone** (r, h, slant *l*) | $\tfrac{1}{3}\pi r^2 h$ | $\pi r l$ | $\pi r(r+l)$ |
| **Sphere** (r) | $\tfrac{4}{3}\pi r^3$ | — | $4\pi r^2$ |
| **Hemisphere** (r) | $\tfrac{2}{3}\pi r^3$ | $2\pi r^2$ | $3\pi r^2$ |

**Diagonals:**
$$\text{Cube: } d = a\sqrt{3} \qquad \text{Cuboid: } d = \sqrt{l^2+b^2+h^2}$$

**Cone slant height:**
$$l = \sqrt{r^2 + h^2}$$

> **The cone–cylinder relationship worth memorising:** a cone is exactly **one-third** of the cylinder with the same base and height.
> $$V_{\text{cone}} : V_{\text{sphere}} : V_{\text{cylinder}} = 1 : 2 : 3 \quad \text{(same } r, \text{ and } h = 2r)$$

### 2.6 ⭐ Scaling laws (the highest-yield concept here)

If every linear dimension of a figure is multiplied by *k*:

$$\boxed{\text{Length} \times k \qquad \text{Area} \times k^2 \qquad \text{Volume} \times k^3}$$

**Run backwards, this is even more useful:**

| Given ratio | Linear ratio | Area ratio | Volume ratio |
|---|---|---|---|
| Sides 2 : 3 | 2 : 3 | 4 : 9 | 8 : 27 |
| Areas 4 : 9 | **2 : 3** | 4 : 9 | 8 : 27 |
| Volumes 8 : 27 | **2 : 3** | **4 : 9** | 8 : 27 |

> "The ratio of the volumes of two cubes is 8 : 27. Find the ratio of their surface areas."
> Take cube roots for the sides: 2 : 3. Square for areas: **4 : 9**.

### 2.7 Percentage change in dimensions

Apply the multiplier method from [Topic 1](01-percentages.md).

> **Side of a square increased by 20% — change in area?**
> Area multiplier = 1.20² = **1.44** ⇒ area rises **44%**

> **Length +25%, breadth −20% — change in a rectangle's area?**
> 1.25 × 0.80 = **1.00** ⇒ **no change**

**For a rectangle with length +a% and breadth +b%:**
$$\text{Net area change} = a + b + \frac{ab}{100}\%$$

### 2.8 Angles and polygons

| Property | Formula |
|---|---|
| Sum of interior angles of an *n*-gon | $(n-2) \times 180°$ |
| Each interior angle (regular) | $\dfrac{(n-2)\times 180°}{n}$ |
| Sum of exterior angles | **360°** (always, any polygon) |
| Each exterior angle (regular) | $\dfrac{360°}{n}$ |
| Number of diagonals | $\dfrac{n(n-3)}{2}$ |

**Regular polygons worth knowing:**

| Polygon | Sides | Interior angle | Exterior angle |
|---|---|---|---|
| Triangle | 3 | 60° | 120° |
| Square | 4 | 90° | 90° |
| Pentagon | 5 | 108° | 72° |
| Hexagon | 6 | 120° | 60° |
| Octagon | 8 | 135° | 45° |
| Decagon | 10 | 144° | 36° |

**Triangle facts:**
- Angles sum to 180°
- Exterior angle = sum of the two opposite interior angles
- The longest side lies opposite the largest angle

**Circle facts:**
- Angle in a semicircle = 90°
- Angle at the centre = twice the angle at the circumference (same arc)
- The radius drawn to a point of tangency is perpendicular to the tangent

### 2.9 Paths and borders

**Path OUTSIDE a rectangle**, width *w*:
$$\text{Outer dimensions} = (l + 2w) \times (b + 2w)$$
$$\text{Path area} = (l+2w)(b+2w) - lb$$

**Path INSIDE a rectangle**, width *w*:
$$\text{Inner dimensions} = (l - 2w) \times (b - 2w)$$
$$\text{Path area} = lb - (l-2w)(b-2w)$$

**Circular path (annulus)**, outer radius *R*, inner *r*:
$$\text{Area} = \pi(R^2 - r^2) = \pi(R+r)(R-r)$$

> **The factor of 2 in "2w":** the path runs along *both* sides of each dimension. Forgetting it is the standard error in this question type.

### 2.10 Melting and recasting

The **volume is conserved**. Nothing else is.

$$\text{Volume of the original solid} = \text{Total volume of the new solids}$$

$$\text{Number of new pieces} = \frac{V_{\text{original}}}{V_{\text{one piece}}}$$

> A cone (r = 6, h = 24) melted into spheres of radius 3:
> $$V_{\text{cone}} = \tfrac{1}{3}\pi(36)(24) = 288\pi \qquad V_{\text{sphere}} = \tfrac{4}{3}\pi(27) = 36\pi$$
> $$\text{Number} = \frac{288\pi}{36\pi} = \mathbf{8}$$

> **Surface area is NOT conserved.** Melting a solid and reshaping it changes the surface area completely — only volume carries across.

---

## 3. Formula Bank

| # | Figure/Solid | Formula |
|---|---|---|
| 1 | Square | Area $a^2$; Perimeter $4a$; Diagonal $a\sqrt2$; Area from diagonal $\tfrac{d^2}{2}$ |
| 2 | Rectangle | Area $lb$; Perimeter $2(l+b)$; Diagonal $\sqrt{l^2+b^2}$ |
| 3 | Triangle | Area $\tfrac12 bh$ |
| 4 | Heron's formula | $\sqrt{s(s-a)(s-b)(s-c)}$, $s = \tfrac{a+b+c}{2}$ |
| 5 | Equilateral triangle | Area $\tfrac{\sqrt3}{4}a^2$; Height $\tfrac{\sqrt3}{2}a$ |
| 6 | Parallelogram | Area $bh$ |
| 7 | Rhombus | Area $\tfrac12 d_1 d_2$ |
| 8 | Trapezium | Area $\tfrac12(a+b)h$ |
| 9 | Circle | Area $\pi r^2$; Circumference $2\pi r$ |
| 10 | Sector | Area $\tfrac{\theta}{360}\pi r^2$; Arc $\tfrac{\theta}{360}2\pi r$ |
| 11 | Ring | $\pi(R^2-r^2)$ |
| 12 | Cube | $V = a^3$; TSA $6a^2$; LSA $4a^2$; Diagonal $a\sqrt3$ |
| 13 | Cuboid | $V = lbh$; TSA $2(lb+bh+hl)$; Diagonal $\sqrt{l^2+b^2+h^2}$ |
| 14 | Cylinder | $V = \pi r^2h$; CSA $2\pi rh$; TSA $2\pi r(r+h)$ |
| 15 | Cone | $V = \tfrac13\pi r^2h$; CSA $\pi rl$; TSA $\pi r(r+l)$; $l=\sqrt{r^2+h^2}$ |
| 16 | Sphere | $V = \tfrac43\pi r^3$; SA $4\pi r^2$ |
| 17 | Hemisphere | $V = \tfrac23\pi r^3$; CSA $2\pi r^2$; TSA $3\pi r^2$ |
| 18 | Scaling | Length ×k, Area ×k², Volume ×k³ |
| 19 | Polygon interior sum | $(n-2)180°$ |
| 20 | Regular polygon exterior angle | $\tfrac{360°}{n}$ |
| 21 | Diagonals of an *n*-gon | $\tfrac{n(n-3)}{2}$ |
| 22 | Path outside a rectangle | $(l+2w)(b+2w) - lb$ |

---

## 4. Shortcuts & Tricks

### 4.1 Use π = 22/7 when the radius is a multiple of 7

| r | πr² (using 22/7) | 2πr |
|---|---|---|
| 7 | 154 | 44 |
| 14 | 616 | 88 |
| 21 | 1,386 | 132 |
| 3.5 | 38.5 | 22 |

These four rows cover the large majority of circle questions in placement tests.

### 4.2 The scaling shortcut

```
Linear ratio a : b
    →  Area ratio    a² : b²
    →  Volume ratio  a³ : b³

Given AREAS a:b     →  take √ for linear
Given VOLUMES a:b   →  take ∛ for linear
```

| Change | Area becomes | Volume becomes |
|---|---|---|
| +10% | +21% | +33.1% |
| +20% | +44% | +72.8% |
| +50% | +125% | +237.5% |
| ×2 | ×4 | ×8 |
| ×3 | ×9 | ×27 |
| −10% | −19% | −27.1% |

### 4.3 Pythagorean triples on sight

```
3-4-5     6-8-10    9-12-15   12-16-20   15-20-25   30-40-50
5-12-13   10-24-26  15-36-39
8-15-17   16-30-34
7-24-25   9-40-41   20-21-29
```

Recognising 6-8-10 instantly beats computing √(36 + 64).

### 4.4 The volume-conservation template

```
MELTING / RECASTING  →  Volume is conserved

Number of pieces = V_original / V_one_piece

Cancel π and any common factors BEFORE dividing.
```

> Cone 288π into spheres of 36π ⇒ 288/36 = **8** (the π cancels immediately)

### 4.5 The 1 : 2 : 3 solid relationship

For a cone, a sphere and a cylinder all with radius *r*, where the cone and cylinder have height 2*r*:

$$V_{\text{cone}} : V_{\text{sphere}} : V_{\text{cylinder}} = 1 : 2 : 3$$

And more generally, for the **same base and height**:
$$V_{\text{cone}} = \frac{1}{3} V_{\text{cylinder}}$$

### 4.6 Reverse questions — rearrange, don't re-derive

| Given | Find | Rearrangement |
|---|---|---|
| Area of a square | Side | $a = \sqrt{A}$ |
| Circumference | Radius | $r = \dfrac{C}{2\pi}$ |
| Area of a circle | Radius | $r = \sqrt{A/\pi}$ |
| Diagonal of a square | Area | $A = \dfrac{d^2}{2}$ |
| Trapezium area + parallel sides | Height | $h = \dfrac{2A}{a+b}$ |
| Volume of a cube | Edge | $a = \sqrt[3]{V}$ |
| Cube diagonal | Edge | $a = \dfrac{d}{\sqrt3}$ |

### 4.7 Squares and cubes to know

| n | n² | n³ | | n | n² | n³ |
|---|---|---|---|---|---|---|
| 11 | 121 | 1,331 | | 16 | 256 | 4,096 |
| 12 | 144 | 1,728 | | 17 | 289 | — |
| 13 | 169 | 2,197 | | 18 | 324 | — |
| 14 | 196 | 2,744 | | 20 | 400 | 8,000 |
| 15 | 225 | 3,375 | | 25 | 625 | 15,625 |

$$\sqrt2 \approx 1.414 \qquad \sqrt3 \approx 1.732 \qquad \sqrt5 \approx 2.236$$

### 4.8 Sanity checks

```
✓ A cone's volume is ALWAYS one-third of the cylinder with the same r and h
✓ Slant height > vertical height (l = √(r²+h²) > h)
✓ Diagonal > any side
✓ TSA > CSA for every closed solid
✓ Scaling: area grows as the SQUARE, volume as the CUBE
✓ Melting conserves VOLUME, never surface area
✓ Path questions: always 2w, never w
```

---

## 5. Solved Examples

### Example 1 — Circle with a clean radius

**Q.** Find the area and circumference of a circle of radius 21 cm. (Take π = 22/7.)

**Step 1 — Area.**
$$A = \pi r^2 = \frac{22}{7} \times 21 \times 21$$

Cancel the 7 into one of the 21s:
$$= 22 \times 3 \times 21 = 1{,}386 \text{ cm}^2$$

**Step 2 — Circumference.**
$$C = 2\pi r = 2 \times \frac{22}{7} \times 21 = 2 \times 22 \times 3 = 132 \text{ cm}$$

**Answer: Area = 1,386 cm²; Circumference = 132 cm**

> **Always cancel before multiplying.** Writing 22/7 × 441 forces you into an awkward division; cancelling the 7 first keeps everything in single-digit multiplication.

---

### Example 2 — Percentage change in dimensions

**Q.** The length of a rectangle is increased by 30% and its breadth is decreased by 10%. Find the percentage change in its area.

**Step 1 — Convert to multipliers.**
$$\text{Length} \times 1.30 \qquad \text{Breadth} \times 0.90$$

**Step 2 — Area is length × breadth, so multiply the factors.**
$$1.30 \times 0.90 = 1.17$$

**Step 3 — Read off the change.**
$$1.17 \implies \text{a 17\% increase}$$

**Verification with numbers.** Take l = 100, b = 100 ⇒ area = 10,000.
New: l = 130, b = 90 ⇒ area = 11,700.
$$\frac{11{,}700 - 10{,}000}{10{,}000} \times 100 = 17\% \checkmark$$

**Answer: 17% increase**

> **Formula alternative:** a + b + ab/100 = 30 − 10 + (30 × −10)/100 = 20 − 3 = 17% ✓

---

### Example 3 — Heron's formula

**Q.** Find the area of a triangle whose sides measure 9 cm, 12 cm and 15 cm.

**Step 1 — Check for a Pythagorean triple first.**
$$9^2 + 12^2 = 81 + 144 = 225 = 15^2 \checkmark$$

This is a **right-angled triangle** (the 3-4-5 triple × 3), so the simple formula applies with the two legs as base and height:
$$\text{Area} = \frac{1}{2} \times 9 \times 12 = 54 \text{ cm}^2$$

**Step 2 — Confirm with Heron's formula.**
$$s = \frac{9 + 12 + 15}{2} = 18$$
$$\text{Area} = \sqrt{18(18-9)(18-12)(18-15)} = \sqrt{18 \times 9 \times 6 \times 3}$$
$$= \sqrt{2{,}916} = 54 \checkmark$$

**Answer: 54 cm²**

> **Always test for a triple before reaching for Heron.** The check takes five seconds and, when it succeeds, saves you a four-factor square root.

---

### Example 4 — Cylinder, full surface area

**Q.** A closed cylindrical tank has radius 7 m and height 10 m. Find its volume, curved surface area and total surface area. (π = 22/7)

**Step 1 — Volume.**
$$V = \pi r^2 h = \frac{22}{7} \times 49 \times 10 = 22 \times 7 \times 10 = 1{,}540 \text{ m}^3$$

**Step 2 — Curved surface area.**
$$\text{CSA} = 2\pi r h = 2 \times \frac{22}{7} \times 7 \times 10 = 440 \text{ m}^2$$

**Step 3 — Total surface area (add the two circular ends).**
$$\text{TSA} = 2\pi r(r + h) = 2 \times \frac{22}{7} \times 7 \times (7 + 10) = 44 \times 17 = 748 \text{ m}^2$$

**Cross-check:** TSA = CSA + 2 × (area of a circular end) = 440 + 2 × 154 = 748 ✓

**Answer: V = 1,540 m³; CSA = 440 m²; TSA = 748 m²**

> **Read whether the solid is open or closed.** An open tank (no lid) has TSA = CSA + one circle = 440 + 154 = 594 m². Questions specify this deliberately.

---

### Example 5 — Melting and recasting

**Q.** A solid metallic sphere of radius 9 cm is melted and recast into small spheres of radius 3 cm each. How many small spheres are formed?

**Step 1 — Recognise the governing principle.**
Melting conserves **volume**.

**Step 2 — Volume of the large sphere.**
$$V = \frac{4}{3}\pi (9)^3 = \frac{4}{3}\pi \times 729 = 972\pi$$

**Step 3 — Volume of one small sphere.**
$$v = \frac{4}{3}\pi (3)^3 = \frac{4}{3}\pi \times 27 = 36\pi$$

**Step 4 — Divide.**
$$\frac{972\pi}{36\pi} = 27$$

**Answer: 27 spheres**

**⚡ Scaling shortcut:** the radius ratio is 9 : 3 = 3 : 1, so the volume ratio is 3³ : 1 = **27 : 1**. The answer follows without computing either volume.

---

### Example 6 — Path around a rectangular field

**Q.** A rectangular garden measures 50 m by 30 m. A path 2.5 m wide is laid all around it on the outside. Find the area of the path.

**Step 1 — Compute the outer dimensions.**
The path adds its width on **both** sides of each dimension:
$$\text{Length} = 50 + 2(2.5) = 55 \text{ m}$$
$$\text{Breadth} = 30 + 2(2.5) = 35 \text{ m}$$

**Step 2 — Outer area.**
$$55 \times 35 = 1{,}925 \text{ m}^2$$

**Step 3 — Inner (garden) area.**
$$50 \times 30 = 1{,}500 \text{ m}^2$$

**Step 4 — Path area = outer − inner.**
$$1{,}925 - 1{,}500 = 425 \text{ m}^2$$

**Answer: 425 m²**

> **The classic error** is adding 2.5 instead of 5 to each dimension, giving 52.5 × 32.5 = 1,706.25 and a path area of 206.25 m². The path exists on *both* sides — always **2w**.

---

### Example 7 — Scaling ratios

**Q.** The ratio of the surface areas of two spheres is 16 : 25. Find the ratio of their volumes.

**Step 1 — Move from areas to linear dimensions (take square roots).**
$$\text{Area ratio } 16 : 25 \implies \text{radius ratio } \sqrt{16} : \sqrt{25} = 4 : 5$$

**Step 2 — Move from linear to volumes (cube).**
$$\text{Volume ratio} = 4^3 : 5^3 = 64 : 125$$

**Answer: 64 : 125**

**Verification.** Let the radii be 4 and 5.
- Surface areas: 4π(16) = 64π and 4π(25) = 100π ⇒ 64 : 100 = **16 : 25** ✓
- Volumes: (4/3)π(64) and (4/3)π(125) ⇒ **64 : 125** ✓

> **The universal chain:** Area → (√) → Linear → (cube) → Volume. Any two of the three can be converted through the linear ratio.

---

### Example 8 — Reverse problem with a trapezium

**Q.** The area of a trapezium is 336 cm². Its parallel sides measure 20 cm and 36 cm. Find its height.

**Step 1 — Write the formula.**
$$A = \frac{1}{2}(a + b)h$$

**Step 2 — Substitute.**
$$336 = \frac{1}{2}(20 + 36)h = \frac{1}{2}(56)h = 28h$$

**Step 3 — Solve.**
$$h = \frac{336}{28} = 12 \text{ cm}$$

**Verification:** ½(20 + 36)(12) = ½(56)(12) = 336 ✓

**Answer: 12 cm**

---

## 6. Practice Questions

**Instructions:** 50 questions. Easy (1–20), Medium (21–40), Hard (41–50).
Take π = 22/7 unless stated otherwise.
Full solutions in [Section 7](#7-detailed-solutions).

### 🟢 EASY (Questions 1–20)

**Q1.** Find the area of a rectangle of length 12 cm and breadth 8 cm.
(a) 40 cm²  (b) 80 cm²  (c) 96 cm²  (d) 108 cm²

**Q2.** Find the perimeter of a square of side 15 cm.
(a) 45 cm  (b) 60 cm  (c) 75 cm  (d) 225 cm

**Q3.** Find the area of a circle of radius 7 cm.
(a) 132 cm²  (b) 144 cm²  (c) 154 cm²  (d) 176 cm²

**Q4.** Find the circumference of a circle of radius 14 cm.
(a) 44 cm  (b) 66 cm  (c) 88 cm  (d) 176 cm

**Q5.** Find the area of a triangle with base 10 cm and height 6 cm.
(a) 24 cm²  (b) 30 cm²  (c) 48 cm²  (d) 60 cm²

**Q6.** Find the volume of a cube of edge 5 cm.
(a) 25 cm³  (b) 75 cm³  (c) 100 cm³  (d) 125 cm³

**Q7.** Find the area of a square whose diagonal is 8 cm.
(a) 16 cm²  (b) 32 cm²  (c) 48 cm²  (d) 64 cm²

**Q8.** Find the perimeter of a rectangle 20 cm long and 15 cm wide.
(a) 35 cm  (b) 50 cm  (c) 70 cm  (d) 300 cm

**Q9.** Find the volume of a cuboid measuring 6 cm × 4 cm × 5 cm.
(a) 60 cm³  (b) 100 cm³  (c) 120 cm³  (d) 150 cm³

**Q10.** Find the total surface area of a cube of edge 4 cm.
(a) 64 cm²  (b) 80 cm²  (c) 96 cm²  (d) 128 cm²

**Q11.** Find the area of a parallelogram with base 12 cm and height 7 cm.
(a) 42 cm²  (b) 76 cm²  (c) 84 cm²  (d) 96 cm²

**Q12.** Find the area of a trapezium whose parallel sides are 8 cm and 12 cm and whose height is 5 cm.
(a) 40 cm²  (b) 50 cm²  (c) 60 cm²  (d) 100 cm²

**Q13.** Find the curved surface area of a cylinder of radius 7 cm and height 10 cm.
(a) 220 cm²  (b) 440 cm²  (c) 660 cm²  (d) 748 cm²

**Q14.** Find the volume of a cylinder of radius 7 cm and height 10 cm.
(a) 1,232 cm³  (b) 1,386 cm³  (c) 1,540 cm³  (d) 1,760 cm³

**Q15.** Find the volume of a sphere of radius 3 cm (leave the answer in terms of π).
(a) 12π cm³  (b) 27π cm³  (c) 36π cm³  (d) 108π cm³

**Q16.** Find the sum of the interior angles of a pentagon.
(a) 360°  (b) 450°  (c) 540°  (d) 720°

**Q17.** Find each interior angle of a regular hexagon.
(a) 60°  (b) 108°  (c) 120°  (d) 135°

**Q18.** Find the hypotenuse of a right-angled triangle whose legs are 6 cm and 8 cm.
(a) 9 cm  (b) 10 cm  (c) 12 cm  (d) 14 cm

**Q19.** Find the area of an equilateral triangle of side 4 cm.
(a) 2√3 cm²  (b) 4√3 cm²  (c) 8√3 cm²  (d) 16√3 cm²

**Q20.** Find the diagonal of a rectangle measuring 12 cm by 5 cm.
(a) 12 cm  (b) 13 cm  (c) 15 cm  (d) 17 cm

---

### 🟡 MEDIUM (Questions 21–40)

**Q21.** If the side of a square is increased by 20%, by what percentage does its area increase?
(a) 20%  (b) 40%  (c) 44%  (d) 48%

**Q22.** Find the area of a rhombus whose diagonals measure 16 cm and 12 cm.
(a) 48 cm²  (b) 96 cm²  (c) 144 cm²  (d) 192 cm²

**Q23.** The perimeter of a rectangle is 60 cm and its length is twice its breadth. Find its area.
(a) 150 cm²  (b) 180 cm²  (c) 200 cm²  (d) 240 cm²

**Q24.** Find the volume of a cone of radius 6 cm and height 8 cm (in terms of π).
(a) 48π cm³  (b) 96π cm³  (c) 144π cm³  (d) 288π cm³

**Q25.** Find the total surface area of a closed cylinder of radius 7 cm and height 10 cm.
(a) 440 cm²  (b) 594 cm²  (c) 748 cm²  (d) 880 cm²

**Q26.** A wire bent in the form of a circle of radius 14 cm is re-bent into a square. Find the side of the square.
(a) 20 cm  (b) 22 cm  (c) 24 cm  (d) 28 cm

**Q27.** The ratio of the areas of two circles is 4 : 9. Find the ratio of their radii.
(a) 2 : 3  (b) 4 : 9  (c) 8 : 27  (d) 16 : 81

**Q28.** Find the area of a triangle whose sides measure 13 cm, 14 cm and 15 cm.
(a) 78 cm²  (b) 84 cm²  (c) 90 cm²  (d) 96 cm²

**Q29.** A cube of edge 6 cm is cut into smaller cubes of edge 2 cm. How many small cubes are obtained?
(a) 9  (b) 18  (c) 27  (d) 36

**Q30.** The diagonal of a cube is 6√3 cm. Find its volume.
(a) 108 cm³  (b) 144 cm³  (c) 216 cm³  (d) 288 cm³

**Q31.** A rectangular field measures 40 m by 30 m. A path 2 m wide is laid all around it on the outside. Find the area of the path.
(a) 276 m²  (b) 288 m²  (c) 296 m²  (d) 304 m²

**Q32.** Find the curved surface area of a cone whose radius is 7 cm and slant height is 25 cm.
(a) 440 cm²  (b) 495 cm²  (c) 550 cm²  (d) 704 cm²

**Q33.** If the radius of a sphere is doubled, by what factor does its volume increase?
(a) 2  (b) 4  (c) 6  (d) 8

**Q34.** Find the slant height of a cone whose radius is 5 cm and vertical height is 12 cm.
(a) 11 cm  (b) 13 cm  (c) 15 cm  (d) 17 cm

**Q35.** Find the area of a sector of a circle of radius 14 cm subtending an angle of 90° at the centre.
(a) 132 cm²  (b) 144 cm²  (c) 154 cm²  (d) 176 cm²

**Q36.** The circumference of a circle is 44 cm. Find its area.
(a) 132 cm²  (b) 144 cm²  (c) 154 cm²  (d) 176 cm²

**Q37.** A cylinder and a cone have the same radius and the same height. Find the ratio of their volumes.
(a) 1 : 3  (b) 2 : 1  (c) 3 : 1  (d) 3 : 2

**Q38.** The area of a square is 144 cm². Find the length of its diagonal.
(a) 12 cm  (b) 12√2 cm  (c) 24 cm  (d) 144√2 cm

**Q39.** Find the volume of a hemisphere of radius 3 cm (in terms of π).
(a) 9π cm³  (b) 18π cm³  (c) 27π cm³  (d) 36π cm³

**Q40.** The sum of the interior angles of a polygon is 1,440°. How many sides does it have?
(a) 8  (b) 9  (c) 10  (d) 12

---

### 🔴 HARD (Questions 41–50)

**Q41.** A solid cone of radius 6 cm and height 24 cm is melted and recast into spheres of radius 3 cm each. How many spheres are formed?
(a) 6  (b) 8  (c) 10  (d) 12

**Q42.** The length of a rectangle is increased by 25% and its breadth is decreased by 20%. Find the percentage change in its area.
(a) 5% increase  (b) 5% decrease  (c) No change  (d) 10% increase

**Q43.** A hollow cylindrical pipe has an outer radius of 8 cm, an inner radius of 6 cm and a length of 21 cm. Find the volume of the material used.
(a) 1,584 cm³  (b) 1,760 cm³  (c) 1,848 cm³  (d) 2,112 cm³

**Q44.** The area of a trapezium is 240 cm² and its parallel sides measure 20 cm and 28 cm. Find its height.
(a) 8 cm  (b) 10 cm  (c) 12 cm  (d) 15 cm

**Q45.** A rectangular tank 11 m × 8 m × 7 m is full of water. The water is transferred to a cylindrical tank of radius 7 m. Find the depth of water in the cylindrical tank.
(a) 3 m  (b) 4 m  (c) 5 m  (d) 6 m

**Q46.** Two cubes, each of volume 64 cm³, are joined end to end. Find the surface area of the resulting cuboid.
(a) 128 cm²  (b) 144 cm²  (c) 160 cm²  (d) 192 cm²

**Q47.** A circular park of radius 21 m is surrounded by a path 3.5 m wide. Find the area of the path.
(a) 462.0 m²  (b) 500.5 m²  (c) 539.0 m²  (d) 577.5 m²

**Q48.** The sides of a triangle are in the ratio 3 : 4 : 5 and its perimeter is 144 cm. Find its area.
(a) 720 cm²  (b) 810 cm²  (c) 864 cm²  (d) 960 cm²

**Q49.** A sphere of radius 6 cm is melted and recast into a cylinder of radius 4 cm. Find the height of the cylinder.
(a) 12 cm  (b) 15 cm  (c) 18 cm  (d) 24 cm

**Q50.** The ratio of the volumes of two cubes is 8 : 27. Find the ratio of their surface areas.
(a) 2 : 3  (b) 4 : 9  (c) 8 : 27  (d) 16 : 81

---

## 7. Detailed Solutions

### 🟢 EASY — Solutions 1–20

---

**Q1. Area of a 12 × 8 rectangle. → (c) 96 cm²**

$$A = l \times b = 12 \times 8 = 96$$

**Answer: (c) 96 cm²**

---

**Q2. Perimeter of a square of side 15. → (b) 60 cm**

$$P = 4a = 4 \times 15 = 60$$

> Option (d) 225 is the *area*, not the perimeter — read which is asked.

**Answer: (b) 60 cm**

---

**Q3. Area of a circle, r = 7. → (c) 154 cm²**

$$A = \pi r^2 = \frac{22}{7} \times 49 = 22 \times 7 = 154$$

**Answer: (c) 154 cm²**

---

**Q4. Circumference, r = 14. → (c) 88 cm**

$$C = 2\pi r = 2 \times \frac{22}{7} \times 14 = 2 \times 22 \times 2 = 88$$

**Answer: (c) 88 cm**

---

**Q5. Area of a triangle, base 10, height 6. → (b) 30 cm²**

$$A = \frac{1}{2}bh = \frac{1}{2} \times 10 \times 6 = 30$$

**Answer: (b) 30 cm²**

---

**Q6. Volume of a cube, edge 5. → (d) 125 cm³**

$$V = a^3 = 125$$

**Answer: (d) 125 cm³**

---

**Q7. Area of a square with diagonal 8. → (b) 32 cm²**

**Formula used:** A = d²/2

$$A = \frac{8^2}{2} = \frac{64}{2} = 32$$

**Derivation check:** d = a√2 ⇒ a = 8/√2 = 4√2 ⇒ A = (4√2)² = 32 ✓

**Answer: (b) 32 cm²**

---

**Q8. Perimeter of a 20 × 15 rectangle. → (c) 70 cm**

$$P = 2(l+b) = 2(35) = 70$$

**Answer: (c) 70 cm**

---

**Q9. Volume of a 6 × 4 × 5 cuboid. → (c) 120 cm³**

$$V = lbh = 6 \times 4 \times 5 = 120$$

**Answer: (c) 120 cm³**

---

**Q10. TSA of a cube, edge 4. → (c) 96 cm²**

$$\text{TSA} = 6a^2 = 6 \times 16 = 96$$

**Answer: (c) 96 cm²**

---

**Q11. Area of a parallelogram, base 12, height 7. → (c) 84 cm²**

$$A = bh = 12 \times 7 = 84$$

**Answer: (c) 84 cm²**

---

**Q12. Area of a trapezium, sides 8 and 12, height 5. → (b) 50 cm²**

$$A = \frac{1}{2}(a+b)h = \frac{1}{2}(20)(5) = 50$$

**Answer: (b) 50 cm²**

---

**Q13. CSA of a cylinder, r = 7, h = 10. → (b) 440 cm²**

$$\text{CSA} = 2\pi rh = 2 \times \frac{22}{7} \times 7 \times 10 = 44 \times 10 = 440$$

**Answer: (b) 440 cm²**

---

**Q14. Volume of a cylinder, r = 7, h = 10. → (c) 1,540 cm³**

$$V = \pi r^2 h = \frac{22}{7} \times 49 \times 10 = 154 \times 10 = 1{,}540$$

**Answer: (c) 1,540 cm³**

---

**Q15. Volume of a sphere, r = 3. → (c) 36π cm³**

$$V = \frac{4}{3}\pi r^3 = \frac{4}{3}\pi \times 27 = 36\pi$$

**Answer: (c) 36π cm³**

---

**Q16. Sum of interior angles of a pentagon. → (c) 540°**

**Formula used:** (n − 2) × 180°

$$(5-2) \times 180° = 540°$$

**Answer: (c) 540°**

---

**Q17. Interior angle of a regular hexagon. → (c) 120°**

**Method 1 — via the interior sum.**
$$\frac{(6-2) \times 180°}{6} = \frac{720°}{6} = 120°$$

**Method 2 — via the exterior angle (faster).**
Exterior angle = 360°/6 = 60°, so the interior angle = 180° − 60° = **120°**

**Answer: (c) 120°**

---

**Q18. Hypotenuse with legs 6 and 8. → (b) 10 cm**

**Recognise the triple:** 6-8-10 is the 3-4-5 triple doubled.

$$c = \sqrt{36 + 64} = \sqrt{100} = 10$$

**Answer: (b) 10 cm**

---

**Q19. Area of an equilateral triangle of side 4. → (b) 4√3 cm²**

**Formula used:** (√3/4)a²

$$\frac{\sqrt3}{4} \times 16 = 4\sqrt3$$

**Answer: (b) 4√3 cm²**

---

**Q20. Diagonal of a 12 × 5 rectangle. → (b) 13 cm**

**Recognise the triple:** 5-12-13.

$$d = \sqrt{144 + 25} = \sqrt{169} = 13$$

**Answer: (b) 13 cm**

---

### 🟡 MEDIUM — Solutions 21–40

---

**Q21. Side of a square +20% — change in area? → (c) 44%**

**Step 1 — Area scales as the square of the linear factor.**
$$(1.20)^2 = 1.44$$

**Step 2 — Read off the change.**
$$1.44 \implies 44\% \text{ increase}$$

**Verification:** side 10 ⇒ area 100. Side 12 ⇒ area 144. Increase = 44/100 = 44% ✓

> **Trap:** answering 20%. Area is two-dimensional — the increase applies to both length and width.

**Answer: (c) 44%**

---

**Q22. Area of a rhombus, diagonals 16 and 12. → (b) 96 cm²**

**Formula used:** ½ d₁d₂

$$\frac{1}{2} \times 16 \times 12 = 96$$

> **Trap:** answering 192 by forgetting the ½.

**Answer: (b) 96 cm²**

---

**Q23. Rectangle: perimeter 60, length = 2 × breadth. Area? → (c) 200 cm²**

**Step 1 — Set up.** Let breadth = *b*, so length = 2*b*.

**Step 2 — Use the perimeter.**
$$2(2b + b) = 60$$
$$6b = 60 \implies b = 10$$

**Step 3 — Find the length and the area.**
$$l = 20 \implies A = 20 \times 10 = 200$$

**Check:** perimeter = 2(20 + 10) = 60 ✓

**Answer: (c) 200 cm²**

---

**Q24. Volume of a cone, r = 6, h = 8. → (b) 96π cm³**

$$V = \frac{1}{3}\pi r^2 h = \frac{1}{3}\pi \times 36 \times 8 = 12\pi \times 8 = 96\pi$$

> **Trap:** answering 288π by forgetting the ⅓ — that is the *cylinder's* volume with the same base and height.

**Answer: (b) 96π cm³**

---

**Q25. TSA of a closed cylinder, r = 7, h = 10. → (c) 748 cm²**

**Formula used:** TSA = 2πr(r + h)

$$= 2 \times \frac{22}{7} \times 7 \times 17 = 44 \times 17 = 748$$

**Breakdown:** CSA (440) + two circular ends (2 × 154 = 308) = **748** ✓

**Answer: (c) 748 cm²**

---

**Q26. Circle of radius 14 re-bent into a square. Side? → (b) 22 cm**

**Step 1 — The wire's length is conserved.**
$$\text{Circumference} = 2\pi r = 2 \times \frac{22}{7} \times 14 = 88 \text{ cm}$$

**Step 2 — That becomes the square's perimeter.**
$$4a = 88 \implies a = 22 \text{ cm}$$

**Answer: (b) 22 cm**

> **The governing principle:** re-bending a wire conserves **length**, not area. (The circle's area was 616 cm²; the square's is only 484 cm².)

---

**Q27. Areas of two circles in 4 : 9. Ratio of radii? → (a) 2 : 3**

**Concept:** area scales as the square of the linear dimension, so take square roots.

$$\sqrt{4} : \sqrt{9} = 2 : 3$$

**Answer: (a) 2 : 3**

---

**Q28. Area of a triangle with sides 13, 14, 15. → (b) 84 cm²**

**Formula used:** Heron's formula.

**Step 1 — Semi-perimeter.**
$$s = \frac{13 + 14 + 15}{2} = 21$$

**Step 2 — Apply the formula.**
$$A = \sqrt{21(21-13)(21-14)(21-15)} = \sqrt{21 \times 8 \times 7 \times 6}$$

**Step 3 — Simplify inside the root.**
$$21 \times 8 = 168; \quad 7 \times 6 = 42; \quad 168 \times 42 = 7{,}056$$
$$A = \sqrt{7{,}056} = 84$$

> **Recognising 7,056:** 84² = 7,056. This particular triangle (13-14-15, area 84) appears often enough to be worth memorising.

**Answer: (b) 84 cm²**

---

**Q29. Cube of edge 6 cut into cubes of edge 2. How many? → (c) 27**

**Method 1 — Volume ratio.**
$$\frac{6^3}{2^3} = \frac{216}{8} = 27$$

**Method 2 — Count along each dimension.**
Each edge of 6 cm yields 6/2 = 3 pieces, so:
$$3 \times 3 \times 3 = 27$$

**Answer: (c) 27**

---

**Q30. Cube with diagonal 6√3. Volume? → (c) 216 cm³**

**Step 1 — Use the cube-diagonal formula.**
$$d = a\sqrt3 \implies 6\sqrt3 = a\sqrt3 \implies a = 6$$

**Step 2 — Compute the volume.**
$$V = 6^3 = 216$$

**Answer: (c) 216 cm³**

---

**Q31. 2 m path around a 40 × 30 field. Area of the path? → (c) 296 m²**

**Step 1 — Outer dimensions (add 2w to each).**
$$40 + 2(2) = 44 \text{ m} \qquad 30 + 2(2) = 34 \text{ m}$$

**Step 2 — Outer area.**
$$44 \times 34 = 1{,}496 \text{ m}^2$$

**Step 3 — Inner area.**
$$40 \times 30 = 1{,}200 \text{ m}^2$$

**Step 4 — Path area.**
$$1{,}496 - 1{,}200 = 296 \text{ m}^2$$

> **The 2w rule.** Adding only 2 (giving 42 × 32 = 1,344 and a path of 144 m²) is the standard mistake. The path runs along both sides of every dimension.

**Answer: (c) 296 m²**

---

**Q32. CSA of a cone, r = 7, slant l = 25. → (c) 550 cm²**

**Formula used:** CSA = πrl

$$= \frac{22}{7} \times 7 \times 25 = 22 \times 25 = 550$$

> **Note:** the *slant* height is used for surface area, never the vertical height. (Here h would be √(625 − 49) = 24.)

**Answer: (c) 550 cm²**

---

**Q33. Radius of a sphere doubled — volume factor? → (d) 8**

**Concept:** volume scales as the **cube** of the linear dimension.

$$2^3 = 8$$

**Verification:** r = 1 ⇒ V = 4π/3. r = 2 ⇒ V = 32π/3. Ratio = 8 ✓

**Answer: (d) 8**

---

**Q34. Slant height of a cone, r = 5, h = 12. → (b) 13 cm**

**Formula used:** l = √(r² + h²)

$$l = \sqrt{25 + 144} = \sqrt{169} = 13$$

*(The 5-12-13 triple.)*

**Answer: (b) 13 cm**

---

**Q35. Area of a 90° sector, r = 14. → (c) 154 cm²**

**Formula used:** (θ/360) × πr²

**Step 1 — The fraction of the circle.**
$$\frac{90}{360} = \frac{1}{4}$$

**Step 2 — Full circle area.**
$$\pi r^2 = \frac{22}{7} \times 196 = 616 \text{ cm}^2$$

**Step 3 — Take one quarter.**
$$\frac{616}{4} = 154 \text{ cm}^2$$

**Answer: (c) 154 cm²**

---

**Q36. Circumference 44 cm. Area? → (c) 154 cm²**

**Step 1 — Find the radius.**
$$2\pi r = 44 \implies 2 \times \frac{22}{7} \times r = 44 \implies \frac{44r}{7} = 44 \implies r = 7$$

**Step 2 — Compute the area.**
$$A = \pi r^2 = \frac{22}{7} \times 49 = 154 \text{ cm}^2$$

**Answer: (c) 154 cm²**

---

**Q37. Cylinder and cone, same r and h. Ratio of volumes? → (c) 3 : 1**

$$V_{\text{cylinder}} = \pi r^2 h \qquad V_{\text{cone}} = \frac{1}{3}\pi r^2 h$$

$$\text{Ratio} = \pi r^2 h : \frac{1}{3}\pi r^2 h = 3 : 1$$

> **Watch the order.** The question asks cylinder **to** cone ⇒ 3 : 1. Reversed it would be 1 : 3 — option (a), a deliberate distractor.

**Answer: (c) 3 : 1**

---

**Q38. Square of area 144. Diagonal? → (b) 12√2 cm**

**Step 1 — Find the side.**
$$a = \sqrt{144} = 12$$

**Step 2 — Apply the diagonal formula.**
$$d = a\sqrt2 = 12\sqrt2 \approx 16.97 \text{ cm}$$

**Answer: (b) 12√2 cm**

---

**Q39. Volume of a hemisphere, r = 3. → (b) 18π cm³**

**Formula used:** ⅔πr³

$$V = \frac{2}{3}\pi \times 27 = 18\pi$$

**Cross-check:** a full sphere of radius 3 has volume 36π; half of that is 18π ✓

**Answer: (b) 18π cm³**

---

**Q40. Interior angle sum 1,440°. Number of sides? → (c) 10**

**Formula used:** (n − 2) × 180° = 1,440°

$$n - 2 = \frac{1{,}440}{180} = 8$$
$$n = 10$$

**Answer: (c) 10**

---

### 🔴 HARD — Solutions 41–50

---

**Q41. Cone (r = 6, h = 24) melted into spheres of radius 3. How many? → (b) 8**

**Governing principle: volume is conserved.**

**Step 1 — Volume of the cone.**
$$V = \frac{1}{3}\pi r^2 h = \frac{1}{3}\pi (36)(24) = \frac{1}{3}\pi \times 864 = 288\pi$$

**Step 2 — Volume of one sphere.**
$$v = \frac{4}{3}\pi r^3 = \frac{4}{3}\pi (27) = 36\pi$$

**Step 3 — Divide (π cancels).**
$$\frac{288\pi}{36\pi} = 8$$

**Answer: (b) 8**

> **Cancel π immediately.** Carrying 22/7 through both volumes wastes time and introduces rounding error — the π always cancels in recasting problems.

---

**Q42. Length +25%, breadth −20%. Change in area? → (c) No change**

**Step 1 — Multiply the factors.**
$$1.25 \times 0.80 = 1.00$$

**Step 2 — Interpret.**
A multiplier of exactly 1 means the area is **unchanged**.

**Verification:** l = 100, b = 100 ⇒ area 10,000.
New: l = 125, b = 80 ⇒ area = 10,000 ✓

> **The inverse pair:** +25% and −20% cancel exactly, because 5/4 × 4/5 = 1. The same holds for +20%/−16⅔%, +50%/−33⅓% and +100%/−50%.

**Answer: (c) No change**

---

**Q43. Hollow pipe: R = 8, r = 6, length 21. Volume of material? → (c) 1,848 cm³**

**Step 1 — The material occupies the annular cross-section.**
$$V = \pi(R^2 - r^2) \times h$$

**Step 2 — Compute the difference of squares.**
$$8^2 - 6^2 = 64 - 36 = 28$$

**Step 3 — Substitute.**
$$V = \frac{22}{7} \times 28 \times 21$$

**Step 4 — Cancel and multiply.**
$$= 22 \times 4 \times 21 = 88 \times 21 = 1{,}848 \text{ cm}^3$$

**Answer: (c) 1,848 cm³**

> **Use (R² − r²), not (R − r)².** The material is the difference of two circular areas, not the square of the wall thickness.

---

**Q44. Trapezium area 240, parallel sides 20 and 28. Height? → (b) 10 cm**

**Formula used:** A = ½(a + b)h

**Step 1 — Substitute.**
$$240 = \frac{1}{2}(20 + 28)h = \frac{1}{2}(48)h = 24h$$

**Step 2 — Solve.**
$$h = \frac{240}{24} = 10 \text{ cm}$$

**Verification:** ½(48)(10) = 240 ✓

**Answer: (b) 10 cm**

---

**Q45. Tank 11 × 8 × 7 m emptied into a cylinder of radius 7 m. Depth? → (b) 4 m**

**Governing principle: volume is conserved.**

**Step 1 — Volume of water.**
$$V = 11 \times 8 \times 7 = 616 \text{ m}^3$$

**Step 2 — Set it equal to the cylinder's volume.**
$$\pi r^2 h = 616$$
$$\frac{22}{7} \times 49 \times h = 616$$
$$154h = 616$$

**Step 3 — Solve.**
$$h = \frac{616}{154} = 4 \text{ m}$$

**Answer: (b) 4 m**

---

**Q46. Two cubes of volume 64 cm³ joined end to end. Surface area? → (c) 160 cm²**

**Step 1 — Find each cube's edge.**
$$a = \sqrt[3]{64} = 4 \text{ cm}$$

**Step 2 — Determine the cuboid's dimensions.**
Joining two 4 cm cubes end to end gives:
$$8 \text{ cm} \times 4 \text{ cm} \times 4 \text{ cm}$$

**Step 3 — Apply the cuboid surface-area formula.**
$$\text{SA} = 2(lb + bh + hl) = 2\left[(8)(4) + (4)(4) + (4)(8)\right]$$
$$= 2[32 + 16 + 32] = 2 \times 80 = 160 \text{ cm}^2$$

**Cross-check by counting faces.** Two separate cubes have 2 × 6 × 16 = 192 cm² of surface. Joining them hides two 4 × 4 faces:
$$192 - 2(16) = 192 - 32 = 160 \text{ cm}^2 \checkmark$$

> **The joined faces disappear.** This is why the answer is less than the sum of the two individual surface areas — a point the "192" distractor tests.

**Answer: (c) 160 cm²**

---

**Q47. Circular park of radius 21 m with a 3.5 m path around it. Area of the path? → (b) 500.5 m²**

**Step 1 — Outer radius.**
$$R = 21 + 3.5 = 24.5 \text{ m}$$

**Step 2 — Apply the annulus formula.**
$$A = \pi(R^2 - r^2) = \frac{22}{7}(24.5^2 - 21^2)$$

**Step 3 — Use the difference of squares (much easier than squaring 24.5).**
$$R^2 - r^2 = (R+r)(R-r) = (24.5 + 21)(24.5 - 21) = 45.5 \times 3.5 = 159.25$$

**Step 4 — Multiply.**
$$A = \frac{22}{7} \times 159.25 = 22 \times 22.75 = 500.5 \text{ m}^2$$

**Answer: (b) 500.5 m²**

> **Note the difference from a rectangular path:** for a circle you add the width **once** to the radius (not twice), because the radius already runs from centre to edge.

---

**Q48. Triangle with sides in 3 : 4 : 5, perimeter 144. Area? → (c) 864 cm²**

**Step 1 — Find the actual sides.**
Total ratio parts = 3 + 4 + 5 = 12 ⇒ one part = 144/12 = 12
$$\text{Sides} = 36, \; 48, \; 60 \text{ cm}$$

**Step 2 — Recognise the right angle.**
A 3 : 4 : 5 triangle is always right-angled:
$$36^2 + 48^2 = 1{,}296 + 2{,}304 = 3{,}600 = 60^2 \checkmark$$

**Step 3 — Use the two legs as base and height.**
$$A = \frac{1}{2} \times 36 \times 48 = 18 \times 48 = 864 \text{ cm}^2$$

**Heron cross-check:**
$$s = 72; \quad A = \sqrt{72 \times 36 \times 24 \times 12} = \sqrt{746{,}496} = 864 \checkmark$$

**Answer: (c) 864 cm²**

> **Spotting the 3 : 4 : 5 ratio converts a Heron problem into a one-line calculation.** Always test the sides for a Pythagorean relationship first.

---

**Q49. Sphere of radius 6 recast into a cylinder of radius 4. Height? → (c) 18 cm**

**Governing principle: volume is conserved.**

**Step 1 — Volume of the sphere.**
$$V = \frac{4}{3}\pi (6)^3 = \frac{4}{3}\pi \times 216 = 288\pi$$

**Step 2 — Set it equal to the cylinder's volume.**
$$\pi (4)^2 h = 288\pi$$
$$16h = 288$$

**Step 3 — Solve.**
$$h = 18 \text{ cm}$$

**Answer: (c) 18 cm**

---

**Q50. Volumes of two cubes in 8 : 27. Ratio of surface areas? → (b) 4 : 9**

**Step 1 — Move from volumes to linear dimensions (cube roots).**
$$\sqrt[3]{8} : \sqrt[3]{27} = 2 : 3$$

**Step 2 — Move from linear to areas (square).**
$$2^2 : 3^2 = 4 : 9$$

**Verification.** Take edges 2 and 3.
- Volumes: 8 and 27 ⇒ **8 : 27** ✓
- Surface areas: 6(4) = 24 and 6(9) = 54 ⇒ 24 : 54 = **4 : 9** ✓

**Answer: (b) 4 : 9**

> **The universal chain:** Volume → (∛) → Linear → (square) → Area. Never convert directly between volume and area ratios.

---

## 8. Quick Revision Sheet

> **One page. Read 48 hours after study, and again the night before the test.**

### 2D — Area and perimeter

```
Square       A = a²           P = 4a       d = a√2       A = d²/2
Rectangle    A = lb           P = 2(l+b)   d = √(l²+b²)
Triangle     A = ½bh
Equilateral  A = (√3/4)a²     h = (√3/2)a
Parallelogram A = bh
Rhombus      A = ½d₁d₂
Trapezium    A = ½(a+b)h
Circle       A = πr²          C = 2πr
Sector       A = (θ/360)πr²   arc = (θ/360)2πr
Ring         A = π(R² − r²) = π(R+r)(R−r)

HERON:  s = (a+b+c)/2;  A = √[s(s−a)(s−b)(s−c)]
```

### 3D — Volume and surface area

```
Cube       V = a³        TSA = 6a²        LSA = 4a²     d = a√3
Cuboid     V = lbh       TSA = 2(lb+bh+hl)              d = √(l²+b²+h²)
Cylinder   V = πr²h      CSA = 2πrh       TSA = 2πr(r+h)
Cone       V = ⅓πr²h     CSA = πrl        TSA = πr(r+l)    l = √(r²+h²)
Sphere     V = (4/3)πr³  SA  = 4πr²
Hemisphere V = (2/3)πr³  CSA = 2πr²       TSA = 3πr²

Cone = ⅓ of the cylinder with the same r and h
Cone : Sphere : Cylinder = 1 : 2 : 3   (same r, h = 2r)
```

### ⭐ Scaling laws

```
Linear × k   →   Area × k²   →   Volume × k³

Given AREAS   a:b  →  linear = √a : √b
Given VOLUMES a:b  →  linear = ∛a : ∛b

+10% → area +21%, volume +33.1%
+20% → area +44%, volume +72.8%
×2   → area ×4,   volume ×8
```

### π = 22/7 values

```
r =  7  →  A = 154    C =  44
r = 14  →  A = 616    C =  88
r = 21  →  A = 1386   C = 132
r = 3.5 →  A = 38.5   C =  22
```

### Pythagorean triples

```
3-4-5 (and 6-8-10, 9-12-15, 12-16-20, 15-20-25, 30-40-50)
5-12-13 (and 10-24-26)      8-15-17      7-24-25      9-40-41
```

### Polygons

```
Interior sum        = (n − 2) × 180°
Each interior (reg) = (n−2)180°/n
Exterior sum        = 360°  ALWAYS
Each exterior (reg) = 360°/n
Diagonals           = n(n−3)/2

Triangle 60° · Square 90° · Pentagon 108° · Hexagon 120° · Octagon 135°
```

### Path and recasting templates

```
PATH outside a rectangle, width w
    Outer = (l + 2w)(b + 2w)        ← 2w, always
    Path  = Outer − lb

PATH around a circle, width w
    Outer radius = r + w            ← w only, once
    Path = π[(r+w)² − r²]

MELTING / RECASTING
    Volume is CONSERVED (surface area is NOT)
    Number of pieces = V_original / V_piece
    Cancel π before dividing

WIRE RE-BENT
    LENGTH is conserved (perimeter = circumference)
```

### Sanity checks

```
✓ Cone volume = ⅓ × cylinder (same r, h)
✓ Slant height > vertical height
✓ TSA > CSA for closed solids
✓ Diagonal > any side
✓ Area grows as k², volume as k³
✓ Joining solids HIDES faces — surface area drops
```

---

## 9. Common Mistakes

| # | Mistake | Example | Correction |
|---|---|---|---|
| 1 | **Forgetting ⅓ in a cone** | V = πr²h | V = ⅓πr²h |
| 2 | **Forgetting ½ in a rhombus/triangle** | A = d₁d₂ | A = ½d₁d₂ |
| 3 | **Vertical height used for cone CSA** | πrh | Use the **slant** height: πrl |
| 4 | **Path width added once** | (l + w)(b + w) | Add **2w**: (l + 2w)(b + 2w) |
| 5 | **Circular path treated like a rectangle** | R = r + 2w | For a circle, R = r + w |
| 6 | **Linear % applied to area** | Side +20% ⇒ area +20% | Area ×1.2² ⇒ +44% |
| 7 | **Volume ratio squared instead of cube-rooted** | Volumes 8:27 ⇒ areas 64:729 | ∛ then square: 4 : 9 |
| 8 | **Surface area assumed conserved in melting** | Equating surface areas | Only **volume** is conserved |
| 9 | **(R − r)² instead of (R² − r²)** | Pipe material | Use R² − r² |
| 10 | **Open vs closed solid ignored** | TSA of an open tank | Subtract the missing face |
| 11 | **Joined solids: faces not removed** | Two cubes ⇒ 192 cm² | Subtract the two hidden faces ⇒ 160 |
| 12 | **Ratio order reversed** | Cylinder : cone given as 1 : 3 | Cylinder is larger ⇒ 3 : 1 |
| 13 | **Heron used when a triple exists** | 9-12-15 through Heron | Right-angled ⇒ ½ × 9 × 12 |
| 14 | **π not cancelled** | Carrying 22/7 through both volumes | It always cancels in recasting |

---

## Practice Answer Key

| Q | Ans | Q | Ans | Q | Ans | Q | Ans | Q | Ans |
|---|---|---|---|---|---|---|---|---|---|
| 1 | c | 11 | c | 21 | c | 31 | c | 41 | b |
| 2 | b | 12 | b | 22 | b | 32 | c | 42 | c |
| 3 | c | 13 | b | 23 | c | 33 | d | 43 | c |
| 4 | c | 14 | c | 24 | b | 34 | b | 44 | b |
| 5 | b | 15 | c | 25 | c | 35 | c | 45 | b |
| 6 | d | 16 | c | 26 | b | 36 | c | 46 | c |
| 7 | b | 17 | c | 27 | a | 37 | c | 47 | b |
| 8 | c | 18 | b | 28 | b | 38 | b | 48 | c |
| 9 | c | 19 | b | 29 | c | 39 | b | 49 | c |
| 10 | c | 20 | b | 30 | c | 40 | c | 50 | b |

**Scoring guide:** 45+/50 → strong. 35–44 → solid; re-drill the formula bank until recall is instant. Below 35 → this topic is pure memory — write out Section 3 by hand twice, then redo the whole set.

---

**⬅️ Back:** [Topic 10 — Permutation, Combination & Probability](10-permutation-combination-probability.md) · **➡️ Next:** [Topic 12 — Ages, Clocks & Calendars](12-ages-clocks-calendars.md)
