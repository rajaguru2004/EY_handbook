# Topic 18 — Data Sufficiency & Critical Reasoning

### EY Placement Aptitude Handbook · Priority Rank #19 · 🟠 High

> **Questions in this file are original, modelled on publicly reported EY test patterns. They are not claimed to be actual previous-year EY questions.**

---

## Contents

1. [Why This Topic Matters for EY](#1-why-this-topic-matters-for-ey)
2. [Core Concepts — Data Sufficiency](#2-core-concepts--part-a-data-sufficiency)
3. [Core Concepts — Critical Reasoning](#3-core-concepts--part-b-critical-reasoning)
4. [Shortcuts & Tricks](#4-shortcuts--tricks)
5. [Solved Examples](#5-solved-examples)
6. [Practice Questions (50)](#6-practice-questions)
7. [Detailed Solutions](#7-detailed-solutions)
8. [Quick Revision Sheet](#8-quick-revision-sheet)
9. [Common Mistakes](#9-common-mistakes)

---

## 1. Why This Topic Matters for EY

**Weightage:** Data sufficiency 6–8% · Critical reasoning 6–8% of the reasoning section. Together: **1–2 questions**.

**Why this topic suits EY specifically:** both formats mirror professional judgement. Data sufficiency asks *"do I have enough information to decide?"* — the central question in audit and consulting. Critical reasoning asks *"what does this evidence actually support?"* — the discipline behind every client recommendation. Expect EY to weight these more heavily than a generic engineering test would.

**The good news:** both are **format-trainable**. The reasoning is not hard; the *conventions* are unfamiliar. Learn the conventions in one sitting and the questions become routine.

**Question styles reported:**

| Sub-topic | Format |
|---|---|
| **Data sufficiency** | Question + two statements; decide what is sufficient |
| **Statement–Assumption** | What must be taken for granted? |
| **Statement–Conclusion** | What definitely follows? |
| **Course of Action** | What should be done? |
| **Statement–Argument** | Which argument is strong? |
| **Cause and Effect** | Which is the cause and which the effect? |
| **Strengthen / Weaken** | Which option supports or undermines the argument? |
| **Inference** | What can be concluded from the passage? |

---

## 2. Core Concepts — PART A: DATA SUFFICIENCY

### 2.1 The format

You are given a **question** and **two statements**. You must decide **whether the statements are sufficient to answer** — **not** what the answer is.

**The standard option set:**

```
(a)  Statement I ALONE is sufficient, but statement II alone is not
(b)  Statement II ALONE is sufficient, but statement I alone is not
(c)  BOTH statements TOGETHER are sufficient, but NEITHER alone is
(d)  EACH statement ALONE is sufficient
(e)  Both statements TOGETHER are NOT sufficient
```

> **The single most important discipline: do not solve the problem.** You only need to know whether a *unique* answer exists. If you find yourself computing the actual value, you are wasting time — and risking the classic error of assuming sufficiency because you happened to reach a number.

### 2.2 ⭐ The decision procedure

```
STEP 1:  Read the QUESTION carefully. What exactly is being asked?
STEP 2:  Consider statement I ALONE.  (Cover statement II with your hand.)
             Sufficient?  →  YES or NO
STEP 3:  Consider statement II ALONE. (Cover statement I.)
             Sufficient?  →  YES or NO
STEP 4:  Apply the decision table below.
STEP 5:  If neither alone works, combine them and re-test.
```

**The decision table:**

| I alone | II alone | Answer |
|---|---|---|
| ✅ | ✅ | **(d)** Each alone is sufficient |
| ✅ | ❌ | **(a)** I alone |
| ❌ | ✅ | **(b)** II alone |
| ❌ | ❌ | Combine → sufficient? **(c)** : **(e)** |

> **Step 3 is where candidates lose marks.** Having read statement I, it is very hard to un-know it. **Physically cover statement I** with your finger while evaluating II. This one habit prevents the most common error in the entire format.

### 2.3 The "unique answer" test

A statement is sufficient only if it pins the answer down to **exactly one** value or outcome.

| Situation | Sufficient? |
|---|---|
| x = 7 | ✅ Yes |
| x = ±4 | ❌ No — two values |
| x is a prime between 10 and 20 | ❌ No — 11, 13, 17, 19 |
| x is an even prime | ✅ Yes — only 2 |
| The answer is definitively "No" | ✅ Yes — a definite No is an answer |

> **A definite "no" counts as sufficient.** For a yes/no question, sufficiency means you can answer *either* yes or no with certainty — not that the answer must be yes.

### 2.4 Common traps

| Trap | Example |
|---|---|
| **Squares hide a sign** | x² = 16 gives x = ±4 ⇒ insufficient. But x³ = 64 gives only x = 4 ⇒ sufficient. |
| **Statements repeat each other** | "3 pens cost ₹45" and "1 pen costs ₹15" say the same thing ⇒ answer (d), not (c). |
| **Redundant combination** | If I alone suffices, the answer can never be (c). |
| **Ratio without a total** | A ratio alone never gives absolute values. |
| **One data point without a rate** | "Covers 300 km" is useless without the time. |

---

## 3. Core Concepts — PART B: CRITICAL REASONING

### 3.1 Statement–Assumption

An **assumption** is something the speaker must be taking for granted for the statement to make sense. It is **unstated but necessary**.

**The negation test — the single most reliable tool:**

```
Negate the proposed assumption.
    Does the statement now collapse or become absurd?
        YES  →  the assumption IS implicit
        NO   →  it is NOT implicit
```

> Statement: *"Use our shampoo for silky hair."*
> Proposed assumption: *People want silky hair.*
> **Negate it:** "People do not want silky hair." The advertisement would then be pointless ⇒ the assumption **is implicit** ✓

**Rules for assumptions:**

| Rule | Consequence |
|---|---|
| Must be **necessary**, not merely possible | "Competitors offer worse products" is usually not implicit |
| Must be **unstated** | Anything restated from the statement is not an assumption |
| Avoid **extreme** wording | "Always", "only", "never" rarely appear in valid assumptions |
| Comparisons are rarely implicit | Advertising a product doesn't assume it beats every rival |

### 3.2 Statement–Conclusion

A conclusion **definitely follows** if it cannot be false given the statement. Apply the same strictness as syllogisms.

**Watch for the two valid deductive forms:**

$$\text{If P then Q; P is true} \implies Q \text{ is true} \qquad (\textit{modus ponens})$$
$$\text{If P then Q; Q is false} \implies P \text{ is false} \qquad (\textit{modus tollens — the contrapositive})$$

**And the two invalid ones:**

$$\text{If P then Q; Q is true} \nRightarrow P \text{ is true} \qquad (\text{affirming the consequent})$$
$$\text{If P then Q; P is false} \nRightarrow Q \text{ is false} \qquad (\text{denying the antecedent})$$

> "All who completed the training got a bonus. Rahul got no bonus."
> ⇒ **Rahul did not complete the training** ✓ (contrapositive)
>
> "…Rahul got a bonus."
> ⇒ Rahul completed the training? **✗** — he might have received it for another reason.

### 3.3 Course of Action

A course of action follows if it is **practical, relevant and proportionate**.

```
✅ ACCEPT:  addresses the actual problem
            is feasible and specific
            is proportionate to the severity

❌ REJECT:  extreme ("ban all", "abolish entirely", "close permanently")
            impractical or unaffordable
            addresses a different problem
            merely restates the problem
```

> Statement: *Heavy rains have flooded several districts.*
> I. Relief teams should be sent immediately ⇒ **follows** ✓ (relevant, proportionate)
> II. People should be permanently relocated ⇒ **does not follow** ✗ (extreme, disproportionate)

### 3.4 Statement–Argument

An argument is **strong** if it is relevant, substantial and directly addresses the question.

```
✅ STRONG:   directly relevant
             establishes a real consequence
             substantial, not trivial

❌ WEAK:     restates the question
             appeals to personal preference ("people like it")
             raises an unrelated issue
             is ambiguous or trivially obvious
```

> Should mobile phones be banned in schools?
> I. Yes — they distract students from learning ⇒ **strong** ✓ (a real, relevant consequence)
> II. No — students like using them ⇒ **weak** ✗ (mere preference)

### 3.5 Cause and Effect

Given two statements, decide which is cause and which is effect.

**The tests:**

```
1.  TIME:  the cause must come first
2.  MECHANISM: is there a plausible causal pathway?
3.  DIRECTION: could the arrow run the other way?
4.  THIRD FACTOR: could a common cause explain both?
```

**The standard option set:**

```
(a)  I is the cause and II is its effect
(b)  II is the cause and I is its effect
(c)  Both are effects of a common cause
(d)  Both are independent causes
(e)  Both are effects of independent causes
```

> I. The price of onions rose sharply.
> II. Heavy rainfall damaged the onion crop.
> ⇒ **II is the cause, I is the effect** (b) — rainfall precedes the price rise and there is a clear mechanism.

### 3.6 Strengthen and Weaken

Identify the **argument's logical gap** — the unstated link between evidence and conclusion. Then:

```
STRENGTHEN  →  close the gap, or rule out an alternative explanation
WEAKEN      →  widen the gap, or supply an alternative explanation
```

> Argument: *"Sales rose 30% after our new campaign, so the campaign caused the rise."*
>
> **The gap:** something *other than* the campaign might have caused the rise.
>
> **Weakens:** "A major competitor exited the market that same month" — an alternative cause ✓
> **Strengthens:** "Sales in comparable regions without the campaign were flat" — rules out alternatives ✓
> **Irrelevant:** "The campaign was expensive" — cost says nothing about causation ✗

### 3.7 Inference

An inference must follow **from the passage alone** — not from what is likely, or what you know to be true in the world.

```
✅ VALID:    a direct logical consequence of the stated facts
❌ INVALID:  requires outside knowledge
             overstates the evidence ("all", "always", "proves")
             predicts the future without warrant
             restates the passage (that is a summary, not an inference)
```

> Passage: *"Revenue rose 15% but profit fell 5%."*
> ⇒ **Costs rose faster than revenue** ✓ (arithmetically necessary)
> ⇒ "The company is badly managed" ✗ (a judgement, not an inference)

---

## 4. Shortcuts & Tricks

### 4.1 Data sufficiency — the cover-up technique

```
1.  Cover statement II.  Judge statement I alone.  Write ✅ or ❌.
2.  Cover statement I.   Judge statement II alone. Write ✅ or ❌.
3.  Read off the decision table.
4.  Only if both are ❌, uncover both and re-test.
```

Writing the two ticks on your rough sheet before choosing an option eliminates almost every careless error in this format.

### 4.2 The elimination cascade

```
If statement I is sufficient  →  the answer is (a) or (d).  ELIMINATE (b), (c), (e).
If statement I is NOT         →  the answer is (b), (c) or (e). ELIMINATE (a), (d).
```

One judgement removes two or three options immediately.

### 4.3 Watch for statements that say the same thing

If the two statements are **logically equivalent**, the answer is **(d)**, never (c).

> I. "3 pens cost ₹45"  ⇒ ₹15 per pen
> II. "1 pen costs ₹15" ⇒ ₹15 per pen
> Same information ⇒ **(d)**

### 4.4 The negation test for assumptions

```
Negate the assumption.
    Statement collapses  →  IMPLICIT
    Statement survives   →  NOT implicit
```

This converts a vague judgement call into a definite test. Use it every time.

### 4.5 The extreme-language filter

Words that usually signal a **wrong** option in critical reasoning:

```
all · only · never · always · every · none · must · completely
totally · abolish · ban entirely · permanently · immediately close
```

Real-world reasoning is almost never absolute. Options containing these words are wrong far more often than not — though not always, so read before rejecting.

### 4.6 The alternative-cause reflex

For any *"X happened, then Y happened, so X caused Y"* argument, immediately ask:

```
□  Could Y have happened anyway?
□  Could something else have caused Y?
□  Could Y have caused X (reverse direction)?
□  Could a third factor have caused both?
```

The correct **weaken** option is almost always the one that answers "yes" to one of these.

### 4.7 Sanity checks

```
DATA SUFFICIENCY
✓ Do NOT solve — only decide sufficiency
✓ Evaluate each statement in ISOLATION first
✓ A definite "no" IS a sufficient answer
✓ x² = k gives TWO values; x³ = k gives one
✓ If I alone suffices, (c) is impossible

CRITICAL REASONING
✓ Assumptions must be NECESSARY, not merely plausible
✓ Conclusions must be CERTAIN, not likely
✓ Courses of action must be PROPORTIONATE
✓ Arguments must be RELEVANT and SUBSTANTIAL
✓ Inferences must come from the PASSAGE, not from world knowledge
```

---

## 5. Solved Examples

### Example 1 — Data sufficiency, both alone sufficient

**Q.** What is the value of *x*?
**I.** 3x − 6 = 15
**II.** x² − 49 = 0 and x > 0

**Step 1 — Statement I alone.**
$$3x = 21 \implies x = 7$$
A unique value ⇒ **sufficient** ✅

**Step 2 — Statement II alone.**
$$x^2 = 49 \implies x = \pm 7$$
But the condition x > 0 eliminates −7 ⇒ **x = 7**, unique ⇒ **sufficient** ✅

**Step 3 — Decision table.**
Both ✅ ⇒ **(d)**

**Answer: (d) Each statement alone is sufficient**

> **Note the role of "x > 0".** Without it, statement II would give two values and be insufficient, making the answer (a). Squared terms always require a sign check.

---

### Example 2 — Data sufficiency, combination required

**Q.** What is the area of a rectangle?
**I.** Its length is 12 cm.
**II.** Its perimeter is 34 cm.

**Step 1 — Statement I alone.**
Length = 12, breadth unknown ⇒ area cannot be determined ⇒ **insufficient** ❌

**Step 2 — Statement II alone.**
$$2(l + b) = 34 \implies l + b = 17$$
Many pairs satisfy this (12+5, 10+7, 8.5+8.5…), each giving a different area ⇒ **insufficient** ❌

**Step 3 — Combine.**
$$l = 12 \text{ and } l + b = 17 \implies b = 5$$
$$\text{Area} = 12 \times 5 = 60 \text{ cm}^2$$
Unique ⇒ **sufficient** ✅

**Answer: (c) Both statements together are sufficient, but neither alone is**

---

### Example 3 — Data sufficiency, a definite "no"

**Q.** Is the integer *n* odd?
**I.** n is divisible by 6.
**II.** n is greater than 20.

**Step 1 — Statement I alone.**
Any multiple of 6 is even ⇒ n is **definitely not odd**.

The answer to the question is a definite **"No"** ⇒ **sufficient** ✅

**Step 2 — Statement II alone.**
n > 20 could be 21 (odd) or 22 (even) ⇒ **insufficient** ❌

**Answer: (a) Statement I alone is sufficient**

> **A definite "no" is an answer.** Candidates often mark statement I insufficient because it does not make n odd. Sufficiency means the question can be *answered*, not that the answer is yes.

---

### Example 4 — Statement–Assumption with the negation test

**Q.** **Statement:** "Enrol in our online course to secure a placement in a top firm." — advertisement by a training institute.

**Assumptions:**
**I.** People are interested in securing placements at top firms.
**II.** The course improves a candidate's chances of placement.

**Testing assumption I — negate it.**
*"People are not interested in securing placements at top firms."*
The advertisement would be addressed to nobody and would make no sense ⇒ the statement **collapses** ⇒ assumption I is **implicit** ✅

**Testing assumption II — negate it.**
*"The course does not improve a candidate's chances of placement."*
The advertisement's central promise would be empty ⇒ the statement **collapses** ⇒ assumption II is **implicit** ✅

**Answer: Both I and II are implicit**

> **Contrast with a non-assumption.** "Competing courses are less effective" is *not* implicit — the institute can promote its own course without any claim about rivals. Negating it ("competing courses are equally effective") leaves the advertisement perfectly coherent.

---

### Example 5 — Statement–Conclusion (contrapositive)

**Q.** **Statement:** Every employee who submitted the compliance form before Friday received an early-bird bonus. Priya did not receive an early-bird bonus.

**Conclusions:**
**I.** Priya did not submit the compliance form before Friday.
**II.** Priya did not submit the form at all.

**Step 1 — Formalise.**
$$\text{Submitted before Friday} \implies \text{Received bonus}$$
Given: Priya did **not** receive the bonus.

**Step 2 — Apply the contrapositive.**
$$\neg(\text{Received bonus}) \implies \neg(\text{Submitted before Friday})$$
$$\implies \text{Conclusion I \textbf{follows}} \checkmark$$

**Step 3 — Test conclusion II.**
Priya may well have submitted the form — just **after** Friday. Nothing rules that out.
$$\implies \text{Conclusion II does \textbf{not} follow} ✗$$

**Answer: Only conclusion I follows**

---

### Example 6 — Course of Action

**Q.** **Statement:** A large number of road accidents in the city occur at night on poorly lit stretches of highway.

**Courses of action:**
**I.** Street lighting on those stretches should be improved.
**II.** All night-time driving on highways should be prohibited.

**Testing I.**
- Relevant? ✅ It addresses the stated cause (poor lighting)
- Feasible? ✅ Standard municipal work
- Proportionate? ✅

$$\implies \text{I \textbf{follows}} \checkmark$$

**Testing II.**
- Relevant? Partially — it would reduce night accidents
- Feasible? ❌ Prohibiting all night driving would halt freight, emergency services and long-distance travel
- Proportionate? ❌ Extreme relative to the problem

$$\implies \text{II does \textbf{not} follow} ✗$$

**Answer: Only course of action I follows**

> **The word "all" is the tell.** Blanket prohibitions almost never qualify as valid courses of action — a targeted remedy addressing the stated cause does.

---

### Example 7 — Weakening an argument

**Q.** **Argument:** After installing new energy-efficient lighting, a factory's monthly electricity bill fell by 25%. The management concluded that the new lighting caused the reduction.

Which of the following, if true, would most **weaken** this conclusion?

(a) The new lighting was expensive to install.
(b) The factory reduced its operating hours by one shift in the same month.
(c) Employees reported that the new lighting was brighter.
(d) Other factories have also installed similar lighting.

**Step 1 — Identify the argument's gap.**
$$\text{Lighting installed} \; \longrightarrow \; \text{Bill fell 25\%} \; \longrightarrow \; \text{Therefore lighting caused it}$$

The gap: **something else** might have caused the fall.

**Step 2 — Evaluate each option.**

| Option | Effect |
|---|---|
| (a) Cost of installation | **Irrelevant** — cost says nothing about causation |
| (b) Operating hours cut by a shift | **Provides an alternative cause** ⇒ weakens strongly ✅ |
| (c) Brighter lighting | **Irrelevant** — brightness is not consumption |
| (d) Other factories did the same | **Irrelevant** — says nothing about this factory |

**Answer: (b)**

> **The reflex to train:** whenever an argument reads "X happened, then Y happened, so X caused Y", the correct weakener is almost always the option that supplies **another plausible cause of Y**.

---

### Example 8 — Cause and Effect

**Q.** Two statements are given. Decide the relationship between them.

**I.** Several coastal districts have been placed under a cyclone alert.
**II.** All schools and colleges in those districts have been closed for three days.

**Options:**
(a) I is the cause and II is its effect
(b) II is the cause and I is its effect
(c) Both are effects of a common cause
(d) Both are independent causes

**Step 1 — Apply the time test.**
A cyclone alert is issued **before** closures are ordered.

**Step 2 — Apply the mechanism test.**
Authorities close institutions **because** of a weather alert. The pathway is clear and standard.

**Step 3 — Apply the direction test.**
Could closing schools cause a cyclone alert? Obviously not.

**Step 4 — Apply the third-factor test.**
Both are linked to the approaching cyclone, but statement I (the alert) is the immediate, official trigger for statement II. The relationship is direct, not merely correlated.

$$\implies \text{I is the cause, II is the effect}$$

**Answer: (a) I is the cause and II is its effect**

---

## 6. Practice Questions

**Instructions:** Q1–25 are Data Sufficiency; Q26–50 are Critical Reasoning.
Option sets are stated at the head of each block.
Full solutions in [Section 7](#7-detailed-solutions).

---

### PART A — DATA SUFFICIENCY (Questions 1–25)

**For each question, choose from:**
```
(a)  Statement I ALONE is sufficient, but II alone is not
(b)  Statement II ALONE is sufficient, but I alone is not
(c)  BOTH TOGETHER are sufficient, but NEITHER alone is
(d)  EACH statement ALONE is sufficient
(e)  Both together are NOT sufficient
```

**Q1.** What is the value of *x*?
I. x + 5 = 12    II. 2x = 14

**Q2.** What is the area of a rectangle?
I. Its length is 10 cm.    II. Its perimeter is 30 cm.

**Q3.** Is the integer *n* even?
I. n is divisible by 4.    II. n is greater than 10.

**Q4.** What is A's present age?
I. A is 5 years older than B.    II. B is 20 years old.

**Q5.** What is the value of x + y?
I. x = 3    II. y = 5

**Q6.** Is x > 0?
I. x² = 16    II. x³ = 64

**Q7.** What is the average speed of a train?
I. It covers a distance of 300 km.    II. It takes 5 hours for the journey.

**Q8.** How many students are there in a class?
I. 60% of the students are boys.    II. There are 24 girls in the class.

**Q9.** What is the profit percentage on an article?
I. The cost price is ₹200.    II. The selling price is ₹250.

**Q10.** On which day of the week did Ram arrive?
I. He arrived after Tuesday but before Friday.    II. He did not arrive on Wednesday.

**Q11.** What is the two-digit number?
I. The sum of its digits is 9.    II. The number is divisible by 9.

**Q12.** Is the triangle right-angled?
I. Its sides measure 3 cm, 4 cm and 5 cm.    II. One of its angles is 90°.

**Q13.** What is the simple interest earned?
I. A principal of ₹5,000 is invested at 8% per annum.    II. The investment period is 3 years.

**Q14.** Who is the tallest among A, B and C?
I. A is taller than B.    II. C is taller than A.

**Q15.** What is the value of *x*?
I. x is a prime number between 10 and 20.    II. x is an odd number.

**Q16.** How many days will A and B take to complete a work together?
I. A alone can complete it in 12 days.    II. B alone can complete it in 18 days.

**Q17.** What is the code for the word "good" in a certain language?
I. In that language, "good boy" is written as "ta la".
II. In that language, "good girl" is written as "ta ma".

**Q18.** Is the integer *n* divisible by 6?
I. n is divisible by 2.    II. n is divisible by 3.

**Q19.** What is the average of five numbers?
I. Their sum is 200.    II. The largest of them is 60.

**Q20.** In which direction is P from Q?
I. P is 5 km north of R.    II. R is 3 km east of Q.

**Q21.** What is B's rank from the bottom of the class?
I. B is 7th from the top.    II. There are 30 students in the class.

**Q22.** What is the cost of 5 pens?
I. 3 pens cost ₹45.    II. 1 pen costs ₹15.

**Q23.** Is *x* an integer?
I. x/2 is an integer.    II. 2x is an integer.

**Q24.** How many days will 10 men take to complete a piece of work?
I. 5 men can complete it in 12 days.    II. The work requires 60 man-days.

**Q25.** What is the ratio of milk to water in a mixture?
I. The mixture measures 40 litres.    II. It contains 10 litres of water.

---

### PART B — CRITICAL REASONING (Questions 26–50)

---

#### B1. Statement–Assumption (Questions 26–30)

**Choose from:**
```
(a) Only assumption I is implicit
(b) Only assumption II is implicit
(c) Either I or II is implicit
(d) Neither I nor II is implicit
(e) Both I and II are implicit
```

**Q26.** **Statement:** "Use our shampoo for silky, healthy hair." — an advertisement.
**Assumptions:** I. People want silky, healthy hair.  II. The shampoo is effective.

**Q27.** **Statement:** The company has decided to increase the salaries of all its employees by 10%.
**Assumptions:** I. The company has the funds to do so.  II. Employees will be motivated by the increase.

**Q28.** **Statement:** "Please do not use the lift during a power failure." — a notice in an office building.
**Assumptions:** I. The lift may stop working during a power failure.  II. People in the building generally use the lift.

**Q29.** **Statement:** The government has banned smoking in all public places.
**Assumptions:** I. Smoking in public places is harmful.  II. People will comply with the ban.

**Q30.** **Statement:** "Buy our laptop — it comes with a two-year on-site warranty." — an advertisement.
**Assumptions:** I. Warranty terms influence customers' buying decisions.  II. All competing brands offer shorter warranties.

---

#### B2. Course of Action (Questions 31–33)

**Choose from:**
```
(a) Only I follows        (b) Only II follows
(c) Either I or II follows (d) Neither follows
(e) Both I and II follow
```

**Q31.** **Statement:** Heavy rains over the past week have flooded several low-lying districts.
**Courses of action:** I. Relief teams should be dispatched to the affected districts immediately.  II. Residents should be permanently relocated away from those districts.

**Q32.** **Statement:** A large proportion of candidates fail the state entrance examination every year.
**Courses of action:** I. The quality of preparatory coaching should be reviewed and improved.  II. The entrance examination should be abolished.

**Q33.** **Statement:** Air quality in the city has deteriorated sharply over the past six months.
**Courses of action:** I. Emission standards for industrial units should be tightened and enforced.  II. All private vehicles should be banned from the city permanently.

---

#### B3. Strengthen and Weaken (Questions 34–35, 47, 50)

**Q34.** **Argument:** Company X's sales rose 30% in the quarter following the launch of its new advertising campaign. The management concluded that the campaign caused the increase.
Which of the following, if true, would most **weaken** this conclusion?
(a) The campaign was more expensive than the previous one.
(b) A major competitor withdrew from the market during the same quarter.
(c) Sales had also risen in the corresponding quarter of the previous year.
(d) The campaign was widely praised by industry commentators.

**Q35.** **Argument:** Employees who work from home are more productive than those who work in the office.
Which of the following, if true, would most **strengthen** this claim?
(a) Employees working from home report higher job satisfaction.
(b) A controlled study found that home-based employees completed 20% more assigned tasks per week.
(c) Office environments are often noisy and full of interruptions.
(d) Commuting to the office is tiring for most employees.

---

#### B4. Cause and Effect (Questions 36–37, 49)

**Choose from:**
```
(a) I is the cause and II is its effect
(b) II is the cause and I is its effect
(c) Both are effects of a common cause
(d) Both are independent causes
```

**Q36.** I. The retail price of onions has risen sharply in the past month.
II. Unseasonal heavy rainfall damaged the onion crop in the main growing regions.

**Q37.** I. The district administration declared a two-day holiday for all schools.
II. The meteorological department issued a severe cyclone warning for the district.

---

#### B5. Statement–Argument (Questions 38–40)

**Choose from:**
```
(a) Only argument I is strong     (b) Only argument II is strong
(c) Either I or II is strong      (d) Neither is strong
(e) Both I and II are strong
```

**Q38.** **Statement:** Should written examinations be abolished in schools?
**Arguments:** I. Yes, because they cause stress among students.  II. No, because they provide a structured measure of what students have learned.

**Q39.** **Statement:** Should public transport in large cities be made free of charge?
**Arguments:** I. Yes, it would reduce the use of private vehicles and lower urban air pollution.  II. No, it would impose a substantial and recurring cost on the public exchequer.

**Q40.** **Statement:** Should mobile phones be banned inside school classrooms?
**Arguments:** I. Yes, because they distract students from classroom learning.  II. No, because students enjoy using them.

---

#### B6. Inference and Conclusion (Questions 41–46, 48)

**Q41.** **Passage:** Company Z reported a 15% increase in revenue this year but a 5% decline in profit.
Which of the following can be inferred?
(a) The company sold fewer units this year.
(b) Costs rose faster than revenue.
(c) The company is poorly managed.
(d) Competitors performed better.

**Q42.** **Statement:** All employees who completed the safety training received a certificate. Rahul did not receive a certificate.
Which conclusion definitely follows?
(a) Rahul is not an employee.
(b) Rahul did not complete the safety training.
(c) Rahul failed the training.
(d) The training was not held.

**Q43.** **Statement:** If it rains, the cricket match will be cancelled. The match was not cancelled.
Which conclusion definitely follows?
(a) It rained.
(b) It did not rain.
(c) The match was postponed.
(d) Nothing definite can be concluded.

**Q44.** **Statements:** Some managers are engineers. All engineers are graduates.
Which conclusion definitely follows?
(a) All managers are graduates.
(b) Some managers are graduates.
(c) All graduates are managers.
(d) No manager is a graduate.

**Q45.** **Statement:** Sales of electric cars in the country have doubled over the past two years.
Which is the most logical conclusion?
(a) Petrol cars will disappear within five years.
(b) Consumer demand for electric cars is growing.
(c) Electric cars are now cheaper than petrol cars.
(d) The government has banned petrol cars.

**Q46.** **Argument:** Since the new traffic regulations were introduced, road accidents in the city have fallen by 40%. The regulations are therefore working.
Which assumption is **required** by this argument?
(a) The regulations are popular with drivers.
(b) No other significant factor contributed to the reduction in accidents.
(c) Accidents will continue to fall.
(d) Other cities should adopt the same regulations.

**Q47.** **Statement:** A restaurant advertises that half of its customers return within a month, and claims this proves a high level of customer satisfaction.
Which of the following, if true, would most **weaken** the restaurant's claim?
(a) The restaurant recently expanded its menu.
(b) It is the only restaurant within a ten-kilometre radius.
(c) The restaurant has been operating for five years.
(d) Its prices are comparable to those of similar establishments.

**Q48.** **Statement:** "Attend our two-day seminar to improve your interview skills." — an advertisement by a training company.
**Assumptions:** I. Some people wish to improve their interview skills.  II. The seminar is capable of improving interview skills.
```
(a) Only I is implicit   (b) Only II is implicit
(c) Either is implicit   (d) Neither is implicit
(e) Both are implicit
```

**Q49.** I. A technology company announced the retrenchment of 200 employees.
II. The company's quarterly financial results showed a widening operating loss.
```
(a) I is the cause and II is its effect
(b) II is the cause and I is its effect
(c) Both are effects of a common cause
(d) Both are independent causes
```

**Q50.** **Statement:** A software vendor claims that its new product reduces document-processing time by 60%.
Which of the following would most **strengthen** this claim?
(a) The product has an attractive user interface.
(b) An independent audit firm measured processing times before and after deployment and confirmed a 60% reduction.
(c) The vendor has been in business for twenty years.
(d) Several clients have expressed interest in the product.

---

## 7. Detailed Solutions

### PART A — DATA SUFFICIENCY: Solutions 1–25

---

**Q1. Value of x? I. x + 5 = 12  II. 2x = 14 → (d)**

**Statement I alone:** x = 7 ⇒ unique ⇒ **sufficient** ✅
**Statement II alone:** x = 7 ⇒ unique ⇒ **sufficient** ✅

Both alone are sufficient.

**Answer: (d) Each statement alone is sufficient**

---

**Q2. Area of a rectangle? I. l = 10  II. Perimeter = 30 → (c)**

**Statement I alone:** length known, breadth unknown ⇒ **insufficient** ❌
**Statement II alone:** l + b = 15, many possibilities ⇒ **insufficient** ❌

**Together:** 10 + b = 15 ⇒ b = 5 ⇒ area = 50 cm² ⇒ **sufficient** ✅

**Answer: (c) Both together are sufficient, neither alone**

---

**Q3. Is n even? I. n divisible by 4  II. n > 10 → (a)**

**Statement I alone:** every multiple of 4 is even ⇒ definite **Yes** ⇒ **sufficient** ✅
**Statement II alone:** n could be 11 (odd) or 12 (even) ⇒ **insufficient** ❌

**Answer: (a) Statement I alone is sufficient**

---

**Q4. A's age? I. A = B + 5  II. B = 20 → (c)**

**Statement I alone:** relative only ⇒ **insufficient** ❌
**Statement II alone:** tells us nothing about A ⇒ **insufficient** ❌

**Together:** A = 20 + 5 = 25 ⇒ **sufficient** ✅

**Answer: (c) Both together are sufficient**

---

**Q5. Value of x + y? I. x = 3  II. y = 5 → (c)**

**Statement I alone:** y unknown ⇒ ❌
**Statement II alone:** x unknown ⇒ ❌
**Together:** 3 + 5 = 8 ⇒ ✅

**Answer: (c) Both together are sufficient**

---

**Q6. Is x > 0? I. x² = 16  II. x³ = 64 → (b)**

**Statement I alone:**
$$x^2 = 16 \implies x = +4 \text{ or } -4$$
The answer could be yes or no ⇒ **insufficient** ❌

**Statement II alone:**
$$x^3 = 64 \implies x = 4 \text{ only}$$
*(A cube preserves sign — a negative number cubed is negative, so −4 is impossible.)*
⇒ definite **Yes** ⇒ **sufficient** ✅

**Answer: (b) Statement II alone is sufficient**

> **The key distinction:** even powers lose the sign; odd powers preserve it. x² = k gives two roots; x³ = k gives one.

---

**Q7. Average speed? I. Distance 300 km  II. Time 5 hours → (c)**

**Statement I alone:** no time ⇒ ❌
**Statement II alone:** no distance ⇒ ❌
**Together:** 300/5 = 60 km/h ⇒ ✅

**Answer: (c) Both together are sufficient**

---

**Q8. Number of students? I. 60% are boys  II. 24 girls → (c)**

**Statement I alone:** a proportion with no absolute figure ⇒ ❌
**Statement II alone:** the girls' count without their share ⇒ ❌

**Together:** if 60% are boys, girls are 40%.
$$0.40 \times \text{Total} = 24 \implies \text{Total} = 60$$
⇒ **sufficient** ✅

**Answer: (c) Both together are sufficient**

---

**Q9. Profit percentage? I. CP = ₹200  II. SP = ₹250 → (c)**

**Statement I alone:** no selling price ⇒ ❌
**Statement II alone:** no cost price ⇒ ❌

**Together:**
$$\frac{250 - 200}{200} \times 100 = 25\%$$
⇒ **sufficient** ✅

**Answer: (c) Both together are sufficient**

---

**Q10. Day of arrival? I. After Tue, before Fri  II. Not Wednesday → (c)**

**Statement I alone:** Wednesday or Thursday ⇒ two possibilities ⇒ ❌
**Statement II alone:** rules out one day of seven ⇒ ❌

**Together:** from {Wed, Thu}, remove Wed ⇒ **Thursday** ⇒ **sufficient** ✅

**Answer: (c) Both together are sufficient**

---

**Q11. The two-digit number? I. Digit sum is 9  II. Divisible by 9 → (e)**

**Statement I alone:** 18, 27, 36, 45, 54, 63, 72, 81, 90 ⇒ **insufficient** ❌

**Statement II alone:** a two-digit number divisible by 9 is exactly one of the same nine numbers ⇒ **insufficient** ❌

**Together:** the two statements are **logically equivalent** (a number is divisible by 9 precisely when its digit sum is a multiple of 9). Combining them adds nothing ⇒ still nine candidates ⇒ **insufficient** ❌

**Answer: (e) Both together are not sufficient**

> **Watch for equivalent statements.** When two statements say the same thing, combining them cannot help. Recognising the equivalence saves you from wrongly choosing (c).

---

**Q12. Is the triangle right-angled? I. Sides 3, 4, 5  II. One angle is 90° → (d)**

**Statement I alone:**
$$3^2 + 4^2 = 9 + 16 = 25 = 5^2$$
By the converse of Pythagoras' theorem, the triangle **is** right-angled ⇒ definite **Yes** ⇒ **sufficient** ✅

**Statement II alone:** a 90° angle is the definition of a right-angled triangle ⇒ definite **Yes** ⇒ **sufficient** ✅

**Answer: (d) Each statement alone is sufficient**

---

**Q13. Simple interest? I. P = ₹5,000 at 8% p.a.  II. Period = 3 years → (c)**

**Statement I alone:** no time period ⇒ ❌
**Statement II alone:** no principal or rate ⇒ ❌

**Together:**
$$SI = \frac{5000 \times 8 \times 3}{100} = ₹1{,}200$$
⇒ **sufficient** ✅

**Answer: (c) Both together are sufficient**

---

**Q14. Tallest of A, B, C? I. A > B  II. C > A → (c)**

**Statement I alone:** says nothing about C ⇒ ❌
**Statement II alone:** says nothing about B ⇒ ❌

**Together:**
$$C > A > B \implies \textbf{C is tallest}$$
⇒ **sufficient** ✅

**Answer: (c) Both together are sufficient**

---

**Q15. Value of x? I. Prime between 10 and 20  II. x is odd → (e)**

**Statement I alone:** 11, 13, 17, 19 ⇒ four candidates ⇒ ❌
**Statement II alone:** infinitely many odd numbers ⇒ ❌

**Together:** all four primes in that range are already odd, so statement II eliminates nothing ⇒ still four candidates ⇒ **insufficient** ❌

**Answer: (e) Both together are not sufficient**

> **A statement that eliminates nothing adds nothing.** Statement II is implied by statement I, so combining them is pointless.

---

**Q16. Days for A and B together? I. A alone 12 days  II. B alone 18 days → (c)**

**Statement I alone:** B's rate unknown ⇒ ❌
**Statement II alone:** A's rate unknown ⇒ ❌

**Together:**
$$T = \frac{12 \times 18}{12 + 18} = \frac{216}{30} = 7.2 \text{ days}$$
⇒ **sufficient** ✅

**Answer: (c) Both together are sufficient**

---

**Q17. Code for "good"? I. "good boy" = "ta la"  II. "good girl" = "ta ma" → (c)**

**Statement I alone:** "ta" and "la" map to "good" and "boy" in some order ⇒ **insufficient** ❌
**Statement II alone:** "ta" and "ma" map to "good" and "girl" in some order ⇒ **insufficient** ❌

**Together:** the common code word is **"ta"** and the common meaning is **"good"**.
$$\implies \textbf{ta} = \textbf{good}$$
⇒ **sufficient** ✅

**Answer: (c) Both together are sufficient**

---

**Q18. Is n divisible by 6? I. n divisible by 2  II. n divisible by 3 → (c)**

**Statement I alone:** n = 4 is divisible by 2 but not by 6 ⇒ ❌
**Statement II alone:** n = 9 is divisible by 3 but not by 6 ⇒ ❌

**Together:** divisible by both 2 and 3, which are co-prime ⇒ divisible by 6 ⇒ definite **Yes** ⇒ **sufficient** ✅

**Answer: (c) Both together are sufficient**

---

**Q19. Average of five numbers? I. Sum = 200  II. Largest = 60 → (a)**

**Statement I alone:**
$$\text{Average} = \frac{200}{5} = 40$$
⇒ **sufficient** ✅

**Statement II alone:** knowing only the largest value tells us nothing about the average ⇒ ❌

**Answer: (a) Statement I alone is sufficient**

> **Note that (c) is impossible here.** Once statement I is sufficient on its own, the answer must be (a) or (d).

---

**Q20. Direction of P from Q? I. P is 5 km north of R  II. R is 3 km east of Q → (c)**

**Statement I alone:** Q's position is unknown ⇒ ❌
**Statement II alone:** P's position is unknown ⇒ ❌

**Together:** place Q at the origin.
$$R = (3, 0), \qquad P = (3, 5)$$
Both coordinates positive ⇒ P is **north-east** of Q ⇒ **sufficient** ✅

**Answer: (c) Both together are sufficient**

---

**Q21. B's rank from the bottom? I. B is 7th from the top  II. 30 students → (c)**

**Statement I alone:** the class size is unknown ⇒ ❌
**Statement II alone:** B's position is unknown ⇒ ❌

**Together:**
$$\text{Rank from the bottom} = 30 - 7 + 1 = 24$$
⇒ **sufficient** ✅

**Answer: (c) Both together are sufficient**

---

**Q22. Cost of 5 pens? I. 3 pens cost ₹45  II. 1 pen costs ₹15 → (d)**

**Statement I alone:** ₹45/3 = ₹15 per pen ⇒ 5 pens cost ₹75 ⇒ **sufficient** ✅
**Statement II alone:** ₹15 per pen ⇒ 5 pens cost ₹75 ⇒ **sufficient** ✅

The two statements convey **identical information**.

**Answer: (d) Each statement alone is sufficient**

> **Equivalent statements ⇒ (d), never (c).** Option (c) requires that *neither* alone works.

---

**Q23. Is x an integer? I. x/2 is an integer  II. 2x is an integer → (a)**

**Statement I alone:**
$$\frac{x}{2} = k \text{ (integer)} \implies x = 2k$$
Twice an integer is an integer ⇒ definite **Yes** ⇒ **sufficient** ✅

**Statement II alone:**
$$2x = m \text{ (integer)} \implies x = \frac{m}{2}$$
If m = 4, x = 2 (integer). If m = 3, x = 1.5 (**not** an integer).
Both outcomes are possible ⇒ **insufficient** ❌

**Answer: (a) Statement I alone is sufficient**

---

**Q24. Days for 10 men? I. 5 men take 12 days  II. Work needs 60 man-days → (d)**

**Statement I alone:**
$$\text{Total work} = 5 \times 12 = 60 \text{ man-days} \implies \frac{60}{10} = 6 \text{ days}$$
⇒ **sufficient** ✅

**Statement II alone:**
$$\frac{60}{10} = 6 \text{ days}$$
⇒ **sufficient** ✅

**Answer: (d) Each statement alone is sufficient**

---

**Q25. Ratio of milk to water? I. Mixture is 40 L  II. It contains 10 L water → (c)**

**Statement I alone:** the composition is unknown ⇒ ❌
**Statement II alone:** the total is unknown, so the milk quantity is unknown ⇒ ❌

**Together:**
$$\text{Milk} = 40 - 10 = 30 \text{ L} \implies \text{Milk : Water} = 30 : 10 = 3 : 1$$
⇒ **sufficient** ✅

**Answer: (c) Both together are sufficient**

---

### PART B — CRITICAL REASONING: Solutions 26–50

---

**Q26. Shampoo advertisement. → (e) Both are implicit**

**Assumption I — "People want silky, healthy hair."**
*Negation:* "People do not want silky, healthy hair."
The advertisement would then appeal to nobody and be pointless ⇒ **implicit** ✅

**Assumption II — "The shampoo is effective."**
*Negation:* "The shampoo does not produce silky hair."
The advertisement's core promise would be empty ⇒ **implicit** ✅

**Answer: (e) Both I and II are implicit**

---

**Q27. Salary increase of 10%. → (e) Both are implicit**

**Assumption I — "The company has the funds."**
*Negation:* "The company cannot afford it."
The decision would be impossible to implement ⇒ **implicit** ✅

**Assumption II — "Employees will be motivated."**
*Negation:* "Employees will not be motivated by the increase."
The rationale for granting the raise disappears — organisations raise pay expecting a positive response ⇒ **implicit** ✅

**Answer: (e) Both I and II are implicit**

---

**Q28. Notice about the lift. → (e) Both are implicit**

**Assumption I — "The lift may stop during a power failure."**
*Negation:* "The lift works normally during power failures."
The notice would be pointless ⇒ **implicit** ✅

**Assumption II — "People generally use the lift."**
*Negation:* "Nobody uses the lift."
There would be no reason to post the notice ⇒ **implicit** ✅

**Answer: (e) Both I and II are implicit**

---

**Q29. Ban on smoking in public places. → (e) Both are implicit**

**Assumption I — "Smoking in public places is harmful."**
*Negation:* "It is harmless."
The ban would have no justification ⇒ **implicit** ✅

**Assumption II — "People will comply."**
*Negation:* "Nobody will comply."
The ban would be futile — governments impose bans expecting at least partial compliance ⇒ **implicit** ✅

**Answer: (e) Both I and II are implicit**

---

**Q30. Laptop warranty advertisement. → (a) Only I is implicit**

**Assumption I — "Warranty terms influence buying decisions."**
*Negation:* "Warranty terms have no bearing on purchase decisions."
Advertising the warranty would then be pointless ⇒ **implicit** ✅

**Assumption II — "All competing brands offer shorter warranties."**
*Negation:* "Some competitors offer equally long or longer warranties."
The advertisement still makes perfect sense — a company can promote its own warranty without any claim about rivals ⇒ **not implicit** ✗

**Answer: (a) Only assumption I is implicit**

> **Comparative claims are rarely implicit.** Promoting a feature does not assume that no competitor has it. Watch for the word "all" in a proposed assumption — it usually signals an overreach.

---

**Q31. Flooding in low-lying districts. → (a) Only I follows**

**Course I — "Dispatch relief teams immediately."**
- Relevant ✅ · Feasible ✅ · Proportionate ✅
⇒ **follows** ✓

**Course II — "Permanently relocate residents."**
- Extreme and disproportionate to a single week of flooding
- Enormously costly and impractical
⇒ **does not follow** ✗

**Answer: (a) Only course of action I follows**

---

**Q32. High failure rate in the entrance examination. → (a) Only I follows**

**Course I — "Review and improve preparatory coaching."**
- Addresses a plausible cause of the failures
- Feasible and proportionate
⇒ **follows** ✓

**Course II — "Abolish the entrance examination."**
- Extreme; a high failure rate is not a reason to abandon selection altogether
- Removes the assessment rather than addressing the preparation
⇒ **does not follow** ✗

**Answer: (a) Only course of action I follows**

---

**Q33. Deteriorating air quality. → (a) Only I follows**

**Course I — "Tighten and enforce industrial emission standards."**
- Directly targets a major source of pollution
- Standard, feasible regulatory action
⇒ **follows** ✓

**Course II — "Ban all private vehicles permanently."**
- The word "all" and "permanently" make it extreme
- Would paralyse the city; disproportionate
⇒ **does not follow** ✗

**Answer: (a) Only course of action I follows**

---

**Q34. Sales rose 30% after a new campaign. What weakens it? → (b)**

**Step 1 — Identify the gap.**
The argument assumes **nothing else** caused the sales rise.

**Step 2 — Evaluate the options.**

| Option | Assessment |
|---|---|
| (a) The campaign was expensive | **Irrelevant** — cost says nothing about causation |
| **(b) A competitor withdrew from the market** | **Supplies an alternative cause** ⇒ weakens strongly ✅ |
| (c) Sales rose in the same quarter last year | Suggests seasonality — a mild weakener, but far less direct than (b) |
| (d) The campaign was praised | If anything, **strengthens** the argument |

**Answer: (b) A major competitor withdrew from the market during the same quarter**

> **Option (c) deserves a second look.** It hints at a seasonal pattern, which is a genuine alternative explanation — but it says only that sales "also rose", not that they rose by a comparable amount. Option (b) identifies a specific, substantial competing cause in the same period, so it weakens the conclusion far more decisively.

---

**Q35. Home workers are more productive. What strengthens it? → (b)**

**Step 1 — Identify what the claim needs.**
It needs **direct evidence of productivity**, not of satisfaction or convenience.

**Step 2 — Evaluate the options.**

| Option | Assessment |
|---|---|
| (a) Higher job satisfaction | Satisfaction ≠ productivity ✗ |
| **(b) A controlled study found 20% more tasks completed** | **Direct, quantified, controlled evidence** ✅ |
| (c) Offices are noisy | Offers a *mechanism* but no evidence of the outcome ✗ |
| (d) Commuting is tiring | Same problem — plausible mechanism, no measurement ✗ |

**Answer: (b) A controlled study found that home-based employees completed 20% more assigned tasks per week**

> **Prefer direct measurement over plausible mechanism.** Options (c) and (d) explain *why* the claim might be true; only (b) provides evidence that it *is*.

---

**Q36. Onion prices rose; heavy rainfall damaged the crop. → (b)**

**Time test:** the rainfall and crop damage precede the price rise ✓
**Mechanism test:** reduced supply → higher prices — a textbook causal pathway ✓
**Direction test:** could high onion prices cause rainfall? Clearly not ✓

$$\implies \text{II is the cause; I is the effect}$$

**Answer: (b) II is the cause and I is its effect**

---

**Q37. Schools closed; cyclone warning issued. → (b)**

**Time test:** the warning is issued first; the closure follows ✓
**Mechanism test:** authorities close institutions in response to weather alerts ✓
**Direction test:** closing schools cannot cause a cyclone warning ✓

$$\implies \text{II is the cause; I is the effect}$$

**Answer: (b) II is the cause and I is its effect**

---

**Q38. Should examinations be abolished? → (b) Only II is strong**

**Argument I — "Yes, because they cause stress."**
Stress is a real consideration, but it is not decisive: almost every form of assessment causes some stress, and the argument offers no alternative. It identifies a drawback without weighing it against the purpose examinations serve.
⇒ **weak** ✗

**Argument II — "No, they provide a structured measure of learning."**
This addresses the core function of examinations and identifies what would be lost by abolishing them. Substantial and directly relevant.
⇒ **strong** ✓

**Answer: (b) Only argument II is strong**

---

**Q39. Should public transport be free? → (e) Both are strong**

**Argument I — "Yes, it would reduce private vehicle use and lower pollution."**
Identifies a specific, substantial and plausible public benefit ⇒ **strong** ✓

**Argument II — "No, it would impose a substantial recurring cost on the exchequer."**
Identifies a specific, substantial and real financial constraint ⇒ **strong** ✓

Both arguments engage the actual policy trade-off from opposite sides.

**Answer: (e) Both arguments I and II are strong**

> **Both sides can be strong.** A strong argument need not be the winning one — only relevant and substantial. Questions of genuine policy trade-off often produce two strong arguments.

---

**Q40. Should mobile phones be banned in classrooms? → (a) Only I is strong**

**Argument I — "Yes, they distract students from learning."**
Identifies a concrete, relevant harm to the classroom's core purpose ⇒ **strong** ✓

**Argument II — "No, students enjoy using them."**
An appeal to mere preference. Enjoyment is not a relevant criterion for classroom policy ⇒ **weak** ✗

**Answer: (a) Only argument I is strong**

---

**Q41. Revenue +15%, profit −5%. What can be inferred? → (b)**

**The arithmetic.**
$$\text{Profit} = \text{Revenue} - \text{Costs}$$

If revenue rose 15% but profit fell, costs must have risen by **more than** revenue did — in both absolute and proportional terms.

| Option | Assessment |
|---|---|
| (a) Sold fewer units | Not inferable — revenue rose; prices might have changed ✗ |
| **(b) Costs rose faster than revenue** | **Arithmetically necessary** ✅ |
| (c) Poorly managed | A judgement, not an inference ✗ |
| (d) Competitors did better | No information about competitors ✗ |

**Answer: (b) Costs rose faster than revenue**

---

**Q42. All who completed training got a certificate; Rahul got none. → (b)**

**Formalise:**
$$\text{Completed training} \implies \text{Received certificate}$$
Given: Rahul did **not** receive a certificate.

**Apply the contrapositive:**
$$\neg\text{Certificate} \implies \neg\text{Completed training}$$

| Option | Assessment |
|---|---|
| (a) Not an employee | Unsupported ✗ |
| **(b) Did not complete the training** | **Contrapositive — valid** ✅ |
| (c) Failed the training | Overstates — he may never have attended ✗ |
| (d) Training was not held | Contradicted by the statement ✗ |

**Answer: (b) Rahul did not complete the safety training**

---

**Q43. If it rains, the match is cancelled. The match was not cancelled. → (b)**

**Formalise:**
$$\text{Rain} \implies \text{Cancelled}$$
Given: **not** cancelled.

**Apply the contrapositive:**
$$\neg\text{Cancelled} \implies \neg\text{Rain}$$

$$\implies \textbf{It did not rain}$$

**Answer: (b) It did not rain**

> **This is *modus tollens*, and it is always valid.** Contrast it with the invalid form: "the match was cancelled ⇒ it rained" — the match could have been cancelled for another reason entirely.

---

**Q44. Some managers are engineers; all engineers are graduates. → (b)**

**Apply the syllogism rule:** Some A are B + All B are C ⇒ **Some A are C**.

Those managers who are engineers must be graduates.

| Option | Assessment |
|---|---|
| (a) All managers are graduates | Only *some* managers are engineers ✗ |
| **(b) Some managers are graduates** | **Valid (Rule 3)** ✅ |
| (c) All graduates are managers | Invalid conversion ✗ |
| (d) No manager is a graduate | Contradicted ✗ |

**Answer: (b) Some managers are graduates**

---

**Q45. Electric car sales have doubled. Most logical conclusion? → (b)**

| Option | Assessment |
|---|---|
| (a) Petrol cars will disappear in five years | Wild extrapolation ✗ |
| **(b) Consumer demand is growing** | **Directly supported — doubled sales mean more buyers** ✅ |
| (c) Electric cars are now cheaper | Price is not mentioned ✗ |
| (d) Petrol cars have been banned | No evidence ✗ |

**Answer: (b) Consumer demand for electric cars is growing**

> **Prefer the modest conclusion.** Options that predict the future or assert a specific cause go beyond the evidence. The correct inference restates what the data logically implies and no more.

---

**Q46. New traffic rules; accidents fell 40%. Required assumption? → (b)**

**Step 1 — Identify the argument's structure.**
$$\text{Rules introduced} \; \to \; \text{Accidents fell 40\%} \; \to \; \text{Therefore the rules work}$$

**Step 2 — Find the necessary link.**
The conclusion holds only if the reduction is attributable to the rules — i.e. **nothing else** caused it.

**Step 3 — Apply the negation test to option (b).**
*Negation:* "Another significant factor did contribute to the reduction."
The argument's conclusion would no longer follow ⇒ the assumption is **required** ✅

| Option | Assessment |
|---|---|
| (a) The rules are popular | Popularity ≠ effectiveness ✗ |
| **(b) No other significant factor contributed** | **Required** ✅ |
| (c) Accidents will keep falling | A prediction, not an assumption ✗ |
| (d) Other cities should adopt them | A recommendation, not an assumption ✗ |

**Answer: (b) No other significant factor contributed to the reduction in accidents**

---

**Q47. Half of customers return; the restaurant claims high satisfaction. What weakens it? → (b)**

**Step 1 — Identify the assumed link.**
The claim assumes customers return **because they are satisfied**.

**Step 2 — Find the alternative explanation.**

| Option | Assessment |
|---|---|
| (a) Expanded menu | Neutral or mildly strengthening ✗ |
| **(b) Only restaurant within 10 km** | **Customers may return from lack of choice, not satisfaction** ✅ |
| (c) Operating five years | Irrelevant to why customers return ✗ |
| (d) Comparable prices | Irrelevant ✗ |

**Answer: (b) It is the only restaurant within a ten-kilometre radius**

> **The pattern to recognise:** the argument reads "behaviour X ⇒ attitude Y". The weakener supplies a **different reason for behaviour X**. Here, monopoly explains repeat visits without any satisfaction at all.

---

**Q48. Interview-skills seminar advertisement. → (e) Both are implicit**

**Assumption I — "Some people wish to improve their interview skills."**
*Negation:* "Nobody wishes to improve their interview skills."
The advertisement would have no audience ⇒ **implicit** ✅

**Assumption II — "The seminar is capable of improving interview skills."**
*Negation:* "The seminar cannot improve interview skills."
The advertisement's promise would be hollow ⇒ **implicit** ✅

**Answer: (e) Both are implicit**

> **Note the careful wording of assumption I:** "*Some* people wish to…" rather than "all people". Moderate phrasing survives the negation test; extreme phrasing usually does not.

---

**Q49. 200 employees retrenched; quarterly losses widened. → (b)**

**Time test:** losses appear in the quarterly results, which precede and prompt the workforce decision ✓
**Mechanism test:** deteriorating finances → cost-cutting → retrenchment. A standard corporate sequence ✓
**Direction test:** could retrenching 200 employees have *caused* the widening loss? Redundancy payments are a one-off cost, but the fundamental driver runs the other way — companies cut staff **because** results are poor ✓

$$\implies \text{II is the cause; I is the effect}$$

**Answer: (b) II is the cause and I is its effect**

---

**Q50. Software claims a 60% reduction. What strengthens it? → (b)**

| Option | Assessment |
|---|---|
| (a) Attractive interface | Irrelevant to processing speed ✗ |
| **(b) Independent audit confirmed a 60% reduction** | **Third-party, quantified, before-and-after verification** ✅ |
| (c) Twenty years in business | Longevity ≠ product performance ✗ |
| (d) Clients expressed interest | Interest ≠ evidence of the claim ✗ |

**Answer: (b) An independent audit firm measured processing times before and after deployment and confirmed a 60% reduction**

> **The strongest evidence has three features:** it is **independent** (not the vendor's own claim), **quantified** (matches the specific figure), and **comparative** (before and after). Option (b) has all three.

---

## 8. Quick Revision Sheet

> **One page. Read 48 hours after study, and again the night before the test.**

### DATA SUFFICIENCY

```
THE OPTIONS
(a) I alone sufficient, II not
(b) II alone sufficient, I not
(c) BOTH together sufficient, NEITHER alone
(d) EACH alone sufficient
(e) Both together NOT sufficient

⭐ THE PROCEDURE
1.  Read the QUESTION precisely
2.  COVER statement II — judge I alone → ✅ or ❌
3.  COVER statement I  — judge II alone → ✅ or ❌
4.  Read off the table
5.  Only if both ❌, combine and re-test

    I    II    ANSWER
    ✅   ✅     (d)
    ✅   ❌     (a)
    ❌   ✅     (b)
    ❌   ❌     combine → (c) or (e)

DO NOT SOLVE. Only decide whether a UNIQUE answer exists.
```

**Traps**

```
x² = k    →  TWO values  →  usually insufficient
x³ = k    →  ONE value   →  sufficient
Equivalent statements  →  (d), never (c)
A statement that eliminates nothing  →  adds nothing
A definite "NO" IS sufficient
If I alone suffices, (c) is IMPOSSIBLE
Ratio without a total → insufficient
One data point without a rate → insufficient
```

### CRITICAL REASONING

**Statement–Assumption — the negation test**

```
Negate the proposed assumption.
    Statement collapses  →  IMPLICIT ✅
    Statement survives   →  NOT implicit ✗

Assumptions must be NECESSARY, not merely plausible.
Comparative claims ("all competitors are worse") are rarely implicit.
Extreme words (all, only, never) usually signal a wrong option.
```

**Statement–Conclusion — the valid forms**

```
VALID
    If P then Q; P true   ⇒  Q true       (modus ponens)
    If P then Q; Q false  ⇒  P false      (contrapositive)

INVALID
    If P then Q; Q true   ⇏  P true
    If P then Q; P false  ⇏  Q false
```

**Course of Action**

```
✅ relevant · feasible · proportionate
❌ extreme (ban all / abolish / permanently) · impractical
   · addresses a different problem · restates the problem
```

**Statement–Argument**

```
✅ STRONG: directly relevant · establishes a real consequence · substantial
❌ WEAK:   restates the question · mere preference ("people like it")
           · unrelated · trivial

Both arguments CAN be strong when a genuine trade-off exists.
```

**Cause and Effect**

```
1.  TIME — the cause comes first
2.  MECHANISM — is there a plausible pathway?
3.  DIRECTION — could the arrow reverse?
4.  THIRD FACTOR — could a common cause explain both?
```

**Strengthen / Weaken**

```
Find the GAP between evidence and conclusion.

WEAKEN     →  supply an ALTERNATIVE CAUSE
              or show the effect would have happened anyway
STRENGTHEN →  rule out alternatives
              or supply direct, quantified, independent evidence

For "X then Y, so X caused Y", ALWAYS ask:
    □ Could Y have happened anyway?
    □ Could something else have caused Y?
    □ Could Y have caused X?
    □ Could a third factor have caused both?
```

**Inference**

```
✅ a direct logical consequence of the STATED facts
❌ needs outside knowledge · overstates ("all", "proves")
   · predicts the future · merely restates the passage

Prefer the MODEST conclusion over the dramatic one.
```

---

## 9. Common Mistakes

| # | Mistake | Example | Correction |
|---|---|---|---|
| 1 | **Solving instead of deciding** | Computing the full answer | Only test whether a unique answer exists |
| 2 | **Statement I leaks into II** | Judging II with I in mind | **Cover** statement I physically |
| 3 | **A definite "no" called insufficient** | "n divisible by 4" for "is n odd?" | A definite No is an answer |
| 4 | **Even powers' sign ignored** | x² = 16 ⇒ x = 4 | x = ±4 ⇒ insufficient |
| 5 | **Equivalent statements marked (c)** | "3 pens ₹45" and "1 pen ₹15" | Same information ⇒ (d) |
| 6 | **(c) chosen when I alone suffices** | Both used unnecessarily | (c) requires *neither* alone to work |
| 7 | **Plausible taken as implicit** | "Competitors are worse" | Apply the negation test |
| 8 | **Contrapositive vs converse confused** | Q true ⇒ P true | Only ¬Q ⇒ ¬P is valid |
| 9 | **Extreme course of action accepted** | "Ban all vehicles" | Must be proportionate |
| 10 | **Preference treated as an argument** | "Students like phones" | Preference is not relevant grounds |
| 11 | **Correlation read as causation** | X then Y ⇒ X caused Y | Test for alternative causes |
| 12 | **Mechanism accepted as evidence** | "Offices are noisy" | Prefer direct measurement |
| 13 | **Inference overreaches** | "Petrol cars will vanish" | Stay within the stated facts |
| 14 | **Irrelevant strengtheners chosen** | "The vendor is 20 years old" | Evidence must address the claim itself |

---

## Practice Answer Key

| Q | Ans | Q | Ans | Q | Ans | Q | Ans | Q | Ans |
|---|---|---|---|---|---|---|---|---|---|
| 1 | d | 11 | e | 21 | c | 31 | a | 41 | b |
| 2 | c | 12 | d | 22 | d | 32 | a | 42 | b |
| 3 | a | 13 | c | 23 | a | 33 | a | 43 | b |
| 4 | c | 14 | c | 24 | d | 34 | b | 44 | b |
| 5 | c | 15 | e | 25 | c | 35 | b | 45 | b |
| 6 | b | 16 | c | 26 | e | 36 | b | 46 | b |
| 7 | c | 17 | c | 27 | e | 37 | b | 47 | b |
| 8 | c | 18 | c | 28 | e | 38 | b | 48 | e |
| 9 | c | 19 | a | 29 | e | 39 | e | 49 | b |
| 10 | c | 20 | c | 30 | a | 40 | a | 50 | b |

**Scoring guide:** 42+/50 → strong. 32–41 → solid; drill the cover-up technique and the negation test until both are automatic. Below 32 → these are *format* problems, not reasoning problems. Re-read Sections 2.2 and 3.1, then redo the set.

---

**⬅️ Back:** [Topic 17 — Syllogisms & Venn Diagrams](17-syllogisms-venn-diagrams.md) · **➡️ Next:** [Topic 19 — Cubes, Dice & Non-verbal Reasoning](19-nonverbal-cubes-dice-figures.md)
