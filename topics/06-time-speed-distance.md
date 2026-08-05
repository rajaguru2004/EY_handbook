# Topic 6 — Time, Speed & Distance (with Trains, Boats & Streams)

### EY Placement Aptitude Handbook · Priority Rank #5 · 🔴 Critical

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

**Weightage:** 8–10% of the quantitative section — a **near-guaranteed appearance**. Trains and boats-and-streams are sub-topics of the same core relation, so all three are covered here.

**Question styles reported:**

| Style | Frequency | Typical shape |
|---|---|---|
| Basic speed/time/distance | Very high | "240 km in 4 hours — find the speed" |
| Unit conversion | Very high | "Convert 72 km/h to m/s" |
| Average speed (out and back) | High | "40 km/h out, 60 km/h back" |
| Train crossing a pole/platform | High | "180 m train crosses a pole in 9 s" |
| Two trains crossing | High | "Opposite directions at 54 and 36 km/h" |
| Boats: upstream/downstream | High | "24 km down in 3 h, back in 4 h" |
| Relative speed (meeting/overtaking) | Medium | "Two cars 45 km apart after how long?" |
| Late/early (the "x minutes late" type) | Medium | "4 km/h → 8 min late; 5 km/h → 7 min early" |
| Fractional-speed type | Medium | "At 4/5 of usual speed, 20 minutes late" |
| Mixed-mode journey | Medium | "Part by train at 100, part by car at 60" |

---

## 2. Core Concepts

### 2.1 The master relation

$$\boxed{\text{Distance} = \text{Speed} \times \text{Time}}$$

$$\text{Speed} = \frac{\text{Distance}}{\text{Time}} \qquad\qquad \text{Time} = \frac{\text{Distance}}{\text{Speed}}$$

A useful memory device:

```
        ┌─────────────┐
        │      D      │      Cover the quantity you want:
        ├──────┬──────┤        D  →  S × T
        │  S   │   T  │        S  →  D / T
        └──────┴──────┘        T  →  D / S
```

### 2.2 Unit conversion — the two numbers to memorise

$$\boxed{1 \text{ km/h} = \frac{5}{18} \text{ m/s}} \qquad\qquad \boxed{1 \text{ m/s} = \frac{18}{5} \text{ km/h}}$$

```
km/h  →  m/s    :   multiply by 5/18
m/s   →  km/h   :   multiply by 18/5
```

**Values worth knowing on sight:**

| km/h | m/s | | km/h | m/s |
|---|---|---|---|---|
| 18 | 5 | | 72 | 20 |
| 36 | 10 | | 90 | 25 |
| 45 | 12.5 | | 108 | 30 |
| 54 | 15 | | 126 | 35 |
| 60 | 16⅔ | | 144 | 40 |

> **Rule of thumb:** any multiple of 18 km/h gives a whole number of m/s. Exam-setters exploit this — if you see 36, 54, 72, 90 or 108 km/h, expect clean arithmetic.

### 2.3 The inverse relationship

**For a fixed distance, speed and time are inversely proportional:**

$$S_1 T_1 = S_2 T_2 \qquad \implies \qquad \frac{S_1}{S_2} = \frac{T_2}{T_1}$$

$$\boxed{\text{Speed ratio } a : b \implies \text{Time ratio } b : a}$$

> Speeds in the ratio 3 : 4 ⇒ times in the ratio 4 : 3.
> Speed increased by 25% (ratio 5 : 4) ⇒ time falls to 4/5 of the original (a 20% reduction).

**This is the engine behind the "fractional speed" family of questions** — see §2.8.

### 2.4 Average speed

$$\text{Average speed} = \frac{\text{Total distance}}{\text{Total time}}$$

**Never** the arithmetic mean of the speeds — unless the *times* are equal.

| Situation | Average speed |
|---|---|
| Equal **distances** at *u* and *v* | $\dfrac{2uv}{u+v}$ (harmonic mean) |
| Equal **distances** at *u*, *v*, *w* | $\dfrac{3uvw}{uv+vw+wu}$ |
| Equal **times** at *u* and *v* | $\dfrac{u+v}{2}$ (arithmetic mean) |
| General | Total distance ÷ total time |

> Out at 40 km/h, back at 60 km/h ⇒ 2(40)(60)/100 = **48 km/h** (not 50).
> The traveller spends more time at the slower speed, so the average is dragged below the midpoint.

### 2.5 Relative speed

| Situation | Relative speed |
|---|---|
| Moving **towards** each other (or opposite directions) | $S_1 + S_2$ |
| Moving in the **same** direction | $|S_1 - S_2|$ |

**Time to meet / overtake:**

$$\text{Time} = \frac{\text{Distance between them (+ lengths, for trains)}}{\text{Relative speed}}$$

> Two trains 300 km apart moving towards each other at 40 and 60 km/h:
> Relative speed = 100 km/h ⇒ they meet after 300/100 = **3 hours**.

> Two cars from the same point, same direction, at 50 and 65 km/h:
> Relative speed = 15 km/h ⇒ 45 km apart after 45/15 = **3 hours**.

### 2.6 Trains — the length rule

**The key idea: a train must travel its own length plus the length of whatever it is crossing.**

| Crossing | Distance covered |
|---|---|
| A pole / a man / a signal post / a tree | **Length of the train** |
| A platform / bridge / tunnel | **Train length + platform length** |
| Another train (either direction) | **Sum of both train lengths** |
| A man walking (same direction) | Train length, at relative speed (S_train − S_man) |
| A man walking (opposite direction) | Train length, at relative speed (S_train + S_man) |

$$\text{Time to cross} = \frac{\text{Total length}}{\text{Relative speed}}$$

> A 180 m train crosses a pole in 9 s ⇒ speed = 180/9 = 20 m/s = 72 km/h.
> The same train crosses a platform in 20 s ⇒ total distance = 20 × 20 = 400 m ⇒ **platform = 400 − 180 = 220 m**.

> **Point objects have zero length.** A pole, a man, a signal — all contribute nothing to the distance. A platform, bridge or second train does.

### 2.7 Boats & Streams

Let *b* = speed of the boat in still water, *s* = speed of the stream.

$$\boxed{\text{Downstream speed} = b + s} \qquad \boxed{\text{Upstream speed} = b - s}$$

Reversing these:

$$\boxed{b = \frac{\text{Down} + \text{Up}}{2}} \qquad\qquad \boxed{s = \frac{\text{Down} - \text{Up}}{2}}$$

> A boat covers 24 km downstream in 3 h and returns in 4 h.
> Down = 8 km/h, Up = 6 km/h.
> Boat = (8 + 6)/2 = **7 km/h**; Stream = (8 − 6)/2 = **1 km/h**.

**Useful derived results:**

| Given | Result |
|---|---|
| Same distance *d* each way, total time *T* | $\dfrac{d}{b+s} + \dfrac{d}{b-s} = T$ |
| Upstream takes *k* times as long as downstream | $b + s = k(b - s)$ |
| Round trip, average speed | $\dfrac{2(b+s)(b-s)}{2b} = \dfrac{b^2 - s^2}{b}$ |

> **The two-equation type.** "16 km up + 24 km down in 6 h; 12 km up + 36 km down in 6 h" — substitute *a* = 1/u and *b* = 1/d to turn it into a pair of **linear** equations. See Solved Example 8.

### 2.8 The fractional-speed family

> *"Travelling at a/b of his usual speed, a man is *t* minutes late. Find his usual time."*

**Logic:** speed × (a/b) ⇒ time × (b/a). The extra time is the difference.

$$T_{\text{new}} = \frac{b}{a} T_{\text{usual}} \implies \text{Delay} = \left(\frac{b}{a} - 1\right) T_{\text{usual}} = t$$

$$\boxed{T_{\text{usual}} = \frac{t}{\frac{b}{a} - 1} = \frac{a \, t}{b - a}}$$

| Speed becomes | Time becomes | Delay as a fraction of usual time |
|---|---|---|
| 3/4 of usual | 4/3 | T/3 |
| 4/5 of usual | 5/4 | T/4 |
| 5/6 of usual | 6/5 | T/5 |
| 2/3 of usual | 3/2 | T/2 |
| 6/7 of usual | 7/6 | T/6 |

> At 3/4 speed he is 20 minutes late ⇒ T/3 = 20 ⇒ **usual time = 60 minutes**.
> At 4/5 speed he is 20 minutes late ⇒ T/4 = 20 ⇒ **usual time = 80 minutes**.

### 2.9 The late-and-early type

> *"At *u* km/h he is *p* minutes late; at *v* km/h he is *q* minutes early. Find the distance."*

The **time difference between the two journeys is (p + q) minutes**:

$$\frac{d}{u} - \frac{d}{v} = \frac{p + q}{60} \text{ hours}$$

> At 4 km/h he is 8 min late; at 5 km/h, 7 min early.
> Time difference = 15 min = 1/4 h.
> $$\frac{d}{4} - \frac{d}{5} = \frac{1}{4} \implies \frac{d}{20} = \frac{1}{4} \implies d = 5 \text{ km}$$

> **The common error:** using (p − q) instead of (p + q). One journey is late and the other early, so the gap between them is the *sum* of the two deviations from the scheduled time.

---

## 3. Formula Bank

| # | Concept | Formula |
|---|---|---|
| 1 | Master relation | $D = S \times T$ |
| 2 | km/h → m/s | $\times \dfrac{5}{18}$ |
| 3 | m/s → km/h | $\times \dfrac{18}{5}$ |
| 4 | Fixed distance | $S_1T_1 = S_2T_2$ |
| 5 | Speed ratio ⇒ time ratio | $a : b \implies b : a$ |
| 6 | Average speed (general) | $\dfrac{\text{Total distance}}{\text{Total time}}$ |
| 7 | Equal distances, 2 speeds | $\dfrac{2uv}{u+v}$ |
| 8 | Equal distances, 3 speeds | $\dfrac{3uvw}{uv+vw+wu}$ |
| 9 | Equal times, 2 speeds | $\dfrac{u+v}{2}$ |
| 10 | Relative speed (opposite) | $S_1 + S_2$ |
| 11 | Relative speed (same direction) | $|S_1 - S_2|$ |
| 12 | Train crossing a pole | $t = \dfrac{L_{\text{train}}}{S}$ |
| 13 | Train crossing a platform | $t = \dfrac{L_{\text{train}} + L_{\text{platform}}}{S}$ |
| 14 | Two trains crossing | $t = \dfrac{L_1 + L_2}{S_{\text{rel}}}$ |
| 15 | Downstream speed | $b + s$ |
| 16 | Upstream speed | $b - s$ |
| 17 | Boat speed in still water | $\dfrac{\text{Down} + \text{Up}}{2}$ |
| 18 | Stream speed | $\dfrac{\text{Down} - \text{Up}}{2}$ |
| 19 | Round trip average (boat) | $\dfrac{b^2 - s^2}{b}$ |
| 20 | Fractional speed a/b, late by *t* | $T_{\text{usual}} = \dfrac{a\,t}{b-a}$ |
| 21 | Late *p*, early *q* | $\dfrac{d}{u} - \dfrac{d}{v} = \dfrac{p+q}{60}$ |
| 22 | Two bodies meeting, distance ratio | Distances are in the ratio of the speeds |

---

## 4. Shortcuts & Tricks

### 4.1 Convert units FIRST, always

Before writing anything else, put every speed into a single unit system. Most train problems are cleanest in **m/s**; most journey problems in **km/h**.

```
Train problems  →  work in metres and seconds
Journey problems →  work in kilometres and hours
Mixed problem   →  convert to whichever avoids fractions
```

The single most common error in this entire topic is mixing km/h with metres and seconds.

### 4.2 The speed–time inverse ratio

Whenever the distance is fixed, convert the speed change into a **ratio** and flip it.

| Speed change | Speed ratio | Time ratio | Effect on time |
|---|---|---|---|
| ×2 | 2 : 1 | 1 : 2 | Halved |
| +25% | 5 : 4 | 4 : 5 | Down 20% |
| +50% | 3 : 2 | 2 : 3 | Down 33⅓% |
| −20% | 4 : 5 | 5 : 4 | Up 25% |
| ×3/4 | 3 : 4 | 4 : 3 | Up 33⅓% |

### 4.3 Train problems — the two-step template

```
Step 1:  What total distance must the train cover?
             pole/man     →  L_train
             platform     →  L_train + L_platform
             other train  →  L_1 + L_2

Step 2:  What is the relevant speed?
             stationary object →  train's own speed
             opposite direction →  S_1 + S_2
             same direction     →  |S_1 − S_2|

Time = Step 1 ÷ Step 2
```

### 4.4 The pole-and-platform pair

If a train crosses a **pole** in *t*₁ seconds and a **platform** in *t*₂ seconds:

$$\text{Speed} = \frac{L_{\text{platform}}}{t_2 - t_1} \qquad\qquad L_{\text{train}} = \text{Speed} \times t_1$$

> Crosses a pole in 8 s and a 264 m platform in 20 s.
> Speed = 264/(20 − 8) = 264/12 = **22 m/s**; length = 22 × 8 = **176 m**.

This bypasses simultaneous equations entirely.

### 4.5 Boats — always find Down and Up first

```
Step 1:  Compute downstream speed  =  distance ÷ time (downstream leg)
Step 2:  Compute upstream speed    =  distance ÷ time (upstream leg)
Step 3:  Boat   = (Down + Up)/2
         Stream = (Down − Up)/2
```

Never try to set up simultaneous equations in *b* and *s* directly — reduce to Down and Up first.

### 4.6 The 1/u, 1/v substitution

For boat problems giving **two** combinations of upstream and downstream distances:

$$\text{Let } a = \frac{1}{\text{upstream speed}}, \qquad b = \frac{1}{\text{downstream speed}}$$

The equations become **linear** in *a* and *b*, and standard elimination applies.

> 30 km up + 44 km down in 10 h; 40 km up + 55 km down in 13 h
> $$30a + 44b = 10 \qquad 40a + 55b = 13$$
> Eliminate as usual → *b* = 1/11 and *a* = 1/5 → Down = 11, Up = 5 → **stream = 3 km/h**

### 4.7 The meeting-point ratio

When two bodies start simultaneously from opposite ends and meet:

$$\frac{\text{Distance covered by A}}{\text{Distance covered by B}} = \frac{\text{Speed of A}}{\text{Speed of B}}$$

(They travelled for the same time, so distance ∝ speed.)

> Speeds 60 and 90 km/h; one has travelled 120 km more when they meet.
> Distance ratio = 2 : 3 ⇒ the difference is **1 part** = 120 km.
> Total = 5 parts = **600 km**.

### 4.8 The dog-between-two-walkers trick

A classic that looks hard and is trivial.

> *"Two men 27 km apart walk towards each other at 4 and 5 km/h. A dog runs back and forth between them at 10 km/h. How far does the dog run?"*

**Don't model the zigzag.** Ask only: **for how long does the dog run?**

The men meet after 27/(4 + 5) = **3 hours**. The dog runs continuously for those 3 hours.
$$\text{Distance} = 10 \times 3 = \mathbf{30 \text{ km}}$$

### 4.9 Sanity checks

```
✓ Average speed (equal distances) is ALWAYS less than the arithmetic mean
✓ Average speed always lies BETWEEN the slowest and fastest speed
✓ Downstream speed > still-water speed > upstream speed
✓ Train crossing a platform takes LONGER than crossing a pole
✓ Same-direction relative speed < opposite-direction relative speed
✓ If speed goes up, time must come down
```

---

## 5. Solved Examples

### Example 1 — Unit conversion and basic computation

**Q.** A train covers 315 km in 3.5 hours. Express its speed in m/s.

**Step 1 — Compute the speed in km/h.**
$$S = \frac{315}{3.5} = 90 \text{ km/h}$$

**Step 2 — Convert to m/s.**
$$90 \times \frac{5}{18} = 5 \times 5 = 25 \text{ m/s}$$

**Answer: 25 m/s**

> **The clean-division trick:** dividing by 18 first is usually easier than multiplying by 5 first. Here 90 ÷ 18 = 5, then × 5 = 25.

---

### Example 2 — Average speed for a round trip

**Q.** A cyclist rides from town A to town B at 15 km/h and returns along the same road at 10 km/h. Find the average speed for the whole journey.

**Step 1 — Recognise equal distances ⇒ use the harmonic mean.**
$$\text{Average} = \frac{2uv}{u+v} = \frac{2 \times 15 \times 10}{25} = \frac{300}{25} = 12 \text{ km/h}$$

**Step 2 — Verify from first principles.** Let the one-way distance be 30 km (LCM of 15 and 10).
$$\text{Time out} = \frac{30}{15} = 2 \text{ h}, \qquad \text{Time back} = \frac{30}{10} = 3 \text{ h}$$
$$\text{Average} = \frac{60}{5} = 12 \text{ km/h} \checkmark$$

**Answer: 12 km/h**

> **Why not 12.5?** He spends 3 hours at the slow speed but only 2 at the fast one. More time at 10 km/h pulls the average below the midpoint.

---

### Example 3 — Train crossing a platform

**Q.** A train 200 m long, running at 72 km/h, crosses a platform in 25 seconds. Find the length of the platform.

**Step 1 — Convert the speed to m/s.**
$$72 \times \frac{5}{18} = 20 \text{ m/s}$$

**Step 2 — Compute the total distance covered.**
$$D = S \times T = 20 \times 25 = 500 \text{ m}$$

**Step 3 — Subtract the train's own length.**
When crossing a platform, the train covers (its own length + platform length):
$$L_{\text{platform}} = 500 - 200 = 300 \text{ m}$$

**Answer: 300 m**

**Cross-check:** total = 200 + 300 = 500 m at 20 m/s = 25 s ✓

---

### Example 4 — Two trains crossing each other

**Q.** Two trains of lengths 150 m and 100 m run on parallel tracks in opposite directions at 54 km/h and 36 km/h. How long will they take to cross each other completely?

**Step 1 — Compute the relative speed.**
Opposite directions ⇒ speeds add:
$$54 + 36 = 90 \text{ km/h}$$

**Step 2 — Convert to m/s.**
$$90 \times \frac{5}{18} = 25 \text{ m/s}$$

**Step 3 — Compute the total distance to be covered.**
To cross *completely*, the trains together traverse both lengths:
$$150 + 100 = 250 \text{ m}$$

**Step 4 — Time.**
$$\frac{250}{25} = 10 \text{ seconds}$$

**Answer: 10 seconds**

> **If they had run in the same direction**, the relative speed would be 54 − 36 = 18 km/h = 5 m/s, and the crossing would take 250/5 = **50 seconds** — five times as long.

---

### Example 5 — Train and a walking man

**Q.** A train 150 m long passes a man walking at 6 km/h in the opposite direction in 7.5 seconds. Find the speed of the train.

**Step 1 — Identify the distance covered.**
A man is a *point object* — he has no length. So the train covers only its own length:
$$D = 150 \text{ m}$$

**Step 2 — Compute the relative speed.**
$$S_{\text{rel}} = \frac{150}{7.5} = 20 \text{ m/s}$$

**Step 3 — Convert to km/h.**
$$20 \times \frac{18}{5} = 72 \text{ km/h}$$

**Step 4 — Extract the train's own speed.**
They move in opposite directions, so the relative speed is the **sum**:
$$S_{\text{train}} + 6 = 72 \implies S_{\text{train}} = 66 \text{ km/h}$$

**Answer: 66 km/h**

> **If the man had been walking in the same direction**, the relative speed would be the *difference*, giving S_train − 6 = 72 ⇒ **78 km/h**. Read the direction carefully.

---

### Example 6 — Boats and streams, both speeds

**Q.** A boat covers 36 km downstream in 3 hours and the same distance upstream in 6 hours. Find the speed of the boat in still water and the speed of the stream.

**Step 1 — Compute the two effective speeds.**
$$\text{Downstream} = \frac{36}{3} = 12 \text{ km/h}$$
$$\text{Upstream} = \frac{36}{6} = 6 \text{ km/h}$$

**Step 2 — Apply the half-sum and half-difference formulas.**
$$b = \frac{\text{Down} + \text{Up}}{2} = \frac{12 + 6}{2} = 9 \text{ km/h}$$
$$s = \frac{\text{Down} - \text{Up}}{2} = \frac{12 - 6}{2} = 3 \text{ km/h}$$

**Verification:**
- Downstream = 9 + 3 = 12 ✓
- Upstream = 9 − 3 = 6 ✓

**Answer: Boat = 9 km/h, Stream = 3 km/h**

> **Sanity check:** the stream speed must always be less than the boat speed, otherwise the boat could never go upstream. 3 < 9 ✓

---

### Example 7 — The late-and-early problem

**Q.** A student walking to school at 3 km/h arrives 10 minutes late. Walking at 4 km/h, he arrives 5 minutes early. Find the distance to the school.

**Step 1 — Find the time difference between the two journeys.**
One journey ends 10 minutes *after* the bell, the other 5 minutes *before* it. The gap between them is:
$$10 + 5 = 15 \text{ minutes} = \frac{1}{4} \text{ hour}$$

**Step 2 — Write the equation.**
$$\frac{d}{3} - \frac{d}{4} = \frac{1}{4}$$

**Step 3 — Combine the left side.**
$$\frac{4d - 3d}{12} = \frac{d}{12}$$

**Step 4 — Solve.**
$$\frac{d}{12} = \frac{1}{4} \implies d = 3 \text{ km}$$

**Verification:**
- At 3 km/h: time = 1 hour = 60 minutes
- At 4 km/h: time = 0.75 hour = 45 minutes
- Difference = 15 minutes ✓ (10 late + 5 early)
- Scheduled time = 50 minutes: 60 is 10 late ✓, 45 is 5 early ✓

**Answer: 3 km**

> **The critical step is Step 1.** Adding the late and early amounts — not subtracting them — is what makes this problem work.

---

### Example 8 — Boats with two combined journeys

**Q.** A boat travels 16 km upstream and 24 km downstream in 6 hours. It also travels 12 km upstream and 36 km downstream in 6 hours. Find the speed of the boat in still water.

**Step 1 — Substitute to linearise.**
Let *u* = upstream speed and *d* = downstream speed. Set:
$$a = \frac{1}{u}, \qquad b = \frac{1}{d}$$

**Step 2 — Write both journeys as equations.**
$$16a + 24b = 6 \qquad \text{...(i)}$$
$$12a + 36b = 6 \qquad \text{...(ii)}$$

**Step 3 — Eliminate *a*.**
Multiply (i) by 3 and (ii) by 4 to match the coefficients of *a* (LCM of 16 and 12 is 48):
$$48a + 72b = 18 \qquad \text{...(iii)}$$
$$48a + 144b = 24 \qquad \text{...(iv)}$$

**Step 4 — Subtract (iii) from (iv).**
$$72b = 6 \implies b = \frac{1}{12} \implies d = 12 \text{ km/h}$$

**Step 5 — Back-substitute into (i).**
$$16a + 24\left(\frac{1}{12}\right) = 6$$
$$16a + 2 = 6 \implies 16a = 4 \implies a = \frac{1}{4} \implies u = 4 \text{ km/h}$$

**Step 6 — Compute the boat's still-water speed.**
$$b_{\text{boat}} = \frac{d + u}{2} = \frac{12 + 4}{2} = 8 \text{ km/h}$$

*(And the stream = (12 − 4)/2 = 4 km/h.)*

**Verification of (ii):**
$$\frac{12}{4} + \frac{36}{12} = 3 + 3 = 6 \text{ hours} \checkmark$$

**Answer: 8 km/h**

> **Why substitute?** Written in terms of *b* and *s* directly, these equations are non-linear (16/(b−s) + 24/(b+s) = 6) and painful. The 1/u, 1/v substitution makes them ordinary simultaneous linear equations.

---

## 6. Practice Questions

**Instructions:** 50 questions. Easy (1–20), Medium (21–40), Hard (41–50).
Target times: Easy 30 s · Medium 60 s · Hard 90 s.
Full solutions in [Section 7](#7-detailed-solutions).

### 🟢 EASY (Questions 1–20)

**Q1.** A car travels 240 km in 4 hours. Find its speed.
(a) 50 km/h  (b) 55 km/h  (c) 60 km/h  (d) 65 km/h

**Q2.** Convert 72 km/h into m/s.
(a) 15 m/s  (b) 18 m/s  (c) 20 m/s  (d) 25 m/s

**Q3.** Convert 25 m/s into km/h.
(a) 75 km/h  (b) 80 km/h  (c) 90 km/h  (d) 100 km/h

**Q4.** A man walks at 5 km/h for 3 hours. Find the distance covered.
(a) 12 km  (b) 15 km  (c) 18 km  (d) 20 km

**Q5.** How long will it take to cover 180 km at 45 km/h?
(a) 3 hours  (b) 3.5 hours  (c) 4 hours  (d) 4.5 hours

**Q6.** A train 200 m long crosses a pole in 10 seconds. Find its speed in km/h.
(a) 60 km/h  (b) 66 km/h  (c) 72 km/h  (d) 80 km/h

**Q7.** A boat's speed in still water is 12 km/h and the stream flows at 3 km/h. Find the downstream speed.
(a) 9 km/h  (b) 12 km/h  (c) 15 km/h  (d) 18 km/h

**Q8.** Using the data of Q7, find the upstream speed.
(a) 9 km/h  (b) 12 km/h  (c) 15 km/h  (d) 18 km/h

**Q9.** A train travels 300 km in 5 hours. Find its speed in m/s.
(a) 15 m/s  (b) 16⅔ m/s  (c) 18 m/s  (d) 20 m/s

**Q10.** A cyclist covers 30 km in 2.5 hours. Find his speed.
(a) 10 km/h  (b) 12 km/h  (c) 14 km/h  (d) 15 km/h

**Q11.** Two trains move towards each other at 40 km/h and 60 km/h. Find their relative speed.
(a) 20 km/h  (b) 50 km/h  (c) 80 km/h  (d) 100 km/h

**Q12.** Two trains move in the same direction at 70 km/h and 40 km/h. Find their relative speed.
(a) 30 km/h  (b) 55 km/h  (c) 100 km/h  (d) 110 km/h

**Q13.** A car covers a certain distance at 60 km/h in 3 hours. How long would it take at 90 km/h?
(a) 1.5 hours  (b) 2 hours  (c) 2.5 hours  (d) 3 hours

**Q14.** A train 150 m long crosses a platform 250 m long in 20 seconds. Find its speed in km/h.
(a) 60 km/h  (b) 66 km/h  (c) 72 km/h  (d) 80 km/h

**Q15.** A vehicle covers 120 km in 1.5 hours. Find its speed.
(a) 70 km/h  (b) 75 km/h  (c) 80 km/h  (d) 90 km/h

**Q16.** A boat goes 20 km downstream in 2 hours. Find the downstream speed.
(a) 8 km/h  (b) 10 km/h  (c) 12 km/h  (d) 15 km/h

**Q17.** If the speed is doubled, the time taken to cover the same distance becomes:
(a) Doubled  (b) Halved  (c) Unchanged  (d) Four times

**Q18.** A man covers 12 km in 90 minutes. Find his speed in km/h.
(a) 6 km/h  (b) 7 km/h  (c) 8 km/h  (d) 9 km/h

**Q19.** A boat's speed in still water is 10 km/h and its downstream speed is 14 km/h. Find the speed of the stream.
(a) 2 km/h  (b) 3 km/h  (c) 4 km/h  (d) 5 km/h

**Q20.** A train running at 54 km/h crosses a pole in 12 seconds. Find its length.
(a) 150 m  (b) 165 m  (c) 180 m  (d) 200 m

---

### 🟡 MEDIUM (Questions 21–40)

**Q21.** A person travels from A to B at 40 km/h and returns at 60 km/h. Find the average speed for the whole journey.
(a) 45 km/h  (b) 48 km/h  (c) 50 km/h  (d) 52 km/h

**Q22.** A train 120 m long passes a man walking at 6 km/h in the opposite direction in 6 seconds. Find the speed of the train.
(a) 60 km/h  (b) 64 km/h  (c) 66 km/h  (d) 72 km/h

**Q23.** Two trains 100 m and 150 m long run in opposite directions at 54 km/h and 36 km/h. How long will they take to cross each other?
(a) 8 s  (b) 10 s  (c) 12 s  (d) 15 s

**Q24.** A boat covers 24 km downstream in 3 hours and returns upstream in 4 hours. Find the speed of the boat in still water and the speed of the stream.
(a) 6 km/h, 2 km/h  (b) 7 km/h, 1 km/h  (c) 8 km/h, 2 km/h  (d) 7.5 km/h, 0.5 km/h

**Q25.** A man covers half of a journey at 30 km/h and the other half at 60 km/h. Find the average speed.
(a) 35 km/h  (b) 40 km/h  (c) 45 km/h  (d) 50 km/h

**Q26.** A train travelling at 72 km/h crosses a 400 m platform in 30 seconds. Find the length of the train.
(a) 150 m  (b) 180 m  (c) 200 m  (d) 240 m

**Q27.** A car travels the first 60 km at 30 km/h and the next 60 km at 60 km/h. Find the average speed.
(a) 36 km/h  (b) 40 km/h  (c) 45 km/h  (d) 48 km/h

**Q28.** A boat takes 3 hours to travel 12 km upstream and 3 hours to travel 24 km downstream. Find the speed of the stream.
(a) 1 km/h  (b) 2 km/h  (c) 3 km/h  (d) 4 km/h

**Q29.** A man walking at 4 km/h reaches his office 8 minutes late. Walking at 5 km/h he reaches 7 minutes early. Find the distance to his office.
(a) 4 km  (b) 4.5 km  (c) 5 km  (d) 6 km

**Q30.** Two trains start simultaneously from stations 300 km apart and travel towards each other at 40 km/h and 60 km/h. After how long will they meet?
(a) 2 hours  (b) 2.5 hours  (c) 3 hours  (d) 3.5 hours

**Q31.** A train 180 m long crosses a platform in 20 seconds and a pole in 9 seconds. Find the length of the platform.
(a) 180 m  (b) 200 m  (c) 220 m  (d) 240 m

**Q32.** A man rows 30 km downstream in 2 hours and 18 km upstream in 3 hours. Find his speed in still water.
(a) 9 km/h  (b) 10 km/h  (c) 10.5 km/h  (d) 12 km/h

**Q33.** A train travels at 60 km/h for the first 2 hours and 80 km/h for the next 3 hours. Find the average speed.
(a) 68 km/h  (b) 70 km/h  (c) 72 km/h  (d) 75 km/h

**Q34.** Two cars start from the same point in the same direction at 50 km/h and 65 km/h. After how long will they be 45 km apart?
(a) 2 hours  (b) 2.5 hours  (c) 3 hours  (d) 3.5 hours

**Q35.** A boat's speed in still water is 15 km/h. It takes twice as long to travel a certain distance upstream as downstream. Find the speed of the stream.
(a) 3 km/h  (b) 4 km/h  (c) 5 km/h  (d) 6 km/h

**Q36.** A train 250 m long running at 90 km/h crosses a bridge in 30 seconds. Find the length of the bridge.
(a) 400 m  (b) 450 m  (c) 500 m  (d) 550 m

**Q37.** A man travels 600 km, partly by train at 100 km/h and partly by car at 60 km/h. The whole journey takes 8 hours. Find the distance covered by train.
(a) 240 km  (b) 280 km  (c) 300 km  (d) 350 km

**Q38.** Two trains of lengths 120 m and 180 m run on parallel tracks in the same direction at 72 km/h and 54 km/h. How long will the faster train take to overtake the slower one completely?
(a) 40 s  (b) 50 s  (c) 60 s  (d) 75 s

**Q39.** A cyclist covers a distance in 5 hours. If he increases his speed by 2 km/h, he covers the same distance in 4 hours. Find the distance.
(a) 30 km  (b) 36 km  (c) 40 km  (d) 45 km

**Q40.** A boat travels 16 km upstream and 24 km downstream in 6 hours. It also travels 12 km upstream and 36 km downstream in 6 hours. Find the speed of the boat in still water.
(a) 6 km/h  (b) 7 km/h  (c) 8 km/h  (d) 10 km/h

---

### 🔴 HARD (Questions 41–50)

**Q41.** A train crosses a man standing on a platform in 8 seconds and crosses the whole platform in 20 seconds. If the platform is 264 m long, find the length of the train.
(a) 154 m  (b) 165 m  (c) 176 m  (d) 198 m

**Q42.** Two trains start at the same time from stations A and B and travel towards each other at 60 km/h and 90 km/h. When they meet, one has travelled 120 km more than the other. Find the distance between A and B.
(a) 480 km  (b) 540 km  (c) 600 km  (d) 660 km

**Q43.** A man can row at 8 km/h in still water. In a river flowing at 2 km/h, it takes him 3 hours 12 minutes to row to a place and return. How far is the place?
(a) 10 km  (b) 12 km  (c) 14 km  (d) 15 km

**Q44.** A train travelling at four-fifths of its usual speed is 20 minutes late. Find its usual travel time.
(a) 60 min  (b) 70 min  (c) 80 min  (d) 100 min

**Q45.** Two men start walking towards each other from points 27 km apart at 4 km/h and 5 km/h. At the same moment a dog starts from the first man and runs back and forth between the two at 10 km/h until they meet. Find the total distance run by the dog.
(a) 24 km  (b) 27 km  (c) 30 km  (d) 33 km

**Q46.** A train 400 m long crosses another train 300 m long running in the opposite direction in 14 seconds. If the speed of the first train is 90 km/h, find the speed of the second train.
(a) 72 km/h  (b) 80 km/h  (c) 90 km/h  (d) 108 km/h

**Q47.** A person travels 60 km. Had he travelled 2 km/h faster, he would have taken 1 hour less. Find his original speed.
(a) 8 km/h  (b) 10 km/h  (c) 12 km/h  (d) 15 km/h

**Q48.** A boat travels 30 km upstream and 44 km downstream in 10 hours. It also travels 40 km upstream and 55 km downstream in 13 hours. Find the speed of the stream.
(a) 2 km/h  (b) 3 km/h  (c) 4 km/h  (d) 5 km/h

**Q49.** A car covers the first third of a journey at 40 km/h, the second third at 60 km/h and the last third at 120 km/h. Find the average speed for the whole journey.
(a) 55 km/h  (b) 60 km/h  (c) 66⅔ km/h  (d) 73⅓ km/h

**Q50.** Walking at three-fourths of his usual speed, a man reaches his office 20 minutes late. Find his usual travel time.
(a) 45 min  (b) 50 min  (c) 60 min  (d) 75 min

---

## 7. Detailed Solutions

### 🟢 EASY — Solutions 1–20

---

**Q1. 240 km in 4 hours. Speed? → (c) 60 km/h**

**Formula used:** S = D / T

$$\frac{240}{4} = 60 \text{ km/h}$$

**Answer: (c) 60 km/h**

---

**Q2. Convert 72 km/h to m/s. → (c) 20 m/s**

**Formula used:** km/h → m/s is × 5/18

$$72 \times \frac{5}{18} = 4 \times 5 = 20 \text{ m/s}$$

*(Divide by 18 first: 72 ÷ 18 = 4, then × 5 = 20.)*

**Answer: (c) 20 m/s**

---

**Q3. Convert 25 m/s to km/h. → (c) 90 km/h**

**Formula used:** m/s → km/h is × 18/5

$$25 \times \frac{18}{5} = 5 \times 18 = 90 \text{ km/h}$$

**Answer: (c) 90 km/h**

---

**Q4. 5 km/h for 3 hours. Distance? → (b) 15 km**

$$D = S \times T = 5 \times 3 = 15 \text{ km}$$

**Answer: (b) 15 km**

---

**Q5. 180 km at 45 km/h. Time? → (c) 4 hours**

$$T = \frac{D}{S} = \frac{180}{45} = 4 \text{ hours}$$

**Answer: (c) 4 hours**

---

**Q6. 200 m train crosses a pole in 10 s. Speed in km/h? → (c) 72 km/h**

**Step 1 — Crossing a pole ⇒ distance = train length.**
$$S = \frac{200}{10} = 20 \text{ m/s}$$

**Step 2 — Convert.**
$$20 \times \frac{18}{5} = 72 \text{ km/h}$$

**Answer: (c) 72 km/h**

---

**Q7. Boat 12 km/h, stream 3 km/h. Downstream speed? → (c) 15 km/h**

**Formula used:** Downstream = b + s

$$12 + 3 = 15 \text{ km/h}$$

**Answer: (c) 15 km/h**

---

**Q8. Same data — upstream speed? → (a) 9 km/h**

**Formula used:** Upstream = b − s

$$12 - 3 = 9 \text{ km/h}$$

**Answer: (a) 9 km/h**

---

**Q9. 300 km in 5 hours. Speed in m/s? → (b) 16⅔ m/s**

**Step 1 — Speed in km/h.**
$$\frac{300}{5} = 60 \text{ km/h}$$

**Step 2 — Convert.**
$$60 \times \frac{5}{18} = \frac{300}{18} = \frac{50}{3} = 16\tfrac{2}{3} \text{ m/s}$$

**Answer: (b) 16⅔ m/s**

---

**Q10. 30 km in 2.5 hours. Speed? → (b) 12 km/h**

$$\frac{30}{2.5} = 12 \text{ km/h}$$

**Answer: (b) 12 km/h**

---

**Q11. Towards each other at 40 and 60 km/h. Relative speed? → (d) 100 km/h**

**Rule:** opposite directions ⇒ speeds **add**.

$$40 + 60 = 100 \text{ km/h}$$

**Answer: (d) 100 km/h**

---

**Q12. Same direction at 70 and 40 km/h. Relative speed? → (a) 30 km/h**

**Rule:** same direction ⇒ speeds **subtract**.

$$70 - 40 = 30 \text{ km/h}$$

**Answer: (a) 30 km/h**

---

**Q13. 60 km/h for 3 hours; how long at 90 km/h? → (b) 2 hours**

**Step 1 — Find the distance.**
$$60 \times 3 = 180 \text{ km}$$

**Step 2 — New time.**
$$\frac{180}{90} = 2 \text{ hours}$$

**⚡ Ratio shortcut:** speed ratio 60 : 90 = 2 : 3 ⇒ time ratio 3 : 2 ⇒ new time = 3 × (2/3) = 2 hours ✓

**Answer: (b) 2 hours**

---

**Q14. 150 m train crosses a 250 m platform in 20 s. Speed? → (c) 72 km/h**

**Step 1 — Total distance = train + platform.**
$$150 + 250 = 400 \text{ m}$$

**Step 2 — Speed in m/s.**
$$\frac{400}{20} = 20 \text{ m/s}$$

**Step 3 — Convert.**
$$20 \times \frac{18}{5} = 72 \text{ km/h}$$

**Answer: (c) 72 km/h**

---

**Q15. 120 km in 1.5 hours. Speed? → (c) 80 km/h**

$$\frac{120}{1.5} = 80 \text{ km/h}$$

**Answer: (c) 80 km/h**

---

**Q16. 20 km downstream in 2 hours. Downstream speed? → (b) 10 km/h**

$$\frac{20}{2} = 10 \text{ km/h}$$

**Answer: (b) 10 km/h**

---

**Q17. Speed doubled ⇒ time becomes? → (b) Halved**

**Concept:** for a fixed distance, speed and time are inversely proportional.

$$S \times 2 \implies T \times \frac{1}{2}$$

**Answer: (b) Halved**

---

**Q18. 12 km in 90 minutes. Speed in km/h? → (c) 8 km/h**

**Step 1 — Convert time to hours.**
$$90 \text{ min} = 1.5 \text{ hours}$$

**Step 2 — Compute.**
$$\frac{12}{1.5} = 8 \text{ km/h}$$

**Answer: (c) 8 km/h**

---

**Q19. Still water 10 km/h, downstream 14 km/h. Stream? → (c) 4 km/h**

**Formula used:** Downstream = b + s

$$10 + s = 14 \implies s = 4 \text{ km/h}$$

**Answer: (c) 4 km/h**

---

**Q20. Train at 54 km/h crosses a pole in 12 s. Length? → (c) 180 m**

**Step 1 — Convert the speed.**
$$54 \times \frac{5}{18} = 15 \text{ m/s}$$

**Step 2 — Crossing a pole ⇒ distance = train length.**
$$L = 15 \times 12 = 180 \text{ m}$$

**Answer: (c) 180 m**

---

### 🟡 MEDIUM — Solutions 21–40

---

**Q21. 40 km/h out, 60 km/h back. Average speed? → (b) 48 km/h**

**Formula used:** Equal distances ⇒ harmonic mean = 2uv/(u+v)

$$\frac{2 \times 40 \times 60}{40 + 60} = \frac{4800}{100} = 48 \text{ km/h}$$

**Verification.** Let the one-way distance be 120 km.
$$T_{\text{out}} = 3 \text{ h}, \qquad T_{\text{back}} = 2 \text{ h}$$
$$\text{Average} = \frac{240}{5} = 48 \text{ km/h} \checkmark$$

> **Trap:** answering 50 km/h. He spends 3 hours at 40 km/h but only 2 at 60 km/h, so the average is pulled below the midpoint.

**Answer: (b) 48 km/h**

---

**Q22. 120 m train passes a man walking at 6 km/h (opposite) in 6 s. Train's speed? → (c) 66 km/h**

**Step 1 — A man has no length ⇒ distance = train length.**
$$S_{\text{rel}} = \frac{120}{6} = 20 \text{ m/s}$$

**Step 2 — Convert to km/h.**
$$20 \times \frac{18}{5} = 72 \text{ km/h}$$

**Step 3 — Opposite directions ⇒ relative speed is the SUM.**
$$S_{\text{train}} + 6 = 72$$
$$S_{\text{train}} = 66 \text{ km/h}$$

> **If the man walked in the same direction**, the answer would be 72 + 6 = 78 km/h. Direction changes the sign.

**Answer: (c) 66 km/h**

---

**Q23. Trains 100 m and 150 m, opposite directions at 54 and 36 km/h. Crossing time? → (b) 10 s**

**Step 1 — Relative speed (opposite ⇒ add).**
$$54 + 36 = 90 \text{ km/h}$$

**Step 2 — Convert to m/s.**
$$90 \times \frac{5}{18} = 25 \text{ m/s}$$

**Step 3 — Total distance = sum of the lengths.**
$$100 + 150 = 250 \text{ m}$$

**Step 4 — Time.**
$$\frac{250}{25} = 10 \text{ seconds}$$

**Answer: (b) 10 s**

---

**Q24. 24 km down in 3 h, up in 4 h. Boat and stream speeds? → (b) 7 km/h, 1 km/h**

**Step 1 — Compute the two effective speeds.**
$$\text{Downstream} = \frac{24}{3} = 8 \text{ km/h}$$
$$\text{Upstream} = \frac{24}{4} = 6 \text{ km/h}$$

**Step 2 — Apply the formulas.**
$$b = \frac{8 + 6}{2} = 7 \text{ km/h}$$
$$s = \frac{8 - 6}{2} = 1 \text{ km/h}$$

**Verification:** 7 + 1 = 8 ✓ and 7 − 1 = 6 ✓

**Answer: (b) 7 km/h, 1 km/h**

---

**Q25. Half at 30 km/h, half at 60 km/h. Average? → (b) 40 km/h**

**Formula used:** Equal distances ⇒ 2uv/(u+v)

$$\frac{2 \times 30 \times 60}{90} = \frac{3600}{90} = 40 \text{ km/h}$$

**Verification.** Take the total journey as 120 km (60 km each half).
$$T_1 = \frac{60}{30} = 2 \text{ h}, \qquad T_2 = \frac{60}{60} = 1 \text{ h}$$
$$\text{Average} = \frac{120}{3} = 40 \text{ km/h} \checkmark$$

**Answer: (b) 40 km/h**

---

**Q26. Train at 72 km/h crosses a 400 m platform in 30 s. Train length? → (c) 200 m**

**Step 1 — Convert the speed.**
$$72 \times \frac{5}{18} = 20 \text{ m/s}$$

**Step 2 — Total distance covered.**
$$20 \times 30 = 600 \text{ m}$$

**Step 3 — Subtract the platform.**
$$L_{\text{train}} = 600 - 400 = 200 \text{ m}$$

**Answer: (c) 200 m**

---

**Q27. 60 km at 30 km/h, then 60 km at 60 km/h. Average? → (b) 40 km/h**

**Step 1 — Compute each leg's time.**
$$T_1 = \frac{60}{30} = 2 \text{ h}, \qquad T_2 = \frac{60}{60} = 1 \text{ h}$$

**Step 2 — Apply the definition.**
$$\text{Average} = \frac{\text{Total distance}}{\text{Total time}} = \frac{120}{3} = 40 \text{ km/h}$$

**Answer: (b) 40 km/h**

---

**Q28. 12 km up in 3 h; 24 km down in 3 h. Stream speed? → (b) 2 km/h**

**Step 1 — Compute the two speeds.**
$$\text{Upstream} = \frac{12}{3} = 4 \text{ km/h}$$
$$\text{Downstream} = \frac{24}{3} = 8 \text{ km/h}$$

**Step 2 — Apply the formula.**
$$s = \frac{\text{Down} - \text{Up}}{2} = \frac{8 - 4}{2} = 2 \text{ km/h}$$

*(And the boat's still-water speed = (8 + 4)/2 = 6 km/h.)*

**Answer: (b) 2 km/h**

---

**Q29. 4 km/h ⇒ 8 min late; 5 km/h ⇒ 7 min early. Distance? → (c) 5 km**

**Step 1 — Find the time difference between the two journeys.**
One arrival is 8 minutes after the target time, the other 7 minutes before it:
$$8 + 7 = 15 \text{ minutes} = \frac{1}{4} \text{ hour}$$

**Step 2 — Set up the equation.**
$$\frac{d}{4} - \frac{d}{5} = \frac{1}{4}$$

**Step 3 — Simplify the left side.**
$$\frac{5d - 4d}{20} = \frac{d}{20}$$

**Step 4 — Solve.**
$$\frac{d}{20} = \frac{1}{4} \implies d = 5 \text{ km}$$

**Verification:**
- At 4 km/h: 5/4 = 1.25 h = 75 minutes
- At 5 km/h: 5/5 = 1 h = 60 minutes
- Difference = 15 minutes ✓ (target time = 67 minutes; 75 is 8 late ✓, 60 is 7 early ✓)

> **Critical:** the gap is late + early, **not** late − early.

**Answer: (c) 5 km**

---

**Q30. 300 km apart, towards each other at 40 and 60 km/h. Meeting time? → (c) 3 hours**

**Step 1 — Relative speed.**
$$40 + 60 = 100 \text{ km/h}$$

**Step 2 — Time to close the gap.**
$$\frac{300}{100} = 3 \text{ hours}$$

**Check:** in 3 hours, train 1 covers 120 km and train 2 covers 180 km. Total = 300 km ✓

**Answer: (c) 3 hours**

---

**Q31. 180 m train crosses a platform in 20 s and a pole in 9 s. Platform length? → (c) 220 m**

**Step 1 — Use the pole crossing to find the speed.**
Crossing a pole ⇒ distance = train length:
$$S = \frac{180}{9} = 20 \text{ m/s}$$

**Step 2 — Use the platform crossing to find the total distance.**
$$D = 20 \times 20 = 400 \text{ m}$$

**Step 3 — Subtract the train's length.**
$$L_{\text{platform}} = 400 - 180 = 220 \text{ m}$$

**⚡ Shortcut:** $L_{\text{platform}} = S \times (t_2 - t_1) = 20 \times (20 - 9) = 220$ m ✓

**Answer: (c) 220 m**

---

**Q32. 30 km down in 2 h, 18 km up in 3 h. Still-water speed? → (c) 10.5 km/h**

**Step 1 — Compute the two speeds.**
$$\text{Downstream} = \frac{30}{2} = 15 \text{ km/h}$$
$$\text{Upstream} = \frac{18}{3} = 6 \text{ km/h}$$

**Step 2 — Half-sum.**
$$b = \frac{15 + 6}{2} = \frac{21}{2} = 10.5 \text{ km/h}$$

*(Stream = (15 − 6)/2 = 4.5 km/h.)*

**Verification:** 10.5 + 4.5 = 15 ✓ and 10.5 − 4.5 = 6 ✓

**Answer: (c) 10.5 km/h**

---

**Q33. 60 km/h for 2 h, then 80 km/h for 3 h. Average? → (c) 72 km/h**

**Step 1 — Distance in each phase.**
$$D_1 = 60 \times 2 = 120 \text{ km}$$
$$D_2 = 80 \times 3 = 240 \text{ km}$$

**Step 2 — Totals.**
$$D_{\text{total}} = 360 \text{ km}, \qquad T_{\text{total}} = 5 \text{ h}$$

**Step 3 — Average speed.**
$$\frac{360}{5} = 72 \text{ km/h}$$

> **Note:** here the *times* are given (not the distances), so the answer is a time-weighted mean. It lies above the midpoint of 70 because more time was spent at the higher speed.

**Answer: (c) 72 km/h**

---

**Q34. Same direction at 50 and 65 km/h. When are they 45 km apart? → (c) 3 hours**

**Step 1 — Relative speed (same direction ⇒ subtract).**
$$65 - 50 = 15 \text{ km/h}$$

**Step 2 — Time to open a 45 km gap.**
$$\frac{45}{15} = 3 \text{ hours}$$

**Check:** in 3 hours they cover 150 km and 195 km ⇒ gap = 45 km ✓

**Answer: (c) 3 hours**

---

**Q35. Boat 15 km/h; upstream takes twice as long as downstream. Stream speed? → (c) 5 km/h**

**Step 1 — Convert the time condition into a speed condition.**
For the same distance, time is inversely proportional to speed. If the upstream trip takes **twice** as long, the downstream speed must be **twice** the upstream speed:
$$b + s = 2(b - s)$$

**Step 2 — Substitute b = 15.**
$$15 + s = 2(15 - s)$$
$$15 + s = 30 - 2s$$

**Step 3 — Solve.**
$$3s = 15 \implies s = 5 \text{ km/h}$$

**Verification:** Downstream = 20 km/h, Upstream = 10 km/h.
For a 20 km trip: down takes 1 h, up takes 2 h — exactly twice ✓

**Answer: (c) 5 km/h**

---

**Q36. 250 m train at 90 km/h crosses a bridge in 30 s. Bridge length? → (c) 500 m**

**Step 1 — Convert the speed.**
$$90 \times \frac{5}{18} = 25 \text{ m/s}$$

**Step 2 — Total distance.**
$$25 \times 30 = 750 \text{ m}$$

**Step 3 — Subtract the train's length.**
$$750 - 250 = 500 \text{ m}$$

**Answer: (c) 500 m**

---

**Q37. 600 km total; train at 100 km/h, car at 60 km/h; total 8 hours. Train distance? → (c) 300 km**

**Step 1 — Define the variable.**
Let the train distance be *x* km. Then the car distance is (600 − x) km.

**Step 2 — Write the time equation.**
$$\frac{x}{100} + \frac{600 - x}{60} = 8$$

**Step 3 — Clear denominators (multiply by 300).**
$$3x + 5(600 - x) = 2400$$
$$3x + 3000 - 5x = 2400$$
$$-2x = -600$$
$$x = 300 \text{ km}$$

**Verification:**
- By train: 300/100 = 3 hours
- By car: 300/60 = 5 hours
- Total = 8 hours ✓ and total distance = 600 km ✓

**Answer: (c) 300 km**

---

**Q38. Trains 120 m and 180 m, same direction at 72 and 54 km/h. Overtaking time? → (c) 60 s**

**Step 1 — Relative speed (same direction ⇒ subtract).**
$$72 - 54 = 18 \text{ km/h}$$

**Step 2 — Convert to m/s.**
$$18 \times \frac{5}{18} = 5 \text{ m/s}$$

**Step 3 — Total distance (both lengths, even for overtaking).**
$$120 + 180 = 300 \text{ m}$$

**Step 4 — Time.**
$$\frac{300}{5} = 60 \text{ seconds}$$

> **Note:** to overtake *completely*, the faster train's rear must clear the slower train's front — so the relative displacement is the sum of both lengths, exactly as in the head-on case. Only the *relative speed* differs.

**Answer: (c) 60 s**

---

**Q39. 5 hours; 2 km/h faster ⇒ 4 hours. Distance? → (c) 40 km**

**Step 1 — Let the original speed be *v* km/h.**
The distance is the same in both scenarios:
$$5v = 4(v + 2)$$

**Step 2 — Solve.**
$$5v = 4v + 8$$
$$v = 8 \text{ km/h}$$

**Step 3 — Compute the distance.**
$$D = 5 \times 8 = 40 \text{ km}$$

**Verification:** at 10 km/h, 40/10 = 4 hours ✓

**Answer: (c) 40 km**

---

**Q40. 16 up + 24 down in 6 h; 12 up + 36 down in 6 h. Still-water speed? → (c) 8 km/h**

**Step 1 — Substitute to linearise.**
Let *a* = 1/(upstream speed) and *b* = 1/(downstream speed).
$$16a + 24b = 6 \qquad \text{...(i)}$$
$$12a + 36b = 6 \qquad \text{...(ii)}$$

**Step 2 — Eliminate *a*.**
Multiply (i) by 3 and (ii) by 4:
$$48a + 72b = 18 \qquad \text{...(iii)}$$
$$48a + 144b = 24 \qquad \text{...(iv)}$$

**Step 3 — Subtract (iii) from (iv).**
$$72b = 6 \implies b = \frac{1}{12} \implies \text{Downstream} = 12 \text{ km/h}$$

**Step 4 — Back-substitute into (i).**
$$16a + 2 = 6 \implies a = \frac{1}{4} \implies \text{Upstream} = 4 \text{ km/h}$$

**Step 5 — Still-water speed.**
$$b_{\text{boat}} = \frac{12 + 4}{2} = 8 \text{ km/h}$$

**Verification of (ii):** 12/4 + 36/12 = 3 + 3 = 6 hours ✓

**Answer: (c) 8 km/h**

---

### 🔴 HARD — Solutions 41–50

---

**Q41. Crosses a man in 8 s; crosses a 264 m platform in 20 s. Train length? → (c) 176 m**

**Step 1 — Set up both crossings.**
Let the train's length be *L* metres and its speed *v* m/s.

- Crossing a man (a point object): distance = *L*
$$L = 8v \qquad \text{...(i)}$$

- Crossing the platform: distance = *L* + 264
$$L + 264 = 20v \qquad \text{...(ii)}$$

**Step 2 — Substitute (i) into (ii).**
$$8v + 264 = 20v$$
$$12v = 264$$
$$v = 22 \text{ m/s}$$

**Step 3 — Find the length.**
$$L = 8 \times 22 = 176 \text{ m}$$

**⚡ Direct shortcut:**
$$v = \frac{L_{\text{platform}}}{t_2 - t_1} = \frac{264}{20 - 8} = 22 \text{ m/s}, \qquad L = v \times t_1 = 176 \text{ m}$$

**Verification:**
- Man: 176/22 = 8 s ✓
- Platform: (176 + 264)/22 = 440/22 = 20 s ✓
- Speed in km/h: 22 × 18/5 = **79.2 km/h**

**Answer: (c) 176 m**

---

**Q42. Trains at 60 and 90 km/h; one travels 120 km more when they meet. Distance AB? → (c) 600 km**

**Step 1 — Key insight: both trains travel for the SAME time.**
Since D = S × T with T equal, the distances are in the ratio of the speeds:
$$\frac{D_1}{D_2} = \frac{60}{90} = \frac{2}{3}$$

**Step 2 — Express in parts.**
$$D_1 = 2k, \qquad D_2 = 3k$$

**Step 3 — Apply the difference condition.**
$$3k - 2k = k = 120 \text{ km}$$

**Step 4 — Total distance.**
$$D_1 + D_2 = 5k = 5 \times 120 = 600 \text{ km}$$

**Verification:**
- Meeting time = 600/(60 + 90) = 4 hours
- Train 1 covers 60 × 4 = 240 km
- Train 2 covers 90 × 4 = 360 km
- Difference = 120 km ✓ · Total = 600 km ✓

**Answer: (c) 600 km**

---

**Q43. Rows 8 km/h in still water; stream 2 km/h; round trip takes 3 h 12 min. Distance? → (b) 12 km**

**Step 1 — Compute the two effective speeds.**
$$\text{Downstream} = 8 + 2 = 10 \text{ km/h}$$
$$\text{Upstream} = 8 - 2 = 6 \text{ km/h}$$

**Step 2 — Convert the total time to hours.**
$$3 \text{ h } 12 \text{ min} = 3 + \frac{12}{60} = 3.2 \text{ hours}$$

**Step 3 — Write the round-trip equation.**
Let the one-way distance be *d* km:
$$\frac{d}{10} + \frac{d}{6} = 3.2$$

**Step 4 — Combine the fractions.**
$$d\left(\frac{1}{10} + \frac{1}{6}\right) = d\left(\frac{3 + 5}{30}\right) = \frac{8d}{30} = \frac{4d}{15}$$

**Step 5 — Solve.**
$$\frac{4d}{15} = 3.2 \implies d = \frac{3.2 \times 15}{4} = 12 \text{ km}$$

**Verification:**
- Downstream: 12/10 = 1.2 h
- Upstream: 12/6 = 2 h
- Total = 3.2 h = 3 h 12 min ✓

**Answer: (b) 12 km**

---

**Q44. At 4/5 of usual speed, 20 minutes late. Usual time? → (c) 80 min**

**Step 1 — Convert the speed change into a time change.**
Speed and time are inversely proportional for a fixed distance:
$$S \times \frac{4}{5} \implies T \times \frac{5}{4}$$

**Step 2 — Express the delay.**
$$T_{\text{new}} - T_{\text{usual}} = \frac{5}{4}T - T = \frac{T}{4}$$

**Step 3 — Set equal to the given delay.**
$$\frac{T}{4} = 20 \implies T = 80 \text{ minutes}$$

**Verification:**
- Usual time = 80 min
- At 4/5 speed: 80 × 5/4 = 100 min
- Delay = 20 min ✓

**Answer: (c) 80 min**

---

**Q45. Two men 27 km apart at 4 and 5 km/h; a dog runs between them at 10 km/h. Total dog distance? → (c) 30 km**

**Do not model the zigzag.** The only question that matters is: **how long does the dog run?**

**Step 1 — Find when the two men meet.**
They approach at a combined speed of:
$$4 + 5 = 9 \text{ km/h}$$
$$T = \frac{27}{9} = 3 \text{ hours}$$

**Step 2 — The dog runs continuously for that entire time.**
$$D_{\text{dog}} = 10 \times 3 = 30 \text{ km}$$

**Answer: (c) 30 km**

> **Why this works:** the dog's path is an infinite series of ever-shorter legs, but it never stops and never changes *speed* — only direction. Total distance = speed × total time, regardless of how convoluted the path is.
>
> **Cross-check:** in 3 hours the men cover 12 km and 15 km, meeting exactly 27 km apart ✓

---

**Q46. 400 m and 300 m trains cross in 14 s (opposite); first at 90 km/h. Second's speed? → (c) 90 km/h**

**Step 1 — Total distance to be covered.**
$$400 + 300 = 700 \text{ m}$$

**Step 2 — Relative speed.**
$$S_{\text{rel}} = \frac{700}{14} = 50 \text{ m/s}$$

**Step 3 — Convert to km/h.**
$$50 \times \frac{18}{5} = 180 \text{ km/h}$$

**Step 4 — Opposite directions ⇒ relative speed is the sum.**
$$90 + S_2 = 180 \implies S_2 = 90 \text{ km/h}$$

**Verification:** both at 90 km/h ⇒ relative 180 km/h = 50 m/s ⇒ 700/50 = 14 s ✓

**Answer: (c) 90 km/h**

---

**Q47. 60 km; 2 km/h faster saves 1 hour. Original speed? → (b) 10 km/h**

**Step 1 — Set up the time equation.**
Let the original speed be *v* km/h:
$$\frac{60}{v} - \frac{60}{v+2} = 1$$

**Step 2 — Combine the left side.**
$$\frac{60(v+2) - 60v}{v(v+2)} = \frac{120}{v(v+2)}$$

**Step 3 — Set equal to 1 and cross-multiply.**
$$\frac{120}{v(v+2)} = 1$$
$$v^2 + 2v = 120$$
$$v^2 + 2v - 120 = 0$$

**Step 4 — Factorise.**
$$(v + 12)(v - 10) = 0$$
$$v = 10 \quad \text{or} \quad v = -12$$

Speed cannot be negative, so **v = 10 km/h**.

**Verification:**
- At 10 km/h: 60/10 = 6 hours
- At 12 km/h: 60/12 = 5 hours
- Saving = 1 hour ✓

**Answer: (b) 10 km/h**

> **Faster route under time pressure:** test the options. 60/10 = 6 and 60/12 = 5 — a difference of exactly 1 hour. Done in five seconds, no quadratic required.

---

**Q48. 30 up + 44 down in 10 h; 40 up + 55 down in 13 h. Stream speed? → (b) 3 km/h**

**Step 1 — Substitute to linearise.**
Let *a* = 1/(upstream speed) and *b* = 1/(downstream speed).
$$30a + 44b = 10 \qquad \text{...(i)}$$
$$40a + 55b = 13 \qquad \text{...(ii)}$$

**Step 2 — Eliminate *a*.** LCM of 30 and 40 is 120. Multiply (i) by 4 and (ii) by 3:
$$120a + 176b = 40 \qquad \text{...(iii)}$$
$$120a + 165b = 39 \qquad \text{...(iv)}$$

**Step 3 — Subtract (iv) from (iii).**
$$11b = 1 \implies b = \frac{1}{11} \implies \text{Downstream} = 11 \text{ km/h}$$

**Step 4 — Back-substitute into (i).**
$$30a + 44 \times \frac{1}{11} = 10$$
$$30a + 4 = 10 \implies 30a = 6 \implies a = \frac{1}{5} \implies \text{Upstream} = 5 \text{ km/h}$$

**Step 5 — Stream speed.**
$$s = \frac{\text{Down} - \text{Up}}{2} = \frac{11 - 5}{2} = 3 \text{ km/h}$$

*(Boat in still water = (11 + 5)/2 = 8 km/h.)*

**Verification of (ii):** 40/5 + 55/11 = 8 + 5 = 13 hours ✓

**Answer: (b) 3 km/h**

---

**Q49. Three equal thirds at 40, 60 and 120 km/h. Average speed? → (b) 60 km/h**

**Formula used:** For three equal distances,
$$\text{Average} = \frac{3uvw}{uv + vw + wu}$$

**Step 1 — Compute the numerator.**
$$3 \times 40 \times 60 \times 120 = 3 \times 288{,}000 = 864{,}000$$

**Step 2 — Compute the denominator.**
$$(40)(60) + (60)(120) + (120)(40) = 2{,}400 + 7{,}200 + 4{,}800 = 14{,}400$$

**Step 3 — Divide.**
$$\frac{864{,}000}{14{,}400} = 60 \text{ km/h}$$

**Verification from first principles.** Let each third be 120 km (total 360 km).
$$T_1 = \frac{120}{40} = 3 \text{ h}, \quad T_2 = \frac{120}{60} = 2 \text{ h}, \quad T_3 = \frac{120}{120} = 1 \text{ h}$$
$$\text{Total time} = 6 \text{ h} \implies \text{Average} = \frac{360}{6} = 60 \text{ km/h} \checkmark$$

> **Note:** the arithmetic mean of 40, 60 and 120 is 73⅓ — offered as option (d). The harmonic mean (60) is correct because the *distances*, not the times, are equal.

**Answer: (b) 60 km/h**

---

**Q50. At 3/4 of usual speed, 20 minutes late. Usual time? → (c) 60 min**

**Step 1 — Convert the speed change into a time change.**
$$S \times \frac{3}{4} \implies T \times \frac{4}{3}$$

**Step 2 — Express the delay.**
$$\frac{4}{3}T - T = \frac{T}{3}$$

**Step 3 — Solve.**
$$\frac{T}{3} = 20 \implies T = 60 \text{ minutes}$$

**Verification:**
- Usual time = 60 min
- At 3/4 speed: 60 × 4/3 = 80 min
- Delay = 20 min ✓

**Answer: (c) 60 min**

> **The general result:** at *a*/*b* of the usual speed, the delay is $\left(\frac{b}{a} - 1\right)T$. Memorise the common cases: 3/4 ⇒ T/3, 4/5 ⇒ T/4, 5/6 ⇒ T/5, 2/3 ⇒ T/2.

---

## 8. Quick Revision Sheet

> **One page. Read 48 hours after study, and again the night before the test.**

### Core

```
D = S × T          S = D/T          T = D/S

km/h → m/s :  × 5/18          m/s → km/h :  × 18/5

  18 km/h =  5 m/s      72 km/h = 20 m/s
  36 km/h = 10 m/s      90 km/h = 25 m/s
  54 km/h = 15 m/s     108 km/h = 30 m/s
```

### Inverse relation (fixed distance)

```
S₁T₁ = S₂T₂        Speed ratio a:b  →  Time ratio b:a

×2 speed   → time halved
+25% speed → time −20%       (5:4 → 4:5)
+50% speed → time −33⅓%      (3:2 → 2:3)
−20% speed → time +25%       (4:5 → 5:4)
```

### Average speed

```
Equal DISTANCES, 2 speeds  →  2uv/(u+v)        ← harmonic
Equal DISTANCES, 3 speeds  →  3uvw/(uv+vw+wu)
Equal TIMES                →  (u+v)/2          ← arithmetic
General                    →  Total D / Total T

40 & 60 → 48     30 & 60 → 40     15 & 10 → 12     20 & 30 → 24
```

### Relative speed

```
Opposite / towards each other  →  S₁ + S₂
Same direction                 →  |S₁ − S₂|

Time to meet/overtake = (gap + lengths) / relative speed
Two bodies meeting: distances are in the RATIO OF SPEEDS
```

### Trains

```
Crossing a POLE / MAN / SIGNAL   →  distance = L_train
Crossing a PLATFORM / BRIDGE     →  distance = L_train + L_platform
Crossing ANOTHER TRAIN           →  distance = L₁ + L₂
   (both for head-on AND for overtaking — only the SPEED differs)

Pole in t₁, platform in t₂:
    Speed = L_platform / (t₂ − t₁)      L_train = Speed × t₁
```

### Boats & Streams

```
Downstream = b + s          Upstream = b − s
b = (Down + Up)/2           s = (Down − Up)/2

Round-trip average = (b² − s²)/b
Up takes k× as long as down  →  b + s = k(b − s)

Two-journey problems: substitute a = 1/u, b = 1/d  →  LINEAR equations
```

### Special patterns

```
FRACTIONAL SPEED  —  at a/b of usual speed, t late:
    T_usual = a·t / (b − a)
    3/4 → T/3     4/5 → T/4     5/6 → T/5     2/3 → T/2

LATE & EARLY  —  u km/h is p late, v km/h is q early:
    d/u − d/v = (p + q)/60        ← SUM, not difference

DOG BETWEEN WALKERS  —  find the MEETING TIME, then dog distance = speed × time
```

### Sanity checks

```
✓ Average speed (equal distances) < arithmetic mean, always
✓ Downstream > still water > upstream
✓ Platform crossing takes longer than pole crossing
✓ Same-direction relative speed < opposite-direction
✓ Speed up ⇒ time down. If not, recheck.
```

---

## 9. Common Mistakes

| # | Mistake | Example | Correction |
|---|---|---|---|
| 1 | **Mixing units** | 72 km/h with metres and seconds | Convert first: 72 km/h = 20 m/s |
| 2 | **Arithmetic mean for average speed** | 40 & 60 ⇒ 50 km/h | 2uv/(u+v) = 48 km/h |
| 3 | **Pole crossing includes platform** | Adding a length for a pole | A pole is a point — distance = train length only |
| 4 | **Overtaking uses only one length** | 120 m train overtakes ⇒ 120 m | Both lengths: 120 + 180 = 300 m |
| 5 | **Wrong relative-speed sign** | Same direction ⇒ add | Same direction ⇒ **subtract** |
| 6 | **Late/early subtracted** | 8 late, 7 early ⇒ 1 minute | The gap is 8 + 7 = **15 minutes** |
| 7 | **Boat formulas flipped** | b = (Down − Up)/2 | b = (Down + Up)/2; s = (Down − Up)/2 |
| 8 | **Fractional speed inverted** | 4/5 speed ⇒ time × 4/5 | Time × **5/4** (inverse) |
| 9 | **Time in minutes used as hours** | 90 minutes entered as 90 | Convert: 90 min = 1.5 h |
| 10 | **Modelling the dog's zigzag** | Summing an infinite series | Find the meeting time; distance = speed × time |
| 11 | **Non-linear boat equations attempted directly** | Solving 16/(b−s) + 24/(b+s) = 6 | Substitute a = 1/u, b = 1/d |
| 12 | **Round-trip distance halved/doubled wrongly** | Using d for total when d is one-way | Read whether *d* is one-way or the round trip |

---

## Practice Answer Key

| Q | Ans | Q | Ans | Q | Ans | Q | Ans | Q | Ans |
|---|---|---|---|---|---|---|---|---|---|
| 1 | c | 11 | d | 21 | b | 31 | c | 41 | c |
| 2 | c | 12 | a | 22 | c | 32 | c | 42 | c |
| 3 | c | 13 | b | 23 | b | 33 | c | 43 | b |
| 4 | b | 14 | c | 24 | b | 34 | c | 44 | c |
| 5 | c | 15 | c | 25 | b | 35 | c | 45 | c |
| 6 | c | 16 | b | 26 | c | 36 | c | 46 | c |
| 7 | c | 17 | b | 27 | b | 37 | c | 47 | b |
| 8 | a | 18 | c | 28 | b | 38 | c | 48 | b |
| 9 | b | 19 | c | 29 | c | 39 | c | 49 | b |
| 10 | b | 20 | c | 30 | c | 40 | c | 50 | c |

**Scoring guide:** 45+/50 → strong. 35–44 → solid; drill unit conversion and train-length rules until automatic. Below 35 → re-read Sections 2.2, 2.6 and 2.7, then redo the Medium set.

---

**⬅️ Back:** [Topic 5 — Time & Work](05-time-and-work.md) · **➡️ Next:** [Topic 7 — Simple & Compound Interest](07-simple-compound-interest.md)
