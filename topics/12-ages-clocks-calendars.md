# Topic 12 — Ages, Clocks & Calendars

### EY Placement Aptitude Handbook · Priority Rank #21 · 🟡 Medium

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

**Weightage:** 3–4% of the quantitative section — roughly **0–1 questions**, and clocks/calendars sometimes appear in the *reasoning* section instead.

**Why cover it anyway:** all three sub-topics are **fully mechanical once learned**. There are exactly three ideas here — the age-equation template, the 5.5°-per-minute clock rule, and the odd-days calendar method. Learn those three and every question in the topic becomes a 30-second exercise. It is the cheapest set of marks in the handbook after Mensuration.

**Question styles reported:**

| Sub-topic | Typical shape |
|---|---|
| **Ages** | "Father is 4 times the son; after 20 years, twice" |
| | "Ratio 4 : 5 now, 5 : 6 in five years" |
| | "Sum of ages 60; six years ago the father was 5 times" |
| **Clocks** | "Angle between the hands at 4:20" |
| | "When do the hands coincide between 3 and 4?" |
| | "A clock gains 5 minutes per hour" |
| **Calendars** | "What day was 15 August 1947?" |
| | "If 1 Jan 2024 is a Monday, what is 1 Jan 2025?" |
| | "In which year can the 2018 calendar be reused?" |

---

## 2. Core Concepts — PART A: AGES

### 2.1 The universal age template

Every age problem follows the same three-step structure:

```
1.  Represent the PRESENT ages with ONE variable
        (use the ratio if given: 4x and 5x)
2.  Shift EVERY age by the same amount for past/future
        "after t years"  →  add t to each
        "t years ago"    →  subtract t from each
3.  Write the equation from the second condition and solve
```

**The single most important rule:** the **difference between two people's ages never changes**. If A is 20 years older than B today, A was 20 years older ten years ago and will be 20 years older in thirty years.

> Father is 4 times the son; after 20 years he will be twice as old.
> $$4s + 20 = 2(s + 20) \implies 4s + 20 = 2s + 40 \implies s = 10, \; f = 40$$
> *Check the invariant:* difference = 30 now, and 60 vs 30 after 20 years — still 30 ✓

### 2.2 Ratio-based age problems

> Present ratio 4 : 5; five years hence it becomes 5 : 6.

$$\frac{4x + 5}{5x + 5} = \frac{5}{6}$$
$$6(4x+5) = 5(5x+5) \implies 24x + 30 = 25x + 25 \implies x = 5$$

Present ages: **20 and 25**.

> **Always use ONE variable.** Writing "let the ages be a and b" doubles the algebra and creates room for sign errors. The ratio hands you the single variable for free.

### 2.3 Useful age shortcuts

| Statement | Equation |
|---|---|
| A is *n* times B | $A = nB$ |
| A is *n* years older than B | $A = B + n$ |
| After *t* years, A will be *m* times B | $A + t = m(B + t)$ |
| *t* years ago, A was *m* times B | $A - t = m(B - t)$ |
| Sum of present ages = S | $A + B = S$ |
| Product of ages = P (with a ratio) | $ax \cdot bx = P$ |

**Average-of-a-family problems** need care: when going back in time, the *number of members may change*.

> A family of 5 averages 30 years; the youngest is 6.
> **Six years ago the family had only 4 members**, each 6 years younger:
> Total now = 150; excluding the youngest = 144; six years ago = 144 − 4(6) = 120
> Average then = 120/4 = **30 years** — not 24.

---

## 3. Core Concepts — PART B: CLOCKS

### 3.1 The two hand speeds (everything follows from these)

| Hand | Full revolution | Speed |
|---|---|---|
| **Minute hand** | 60 minutes | **6° per minute** |
| **Hour hand** | 12 hours = 720 minutes | **0.5° per minute** (30° per hour) |

$$\boxed{\text{Relative speed} = 6 - 0.5 = 5.5° \text{ per minute}}$$

**The minute hand gains 5.5° on the hour hand every minute.** Every clock question is an application of this one number.

### 3.2 ⭐ The angle formula

$$\boxed{\theta = \left|30H - 5.5M\right|}$$

where *H* is the hour and *M* the minutes past the hour.

If the result exceeds 180°, subtract it from 360° to get the smaller angle.

**Derivation:**
- Hour hand position from 12 o'clock: 30H + 0.5M degrees
- Minute hand position: 6M degrees
- Difference: |30H + 0.5M − 6M| = |30H − 5.5M| ∎

**Worked examples:**

> **At 4:20:** |30(4) − 5.5(20)| = |120 − 110| = **10°**
> **At 3:30:** |90 − 165| = **75°**
> **At 7:20:** |210 − 110| = **100°**
> **At 9:00:** |270 − 0| = 270° → 360 − 270 = **90°**

### 3.3 Standard hand positions

$$\text{Hands COINCIDE (0°)} \implies 30H = 5.5M \implies M = \frac{60H}{11}$$

$$\text{Hands OPPOSITE (180°)} \implies |30H - 5.5M| = 180$$

$$\text{Hands at RIGHT ANGLES (90°)} \implies |30H - 5.5M| = 90$$

> **Coincidence between 3 and 4 o'clock:**
> $$M = \frac{60 \times 3}{11} = \frac{180}{11} = 16\tfrac{4}{11} \text{ minutes}$$
> So at **3:16 4/11**.

**Alternative reasoning for coincidences:** at H o'clock, the hour hand is 30H degrees ahead. The minute hand closes that gap at 5.5°/min, so the time to catch up is 30H/5.5 minutes — the same formula.

### 3.4 Frequency counts (memorise)

| Event | In 12 hours | In 24 hours |
|---|---|---|
| Hands **coincide** | 11 | 22 |
| Hands are **opposite** | 11 | 22 |
| Hands are in a **straight line** (0° or 180°) | 22 | 44 |
| Hands at **right angles** | 22 | 44 |

> **Why 11 and not 12?** The hands coincide once roughly every 65 5/11 minutes, not every 60. Over 12 hours there are only 11 such meetings — between 11 o'clock and 1 o'clock there is a single coincidence (at 12:00), not two.

### 3.5 Faulty clocks

**A clock gaining or losing time:**

$$\text{Total error} = \text{Rate of error} \times \text{Number of periods}$$

> A clock gains 5 minutes per hour, set correctly at 12 noon. At 6 pm (true time):
> Gain = 5 × 6 = 30 minutes ⇒ the clock shows **6:30 pm**.

> A clock loses 10 minutes per 24 hours, set right at noon Monday. At noon the following Monday:
> Loss = 10 × 7 = 70 minutes ⇒ the clock shows **10:50 am**.

**Correct-time interval:** if a clock gains *g* minutes in a period during which the true clock advances *T*:
$$\text{Clock's reading} = T + g \quad \text{(gaining)} \qquad T - g \quad \text{(losing)}$$

---

## 4. Core Concepts — PART C: CALENDARS

### 4.1 Odd days — the whole method

An **odd day** is the remainder when a number of days is divided by 7.

$$\text{Odd days} = \text{Total days} \bmod 7$$

Everything in calendar work reduces to counting odd days.

| Period | Days | Odd days |
|---|---|---|
| Ordinary year | 365 = 52×7 + **1** | **1** |
| Leap year | 366 = 52×7 + **2** | **2** |
| 100 years | 76 ordinary + 24 leap | **5** |
| 200 years | — | **3** |
| 300 years | — | **1** |
| 400 years | — | **0** |

**Derivation of the 100-year figure:** in any century there are 24 leap years (not 25, because the century year itself is usually not a leap year).
$$76(1) + 24(2) = 76 + 48 = 124 \implies 124 \bmod 7 = 5 \; ∎$$

The 400-year cycle giving 0 odd days is why **the calendar repeats exactly every 400 years**.

### 4.2 Leap year rules

```
Divisible by 4        →  leap year
   EXCEPT century years (divisible by 100)
      UNLESS also divisible by 400  →  leap year
```

| Year | Leap? | Reason |
|---|---|---|
| 2024 | ✓ | Divisible by 4, not a century |
| 2023 | ✗ | Not divisible by 4 |
| 1900 | ✗ | Century, not divisible by 400 |
| 2000 | ✓ | Century **and** divisible by 400 |
| 2100 | ✗ | Century, not divisible by 400 |

### 4.3 Day codes

$$0 = \text{Sunday}, \; 1 = \text{Monday}, \; 2 = \text{Tuesday}, \; 3 = \text{Wednesday}, \; 4 = \text{Thursday}, \; 5 = \text{Friday}, \; 6 = \text{Saturday}$$

### 4.4 Finding the day for any date — the full procedure

```
Step 1:  Take the COMPLETED years before the given year.
Step 2:  Break them into centuries + remainder.
             1600 → 0 odd days
             1700 → 5 · 1800 → 3 · 1900 → 1 · 2000 → 0
Step 3:  For the remaining years, count leap and ordinary years:
             odd days = 2(leaps) + 1(ordinaries),  then mod 7
Step 4:  Add the days elapsed in the target year up to the date.
Step 5:  Total the odd days, take mod 7, and read off the day code.
```

**Days in each month (for Step 4):**

| Month | Days | Cumulative (non-leap) |
|---|---|---|
| Jan | 31 | 31 |
| Feb | 28 (29) | 59 |
| Mar | 31 | 90 |
| Apr | 30 | 120 |
| May | 31 | 151 |
| Jun | 30 | 181 |
| Jul | 31 | 212 |
| Aug | 31 | 243 |
| Sep | 30 | 273 |
| Oct | 31 | 304 |
| Nov | 30 | 334 |
| Dec | 31 | 365 |

> **The knuckle mnemonic:** knuckles are 31-day months, dips are 30-day months (February excepted). Jan(k) Feb(d) Mar(k) Apr(d) May(k) Jun(d) Jul(k) — then restart at the first knuckle — Aug(k) Sep(d) Oct(k) Nov(d) Dec(k).

### 4.5 Same-day shortcuts

$$\text{Same date next year} = \text{today's day} + 1 \quad \text{(if the intervening year is ordinary)}$$
$$\text{Same date next year} = \text{today's day} + 2 \quad \text{(if the intervening period contains 29 February)}$$

> 1 Jan 2024 is a Monday. 2024 is a leap year (its 29 Feb lies between the two dates), so 1 Jan 2025 = Monday + 2 = **Wednesday**.

### 4.6 Calendar repetition

A year's calendar can be reused when the total odd days between the two years is a multiple of 7 **and** both years are of the same type (both ordinary, or both leap).

| Year type | Typically repeats after |
|---|---|
| Ordinary year following a leap year | 6 years |
| Ordinary year (other positions) | 11 years |
| Leap year | 28 years |

> The 2018 calendar can be reused in **2029** (11 years later — the odd days from 2018 through 2028 total 14, a multiple of 7, and both years are ordinary).

---

## 5. Formula Bank

| # | Concept | Formula |
|---|---|---|
| 1 | Age after *t* years | $A + t$ |
| 2 | Age *t* years ago | $A - t$ |
| 3 | Age difference | **Constant over time** |
| 4 | "After *t*, A is *m* times B" | $A + t = m(B+t)$ |
| 5 | "*t* ago, A was *m* times B" | $A - t = m(B-t)$ |
| 6 | Ratio a : b now, c : d after *t* | $\dfrac{ax+t}{bx+t} = \dfrac{c}{d}$ |
| 7 | Minute-hand speed | 6° per minute |
| 8 | Hour-hand speed | 0.5° per minute (30° per hour) |
| 9 | Relative speed | **5.5° per minute** |
| 10 | **Angle between hands** | $\theta = \lvert 30H - 5.5M \rvert$ |
| 11 | Reflex correction | If θ > 180°, use 360° − θ |
| 12 | Coincidence time past H | $M = \dfrac{60H}{11}$ |
| 13 | Opposite / right angle | $\lvert 30H - 5.5M \rvert = 180$ or $90$ |
| 14 | Coincidences in 12 h / 24 h | 11 / 22 |
| 15 | Straight lines in 12 h / 24 h | 22 / 44 |
| 16 | Right angles in 12 h / 24 h | 22 / 44 |
| 17 | Faulty clock | Error = rate × number of periods |
| 18 | Odd days | Total days mod 7 |
| 19 | Ordinary / leap year odd days | 1 / 2 |
| 20 | 100 / 200 / 300 / 400 years | 5 / 3 / 1 / 0 |
| 21 | Leap year test | ÷4, except centuries unless ÷400 |
| 22 | Day codes | 0=Sun, 1=Mon, …, 6=Sat |

---

## 6. Shortcuts & Tricks

### 6.1 Ages — the one-variable discipline

```
Ratio given?          →  use ax and bx
Difference given?     →  use x and (x + d)
Sum given?            →  use x and (S − x)

NEVER introduce two independent variables when one will do.
```

**Check every answer against the invariant:** the age *difference* must be identical before and after.

### 6.2 Clocks — the 5.5 rule, three ways

```
ANGLE at H:M            →  |30H − 5.5M|      (subtract from 360 if > 180)

COINCIDE past H         →  M = 60H/11
                           3 o'clock → 180/11 = 16 4/11
                           9 o'clock → 540/11 = 49 1/11

ANY target angle θ      →  |30H − 5.5M| = θ,  solve for M
```

**Coincidence times worth recognising:**

| Between | Coincidence at |
|---|---|
| 1 and 2 | 1:05 5/11 |
| 2 and 3 | 2:10 10/11 |
| 3 and 4 | 3:16 4/11 |
| 4 and 5 | 4:21 9/11 |
| 6 and 7 | 6:32 8/11 |
| 9 and 10 | 9:49 1/11 |

### 6.3 Clocks — instant angles

| Time | Angle | Time | Angle |
|---|---|---|---|
| 12:00 | 0° | 3:00 | 90° |
| 1:00 | 30° | 6:00 | 180° |
| 2:00 | 60° | 9:00 | 90° |
| 4:00 | 120° | 3:30 | 75° |
| 5:00 | 150° | 6:30 | 15° |

> **At the half hour**, the hour hand has moved 15° past its mark — that 15° is what makes 3:30 give 75° rather than 90°.

### 6.4 Calendars — the odd-day toolkit

```
CENTURY CODES     1600/2000 → 0     1700 → 5     1800 → 3     1900 → 1

REMAINING YEARS   odd days = (number of leap years) × 2 + (ordinary years) × 1
                  then take mod 7

MONTH TOTALS      Jan 31 · Feb 28/29 · Mar 31 · Apr 30 · May 31 · Jun 30
                  Jul 31 · Aug 31 · Sep 30 · Oct 31 · Nov 30 · Dec 31

DAY CODE          0 Sun · 1 Mon · 2 Tue · 3 Wed · 4 Thu · 5 Fri · 6 Sat
```

### 6.5 Calendars — quick day shifts

```
+1 day per ORDINARY year        +2 days per LEAP year
+n days later  →  today's day + (n mod 7)

45 days after a Tuesday:  45 mod 7 = 3  →  Tuesday + 3 = FRIDAY
100 days after a Sunday:  100 mod 7 = 2 →  Sunday + 2 = TUESDAY
```

### 6.6 Sanity checks

```
✓ AGES: the difference between two ages never changes
✓ AGES: nobody's age can be negative — reject such roots
✓ CLOCKS: the angle answer must lie in [0°, 180°]
✓ CLOCKS: coincidences happen 11 times per 12 hours, not 12
✓ CALENDARS: odd days always lie in {0, 1, 2, 3, 4, 5, 6}
✓ CALENDARS: 400 years → 0 odd days, so the calendar repeats every 400 years
```

---

## 7. Solved Examples

### Example 1 — Ages with a future condition

**Q.** A man is 3 times as old as his son. Fifteen years hence he will be twice as old as his son. Find their present ages.

**Step 1 — Represent with one variable.**
Let the son's present age be *s*. Then the father's is 3*s*.

**Step 2 — Shift both ages by 15 years.**
Son: *s* + 15 · Father: 3*s* + 15

**Step 3 — Apply the future condition.**
$$3s + 15 = 2(s + 15)$$

**Step 4 — Solve.**
$$3s + 15 = 2s + 30$$
$$s = 15$$

**Step 5 — Compute both ages.**
$$\text{Son} = 15, \qquad \text{Father} = 45$$

**Verification:**
- Now: 45 = 3 × 15 ✓
- In 15 years: 60 and 30, and 60 = 2 × 30 ✓
- **Difference invariant:** 30 now, 30 later ✓

**Answer: Son 15, Father 45**

---

### Example 2 — Ages with two ratios

**Q.** The present ages of A and B are in the ratio 5 : 7. Six years hence the ratio will be 3 : 4. Find B's present age.

**Step 1 — Use the ratio to set one variable.**
$$A = 5x, \qquad B = 7x$$

**Step 2 — Ages six years hence.**
$$A = 5x + 6, \qquad B = 7x + 6$$

**Step 3 — Apply the future ratio.**
$$\frac{5x+6}{7x+6} = \frac{3}{4}$$

**Step 4 — Cross-multiply.**
$$4(5x+6) = 3(7x+6)$$
$$20x + 24 = 21x + 18$$
$$x = 6$$

**Step 5 — Find B.**
$$B = 7 \times 6 = 42 \text{ years}$$

**Verification:** Present ages 30 and 42 (ratio 5 : 7 ✓). Six years hence: 36 and 48, ratio 36 : 48 = **3 : 4** ✓

**Answer: 42 years**

---

### Example 3 — Angle between clock hands

**Q.** Find the angle between the hour and minute hands at 5:40.

**Method — the angle formula.**
$$\theta = |30H - 5.5M|$$

**Step 1 — Substitute H = 5 and M = 40.**
$$\theta = |30(5) - 5.5(40)| = |150 - 220| = |-70| = 70°$$

**Step 2 — Check whether it exceeds 180°.**
70° < 180°, so this is already the smaller angle.

**First-principles verification:**
- Minute hand at 40 minutes: 40 × 6 = **240°** from 12
- Hour hand at 5:40: 5 × 30 + 40 × 0.5 = 150 + 20 = **170°** from 12
- Difference: 240 − 170 = **70°** ✓

**Answer: 70°**

---

### Example 4 — When do the hands coincide?

**Q.** At what time between 7 and 8 o'clock will the hands of a clock coincide?

**Method 1 — The coincidence formula.**
$$M = \frac{60H}{11} = \frac{60 \times 7}{11} = \frac{420}{11} = 38\tfrac{2}{11} \text{ minutes}$$

**So the hands coincide at 7:38 2/11.**

**Method 2 — Relative-speed reasoning (worth understanding).**

At exactly 7:00, the hour hand is at 7 × 30 = **210°** and the minute hand at 0°. The minute hand must close a 210° gap.

The minute hand gains on the hour hand at **5.5° per minute**:
$$\text{Time} = \frac{210}{5.5} = \frac{2100}{55} = \frac{420}{11} = 38\tfrac{2}{11} \text{ minutes} \checkmark$$

**Verification with the angle formula:**
$$\left|30(7) - 5.5\left(\frac{420}{11}\right)\right| = \left|210 - \frac{2310}{11}\right| = |210 - 210| = 0° \checkmark$$

**Answer: 7:38 2/11 (approximately 7:38:11)**

---

### Example 5 — A faulty clock

**Q.** A clock gains 4 minutes every hour. It is set correctly at 9:00 am on Monday. What time will it show at 3:00 pm on the same day?

**Step 1 — Find the elapsed true time.**
From 9:00 am to 3:00 pm is **6 hours**.

**Step 2 — Compute the total gain.**
$$4 \text{ min/hour} \times 6 \text{ hours} = 24 \text{ minutes}$$

**Step 3 — Add the gain to the true time.**
$$3{:}00 \text{ pm} + 24 \text{ min} = \mathbf{3{:}24 \text{ pm}}$$

**Answer: 3:24 pm**

> **Sign discipline:** a **gaining** clock runs ahead ⇒ **add** the error. A **losing** clock runs behind ⇒ **subtract** it. Getting this backwards is the standard mistake in faulty-clock questions.

---

### Example 6 — Day of the week for a historical date

**Q.** What day of the week was 15 August 1947?

**Step 1 — Split the completed years.**
The date falls in 1947, so 1946 complete years have elapsed:
$$1946 = 1600 + 300 + 46$$

**Step 2 — Odd days from the century blocks.**
$$1600 \text{ years} \to 0 \text{ odd days}$$
$$300 \text{ years} \to 1 \text{ odd day}$$

**Step 3 — Odd days from the remaining 46 years.**
Leap years among 1901–1946: 1904, 1908, …, 1944 ⇒ **11 leap years**
Ordinary years: 46 − 11 = **35**
$$\text{Odd days} = 11(2) + 35(1) = 22 + 35 = 57$$
$$57 \bmod 7 = 1$$

**Step 4 — Subtotal for the completed years.**
$$0 + 1 + 1 = 2 \text{ odd days}$$

**Step 5 — Days elapsed in 1947 up to 15 August.**
*(1947 is not a leap year, so February has 28 days.)*

| Month | Days |
|---|---|
| Jan | 31 |
| Feb | 28 |
| Mar | 31 |
| Apr | 30 |
| May | 31 |
| Jun | 30 |
| Jul | 31 |
| Aug | 15 |
| **Total** | **227** |

$$227 \bmod 7 = 227 - 224 = 3 \text{ odd days}$$

**Step 6 — Total odd days and the day code.**
$$2 + 3 = 5$$
$$5 \to \textbf{Friday}$$

**Answer: Friday**

*(This is historically correct — India's Independence Day fell on a Friday.)*

---

### Example 7 — Same date, next year

**Q.** If 1 March 2024 is a Friday, what day will 1 March 2025 be?

**Step 1 — Count the days between the two dates.**
The interval runs from 1 March 2024 to 1 March 2025 — a full year.

**Step 2 — Check for 29 February in that interval.**
2024 is a leap year, but its 29 February falls **before** 1 March 2024. The next 29 February would be in 2028. So the interval contains **no leap day** and is 365 days long.

**Step 3 — Odd days.**
$$365 \bmod 7 = 1$$

**Step 4 — Advance the day.**
$$\text{Friday} + 1 = \textbf{Saturday}$$

**Answer: Saturday**

> **The trap in this question type.** It is tempting to say "2024 is a leap year, so add 2". But what matters is whether **29 February lies inside the interval**, not whether the starting year is a leap year. Since the interval begins on 1 March, it misses 2024's leap day entirely.
>
> By contrast, from **1 January 2024** to **1 January 2025** the interval *does* contain 29 February 2024 ⇒ add **2 days**.

---

### Example 8 — Family average with a changing headcount

**Q.** The average age of a family of 6 members is 25 years. The youngest member is 5 years old. What was the average age of the family at the time of the youngest member's birth?

**Step 1 — Present total age.**
$$6 \times 25 = 150 \text{ years}$$

**Step 2 — Total age of the other 5 members now.**
$$150 - 5 = 145 \text{ years}$$

**Step 3 — Roll back 5 years — but only for those 5 members.**
Five years ago, the family had **5 members** (the youngest was not born), each 5 years younger:
$$145 - 5(5) = 145 - 25 = 120 \text{ years}$$

**Step 4 — Average at that time.**
$$\frac{120}{5} = 24 \text{ years}$$

**Answer: 24 years**

> **The two traps here:**
> 1. Subtracting 5 from the present average of 25 to get 20 — wrong, because the divisor changes from 6 to 5.
> 2. Dividing by 6 instead of 5 — the youngest did not exist, so the family had only five members.

---

## 8. Practice Questions

**Instructions:** 50 questions. Easy (1–20), Medium (21–40), Hard (41–50).
Q1–20 mixed · Q21–40 mixed · Q41–50 mixed across all three sub-topics.
Full solutions in [Section 9](#9-detailed-solutions).

### 🟢 EASY (Questions 1–20)

**Q1.** A father is 3 times as old as his son. If the son is 12 years old, how old is the father?
(a) 30  (b) 33  (c) 36  (d) 42

**Q2.** The sum of the ages of A and B is 45 years. If A is 5 years older than B, find A's age.
(a) 20  (b) 22  (c) 25  (d) 28

**Q3.** Five years ago a man was 25 years old. How old will he be 10 years from now?
(a) 35  (b) 38  (c) 40  (d) 45

**Q4.** The ratio of the ages of A and B is 3 : 4. If B is 24 years old, find A's age.
(a) 16  (b) 18  (c) 20  (d) 21

**Q5.** A is 4 years older than B. If B is 16, how old is A?
(a) 18  (b) 20  (c) 22  (d) 24

**Q6.** The average age of three people is 25 years. What is the sum of their ages?
(a) 65  (b) 70  (c) 75  (d) 80

**Q7.** What is the angle between the hands of a clock at exactly 3:00?
(a) 60°  (b) 75°  (c) 90°  (d) 120°

**Q8.** How many degrees does the minute hand of a clock move in one minute?
(a) 0.5°  (b) 1°  (c) 5°  (d) 6°

**Q9.** How many degrees does the hour hand move in one hour?
(a) 6°  (b) 15°  (c) 30°  (d) 60°

**Q10.** What is the angle between the hands of a clock at exactly 6:00?
(a) 90°  (b) 120°  (c) 150°  (d) 180°

**Q11.** How many odd days are there in an ordinary year?
(a) 0  (b) 1  (c) 2  (d) 3

**Q12.** How many odd days are there in a leap year?
(a) 0  (b) 1  (c) 2  (d) 3

**Q13.** Is 2024 a leap year?
(a) Yes  (b) No  (c) Cannot be determined  (d) Only in some calendars

**Q14.** Is 1900 a leap year?
(a) Yes  (b) No  (c) Cannot be determined  (d) Only in the Julian calendar

**Q15.** Is 2000 a leap year?
(a) Yes  (b) No  (c) Cannot be determined  (d) Only in some calendars

**Q16.** How many times do the hands of a clock coincide in 12 hours?
(a) 10  (b) 11  (c) 12  (d) 22

**Q17.** How many times do the hands of a clock coincide in 24 hours?
(a) 11  (b) 22  (c) 24  (d) 44

**Q18.** A man's present age is 40 years. What was his age 12 years ago?
(a) 26  (b) 28  (c) 30  (d) 32

**Q19.** What is the angle between the hands of a clock at exactly 9:00?
(a) 60°  (b) 90°  (c) 180°  (d) 270°

**Q20.** How many days are there in 4 consecutive ordinary years?
(a) 1,456  (b) 1,460  (c) 1,461  (d) 1,464

---

### 🟡 MEDIUM (Questions 21–40)

**Q21.** A father is 4 times as old as his son. After 20 years he will be twice as old. Find the son's present age.
(a) 8  (b) 10  (c) 12  (d) 15

**Q22.** The ratio of the present ages of A and B is 4 : 5. Five years hence the ratio will be 5 : 6. Find A's present age.
(a) 16  (b) 18  (c) 20  (d) 24

**Q23.** Ten years ago the ratio of the ages of A and B was 2 : 3. Their present ratio is 3 : 4. Find B's present age.
(a) 30  (b) 35  (c) 40  (d) 45

**Q24.** The sum of the ages of a father and his son is 60 years. Six years ago the father was 5 times as old as his son. Find their present ages.
(a) 44 and 16  (b) 46 and 14  (c) 48 and 12  (d) 50 and 10

**Q25.** Find the angle between the hands of a clock at 3:30.
(a) 60°  (b) 70°  (c) 75°  (d) 90°

**Q26.** At what time between 3 and 4 o'clock will the hands of a clock coincide?
(a) 3:15  (b) 3:16 4/11  (c) 3:18 2/11  (d) 3:20

**Q27.** Find the angle between the hands of a clock at 4:20.
(a) 0°  (b) 5°  (c) 10°  (d) 20°

**Q28.** What day of the week was 15 August 1947?
(a) Wednesday  (b) Thursday  (c) Friday  (d) Saturday

**Q29.** If 1 January 2024 was a Monday, what day was 1 January 2025?
(a) Tuesday  (b) Wednesday  (c) Thursday  (d) Friday

**Q30.** How many times in 12 hours are the hands of a clock at right angles?
(a) 11  (b) 12  (c) 22  (d) 24

**Q31.** A clock gains 5 minutes every hour. If it is set correctly at 12 noon, what will it show at 6 pm on the same day?
(a) 6:15 pm  (b) 6:25 pm  (c) 6:30 pm  (d) 6:45 pm

**Q32.** The present ages of A and B are in the ratio 5 : 7. Four years hence the ratio will be 3 : 4. Find B's present age.
(a) 20  (b) 24  (c) 28  (d) 35

**Q33.** What day of the week will it be 45 days after a Tuesday?
(a) Wednesday  (b) Thursday  (c) Friday  (d) Saturday

**Q34.** Find the angle between the hands of a clock at 7:20.
(a) 90°  (b) 100°  (c) 110°  (d) 120°

**Q35.** A is twice as old as B was 2 years ago. If A is 26 years old, find B's present age.
(a) 13  (b) 14  (c) 15  (d) 16

**Q36.** If 5 March 2020 was a Thursday, what day was 5 March 2021?
(a) Thursday  (b) Friday  (c) Saturday  (d) Sunday

**Q37.** The average age of a family of 4 members is 30 years. If the youngest member is 6 years old, find the average age of the other three members.
(a) 34  (b) 36  (c) 38  (d) 40

**Q38.** At what time between 4 and 5 o'clock will the hands of a clock first be at right angles?
(a) 4:05 5/11  (b) 4:10  (c) 4:15  (d) 4:38 2/11

**Q39.** How many odd days are there in 100 years?
(a) 3  (b) 4  (c) 5  (d) 6

**Q40.** A person's age 10 years hence will be three times his age 10 years ago. Find his present age.
(a) 15  (b) 20  (c) 25  (d) 30

---

### 🔴 HARD (Questions 41–50)

**Q41.** The ages of A and B are in the ratio 3 : 5. After 9 years the ratio becomes 3 : 4. Find the sum of their present ages.
(a) 20  (b) 22  (c) 24  (d) 28

**Q42.** At what time between 2 and 3 o'clock will the hands of a clock be exactly opposite each other?
(a) 2:40  (b) 2:41 3/11  (c) 2:43 7/11  (d) 2:45

**Q43.** What day of the week was 26 January 1950?
(a) Tuesday  (b) Wednesday  (c) Thursday  (d) Friday

**Q44.** A clock loses 10 minutes every 24 hours. If it is set right at 12 noon on Monday, what will it show at 12 noon on the following Monday?
(a) 10:30 am  (b) 10:50 am  (c) 11:10 am  (d) 11:30 am

**Q45.** The present ages of A, B and C are in the ratio 4 : 7 : 9. Eight years ago the sum of their ages was 56 years. Find their present ages.
(a) 12, 21, 27  (b) 16, 28, 36  (c) 20, 35, 45  (d) 24, 42, 54

**Q46.** How many times in a day (24 hours) do the hands of a clock form a straight line?
(a) 22  (b) 24  (c) 44  (d) 48

**Q47.** A father's age is 3 times his son's age. After 15 years it will be twice his son's age. What is the difference between their present ages?
(a) 20 years  (b) 25 years  (c) 30 years  (d) 35 years

**Q48.** The calendar for the year 2018 can be reused in which year?
(a) 2024  (b) 2026  (c) 2029  (d) 2030

**Q49.** At what time between 9 and 10 o'clock will the hands of a clock coincide?
(a) 9:45  (b) 9:47 3/11  (c) 9:49 1/11  (d) 9:50

**Q50.** The ratio of a father's age to his son's age is 7 : 3, and the product of their ages is 756. Find the father's age after 6 years.
(a) 42  (b) 45  (c) 48  (d) 54

---

## 9. Detailed Solutions

### 🟢 EASY — Solutions 1–20

---

**Q1. Father 3× son, son is 12. → (c) 36**

$$\text{Father} = 3 \times 12 = 36$$

**Answer: (c) 36**

---

**Q2. Sum 45, A is 5 years older. A's age? → (c) 25**

**Step 1 — Set one variable.** Let B = *x*, so A = *x* + 5.

**Step 2 — Use the sum.**
$$x + (x+5) = 45 \implies 2x = 40 \implies x = 20$$

**Step 3 — A's age.**
$$A = 25$$

**⚡ Shortcut:** with a sum S and a difference d, the larger is (S + d)/2 = (45 + 5)/2 = **25**.

**Answer: (c) 25**

---

**Q3. 25 years old five years ago; age in 10 years? → (c) 40**

$$\text{Present age} = 25 + 5 = 30$$
$$\text{In 10 years} = 30 + 10 = 40$$

**⚡ Direct:** the span from "5 years ago" to "10 years hence" is 15 years, so 25 + 15 = **40**.

**Answer: (c) 40**

---

**Q4. Ratio 3 : 4, B is 24. A's age? → (b) 18**

$$\frac{A}{24} = \frac{3}{4} \implies A = 18$$

**Answer: (b) 18**

---

**Q5. A is 4 years older than B = 16. → (b) 20**

$$A = 16 + 4 = 20$$

**Answer: (b) 20**

---

**Q6. Average age of 3 people is 25. Sum? → (c) 75**

$$3 \times 25 = 75$$

**Answer: (c) 75**

---

**Q7. Angle at 3:00. → (c) 90°**

$$\theta = |30(3) - 5.5(0)| = 90°$$

*(The hour hand is at the 3, the minute hand at the 12 — a quarter of the dial apart.)*

**Answer: (c) 90°**

---

**Q8. Minute hand's movement per minute. → (d) 6°**

The minute hand covers 360° in 60 minutes:
$$\frac{360}{60} = 6° \text{ per minute}$$

**Answer: (d) 6°**

---

**Q9. Hour hand's movement per hour. → (c) 30°**

The hour hand covers 360° in 12 hours:
$$\frac{360}{12} = 30° \text{ per hour}$$

*(Equivalently 0.5° per minute.)*

**Answer: (c) 30°**

---

**Q10. Angle at 6:00. → (d) 180°**

$$\theta = |30(6) - 0| = 180°$$

The hands point in exactly opposite directions.

**Answer: (d) 180°**

---

**Q11. Odd days in an ordinary year. → (b) 1**

$$365 = 52 \times 7 + 1 \implies 1 \text{ odd day}$$

**Answer: (b) 1**

---

**Q12. Odd days in a leap year. → (c) 2**

$$366 = 52 \times 7 + 2 \implies 2 \text{ odd days}$$

**Answer: (c) 2**

---

**Q13. Is 2024 a leap year? → (a) Yes**

2024 ÷ 4 = 506 exactly, and 2024 is not a century year.

**Answer: (a) Yes**

---

**Q14. Is 1900 a leap year? → (b) No**

1900 is divisible by 4 **and** by 100, but **not** by 400 (1900 ÷ 400 = 4.75).

Century years must be divisible by 400 to qualify.

**Answer: (b) No**

---

**Q15. Is 2000 a leap year? → (a) Yes**

2000 is a century year, but 2000 ÷ 400 = 5 exactly, so it **is** a leap year.

> **Contrast Q14 and Q15.** 1900 and 2000 are both century years, yet only 2000 is a leap year. This pair is a favourite examiner trap.

**Answer: (a) Yes**

---

**Q16. Coincidences in 12 hours. → (b) 11**

The hands coincide **11 times** in 12 hours.

> **Why not 12?** The hands meet roughly every 65 5/11 minutes, not every 60. Across a 12-hour span there is only one meeting between 11 o'clock and 1 o'clock (at 12:00), so one "expected" meeting is absent.

**Answer: (b) 11**

---

**Q17. Coincidences in 24 hours. → (b) 22**

$$11 \times 2 = 22$$

**Answer: (b) 22**

---

**Q18. Present age 40; age 12 years ago? → (b) 28**

$$40 - 12 = 28$$

**Answer: (b) 28**

---

**Q19. Angle at 9:00. → (b) 90°**

$$\theta = |30(9) - 0| = 270°$$

Since 270° > 180°, take the smaller angle:
$$360° - 270° = 90°$$

> **Always apply the reflex correction.** The answer to an "angle between the hands" question is by convention the smaller of the two angles, so it never exceeds 180°.

**Answer: (b) 90°**

---

**Q20. Days in 4 consecutive ordinary years. → (b) 1,460**

$$4 \times 365 = 1{,}460$$

> **Note the wording.** "Four consecutive **ordinary** years" excludes leap years. Had it said simply "four consecutive years", one would normally be a leap year and the total would be 1,461.

**Answer: (b) 1,460**

---

### 🟡 MEDIUM — Solutions 21–40

---

**Q21. Father 4× son; after 20 years, twice. Son's age? → (b) 10**

**Step 1 — Represent with one variable.**
Son = *s*, Father = 4*s*

**Step 2 — Apply the future condition.**
$$4s + 20 = 2(s + 20)$$

**Step 3 — Solve.**
$$4s + 20 = 2s + 40$$
$$2s = 20 \implies s = 10$$

**Verification:** now 10 and 40 (4× ✓); after 20 years, 30 and 60 (2× ✓). Difference is 30 both times ✓

**Answer: (b) 10**

---

**Q22. Ratio 4 : 5 now, 5 : 6 in 5 years. A's age? → (c) 20**

**Step 1 — Set the variable.**
$$A = 4x, \qquad B = 5x$$

**Step 2 — Apply the future ratio.**
$$\frac{4x+5}{5x+5} = \frac{5}{6}$$

**Step 3 — Cross-multiply.**
$$6(4x+5) = 5(5x+5)$$
$$24x + 30 = 25x + 25$$
$$x = 5$$

**Step 4 — A's present age.**
$$4x = 20$$

**Verification:** 20 and 25 now; 25 and 30 in five years ⇒ 25 : 30 = **5 : 6** ✓

**Answer: (c) 20**

---

**Q23. Ratio 2 : 3 ten years ago, 3 : 4 now. B's present age? → (c) 40**

**Step 1 — Use the PRESENT ratio for the variable** (it is easier to shift backwards than forwards here).
$$A = 3x, \qquad B = 4x$$

**Step 2 — Ages ten years ago.**
$$A = 3x - 10, \qquad B = 4x - 10$$

**Step 3 — Apply the past ratio.**
$$\frac{3x - 10}{4x - 10} = \frac{2}{3}$$

**Step 4 — Cross-multiply.**
$$3(3x-10) = 2(4x-10)$$
$$9x - 30 = 8x - 20$$
$$x = 10$$

**Step 5 — B's present age.**
$$4x = 40$$

**Verification:** present ages 30 and 40 (3 : 4 ✓). Ten years ago: 20 and 30 ⇒ **2 : 3** ✓

**Answer: (c) 40**

---

**Q24. Sum 60; six years ago father was 5× son. → (b) 46 and 14**

**Step 1 — Set the variable.**
Son = *s*, Father = 60 − *s*

**Step 2 — Ages six years ago.**
Son: *s* − 6 · Father: 54 − *s*

**Step 3 — Apply the past condition.**
$$54 - s = 5(s - 6)$$

**Step 4 — Solve.**
$$54 - s = 5s - 30$$
$$84 = 6s \implies s = 14$$

**Step 5 — Father's age.**
$$60 - 14 = 46$$

**Verification:** Six years ago they were 8 and 40, and 40 = 5 × 8 ✓ Sum now = 60 ✓

**Answer: (b) 46 and 14**

---

**Q25. Angle at 3:30. → (c) 75°**

$$\theta = |30(3) - 5.5(30)| = |90 - 165| = 75°$$

**First-principles check:**
- Minute hand at 30 min: 30 × 6 = **180°**
- Hour hand at 3:30: 3 × 30 + 30 × 0.5 = 90 + 15 = **105°**
- Difference = **75°** ✓

> **Trap:** answering 90°. The hour hand has crept 15° past the 3 by the half-hour — it is not still sitting on the numeral.

**Answer: (c) 75°**

---

**Q26. Hands coincide between 3 and 4. → (b) 3:16 4/11**

**Formula used:** M = 60H/11

$$M = \frac{60 \times 3}{11} = \frac{180}{11} = 16\tfrac{4}{11} \text{ minutes}$$

**Relative-speed derivation:**
At 3:00 the hour hand leads by 90°. The minute hand closes the gap at 5.5°/min:
$$\frac{90}{5.5} = \frac{180}{11} = 16\tfrac{4}{11} \text{ min} \checkmark$$

**Answer: (b) 3:16 4/11**

---

**Q27. Angle at 4:20. → (c) 10°**

$$\theta = |30(4) - 5.5(20)| = |120 - 110| = 10°$$

**First-principles check:**
- Minute hand: 20 × 6 = **120°**
- Hour hand: 4 × 30 + 20 × 0.5 = 120 + 10 = **130°**
- Difference = **10°** ✓

> **Trap:** answering 0°, assuming both hands are at the "4". The minute hand is exactly at the 4, but the hour hand has moved a third of the way toward the 5.

**Answer: (c) 10°**

---

**Q28. Day of the week on 15 August 1947. → (c) Friday**

**Step 1 — Split the completed years (1946).**
$$1946 = 1600 + 300 + 46$$

**Step 2 — Century odd days.**
$$1600 \to 0 \qquad 300 \to 1$$

**Step 3 — The remaining 46 years (1901–1946).**
Leap years: 1904, 1908, …, 1944 ⇒ **11**
Ordinary years: 46 − 11 = **35**
$$11(2) + 35(1) = 57 \implies 57 \bmod 7 = 1$$

**Step 4 — Subtotal.**
$$0 + 1 + 1 = 2 \text{ odd days}$$

**Step 5 — Days elapsed in 1947 up to 15 August.**
$$31 + 28 + 31 + 30 + 31 + 30 + 31 + 15 = 227$$
$$227 \bmod 7 = 3$$

**Step 6 — Total and decode.**
$$2 + 3 = 5 \implies \textbf{Friday}$$

**Answer: (c) Friday**

---

**Q29. 1 Jan 2024 is a Monday. What is 1 Jan 2025? → (b) Wednesday**

**Step 1 — Identify the interval.**
1 Jan 2024 to 1 Jan 2025 spans the whole of 2024.

**Step 2 — Check for a leap day inside the interval.**
2024 **is** a leap year, and 29 February 2024 lies within the interval ⇒ **366 days**.

**Step 3 — Odd days.**
$$366 \bmod 7 = 2$$

**Step 4 — Advance.**
$$\text{Monday} + 2 = \textbf{Wednesday}$$

**Answer: (b) Wednesday**

---

**Q30. Right angles in 12 hours. → (c) 22**

The hands form a 90° angle **22 times** in 12 hours — roughly twice per hour, but with two "missing" instances near the 3 o'clock and 9 o'clock positions where the events overlap between adjacent hours.

**Answer: (c) 22**

---

**Q31. Clock gains 5 min/hour; set right at noon. Reading at 6 pm? → (c) 6:30 pm**

**Step 1 — Elapsed true time.**
Noon to 6 pm = **6 hours**

**Step 2 — Total gain.**
$$5 \times 6 = 30 \text{ minutes}$$

**Step 3 — The clock runs ahead, so ADD.**
$$6{:}00 + 0{:}30 = \mathbf{6{:}30 \text{ pm}}$$

**Answer: (c) 6:30 pm**

---

**Q32. Ratio 5 : 7 now, 3 : 4 in four years. B's age? → (c) 28**

**Step 1 — Set the variable.**
$$A = 5x, \qquad B = 7x$$

**Step 2 — Apply the future ratio.**
$$\frac{5x+4}{7x+4} = \frac{3}{4}$$

**Step 3 — Cross-multiply.**
$$4(5x+4) = 3(7x+4)$$
$$20x + 16 = 21x + 12$$
$$x = 4$$

**Step 4 — B's present age.**
$$7x = 28$$

**Verification:** 20 and 28 now; 24 and 32 in four years ⇒ 24 : 32 = **3 : 4** ✓

**Answer: (c) 28**

---

**Q33. 45 days after a Tuesday. → (c) Friday**

**Step 1 — Reduce modulo 7.**
$$45 \bmod 7 = 45 - 42 = 3$$

**Step 2 — Advance three days from Tuesday.**
$$\text{Tuesday} \to \text{Wed} \to \text{Thu} \to \textbf{Friday}$$

**Answer: (c) Friday**

---

**Q34. Angle at 7:20. → (b) 100°**

$$\theta = |30(7) - 5.5(20)| = |210 - 110| = 100°$$

**First-principles check:**
- Minute hand: 120°
- Hour hand: 210 + 10 = 220°
- Difference = 100° ✓

**Answer: (b) 100°**

---

**Q35. A is twice as old as B was 2 years ago; A is 26. B's present age? → (c) 15**

**Step 1 — Translate the statement precisely.**
$$A = 2 \times (B \text{'s age 2 years ago})$$
$$26 = 2(B - 2)$$

**Step 2 — Solve.**
$$B - 2 = 13 \implies B = 15$$

**Verification:** two years ago B was 13, and 2 × 13 = 26 = A's present age ✓

> **Read the tense.** The comparison is between A's *present* age and B's *past* age — a mixed-time statement. Reading it as "A is twice B's present age" would give B = 13, which is offered as a distractor.

**Answer: (c) 15**

---

**Q36. 5 March 2020 was a Thursday. What was 5 March 2021? → (b) Friday**

**Step 1 — Identify the interval.**
5 March 2020 → 5 March 2021.

**Step 2 — Check for 29 February inside the interval.**
2020 is a leap year, but **29 February 2020 falls before 5 March 2020** — outside the interval. The next 29 February is in 2024. So the interval is **365 days**.

**Step 3 — Odd days.**
$$365 \bmod 7 = 1$$

**Step 4 — Advance.**
$$\text{Thursday} + 1 = \textbf{Friday}$$

> **The key discipline:** ask whether 29 February lies **inside the interval**, not whether either endpoint year is a leap year. A start date after 1 March skips that year's leap day entirely.

**Answer: (b) Friday**

---

**Q37. Family of 4 averages 30; youngest is 6. Average of the other 3? → (c) 38**

**Step 1 — Total age of the family.**
$$4 \times 30 = 120$$

**Step 2 — Remove the youngest.**
$$120 - 6 = 114$$

**Step 3 — Average of the remaining three.**
$$\frac{114}{3} = 38$$

**Answer: (c) 38**

---

**Q38. First right angle between 4 and 5 o'clock. → (a) 4:05 5/11**

**Step 1 — Set up the angle equation.**
$$|30(4) - 5.5M| = 90$$
$$|120 - 5.5M| = 90$$

**Step 2 — Solve both branches.**

*Branch 1 (minute hand still behind, gap shrinking to 90°):*
$$120 - 5.5M = 90 \implies 5.5M = 30 \implies M = \frac{30}{5.5} = \frac{60}{11} = 5\tfrac{5}{11}$$

*Branch 2 (minute hand overtakes and opens a 90° lead):*
$$5.5M - 120 = 90 \implies M = \frac{210}{5.5} = \frac{420}{11} = 38\tfrac{2}{11}$$

**Step 3 — Take the FIRST occurrence.**
$$M = 5\tfrac{5}{11} \implies \mathbf{4{:}05\tfrac{5}{11}}$$

**Verification:** at M = 60/11, the angle is |120 − 5.5(60/11)| = |120 − 30| = 90° ✓

> **There are two right angles in most hours.** Read whether the question asks for the first or the second — option (d) is the second one.

**Answer: (a) 4:05 5/11**

---

**Q39. Odd days in 100 years. → (c) 5**

**Step 1 — Count leap years in a century.**
A century contains **24 leap years** (not 25 — the century year itself, e.g. 1900, is usually not a leap year).

**Step 2 — Count ordinary years.**
$$100 - 24 = 76$$

**Step 3 — Total odd days.**
$$24(2) + 76(1) = 48 + 76 = 124$$

**Step 4 — Reduce modulo 7.**
$$124 \bmod 7 = 124 - 119 = 5$$

**Answer: (c) 5**

> **The full century table follows from this:** 100 → 5, 200 → 10 mod 7 = 3, 300 → 15 mod 7 = 1, 400 → 20 mod 7 = 6, but 400 gains one extra day because the 400th year *is* a leap year ⇒ **0**. That zero is why the calendar repeats every 400 years.

---

**Q40. Age in 10 years = 3 × age 10 years ago. Present age? → (b) 20**

**Step 1 — Set up the equation.**
Let the present age be *x*.
$$x + 10 = 3(x - 10)$$

**Step 2 — Solve.**
$$x + 10 = 3x - 30$$
$$40 = 2x \implies x = 20$$

**Verification:** in 10 years he will be 30; 10 years ago he was 10; and 30 = 3 × 10 ✓

**Answer: (b) 20**

---

### 🔴 HARD — Solutions 41–50

---

**Q41. Ratio 3 : 5 now, 3 : 4 after 9 years. Sum of present ages? → (c) 24**

**Step 1 — Set the variable.**
$$A = 3x, \qquad B = 5x$$

**Step 2 — Apply the future ratio.**
$$\frac{3x+9}{5x+9} = \frac{3}{4}$$

**Step 3 — Cross-multiply.**
$$4(3x+9) = 3(5x+9)$$
$$12x + 36 = 15x + 27$$
$$9 = 3x \implies x = 3$$

**Step 4 — Present ages and their sum.**
$$A = 9, \quad B = 15 \implies \text{Sum} = 24$$

**Verification:** 9 : 15 = 3 : 5 ✓ After 9 years: 18 and 24 ⇒ 18 : 24 = **3 : 4** ✓

**Answer: (c) 24**

---

**Q42. Hands opposite between 2 and 3 o'clock. → (c) 2:43 7/11**

**Step 1 — Set up the equation for a 180° separation.**
$$|30(2) - 5.5M| = 180$$
$$|60 - 5.5M| = 180$$

**Step 2 — Solve the viable branch.**

*Branch 1:* 60 − 5.5M = 180 ⇒ M = −120/5.5, negative ⇒ **rejected**

*Branch 2:* 5.5M − 60 = 180
$$5.5M = 240 \implies M = \frac{240}{5.5} = \frac{480}{11} = 43\tfrac{7}{11}$$

**Step 3 — State the time.**
$$\mathbf{2{:}43\tfrac{7}{11}}$$

**Verification:** hour hand at 60 + 0.5(480/11) = 60 + 240/11 ≈ 81.8°; minute hand at 6 × 480/11 ≈ 261.8°. Difference ≈ 180° ✓

**Answer: (c) 2:43 7/11**

---

**Q43. Day of the week on 26 January 1950. → (c) Thursday**

**Step 1 — Split the completed years (1949).**
$$1949 = 1600 + 300 + 49$$

**Step 2 — Century odd days.**
$$1600 \to 0 \qquad 300 \to 1$$

**Step 3 — The remaining 49 years (1901–1949).**
Leap years: 1904, 1908, …, 1948 ⇒ **12**
Ordinary years: 49 − 12 = **37**
$$12(2) + 37(1) = 24 + 37 = 61 \implies 61 \bmod 7 = 5$$

**Step 4 — Subtotal.**
$$0 + 1 + 5 = 6 \text{ odd days}$$

**Step 5 — Days elapsed in 1950 up to 26 January.**
$$26 \implies 26 \bmod 7 = 5$$

**Step 6 — Total and decode.**
$$6 + 5 = 11 \implies 11 \bmod 7 = 4 \implies \textbf{Thursday}$$

**Answer: (c) Thursday**

*(Historically correct — India's first Republic Day fell on a Thursday.)*

---

**Q44. Clock loses 10 min per 24 h; set right noon Monday. Reading at noon next Monday? → (b) 10:50 am**

**Step 1 — Count the elapsed periods.**
Monday noon to the following Monday noon = **7 days**

**Step 2 — Total loss.**
$$10 \times 7 = 70 \text{ minutes} = 1 \text{ hour } 10 \text{ minutes}$$

**Step 3 — The clock runs behind, so SUBTRACT.**
$$12{:}00 \text{ noon} - 1{:}10 = \mathbf{10{:}50 \text{ am}}$$

**Answer: (b) 10:50 am**

> **Sign check:** losing ⇒ behind ⇒ subtract. Gaining ⇒ ahead ⇒ add. Reversing this gives 1:10 pm — a plausible-looking wrong answer.

---

**Q45. Ages in 4 : 7 : 9; eight years ago their sum was 56. Present ages? → (b) 16, 28, 36**

**Step 1 — Set the variable.**
$$A = 4x, \quad B = 7x, \quad C = 9x \implies \text{Present sum} = 20x$$

**Step 2 — Sum eight years ago.**
Each of the three was 8 years younger, so the sum was **24 years less**:
$$20x - 24 = 56$$

**Step 3 — Solve.**
$$20x = 80 \implies x = 4$$

**Step 4 — Present ages.**
$$A = 16, \quad B = 28, \quad C = 36$$

**Verification:** eight years ago they were 8, 20 and 28, summing to **56** ✓ And 16 : 28 : 36 = 4 : 7 : 9 ✓

> **The count matters.** Three people going back eight years reduces the total by 3 × 8 = 24, not by 8.

**Answer: (b) 16, 28, 36**

---

**Q46. Straight lines formed in 24 hours. → (c) 44**

**Concept:** the hands form a straight line when they are either **coincident (0°)** or **opposite (180°)**.

| Event | In 12 hours | In 24 hours |
|---|---|---|
| Coincident | 11 | 22 |
| Opposite | 11 | 22 |
| **Straight line (total)** | **22** | **44** |

**Answer: (c) 44**

---

**Q47. Father 3× son; after 15 years, twice. Difference in ages? → (c) 30 years**

**Step 1 — Set the variable.**
Son = *s*, Father = 3*s*

**Step 2 — Apply the future condition.**
$$3s + 15 = 2(s + 15)$$
$$3s + 15 = 2s + 30$$
$$s = 15$$

**Step 3 — Compute both ages and the difference.**
$$\text{Son} = 15, \quad \text{Father} = 45$$
$$\text{Difference} = 45 - 15 = 30 \text{ years}$$

**Verification:** after 15 years they are 30 and 60, and 60 = 2 × 30 ✓ The difference is still 30 ✓

> **The invariant is the answer.** Because the age gap never changes, this question could equally have asked for the difference at any point in time — the answer would be 30 either way.

**Answer: (c) 30 years**

---

**Q48. The 2018 calendar can be reused in which year? → (c) 2029**

**Requirement:** the total odd days between the two years must be a multiple of 7, **and** both years must be of the same type (both ordinary or both leap).

**Step 1 — Confirm 2018 is an ordinary year.**
2018 ÷ 4 is not exact ⇒ ordinary ✓

**Step 2 — Accumulate odd days year by year.**

| Year | Type | Odd days | Running total |
|---|---|---|---|
| 2018 | Ordinary | 1 | 1 |
| 2019 | Ordinary | 1 | 2 |
| 2020 | **Leap** | 2 | 4 |
| 2021 | Ordinary | 1 | 5 |
| 2022 | Ordinary | 1 | 6 |
| 2023 | Ordinary | 1 | 7 |
| 2024 | **Leap** | 2 | 9 |
| 2025 | Ordinary | 1 | 10 |
| 2026 | Ordinary | 1 | 11 |
| 2027 | Ordinary | 1 | 12 |
| 2028 | **Leap** | 2 | **14** |

**Step 3 — Identify the first multiple of 7 with a matching year type.**
The running total reaches **14** (a multiple of 7) after 2028, which points to **2029**.

**Step 4 — Verify the year type matches.**
2029 ÷ 4 is not exact ⇒ ordinary ✓ — the same type as 2018.

> **Why not 2025?** The total reaches 7 after 2023, pointing to 2024 — but 2024 is a **leap** year while 2018 is ordinary, so their calendars differ. The type must match.

**Answer: (c) 2029**

---

**Q49. Hands coincide between 9 and 10 o'clock. → (c) 9:49 1/11**

**Formula used:** M = 60H/11

$$M = \frac{60 \times 9}{11} = \frac{540}{11} = 49\tfrac{1}{11} \text{ minutes}$$

**Relative-speed derivation:**
At 9:00 the hour hand leads by 270°. The minute hand closes the gap at 5.5°/min:
$$\frac{270}{5.5} = \frac{540}{11} = 49\tfrac{1}{11} \text{ min} \checkmark$$

**Angle-formula check:**
$$\left|30(9) - 5.5\left(\frac{540}{11}\right)\right| = |270 - 270| = 0° \checkmark$$

**Answer: (c) 9:49 1/11**

---

**Q50. Ages in 7 : 3, product 756. Father's age after 6 years? → (c) 48**

**Step 1 — Set the variable.**
$$\text{Father} = 7x, \qquad \text{Son} = 3x$$

**Step 2 — Use the product condition.**
$$7x \times 3x = 756$$
$$21x^2 = 756$$

**Step 3 — Solve.**
$$x^2 = 36 \implies x = 6 \quad (\text{reject } x = -6)$$

**Step 4 — Present ages.**
$$\text{Father} = 42, \qquad \text{Son} = 18$$

**Step 5 — Answer the question asked.**
$$42 + 6 = 48 \text{ years}$$

**Verification:** 42 : 18 = 7 : 3 ✓ and 42 × 18 = 756 ✓

> **Read the final line.** Options (a) 42 is the father's *present* age — a trap for anyone who stops at Step 4.

**Answer: (c) 48**

---

## 10. Quick Revision Sheet

> **One page. Read 48 hours after study, and again the night before the test.**

### AGES

```
1.  Use ONE variable:  ratio a:b  →  ax, bx
2.  Shift EVERY age by the same t
3.  Solve

THE INVARIANT:  the age DIFFERENCE never changes. Use it to check.

"After t, A is m× B"   →  A + t = m(B + t)
"t ago, A was m× B"    →  A − t = m(B − t)
Sum S, difference d    →  larger = (S + d)/2

FAMILY AVERAGES: going back in time may change the HEADCOUNT
    (a member born t years ago did not exist t years ago)
```

### CLOCKS

```
Minute hand   6° per minute
Hour hand     0.5° per minute (30° per hour)
RELATIVE      5.5° per minute      ← everything comes from this

⭐ ANGLE:  θ = |30H − 5.5M|      (if θ > 180°, use 360° − θ)

COINCIDE past hour H  →  M = 60H/11
    3 o'clock → 3:16 4/11      9 o'clock → 9:49 1/11
    Any target angle θ  →  |30H − 5.5M| = θ,  solve for M
    (usually TWO solutions per hour — read "first" or "second")

FREQUENCIES (12 h / 24 h)
    Coincide      11 / 22
    Opposite      11 / 22
    Straight line 22 / 44
    Right angle   22 / 44

FAULTY CLOCK:  error = rate × periods
    GAINING → ADD       LOSING → SUBTRACT

KEY ANGLES: 12:00→0°  3:00→90°  6:00→180°  9:00→90°
            3:30→75°  4:20→10°  7:20→100°  5:40→70°
```

### CALENDARS

```
ODD DAYS = total days mod 7

Ordinary year  →  1        Leap year  →  2
100 years → 5   200 → 3   300 → 1   400 → 0

LEAP YEAR:  ÷4, EXCEPT centuries, UNLESS ÷400
    2024 ✓   2000 ✓   1900 ✗   2100 ✗

DAY CODES:  0 Sun · 1 Mon · 2 Tue · 3 Wed · 4 Thu · 5 Fri · 6 Sat

FINDING A DAY
    1. Completed years → centuries + remainder
    2. Remainder: 2(leaps) + 1(ordinaries), mod 7
    3. Add days elapsed in the target year
    4. Total mod 7 → decode

MONTH DAYS  31 28 31 30 31 30 31 31 30 31 30 31

SAME DATE NEXT YEAR
    +1 day if no 29 Feb in the interval
    +2 days if 29 Feb IS in the interval
    (Check the INTERVAL, not the year label)

CALENDAR REUSE
    odd days between the two years ≡ 0 (mod 7)  AND  same year type
    Ordinary → typically +6 or +11 years    Leap → +28 years
    2018 → 2029
```

### Sanity checks

```
✓ AGES: difference is constant; no negative ages
✓ CLOCKS: the answer angle lies in [0°, 180°]
✓ CLOCKS: 11 coincidences per 12 hours, never 12
✓ CALENDARS: odd days ∈ {0,…,6}
✓ CALENDARS: 400 years → 0 odd days
```

---

## 11. Common Mistakes

| # | Mistake | Example | Correction |
|---|---|---|---|
| 1 | **Only one age shifted** | "After 20 years" applied to the father only | Shift **both** ages |
| 2 | **Two variables used unnecessarily** | Letting the ages be a and b with a ratio given | Use ax and bx |
| 3 | **Mixed tenses misread** | "A is twice B's age 2 years ago" | The comparison spans two different times |
| 4 | **Family headcount unchanged** | Family of 6 rolled back 5 years, still ÷6 | The youngest did not exist ⇒ ÷5 |
| 5 | **Hour hand assumed stationary** | Angle at 3:30 given as 90° | The hour hand has moved 15° ⇒ 75° |
| 6 | **Reflex angle not corrected** | Angle at 9:00 given as 270° | Take 360 − 270 = 90° |
| 7 | **12 coincidences assumed** | "12 per 12 hours" | It is **11** |
| 8 | **Faulty-clock sign reversed** | Losing clock ⇒ time added | Losing ⇒ **subtract** |
| 9 | **Only one branch of the angle equation** | Right angle at 4 o'clock, first solution only | Two solutions per hour — read which is asked |
| 10 | **Century leap-year rule ignored** | 1900 treated as a leap year | Centuries need ÷400 |
| 11 | **25 leap years per century** | 24(2) replaced by 25(2) | A century has **24** leap years |
| 12 | **Leap day counted outside the interval** | 5 Mar 2020 → 5 Mar 2021 given +2 | 29 Feb 2020 precedes the interval ⇒ +1 |
| 13 | **Calendar reuse without a type match** | 2018 → 2024 | 2024 is leap, 2018 ordinary — no match |
| 14 | **Stopping before the question ends** | Giving the present age when "after 6 years" is asked | Re-read the final clause |

---

## Practice Answer Key

| Q | Ans | Q | Ans | Q | Ans | Q | Ans | Q | Ans |
|---|---|---|---|---|---|---|---|---|---|
| 1 | c | 11 | b | 21 | b | 31 | c | 41 | c |
| 2 | c | 12 | c | 22 | c | 32 | c | 42 | c |
| 3 | c | 13 | a | 23 | c | 33 | c | 43 | c |
| 4 | b | 14 | b | 24 | b | 34 | b | 44 | b |
| 5 | b | 15 | a | 25 | c | 35 | c | 45 | b |
| 6 | c | 16 | b | 26 | b | 36 | b | 46 | c |
| 7 | c | 17 | b | 27 | c | 37 | c | 47 | c |
| 8 | d | 18 | b | 28 | c | 38 | a | 48 | c |
| 9 | c | 19 | b | 29 | b | 39 | c | 49 | c |
| 10 | d | 20 | b | 30 | c | 40 | b | 50 | c |

**Scoring guide:** 45+/50 → strong. 35–44 → solid; drill the |30H − 5.5M| formula and the odd-day table. Below 35 → learn just three things — the age template, the 5.5° rule and the odd-day table — then redo the whole set.

---

**⬅️ Back:** [Topic 11 — Mensuration & Geometry](11-mensuration-geometry.md) · **➡️ Next:** [Topic 13 — Number & Letter Series](13-number-letter-series.md)
