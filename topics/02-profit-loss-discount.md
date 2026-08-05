# Topic 2 — Profit, Loss & Discount

### EY Placement Aptitude Handbook · Priority Rank #3 · 🔴 Critical

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

**Weightage:** 10–12% of the quantitative section — typically **1–2 direct questions**.

**Why EY likes it:** the topic is commercially flavoured (margins, discounts, markups), which fits a professional-services assessment. It also blends naturally with percentages, ratios, and DI.

**Question styles reported:**

| Style | Frequency | Example shape |
|---|---|---|
| Direct profit/loss % | Very high | "CP ₹400, SP ₹500 — find profit%" |
| Reverse (find CP from SP + %) | Very high | "SP ₹660 at 10% profit — find CP" |
| Markup + discount chains | High | "Marked 30% above cost, 10% discount — find profit%" |
| Successive discounts | High | "10% then 20% — single equivalent discount?" |
| Two articles, equal SP, ±x% | High | "Sold at ₹1200 each, +20% and −20%" |
| False weights / dishonest dealer | Medium | "Uses 900 g weight for 1 kg" |
| "CP of m articles = SP of n articles" | Medium | Pure ratio manipulation |
| Mixture then sale | Medium | Blend two grades, sell at one price |

**Prerequisite:** [Topic 1 — Percentages](01-percentages.md). Everything here is a percentage problem with commercial vocabulary attached.

---

## 2. Core Concepts

### 2.1 The four quantities

| Symbol | Name | Meaning |
|---|---|---|
| **CP** | Cost Price | What the seller paid (including any purchase-side expenses) |
| **SP** | Selling Price | What the buyer actually paid |
| **MP** | Marked Price (list price, printed price) | The advertised price *before* discount |
| **D** | Discount | The reduction from MP |

The chain runs in this order:

```
      CP  ──── markup ────►  MP  ──── discount ────►  SP
      │                                                │
      └──────────── profit or loss ────────────────────┘
```

**Two separate percentage systems operate here, and mixing them is the #1 source of error:**

| Percentage | Calculated ON |
|---|---|
| **Profit % and Loss %** | **CP** |
| **Markup %** | **CP** |
| **Discount %** | **MP** |

Profit is never a percentage of SP. Discount is never a percentage of CP.

### 2.2 Profit and loss

$$\text{Profit} = SP - CP \qquad \text{(when } SP > CP\text{)}$$
$$\text{Loss} = CP - SP \qquad \text{(when } CP > SP\text{)}$$

$$\text{Profit \%} = \frac{SP - CP}{CP} \times 100 \qquad \text{Loss \%} = \frac{CP - SP}{CP} \times 100$$

**The multiplier form (use this — it is faster and error-proof):**

$$SP = CP \times \left(1 + \frac{\text{Profit\%}}{100}\right) \qquad SP = CP \times \left(1 - \frac{\text{Loss\%}}{100}\right)$$

And crucially, to go **backwards**:

$$CP = \frac{SP}{\left(1 \pm \frac{\%}{100}\right)}$$

> **The reverse trap:** SP = ₹660 at 10% profit.
> **Wrong:** 660 − 10% of 660 = ₹594 ✗
> **Right:** 660 ÷ 1.10 = ₹600 ✓ (check: 600 × 1.10 = 660 ✓)

### 2.3 Markup

$$MP = CP \times \left(1 + \frac{\text{Markup\%}}{100}\right)$$

"Marked 40% above cost" means MP = 1.40 × CP.

### 2.4 Discount

$$\text{Discount} = MP - SP \qquad \text{Discount\%} = \frac{MP - SP}{MP} \times 100$$

$$SP = MP \times \left(1 - \frac{\text{Discount\%}}{100}\right)$$

### 2.5 The master relation

The single equation that solves most markup–discount questions:

$$\boxed{\;MP \times \left(1 - \frac{d}{100}\right) = CP \times \left(1 + \frac{p}{100}\right)\;}$$

where *d* = discount% and *p* = profit%. Both sides equal **SP**.

**Everything follows from this.** Given any three of {CP, MP, d, p}, the fourth is one rearrangement away.

**Worked instance:** Goods marked 30% above cost, sold at 10% discount. Find profit%.

Let CP = 100 ⇒ MP = 130 ⇒ SP = 130 × 0.90 = 117 ⇒ **Profit = 17%**

Or directly as multipliers: 1.30 × 0.90 = 1.17 ⇒ **17%**

### 2.6 Successive discounts

Discounts **never add**. They multiply, exactly like successive percentage changes.

$$SP = MP \times \left(1 - \frac{d_1}{100}\right)\left(1 - \frac{d_2}{100}\right)\left(1 - \frac{d_3}{100}\right)\cdots$$

**Single equivalent discount** for two discounts *a*% and *b*%:

$$D_{\text{eq}} = a + b - \frac{ab}{100}$$

**Worked:** 20% and 25%.
$$20 + 25 - \frac{20 \times 25}{100} = 45 - 5 = 40\%$$
Multiplier check: 0.80 × 0.75 = 0.60 ⇒ 40% off ✓

> **Note the minus sign.** For successive *increases* the formula was a + b + ab/100. For successive *discounts* it is a + b − ab/100, because both terms are negative and the cross-product turns positive. Same formula, signs handled correctly.

### 2.7 The equal-SP trap (a guaranteed EY favourite)

> Two articles are sold at the **same price**. One at *x*% profit, the other at *x*% loss.
> **The result is always a NET LOSS of x²/100 %.**

$$\text{Loss\%} = \frac{x^2}{100}$$

**Why (and why it is never a break-even):**

Let common SP = *S*.
$$CP_1 = \frac{S}{1 + x/100}, \qquad CP_2 = \frac{S}{1 - x/100}$$

The loss-making article had a **higher** cost price, so it contributes more to total CP than the profitable one saves. Total CP always exceeds total SP.

**Numeric check with x = 20, SP = ₹1200 each:**
- CP₁ = 1200/1.20 = ₹1000 (profit ₹200)
- CP₂ = 1200/0.80 = ₹1500 (loss ₹300)
- Total CP = ₹2500, Total SP = ₹2400 ⇒ Loss ₹100 ⇒ 100/2500 = **4%** = 20²/100 ✓

**Memorise the common cases:**

| x | Net loss |
|---|---|
| 10% | 1% |
| 15% | 2.25% |
| 20% | 4% |
| 25% | 6.25% |
| 30% | 9% |

### 2.8 False weights (dishonest dealer)

**Case A — sells at CP but gives less weight:**

$$\text{Gain\%} = \frac{\text{True weight} - \text{Weight given}}{\text{Weight given}} \times 100 = \frac{\text{Error}}{\text{True value}} \times 100$$

> Uses a 900 g weight for 1 kg: Gain% = (1000 − 900)/900 × 100 = **11 1/9 %**

**Note the denominator is the weight actually GIVEN**, because that is what the dealer's cost corresponds to.

**Case B — sells at a stated profit/loss AND cheats on weight (combined):**

$$\text{Overall multiplier} = \left(1 \pm \frac{p}{100}\right) \times \frac{\text{True weight}}{\text{Weight given}}$$

> Sells at 10% loss but gives only 800 g per kg:
> Multiplier = 0.90 × (1000/800) = 0.90 × 1.25 = **1.125 ⇒ 12.5% profit**

The safest approach is always to build a concrete numeric example rather than recall a formula — see Solved Example 8.

### 2.9 "CP of m articles = SP of n articles"

$$\text{Profit\%} = \frac{m - n}{n} \times 100$$

If *m* > *n* it is a profit; if *m* < *n* it is a loss.

**Why:** Let CP of one article = 1. Then CP of *m* articles = *m*, and this equals SP of *n* articles, so SP per article = *m/n*. Profit per article = m/n − 1 = (m − n)/n. ∎

> "CP of 15 articles = SP of 12 articles" ⇒ Profit% = (15 − 12)/12 × 100 = **25%**

### 2.10 Buy-*a*-get-*b*-free

$$\text{Discount\%} = \frac{b}{a + b} \times 100$$

The customer pays for *a* items and receives *a* + *b*.

> Buy 10, get 2 free ⇒ 2/12 × 100 = **16⅔%** discount.

---

## 3. Formula Bank

| # | Concept | Formula |
|---|---|---|
| 1 | Profit | $SP - CP$ |
| 2 | Loss | $CP - SP$ |
| 3 | Profit % | $\dfrac{SP-CP}{CP} \times 100$ |
| 4 | Loss % | $\dfrac{CP-SP}{CP} \times 100$ |
| 5 | SP from CP (profit) | $CP\left(1 + \frac{p}{100}\right)$ |
| 6 | SP from CP (loss) | $CP\left(1 - \frac{l}{100}\right)$ |
| 7 | CP from SP (profit) | $\dfrac{SP}{1 + p/100} = \dfrac{100 \times SP}{100+p}$ |
| 8 | CP from SP (loss) | $\dfrac{SP}{1 - l/100} = \dfrac{100 \times SP}{100-l}$ |
| 9 | Marked price from CP | $CP\left(1 + \frac{m}{100}\right)$ |
| 10 | SP after discount | $MP\left(1 - \frac{d}{100}\right)$ |
| 11 | Discount % | $\dfrac{MP-SP}{MP} \times 100$ |
| 12 | **Master relation** | $MP\left(1-\frac{d}{100}\right) = CP\left(1+\frac{p}{100}\right)$ |
| 13 | Two successive discounts | $D_{eq} = a + b - \dfrac{ab}{100}$ |
| 14 | Three successive discounts | $100\left[1 - (1-\tfrac{a}{100})(1-\tfrac{b}{100})(1-\tfrac{c}{100})\right]$ |
| 15 | Equal SP, +x% and −x% | Net **loss** $= \dfrac{x^2}{100}\%$ |
| 16 | CP of *m* = SP of *n* | Profit% $= \dfrac{m-n}{n} \times 100$ |
| 17 | False weight, sold at CP | Gain% $= \dfrac{\text{True wt} - \text{Given wt}}{\text{Given wt}} \times 100$ |
| 18 | False weight + profit/loss | Multiplier $= \left(1 \pm \frac{p}{100}\right)\times\dfrac{\text{True wt}}{\text{Given wt}}$ |
| 19 | Buy *a* get *b* free | Discount% $= \dfrac{b}{a+b}\times 100$ |
| 20 | Markup needed for profit *p* after discount *d* | $m = \dfrac{100(p+d)}{100-d}$ % |
| 21 | Profit when SP is *k* times CP | $(k-1) \times 100$ % |
| 22 | Equal profit and loss amounts at SP₁, SP₂ | $CP = \dfrac{SP_1 + SP_2}{2}$ |

---

## 4. Shortcuts & Tricks

### 4.1 Always assume CP = 100

Unless the question gives an actual rupee value, set **CP = 100**. Every percentage answer comes out directly and no fractions appear.

> *"Marked 25% above cost, 12% discount — find profit%"*
> CP = 100 → MP = 125 → SP = 125 × 0.88 = 110 → **Profit = 10%**

If the question involves several articles, use **CP = 100 per article** or the LCM of the article counts.

### 4.2 The multiplier chain

Write the whole problem as one product and read the answer off it.

| Statement | Multiplier |
|---|---|
| 20% profit | × 1.20 |
| 15% loss | × 0.85 |
| Marked 40% above cost | × 1.40 |
| 25% discount | × 0.75 |
| Two discounts 10%, 20% | × 0.90 × 0.80 |

> *"Marked 60% above cost, two discounts of 20% and 25%"*
> 1.60 × 0.80 × 0.75 = **0.96** ⇒ a **4% loss**.

One line, no intermediate values, no sign errors.

### 4.3 Ratio thinking for "CP of m = SP of n"

$$\frac{SP}{CP} = \frac{m}{n}$$

Then profit% = (m/n − 1) × 100.

| Statement | SP : CP | Result |
|---|---|---|
| CP of 15 = SP of 12 | 15 : 12 = 5 : 4 | 25% profit |
| CP of 12 = SP of 9 | 12 : 9 = 4 : 3 | 33⅓% profit |
| CP of 20 = SP of 25 | 20 : 25 = 4 : 5 | 20% loss |
| CP of 8 = SP of 10 | 8 : 10 = 4 : 5 | 20% loss |

### 4.4 The "equal difference" shortcut

> If an article gives a **profit of ₹P when sold at SP₁** and a **loss of ₹P when sold at SP₂** (same magnitude), then:

$$CP = \frac{SP_1 + SP_2}{2}$$

> Profit at ₹56 equals loss at ₹42 ⇒ CP = (56 + 42)/2 = **₹49**

### 4.5 The "difference in SP" technique

Many questions say *"if sold for ₹X more, the profit would be y% instead of z%"*. Set it up as a difference of multipliers:

$$CP \times \left(\frac{y - z}{100}\right) = X$$

> *"Sold at 10% loss; ₹100 more would give 15% gain. Find CP."*
> $$CP \times \frac{15 - (-10)}{100} = 100 \implies CP \times 0.25 = 100 \implies CP = ₹400$$

This converts a two-equation problem into one line.

### 4.6 Markup required for a target profit

$$m\% = \frac{100(p + d)}{100 - d}$$

> *"Want 25% profit after a 20% discount. Markup?"*
> $$\frac{100(25 + 20)}{100 - 20} = \frac{4500}{80} = 56.25\%$$

Verify: CP 100 → MP 156.25 → SP = 156.25 × 0.80 = 125 ⇒ 25% profit ✓

### 4.7 Instant successive-discount table

| Discounts | Equivalent single discount |
|---|---|
| 10% + 10% | 19% |
| 10% + 20% | 28% |
| 20% + 20% | 36% |
| 20% + 25% | 40% |
| 25% + 25% | 43.75% |
| 30% + 20% | 44% |
| 10% + 20% + 25% | 46% |
| 50% + 10% | 55% |

### 4.8 Sanity checks that catch errors instantly

```
✓ Profit%  → SP must be > CP
✓ Loss%    → SP must be < CP
✓ Discount → SP must be < MP,  always
✓ MP ≥ SP  in every discount problem
✓ Equal-SP ±x% → the answer is ALWAYS a loss, never zero, never a gain
✓ Successive discounts → equivalent discount is always LESS than the sum
```

If your answer violates one of these, you have made a sign or base error. Re-check before selecting.

---

## 5. Solved Examples

### Example 1 — Basic profit percentage

**Q.** An article is bought for ₹640 and sold for ₹800. Find the profit percentage.

**Step 1 — Compute the profit.**
$$\text{Profit} = SP - CP = 800 - 640 = ₹160$$

**Step 2 — Divide by CP (never by SP).**
$$\text{Profit\%} = \frac{160}{640} \times 100$$

**Step 3 — Simplify first.**
$$\frac{160}{640} = \frac{1}{4} = 25\%$$

**Answer: 25% profit**

> **Check:** 640 × 1.25 = 800 ✓

---

### Example 2 — The reverse calculation

**Q.** By selling an article for ₹918, a shopkeeper makes a profit of 8%. What is the cost price?

**Step 1 — Recognise this is a reverse problem.** SP is given *with* the profit%; find CP.

**Step 2 — Apply the formula.**
$$CP = \frac{SP}{1 + p/100} = \frac{918}{1.08}$$

**Step 3 — Clean the arithmetic.**
$$\frac{918}{1.08} = \frac{91{,}800}{108} = 850$$

**Answer: ₹850**

**Verify:** 850 × 1.08 = 918 ✓

> **The trap:** computing 918 − 8% of 918 = 918 − 73.44 = ₹844.56. That is wrong, and the wrong value is often an option.

---

### Example 3 — Markup and discount together

**Q.** A shopkeeper marks his goods 35% above cost price and then allows a discount of 20%. Find his profit or loss percentage.

**Step 1 — Assume CP = 100.**

**Step 2 — Apply the markup.**
$$MP = 100 \times 1.35 = 135$$

**Step 3 — Apply the discount to MP (not CP).**
$$SP = 135 \times 0.80 = 108$$

**Step 4 — Compare SP to CP.**
$$\text{Profit} = 108 - 100 = 8 \implies 8\%$$

**Answer: 8% profit**

**One-line multiplier method:**
$$1.35 \times 0.80 = 1.08 \implies \textbf{8\% profit}$$

> **The trap:** subtracting 20% from 35% to get "15% profit". The discount applies to the *marked* price, which is larger than CP, so 20% of MP is more than 20% of CP.

---

### Example 4 — Successive discounts

**Q.** A jacket marked at ₹4,000 is sold after successive discounts of 25% and 12%. Find the selling price and the single equivalent discount.

**Step 1 — Apply discounts in sequence.**
$$SP = 4000 \times (1 - 0.25) \times (1 - 0.12)$$
$$= 4000 \times 0.75 \times 0.88$$

**Step 2 — Compute.**
$$4000 \times 0.75 = 3000$$
$$3000 \times 0.88 = 2640$$

**Step 3 — Find the single equivalent discount.**
$$D_{eq} = \frac{4000 - 2640}{4000} \times 100 = \frac{1360}{4000} \times 100 = 34\%$$

**Formula check:**
$$a + b - \frac{ab}{100} = 25 + 12 - \frac{25 \times 12}{100} = 37 - 3 = 34\% \checkmark$$

**Answer: SP = ₹2,640; single equivalent discount = 34%**

> **Sanity check:** 34% < 37% (the naive sum). Successive discounts always give *less* than the sum, because the second discount applies to an already-reduced amount.

---

### Example 5 — Equal selling price, opposite percentages

**Q.** A dealer sells two watches at ₹2,400 each. On one he gains 25%; on the other he loses 25%. Find his overall profit or loss.

**Step 1 — Recognise the pattern.** Equal SP, +x% and −x% ⇒ **always a net loss of x²/100 %**.

$$\text{Loss\%} = \frac{25^2}{100} = \frac{625}{100} = 6.25\%$$

**Step 2 — Verify with actual numbers.**

$$CP_1 = \frac{2400}{1.25} = ₹1920 \quad \text{(profit ₹480)}$$
$$CP_2 = \frac{2400}{0.75} = ₹3200 \quad \text{(loss ₹800)}$$

**Step 3 — Compare totals.**
$$\text{Total CP} = 1920 + 3200 = ₹5120$$
$$\text{Total SP} = 2400 \times 2 = ₹4800$$
$$\text{Net loss} = 5120 - 4800 = ₹320$$

**Step 4 — Loss percentage.**
$$\frac{320}{5120} \times 100 = 6.25\% \checkmark$$

**Answer: 6.25% loss (₹320)**

> **Why it is always a loss:** the article sold at a loss had the *higher* cost price (₹3,200 vs ₹1,920). The larger investment is the one that lost money, so the losses outweigh the gains — every time, for any x.

---

### Example 6 — Finding the required markup

**Q.** A trader wants to earn a profit of 20% after allowing a discount of 25% on the marked price. By what percentage above cost price should he mark his goods?

**Step 1 — Write the master relation.**
$$MP \times (1 - 0.25) = CP \times (1 + 0.20)$$

**Step 2 — Substitute CP = 100.**
$$MP \times 0.75 = 100 \times 1.20 = 120$$

**Step 3 — Solve for MP.**
$$MP = \frac{120}{0.75} = 160$$

**Step 4 — Express as a markup over CP = 100.**
$$\text{Markup} = 160 - 100 = 60\%$$

**Formula check:**
$$m = \frac{100(p+d)}{100-d} = \frac{100(20+25)}{75} = \frac{4500}{75} = 60\% \checkmark$$

**Answer: 60% above cost price**

---

### Example 7 — "CP of m articles = SP of n articles"

**Q.** The cost price of 18 articles equals the selling price of 15 articles. Find the profit percentage.

**Step 1 — Assume CP of one article = ₹1.**
$$\text{CP of 18 articles} = ₹18$$

**Step 2 — Set the given equality.**
$$\text{SP of 15 articles} = ₹18 \implies \text{SP of 1 article} = \frac{18}{15} = ₹1.20$$

**Step 3 — Compute profit per article.**
$$\text{Profit} = 1.20 - 1.00 = ₹0.20 \text{ on a CP of ₹1}$$
$$\text{Profit\%} = \frac{0.20}{1.00} \times 100 = 20\%$$

**Formula check:**
$$\frac{m-n}{n} \times 100 = \frac{18-15}{15} \times 100 = \frac{3}{15} \times 100 = 20\% \checkmark$$

**Answer: 20% profit**

> **Direction rule:** more articles on the CP side ⇒ profit. If it had been "CP of 15 = SP of 18", the ratio flips and it is a loss of (15−18)/18 × 100 = −16⅔%.

---

### Example 8 — Dishonest dealer with a false weight

**Q.** A grocer professes to sell rice at cost price but uses a weight of 850 g in place of 1 kg. Find his gain percentage.

**Step 1 — Build a concrete scenario.**
Let the true cost be ₹1 per gram. The customer pays for 1,000 g, i.e. ₹1,000.

**Step 2 — Identify what the grocer actually gives.**
He hands over only 850 g, which cost him **₹850**.

**Step 3 — Compute the profit.**
$$\text{Profit} = 1000 - 850 = ₹150 \text{ on a cost of ₹850}$$

**Step 4 — Profit percentage (base = his cost).**
$$\frac{150}{850} \times 100 = \frac{15000}{850} = 17.647\% \approx 17\tfrac{11}{17}\%$$

**Formula check:**
$$\frac{\text{True wt} - \text{Given wt}}{\text{Given wt}} \times 100 = \frac{1000-850}{850} \times 100 = 17.65\% \checkmark$$

**Answer: ≈ 17.65% gain (17 11/17 %)**

> **The trap:** dividing by 1,000 instead of 850, giving 15%. The dealer's *cost* corresponds to the 850 g he parted with — that is the base.

---

## 6. Practice Questions

**Instructions:** 50 questions. Easy (1–20), Medium (21–40), Hard (41–50).
Target times: Easy 30 s · Medium 60 s · Hard 90 s.
Full solutions in [Section 7](#7-detailed-solutions).

### 🟢 EASY (Questions 1–20)

**Q1.** An article costing ₹400 is sold for ₹500. Find the profit percentage.
(a) 20%  (b) 25%  (c) 30%  (d) 33⅓%

**Q2.** An article costing ₹250 is sold for ₹200. Find the loss percentage.
(a) 15%  (b) 20%  (c) 25%  (d) 30%

**Q3.** An article bought for ₹800 is sold at a profit of 15%. Find the selling price.
(a) ₹880  (b) ₹900  (c) ₹920  (d) ₹940

**Q4.** By selling an article for ₹660, a man gains 10%. Find the cost price.
(a) ₹580  (b) ₹594  (c) ₹600  (d) ₹620

**Q5.** An article costing ₹1,200 is sold at a loss of 20%. Find the selling price.
(a) ₹940  (b) ₹960  (c) ₹980  (d) ₹1,000

**Q6.** A book marked at ₹500 is sold after a 20% discount. Find the selling price.
(a) ₹380  (b) ₹390  (c) ₹400  (d) ₹420

**Q7.** An article marked at ₹800 is sold for ₹680. Find the discount percentage.
(a) 12%  (b) 15%  (c) 18%  (d) 20%

**Q8.** By selling an article for ₹450, a man loses 10%. Find the cost price.
(a) ₹480  (b) ₹495  (c) ₹500  (d) ₹520

**Q9.** A man buys 12 apples for ₹60 and sells them at ₹6 each. Find the profit percentage.
(a) 15%  (b) 18%  (c) 20%  (d) 25%

**Q10.** If the cost price of 15 articles equals the selling price of 12 articles, find the profit percentage.
(a) 20%  (b) 25%  (c) 30%  (d) 33⅓%

**Q11.** A shopkeeper sells an item for ₹1,080, gaining 20%. Find the cost price.
(a) ₹850  (b) ₹880  (c) ₹900  (d) ₹920

**Q12.** Cost price ₹720, selling price ₹900. Find the profit percentage.
(a) 20%  (b) 22%  (c) 25%  (d) 30%

**Q13.** An item marked at ₹1,000 carries successive discounts of 10% and 20%. Find the selling price.
(a) ₹700  (b) ₹710  (c) ₹720  (d) ₹730

**Q14.** Find the single discount equivalent to successive discounts of 20% and 25%.
(a) 35%  (b) 40%  (c) 45%  (d) 50%

**Q15.** An article marked at ₹1,500 is sold at a 12% discount. Find the selling price.
(a) ₹1,300  (b) ₹1,320  (c) ₹1,350  (d) ₹1,380

**Q16.** An article costing ₹500 is marked 40% above cost. Find the marked price.
(a) ₹640  (b) ₹680  (c) ₹700  (d) ₹720

**Q17.** If the selling price is twice the cost price, find the profit percentage.
(a) 50%  (b) 100%  (c) 150%  (d) 200%

**Q18.** A trader sells goods at a 5% loss. If the cost price is ₹2,400, find the selling price.
(a) ₹2,260  (b) ₹2,280  (c) ₹2,300  (d) ₹2,320

**Q19.** The profit on an article is ₹150, which is 25% of the cost price. Find the cost price.
(a) ₹500  (b) ₹550  (c) ₹600  (d) ₹650

**Q20.** The cost price of 20 pens is ₹240. At what price must each pen be sold to gain 25%?
(a) ₹13  (b) ₹14  (c) ₹15  (d) ₹16

---

### 🟡 MEDIUM (Questions 21–40)

**Q21.** A shopkeeper marks his goods 30% above cost price and allows a discount of 10%. Find his profit percentage.
(a) 15%  (b) 17%  (c) 20%  (d) 22%

**Q22.** By selling an article for ₹720, a man loses 10%. At what price should he sell it to gain 15%?
(a) ₹880  (b) ₹900  (c) ₹920  (d) ₹950

**Q23.** A man sells two articles at ₹1,200 each. On one he gains 20% and on the other he loses 20%. Find his overall profit or loss percentage.
(a) No profit no loss  (b) 4% loss  (c) 4% profit  (d) 2% loss

**Q24.** A dishonest dealer claims to sell at cost price but uses a 900 g weight for 1 kg. Find his profit percentage.
(a) 10%  (b) 11 1/9 %  (c) 12%  (d) 12.5%

**Q25.** The profit made by selling an article for ₹56 equals the loss made by selling it for ₹42. Find the cost price.
(a) ₹47  (b) ₹48  (c) ₹49  (d) ₹50

**Q26.** A shopkeeper gives a 20% discount and still earns a 20% profit. If the cost price is ₹800, find the marked price.
(a) ₹1,100  (b) ₹1,150  (c) ₹1,200  (d) ₹1,250

**Q27.** If an article is sold at a 20% profit instead of a 20% loss, the seller receives ₹200 more. Find the cost price.
(a) ₹400  (b) ₹450  (c) ₹500  (d) ₹550

**Q28.** A trader buys 100 kg of rice at ₹40/kg. He sells 40% of it at a 20% profit and the remainder at a 10% profit. Find his overall profit percentage.
(a) 12%  (b) 13%  (c) 14%  (d) 15%

**Q29.** A man sold an article at a 10% loss. Had he sold it for ₹100 more, he would have gained 15%. Find the cost price.
(a) ₹350  (b) ₹400  (c) ₹450  (d) ₹500

**Q30.** An item marked at ₹2,000 is sold after successive discounts of 10%, 20% and 25%. Find the selling price.
(a) ₹1,020  (b) ₹1,040  (c) ₹1,080  (d) ₹1,120

**Q31.** A shopkeeper wants a 25% profit after allowing a 20% discount. By what percentage above cost price should he mark his goods?
(a) 45%  (b) 50%  (c) 56.25%  (d) 62.5%

**Q32.** If the cost price of 12 articles equals the selling price of 9 articles, find the profit percentage.
(a) 25%  (b) 30%  (c) 33⅓%  (d) 40%

**Q33.** An article is sold for ₹935 at a profit of 10%. What would be the selling price for a 20% loss?
(a) ₹640  (b) ₹660  (c) ₹680  (d) ₹700

**Q34.** A trader mixes 40 kg of rice costing ₹30/kg with 60 kg costing ₹40/kg and sells the mixture at ₹45/kg. Find his profit percentage.
(a) 20%  (b) 22%  (c) 25%  (d) 28%

**Q35.** A shopkeeper offers 2 articles free on the purchase of 10 articles. Find the effective discount percentage.
(a) 15%  (b) 16⅔%  (c) 20%  (d) 25%

**Q36.** A man buys an article for ₹27.50 and sells it for ₹28.60. Find the gain percentage.
(a) 3%  (b) 3.5%  (c) 4%  (d) 4.5%

**Q37.** On selling 17 balls for ₹720, there is a loss equal to the cost price of 5 balls. Find the cost price of one ball.
(a) ₹45  (b) ₹50  (c) ₹55  (d) ₹60

**Q38.** A retailer buys 40 pens for the marked price of 36 pens. If he sells all of them at the marked price, find his profit percentage.
(a) 10%  (b) 11 1/9 %  (c) 12%  (d) 12.5%

**Q39.** An item marked at ₹1,200 is sold after successive discounts of 20% and 10%. Find the single equivalent discount and the selling price.
(a) 30%, ₹840  (b) 28%, ₹864  (c) 28%, ₹840  (d) 30%, ₹864

**Q40.** A man sells an article at a 25% profit. Had he bought it for 20% less and sold it for ₹36.75 less, he would have gained 30%. Find the cost price.
(a) ₹150  (b) ₹165  (c) ₹175  (d) ₹185

---

### 🔴 HARD (Questions 41–50)

**Q41.** A dishonest dealer sells goods at a 10% loss on cost price but uses a weight that is 20% less than the stated weight. Find his overall profit or loss percentage.
(a) 10% profit  (b) 12.5% profit  (c) 10% loss  (d) 12.5% loss

**Q42.** A man bought two horses for a total of ₹8,400. He sold one at a 20% profit and the other at a 10% loss, breaking even overall. Find the cost price of the first horse.
(a) ₹2,400  (b) ₹2,800  (c) ₹3,200  (d) ₹3,600

**Q43.** A shopkeeper marks his goods 50% above cost price. He allows a discount and still earns a 20% profit. Find the discount percentage.
(a) 15%  (b) 20%  (c) 25%  (d) 30%

**Q44.** A trader sells an article at a 25% discount on the marked price and earns a 20% profit. If instead he allows only a 10% discount, find his profit percentage.
(a) 40%  (b) 42%  (c) 44%  (d) 46%

**Q45.** A man purchases 11 oranges for ₹10 and sells 10 oranges for ₹11. Find his profit percentage.
(a) 10%  (b) 15%  (c) 20%  (d) 21%

**Q46.** Two items are each sold for ₹1,980 — one at a 10% profit and the other at a 10% loss. Find the net loss in rupees.
(a) ₹20  (b) ₹40  (c) ₹60  (d) ₹80

**Q47.** A shopkeeper sold an article at two-thirds of its marked price and incurred a loss of 10%. What profit percentage would he have made had he sold it at the marked price?
(a) 30%  (b) 33⅓%  (c) 35%  (d) 40%

**Q48.** The cost price of 20 articles equals the selling price of *x* articles. If the profit is 25%, find *x*.
(a) 14  (b) 15  (c) 16  (d) 18

**Q49.** A trader buys goods worth ₹10,000, marks them 25% above cost, and offers a discount of 8%. Find his profit percentage and profit in rupees.
(a) 15%, ₹1,500  (b) 17%, ₹1,700  (c) 15%, ₹1,250  (d) 12%, ₹1,200

**Q50.** A person sells an article at a 5% loss. Had he sold it for ₹65 more, he would have made an 8% profit. Find the cost price.
(a) ₹450  (b) ₹480  (c) ₹500  (d) ₹520

---

## 7. Detailed Solutions

### 🟢 EASY — Solutions 1–20

---

**Q1. CP ₹400, SP ₹500. Profit%? → (b) 25%**

**Formula used:** Profit% = (SP − CP)/CP × 100

**Step 1 — Profit amount.**
$$500 - 400 = ₹100$$

**Step 2 — Divide by CP.**
$$\frac{100}{400} \times 100 = \frac{1}{4} \times 100 = 25\%$$

**Check:** 400 × 1.25 = 500 ✓

**Answer: (b) 25%**

---

**Q2. CP ₹250, SP ₹200. Loss%? → (b) 20%**

**Formula used:** Loss% = (CP − SP)/CP × 100

**Step 1 — Loss amount.**
$$250 - 200 = ₹50$$

**Step 2 — Divide by CP.**
$$\frac{50}{250} \times 100 = \frac{1}{5} \times 100 = 20\%$$

> **Note:** dividing by SP (200) gives 25% — a common wrong option. The base is always CP.

**Answer: (b) 20%**

---

**Q3. CP ₹800, 15% profit. Find SP. → (c) ₹920**

**Formula used:** SP = CP(1 + p/100)

$$SP = 800 \times 1.15$$

**Mental method:**
```
10% of 800 = 80
 5% of 800 = 40
────────────────
15%        = 120
SP = 800 + 120 = 920
```

**Answer: (c) ₹920**

---

**Q4. SP ₹660 at 10% profit. Find CP. → (c) ₹600**

**Formula used:** CP = SP / (1 + p/100)

$$CP = \frac{660}{1.10} = \frac{6600}{11} = 600$$

**Check:** 600 × 1.10 = 660 ✓

> **Trap:** option (b) ₹594 comes from 660 − 10% of 660. To reverse a percentage you divide, never subtract.

**Answer: (c) ₹600**

---

**Q5. CP ₹1,200, 20% loss. Find SP. → (b) ₹960**

**Formula used:** SP = CP(1 − l/100)

$$SP = 1200 \times 0.80 = 960$$

**Answer: (b) ₹960**

---

**Q6. MP ₹500, 20% discount. Find SP. → (c) ₹400**

**Formula used:** SP = MP(1 − d/100)

$$SP = 500 \times 0.80 = 400$$

**Answer: (c) ₹400**

---

**Q7. MP ₹800, SP ₹680. Discount%? → (b) 15%**

**Formula used:** Discount% = (MP − SP)/MP × 100

**Step 1 — Discount amount.**
$$800 - 680 = ₹120$$

**Step 2 — Divide by MP (not CP).**
$$\frac{120}{800} \times 100 = 15\%$$

**Answer: (b) 15%**

---

**Q8. SP ₹450 at 10% loss. Find CP. → (c) ₹500**

**Formula used:** CP = SP / (1 − l/100)

$$CP = \frac{450}{0.90} = \frac{4500}{9} = 500$$

**Check:** 500 × 0.90 = 450 ✓

**Answer: (c) ₹500**

---

**Q9. 12 apples for ₹60, sold at ₹6 each. Profit%? → (c) 20%**

**Step 1 — Total CP.** ₹60 for 12 apples.

**Step 2 — Total SP.**
$$12 \times 6 = ₹72$$

**Step 3 — Profit%.**
$$\frac{72 - 60}{60} \times 100 = \frac{12}{60} \times 100 = 20\%$$

**Per-unit alternative:** CP each = 60/12 = ₹5; SP each = ₹6; profit = 1/5 = 20% ✓

**Answer: (c) 20%**

---

**Q10. CP of 15 articles = SP of 12 articles. Profit%? → (b) 25%**

**Formula used:** Profit% = (m − n)/n × 100, where m = 15, n = 12

$$\frac{15 - 12}{12} \times 100 = \frac{3}{12} \times 100 = 25\%$$

**First-principles check:** Let CP per article = ₹1.
CP of 15 = ₹15 = SP of 12 ⇒ SP per article = 15/12 = ₹1.25
Profit = ₹0.25 on ₹1 ⇒ 25% ✓

**Answer: (b) 25%**

---

**Q11. SP ₹1,080 at 20% gain. Find CP. → (c) ₹900**

$$CP = \frac{1080}{1.20} = \frac{10800}{12} = 900$$

**Check:** 900 × 1.20 = 1,080 ✓

**Answer: (c) ₹900**

---

**Q12. CP ₹720, SP ₹900. Profit%? → (c) 25%**

$$\frac{900 - 720}{720} \times 100 = \frac{180}{720} \times 100$$

**Simplify:** 180/720 = 1/4 = 25%

**Answer: (c) 25%**

---

**Q13. MP ₹1,000; successive discounts 10% and 20%. SP? → (c) ₹720**

**Formula used:** SP = MP(1 − d₁/100)(1 − d₂/100)

$$SP = 1000 \times 0.90 \times 0.80$$

**Step by step:**
- After 10%: 1000 − 100 = ₹900
- After 20% on ₹900: 900 − 180 = ₹720

$$1000 \times 0.72 = 720$$

> **Trap:** treating it as a flat 30% discount gives ₹700. Successive discounts always leave more than the naive sum suggests.

**Answer: (c) ₹720**

---

**Q14. Single discount equivalent to 20% and 25%? → (b) 40%**

**Formula used:** D_eq = a + b − ab/100

$$20 + 25 - \frac{20 \times 25}{100} = 45 - 5 = 40\%$$

**Multiplier check:**
$$0.80 \times 0.75 = 0.60 \implies 40\% \text{ off} \checkmark$$

**Answer: (b) 40%**

---

**Q15. MP ₹1,500, 12% discount. SP? → (b) ₹1,320**

$$SP = 1500 \times 0.88$$

**Mental method:**
```
10% of 1500 = 150
 2% of 1500 =  30
──────────────────
12%         = 180
SP = 1500 − 180 = 1320
```

**Answer: (b) ₹1,320**

---

**Q16. CP ₹500, marked 40% above cost. MP? → (c) ₹700**

**Formula used:** MP = CP(1 + m/100)

$$MP = 500 \times 1.40 = 700$$

**Answer: (c) ₹700**

---

**Q17. SP = 2 × CP. Profit%? → (b) 100%**

**Formula used:** If SP = k × CP, profit% = (k − 1) × 100

$$(2 - 1) \times 100 = 100\%$$

**Check with numbers:** CP = 100, SP = 200. Profit = 100 on a base of 100 ⇒ 100% ✓

> **Trap:** answering 50%. That would be the profit as a fraction of SP, which is not how profit% is defined.

**Answer: (b) 100%**

---

**Q18. CP ₹2,400, 5% loss. SP? → (b) ₹2,280**

$$SP = 2400 \times 0.95$$

**Mental method:** 5% of 2,400 = 120. SP = 2400 − 120 = ₹2,280

**Answer: (b) ₹2,280**

---

**Q19. Profit ₹150 = 25% of CP. Find CP. → (c) ₹600**

$$0.25 \times CP = 150$$
$$CP = \frac{150}{0.25} = 600$$

**Shortcut:** 25% = 1/4. If a quarter is 150, the whole is 600.

**Check:** SP = 600 + 150 = ₹750 = 600 × 1.25 ✓

**Answer: (c) ₹600**

---

**Q20. CP of 20 pens = ₹240. SP per pen for 25% gain? → (c) ₹15**

**Step 1 — CP per pen.**
$$\frac{240}{20} = ₹12$$

**Step 2 — Apply 25% profit.**
$$SP = 12 \times 1.25 = ₹15$$

**Check:** 20 pens × ₹15 = ₹300; CP ₹240; profit ₹60 = 25% of 240 ✓

**Answer: (c) ₹15**

---

### 🟡 MEDIUM — Solutions 21–40

---

**Q21. Marked 30% above CP, 10% discount. Profit%? → (b) 17%**

**Formula used:** Master relation — MP(1 − d) = CP(1 + p)

**Step 1 — Assume CP = 100.**
$$MP = 100 \times 1.30 = 130$$

**Step 2 — Apply discount to MP.**
$$SP = 130 \times 0.90 = 117$$

**Step 3 — Profit.**
$$117 - 100 = 17 \implies 17\%$$

**One-line multiplier:** 1.30 × 0.90 = 1.17 ⇒ **17%**

> **Trap:** 30 − 10 = 20%. The discount is on 130, not on 100, so it removes 13 — not 10.

**Answer: (b) 17%**

---

**Q22. SP ₹720 at 10% loss. New SP for 15% gain? → (c) ₹920**

**Step 1 — Recover the cost price.**
$$CP = \frac{720}{0.90} = 800$$

**Step 2 — Compute the new selling price.**
$$SP_{\text{new}} = 800 \times 1.15 = 920$$

**Direct multiplier shortcut:**
$$SP_{\text{new}} = 720 \times \frac{1.15}{0.90} = 720 \times \frac{115}{90} = 8 \times 115 = 920$$

**Answer: (c) ₹920**

---

**Q23. Two articles at ₹1,200 each; +20% and −20%. Overall? → (b) 4% loss**

**Formula used:** Equal SP with ±x% ⇒ net **loss** of x²/100 %

$$\text{Loss\%} = \frac{20^2}{100} = 4\%$$

**Full verification:**
$$CP_1 = \frac{1200}{1.20} = ₹1000 \qquad CP_2 = \frac{1200}{0.80} = ₹1500$$
$$\text{Total CP} = ₹2500, \qquad \text{Total SP} = ₹2400$$
$$\text{Loss} = ₹100 \implies \frac{100}{2500} \times 100 = 4\% \checkmark$$

> **Why never break-even:** the loss-making article cost ₹1,500 while the profitable one cost only ₹1,000. The bigger investment is the losing one, so losses always dominate.

**Answer: (b) 4% loss**

---

**Q24. Sells at CP but uses a 900 g weight for 1 kg. Profit%? → (b) 11 1/9 %**

**Formula used:** Gain% = (True wt − Given wt)/Given wt × 100

$$\frac{1000 - 900}{900} \times 100 = \frac{100}{900} \times 100 = \frac{100}{9} = 11\tfrac{1}{9}\% \approx 11.11\%$$

**Concrete check:** Suppose cost is ₹1/g.
- Customer pays for 1,000 g ⇒ pays ₹1,000
- Dealer gives 900 g ⇒ his cost is ₹900
- Profit = ₹100 on a cost of ₹900 ⇒ 11.11% ✓

> **Trap:** dividing by 1,000 gives 10%. The base is the dealer's actual cost (900 g), not the claimed weight.

**Answer: (b) 11 1/9 %**

---

**Q25. Profit at ₹56 = loss at ₹42. Find CP. → (c) ₹49**

**Formula used:** CP = (SP₁ + SP₂)/2 when the profit and loss amounts are equal

$$CP = \frac{56 + 42}{2} = \frac{98}{2} = ₹49$$

**Verification:**
- At ₹56: profit = 56 − 49 = ₹7
- At ₹42: loss = 49 − 42 = ₹7 ✓ Equal.

**Algebraic derivation:** 56 − CP = CP − 42 ⇒ 2CP = 98 ⇒ CP = 49 ✓

**Answer: (c) ₹49**

---

**Q26. 20% discount, 20% profit, CP ₹800. Find MP. → (c) ₹1,200**

**Formula used:** MP(1 − d/100) = CP(1 + p/100)

**Step 1 — Find the required SP.**
$$SP = 800 \times 1.20 = ₹960$$

**Step 2 — SP is 80% of MP.**
$$MP \times 0.80 = 960$$

**Step 3 — Solve.**
$$MP = \frac{960}{0.80} = ₹1200$$

**Check:** ₹1,200 − 20% = ₹960; ₹960 on a CP of ₹800 is a 20% profit ✓

**Answer: (c) ₹1,200**

---

**Q27. 20% profit instead of 20% loss ⇒ ₹200 more. Find CP. → (c) ₹500**

**Formula used:** CP × (difference in multipliers) = difference in SP

**Step 1 — Write both selling prices.**
$$SP_{\text{profit}} = 1.20\,CP \qquad SP_{\text{loss}} = 0.80\,CP$$

**Step 2 — Take the difference.**
$$1.20\,CP - 0.80\,CP = 0.40\,CP = 200$$

**Step 3 — Solve.**
$$CP = \frac{200}{0.40} = ₹500$$

**Check:** 1.20 × 500 = ₹600; 0.80 × 500 = ₹400; difference ₹200 ✓

> **Shortcut:** the gap between +20% and −20% is **40 percentage points of CP**. So 40% of CP = ₹200 ⇒ CP = ₹500.

**Answer: (c) ₹500**

---

**Q28. 100 kg at ₹40/kg; 40% sold at +20%, rest at +10%. Overall profit%? → (c) 14%**

**Step 1 — Total cost.**
$$100 \times 40 = ₹4{,}000$$

**Step 2 — Split the stock.**
- Lot A: 40 kg, CP = 40 × 40 = ₹1,600, sold at +20% ⇒ SP = 1600 × 1.20 = ₹1,920
- Lot B: 60 kg, CP = 60 × 40 = ₹2,400, sold at +10% ⇒ SP = 2400 × 1.10 = ₹2,640

**Step 3 — Total SP.**
$$1920 + 2640 = ₹4{,}560$$

**Step 4 — Overall profit%.**
$$\frac{4560 - 4000}{4000} \times 100 = \frac{560}{4000} \times 100 = 14\%$$

**Weighted-average shortcut:** since all rice has the same cost per kg, the overall profit% is the weighted mean of the two profit rates:
$$0.40 \times 20\% + 0.60 \times 10\% = 8 + 6 = 14\% \checkmark$$

**Answer: (c) 14%**

---

**Q29. 10% loss; ₹100 more would give 15% gain. Find CP. → (b) ₹400**

**Step 1 — Write both selling prices.**
$$SP_{\text{actual}} = 0.90\,CP \qquad SP_{\text{hypothetical}} = 1.15\,CP$$

**Step 2 — The gap is ₹100.**
$$1.15\,CP - 0.90\,CP = 0.25\,CP = 100$$

**Step 3 — Solve.**
$$CP = \frac{100}{0.25} = ₹400$$

**Check:** SP at 10% loss = ₹360. Add ₹100 ⇒ ₹460 = 400 × 1.15 ✓

**Answer: (b) ₹400**

---

**Q30. MP ₹2,000; discounts 10%, 20%, 25%. SP? → (c) ₹1,080**

**Formula used:** SP = MP × (1−d₁)(1−d₂)(1−d₃)

$$SP = 2000 \times 0.90 \times 0.80 \times 0.75$$

**Step by step:**
$$2000 \times 0.90 = 1800$$
$$1800 \times 0.80 = 1440$$
$$1440 \times 0.75 = 1080$$

**Combined factor:** 0.90 × 0.80 × 0.75 = 0.54 ⇒ 46% total discount
$$2000 \times 0.54 = 1080 \checkmark$$

> **Trap:** 10 + 20 + 25 = 55% ⇒ ₹900. Successive discounts compound downward, so the true discount (46%) is less than the sum.

**Answer: (c) ₹1,080**

---

**Q31. 25% profit after 20% discount. Required markup? → (c) 56.25%**

**Formula used:** m = 100(p + d)/(100 − d)

$$m = \frac{100(25 + 20)}{100 - 20} = \frac{4500}{80} = 56.25\%$$

**First-principles derivation:**
Let CP = 100. Required SP = 100 × 1.25 = 125.
SP is 80% of MP, so:
$$MP = \frac{125}{0.80} = 156.25$$
Markup = 156.25 − 100 = **56.25%** ✓

**Answer: (c) 56.25%**

---

**Q32. CP of 12 articles = SP of 9 articles. Profit%? → (c) 33⅓%**

**Formula used:** Profit% = (m − n)/n × 100

$$\frac{12 - 9}{9} \times 100 = \frac{3}{9} \times 100 = \frac{100}{3} = 33\tfrac{1}{3}\%$$

**Check:** Let CP per article = ₹1. CP of 12 = ₹12 = SP of 9 ⇒ SP each = 12/9 = ₹4/3.
Profit = 4/3 − 1 = 1/3 on a base of 1 ⇒ 33⅓% ✓

**Answer: (c) 33⅓%**

---

**Q33. SP ₹935 at 10% profit. SP for 20% loss? → (c) ₹680**

**Step 1 — Find CP.**
$$CP = \frac{935}{1.10} = \frac{9350}{11} = ₹850$$

**Step 2 — Apply a 20% loss.**
$$SP = 850 \times 0.80 = ₹680$$

**Direct multiplier route:**
$$935 \times \frac{0.80}{1.10} = 935 \times \frac{8}{11} = 85 \times 8 = 680$$

**Answer: (c) ₹680**

---

**Q34. 40 kg @ ₹30 + 60 kg @ ₹40, sold at ₹45/kg. Profit%? → (c) 25%**

**Step 1 — Total cost.**
$$40 \times 30 = ₹1{,}200$$
$$60 \times 40 = ₹2{,}400$$
$$\text{Total CP} = ₹3{,}600 \text{ for } 100 \text{ kg}$$

**Step 2 — Cost per kg.**
$$\frac{3600}{100} = ₹36/\text{kg}$$

**Step 3 — Total SP.**
$$100 \times 45 = ₹4{,}500$$

**Step 4 — Profit%.**
$$\frac{4500 - 3600}{3600} \times 100 = \frac{900}{3600} \times 100 = 25\%$$

**Per-kg check:** CP ₹36, SP ₹45 ⇒ profit ₹9 ⇒ 9/36 = 25% ✓

**Answer: (c) 25%**

---

**Q35. Buy 10, get 2 free. Discount%? → (b) 16⅔%**

**Formula used:** Discount% = b/(a + b) × 100, with a = 10, b = 2

$$\frac{2}{12} \times 100 = \frac{1}{6} \times 100 = 16\tfrac{2}{3}\% \approx 16.67\%$$

**Concrete check:** Let each article be marked ₹100.
- Customer receives 12 articles, worth ₹1,200 at list price
- Customer pays for 10 ⇒ ₹1,000
- Discount = ₹200 on ₹1,200 ⇒ 200/1200 = 16.67% ✓

> **Trap:** dividing by 10 (2/10 = 20%). The base is the *total value received* (12 articles), not the number paid for.

**Answer: (b) 16⅔%**

---

**Q36. CP ₹27.50, SP ₹28.60. Gain%? → (c) 4%**

**Step 1 — Gain amount.**
$$28.60 - 27.50 = ₹1.10$$

**Step 2 — Divide by CP.**
$$\frac{1.10}{27.50} \times 100$$

**Step 3 — Clear the decimals.**
$$\frac{110}{2750} \times 100 = \frac{110 \times 100}{2750} = \frac{11000}{2750} = 4\%$$

**Check:** 27.50 × 1.04 = 28.60 ✓

**Answer: (c) 4%**

---

**Q37. 17 balls sold for ₹720; loss = CP of 5 balls. CP of one ball? → (d) ₹60**

**Step 1 — Let the CP of one ball be ₹*c*.**
$$\text{Total CP} = 17c, \qquad \text{Total SP} = ₹720$$

**Step 2 — Express the loss two ways.**
$$\text{Loss} = 17c - 720$$
$$\text{Loss} = 5c \quad \text{(given)}$$

**Step 3 — Equate and solve.**
$$17c - 720 = 5c$$
$$12c = 720$$
$$c = ₹60$$

**Check:** Total CP = 17 × 60 = ₹1,020. SP = ₹720. Loss = ₹300 = 5 × ₹60 ✓

> **Elegant reading:** selling 17 balls but losing the value of 5 means the ₹720 covers exactly 12 balls' worth of cost. Hence 12c = 720.

**Answer: (d) ₹60**

---

**Q38. Buys 40 pens for the marked price of 36; sells at MP. Profit%? → (b) 11 1/9 %**

**Step 1 — Set the marked price of one pen = ₹1.**
$$\text{Total CP for 40 pens} = ₹36$$

**Step 2 — Total SP (all sold at MP).**
$$40 \times ₹1 = ₹40$$

**Step 3 — Profit%.**
$$\frac{40 - 36}{36} \times 100 = \frac{4}{36} \times 100 = \frac{100}{9} = 11\tfrac{1}{9}\%$$

**Answer: (b) 11 1/9 %**

---

**Q39. MP ₹1,200; discounts 20% and 10%. Single discount and SP? → (b) 28%, ₹864**

**Step 1 — Single equivalent discount.**
$$D_{eq} = a + b - \frac{ab}{100} = 20 + 10 - \frac{200}{100} = 30 - 2 = 28\%$$

**Step 2 — Selling price.**
$$SP = 1200 \times 0.80 \times 0.90 = 1200 \times 0.72 = ₹864$$

**Cross-check via the single discount:**
$$1200 \times (1 - 0.28) = 1200 \times 0.72 = ₹864 \checkmark$$

> Note that the order of the two discounts does not matter — multiplication is commutative.

**Answer: (b) 28%, ₹864**

---

**Q40. 25% profit; if CP were 20% less and SP ₹36.75 less, gain would be 30%. Find CP. → (c) ₹175**

**Step 1 — Set up the original scenario.** Let CP = *C*.
$$SP = 1.25\,C$$

**Step 2 — Set up the hypothetical scenario.**
$$CP_{\text{new}} = 0.80\,C$$
$$SP_{\text{new}} = 1.25\,C - 36.75$$

**Step 3 — Apply the 30% gain condition to the new scenario.**
$$SP_{\text{new}} = 1.30 \times CP_{\text{new}} = 1.30 \times 0.80\,C = 1.04\,C$$

**Step 4 — Equate the two expressions for SP_new.**
$$1.25\,C - 36.75 = 1.04\,C$$
$$0.21\,C = 36.75$$

**Step 5 — Solve.**
$$C = \frac{36.75}{0.21} = \frac{3675}{21} = ₹175$$

**Full verification:**
- Original: CP ₹175, SP = 175 × 1.25 = ₹218.75
- Hypothetical CP = 0.80 × 175 = ₹140
- Hypothetical SP = 218.75 − 36.75 = ₹182
- Gain = (182 − 140)/140 = 42/140 = 30% ✓

**Answer: (c) ₹175**

---

### 🔴 HARD — Solutions 41–50

---

**Q41. Sells at 10% loss on CP but uses 20% less weight. Overall? → (b) 12.5% profit**

**Two distortions act at once:** a stated loss on price, and a hidden gain on quantity.

**Step 1 — Build a concrete scenario.**
Let the true cost be ₹1 per gram.
The customer asks for 1 kg (1,000 g).

**Step 2 — What the customer pays.**
The dealer *claims* a 10% loss on the cost of 1 kg:
$$\text{Price charged} = 1000 \times 0.90 = ₹900$$

**Step 3 — What it actually cost the dealer.**
He gives 20% less weight ⇒ 800 g.
$$\text{Dealer's real cost} = 800 \times ₹1 = ₹800$$

**Step 4 — Compute the true profit.**
$$\text{Profit} = 900 - 800 = ₹100 \text{ on a cost of ₹800}$$
$$\text{Profit\%} = \frac{100}{800} \times 100 = 12.5\%$$

**Formula check:**
$$\text{Multiplier} = \left(1 - \frac{10}{100}\right) \times \frac{\text{True wt}}{\text{Given wt}} = 0.90 \times \frac{1000}{800} = 0.90 \times 1.25 = 1.125$$
⇒ **12.5% profit** ✓

> **Key insight:** a 20% weight shortfall gives the dealer a **25%** quantity advantage (1000/800 = 1.25), not 20%. That more than offsets his 10% price concession.

**Answer: (b) 12.5% profit**

---

**Q42. Two horses, total ₹8,400; +20% and −10%, net break-even. CP of the first? → (b) ₹2,800**

**Step 1 — Define variables.**
Let the first horse cost ₹*x*. Then the second cost ₹(8,400 − *x*).

**Step 2 — Write the break-even condition.**
Breaking even means the profit on horse 1 exactly cancels the loss on horse 2:
$$0.20x = 0.10\,(8400 - x)$$

**Step 3 — Expand and solve.**
$$0.20x = 840 - 0.10x$$
$$0.30x = 840$$
$$x = \frac{840}{0.30} = ₹2{,}800$$

**Full verification:**
- Horse 1: CP ₹2,800, sold at +20% ⇒ SP = ₹3,360, profit = ₹560
- Horse 2: CP = 8,400 − 2,800 = ₹5,600, sold at −10% ⇒ SP = ₹5,040, loss = ₹560
- Total CP = ₹8,400; Total SP = 3,360 + 5,040 = ₹8,400 ⇒ break-even ✓

> **Ratio shortcut:** for the amounts to cancel, 20% of x must equal 10% of y, so x : y = 10 : 20 = 1 : 2. Splitting ₹8,400 in 1 : 2 gives ₹2,800 and ₹5,600 ✓

**Answer: (b) ₹2,800**

---

**Q43. Marked 50% above CP; still earns 20% profit. Find the discount%. → (b) 20%**

**Formula used:** MP(1 − d/100) = CP(1 + p/100)

**Step 1 — Assume CP = 100.**
$$MP = 150, \qquad SP = 120$$

**Step 2 — Compute the discount on MP.**
$$\text{Discount} = 150 - 120 = 30$$

**Step 3 — Express as a percentage of MP.**
$$\frac{30}{150} \times 100 = 20\%$$

**Algebraic check:**
$$1.50 \times (1 - d) = 1.20 \implies 1 - d = 0.80 \implies d = 20\%$$

> **Trap:** answering 30%, treating the ₹30 reduction as a percentage of CP. Discount is always a percentage of **MP**.

**Answer: (b) 20%**

---

**Q44. 25% discount ⇒ 20% profit. Profit% at only 10% discount? → (c) 44%**

**Step 1 — Use the first scenario to find MP in terms of CP.**
$$MP \times 0.75 = CP \times 1.20$$
$$MP = \frac{1.20}{0.75}\,CP = 1.60\,CP$$

So the goods are marked **60% above cost**.

**Step 2 — Apply the new discount of 10%.**
$$SP_{\text{new}} = MP \times 0.90 = 1.60\,CP \times 0.90 = 1.44\,CP$$

**Step 3 — Read off the profit.**
$$1.44\,CP \implies 44\% \text{ profit}$$

**Numeric verification (CP = 100):**
- MP = ₹160
- At 25% discount: SP = 160 × 0.75 = ₹120 ⇒ 20% profit ✓ (matches the given)
- At 10% discount: SP = 160 × 0.90 = ₹144 ⇒ **44% profit** ✓

**Answer: (c) 44%**

---

**Q45. Buys 11 oranges for ₹10; sells 10 oranges for ₹11. Profit%? → (d) 21%**

**Step 1 — Cost price per orange.**
$$CP = \frac{10}{11} \text{ per orange}$$

**Step 2 — Selling price per orange.**
$$SP = \frac{11}{10} \text{ per orange}$$

**Step 3 — Profit percentage.**
$$\frac{SP - CP}{CP} \times 100 = \frac{\frac{11}{10} - \frac{10}{11}}{\frac{10}{11}} \times 100$$

**Step 4 — Simplify the ratio directly (cleaner).**
$$\frac{SP}{CP} = \frac{11/10}{10/11} = \frac{11}{10} \times \frac{11}{10} = \frac{121}{100} = 1.21$$

Since SP = 1.21 × CP, the profit is **21%**.

**Alternative — LCM method (avoids all fractions):**
Take 110 oranges (LCM of 11 and 10).
- Cost: 110/11 = 10 lots × ₹10 = **₹100**
- Revenue: 110/10 = 11 lots × ₹11 = **₹121**
- Profit = ₹21 on ₹100 ⇒ **21%** ✓

> **Pattern:** "buy *a* for ₹*b*, sell *b* for ₹*a*" gives a profit ratio of (a/b)². Here (11/10)² = 1.21 ⇒ 21%.

**Answer: (d) 21%**

---

**Q46. Two items at ₹1,980 each; +10% and −10%. Net loss in rupees? → (b) ₹40**

**Step 1 — Recover each cost price.**
$$CP_1 = \frac{1980}{1.10} = ₹1{,}800$$
$$CP_2 = \frac{1980}{0.90} = ₹2{,}200$$

**Step 2 — Compare totals.**
$$\text{Total CP} = 1800 + 2200 = ₹4{,}000$$
$$\text{Total SP} = 1980 \times 2 = ₹3{,}960$$

**Step 3 — Net loss.**
$$4000 - 3960 = ₹40$$

**Percentage check:**
$$\frac{40}{4000} \times 100 = 1\% = \frac{10^2}{100} \checkmark$$

**Answer: (b) ₹40**

---

**Q47. Sold at 2/3 of MP ⇒ 10% loss. Profit% if sold at MP? → (c) 35%**

**Step 1 — Translate the given condition into two expressions for the same SP.**
$$SP = \frac{2}{3} MP \quad \text{and} \quad SP = 0.90\,CP$$

**Step 2 — Equate and solve for MP in terms of CP.**
$$\frac{2}{3} MP = 0.90\,CP$$
$$MP = 0.90 \times \frac{3}{2}\,CP = 1.35\,CP$$

**Step 3 — Selling at the marked price means SP = 1.35 CP.**
$$\text{Profit\%} = (1.35 - 1) \times 100 = 35\%$$

**Numeric verification (CP = 100):**
- MP = ₹135
- Two-thirds of MP = 135 × 2/3 = ₹90
- Selling at ₹90 on a CP of ₹100 is a **10% loss** ✓ (matches the given condition)
- Selling at MP = ₹135 on CP ₹100 ⇒ **35% profit** ✓

**Answer: (c) 35%**

---

**Q48. CP of 20 articles = SP of x articles; profit = 25%. Find x. → (c) 16**

**Formula used:** Profit% = (m − n)/n × 100, with m = 20, n = x

**Step 1 — Set up the equation.**
$$\frac{20 - x}{x} \times 100 = 25$$

**Step 2 — Solve.**
$$\frac{20 - x}{x} = 0.25$$
$$20 - x = 0.25x$$
$$20 = 1.25x$$
$$x = \frac{20}{1.25} = 16$$

**Direct route:** CP of 20 = SP of x means SP/CP = 20/x. For a 25% profit, SP/CP = 1.25.
$$\frac{20}{x} = 1.25 \implies x = 16 \checkmark$$

**Check:** Let CP per article = ₹1. CP of 20 = ₹20 = SP of 16 ⇒ SP each = ₹1.25 ⇒ 25% profit ✓

**Answer: (c) 16**

---

**Q49. CP ₹10,000, marked 25% above cost, 8% discount. Profit% and profit? → (a) 15%, ₹1,500**

**Step 1 — Marked price.**
$$MP = 10{,}000 \times 1.25 = ₹12{,}500$$

**Step 2 — Selling price after discount.**
$$SP = 12{,}500 \times 0.92 = ₹11{,}500$$

*(Working: 8% of 12,500 = 1,000, so SP = 12,500 − 1,000 = 11,500)*

**Step 3 — Profit.**
$$\text{Profit} = 11{,}500 - 10{,}000 = ₹1{,}500$$

**Step 4 — Profit percentage.**
$$\frac{1500}{10{,}000} \times 100 = 15\%$$

**One-line multiplier check:**
$$1.25 \times 0.92 = 1.15 \implies 15\% \text{ profit} \checkmark$$

**Answer: (a) 15%, ₹1,500**

---

**Q50. 5% loss; ₹65 more would give 8% profit. Find CP. → (c) ₹500**

**Step 1 — Write both selling prices in terms of CP.**
$$SP_{\text{actual}} = 0.95\,CP$$
$$SP_{\text{hypothetical}} = 1.08\,CP$$

**Step 2 — The difference is ₹65.**
$$1.08\,CP - 0.95\,CP = 0.13\,CP = 65$$

**Step 3 — Solve.**
$$CP = \frac{65}{0.13} = ₹500$$

**Verification:**
- At 5% loss: SP = 500 × 0.95 = ₹475
- Add ₹65 ⇒ ₹540
- ₹540 on CP ₹500 = 8% profit ✓

> **Shortcut:** the gap from −5% to +8% is **13 percentage points of CP**. So 13% of CP = ₹65 ⇒ 1% of CP = ₹5 ⇒ CP = ₹500.

**Answer: (c) ₹500**

---

## 8. Quick Revision Sheet

> **One page. Read 48 hours after study, and again the night before the test.**

### The chain

```
CP ──markup(on CP)──► MP ──discount(on MP)──► SP
 └──────── profit / loss (on CP) ────────────┘

Profit% and Markup%  → based on CP
Discount%            → based on MP
```

### Core formulas

```
Profit% = (SP − CP)/CP × 100      Loss% = (CP − SP)/CP × 100
SP = CP(1 ± p/100)                CP = SP / (1 ± p/100)   ← DIVIDE to reverse
MP = CP(1 + m/100)                SP = MP(1 − d/100)
Discount% = (MP − SP)/MP × 100

MASTER RELATION:   MP(1 − d/100) = CP(1 + p/100)
```

### Successive discounts

```
Two discounts a%, b%  →  D_eq = a + b − ab/100
n discounts           →  SP = MP × Π(1 − dᵢ/100)

10+10 = 19%    10+20 = 28%    20+20 = 36%    20+25 = 40%
25+25 = 43.75% 30+20 = 44%    50+10 = 55%    10+20+25 = 46%
```

### Special results

```
Equal SP, +x% and −x%   →  ALWAYS a loss of x²/100 %
   x=10 → 1%    x=15 → 2.25%   x=20 → 4%    x=25 → 6.25%   x=30 → 9%

CP of m articles = SP of n   →  Profit% = (m − n)/n × 100
   15=12 → +25%   12=9 → +33⅓%   20=16 → +25%   8=10 → −20%

Buy a get b free        →  Discount% = b/(a+b) × 100
   Buy 10 get 2 → 16⅔%   Buy 3 get 1 → 25%   Buy 4 get 1 → 20%

False weight (sold at CP)  →  Gain% = (True − Given)/Given × 100
   900g for 1kg → 11 1/9 %    800g → 25%    850g → 17.65%

False weight + p% profit/loss  →  Multiplier = (1 ± p/100) × True/Given

Profit ₹P at SP₁ = Loss ₹P at SP₂  →  CP = (SP₁ + SP₂)/2

Markup needed for profit p after discount d  →  m = 100(p+d)/(100−d)
   p=20,d=20 → 50%    p=25,d=20 → 56.25%    p=20,d=25 → 60%
```

### The multiplier method (use for everything)

```
"Marked 60% above cost, discounts of 20% then 25%"
    1.60 × 0.80 × 0.75 = 0.96   →  4% LOSS

"Marked 35% above cost, 20% discount"
    1.35 × 0.80 = 1.08          →  8% PROFIT

"Buy at 25% profit target after 20% discount"
    MP × 0.80 = 1.25 CP  →  MP = 1.5625 CP  →  mark up 56.25%
```

### Sanity checks

```
✓ MP ≥ SP always
✓ Profit ⇒ SP > CP;  Loss ⇒ SP < CP
✓ Equivalent discount < sum of discounts, always
✓ Equal-SP ±x% ⇒ answer is a LOSS, never zero
✓ Reverse a % change by DIVIDING, never subtracting
```

---

## 9. Common Mistakes

| # | Mistake | Example | Correction |
|---|---|---|---|
| 1 | **Profit% based on SP** | CP 250, SP 200 ⇒ 50/200 = 25% loss | Base is CP: 50/250 = 20% loss |
| 2 | **Reversing by subtraction** | SP ₹660 at +10% ⇒ 660 − 66 = ₹594 | Divide: 660/1.10 = ₹600 |
| 3 | **Discount taken on CP** | Marked 30% above cost, 10% off ⇒ 20% profit | Discount is on MP: 1.30 × 0.90 = 1.17 ⇒ 17% |
| 4 | **Adding successive discounts** | 10% + 20% = 30% | 28%: 0.90 × 0.80 = 0.72 |
| 5 | **Equal-SP assumed break-even** | +20% and −20% cancel out | Always a loss: 20²/100 = 4% |
| 6 | **False weight: wrong base** | 900 g for 1 kg ⇒ 100/1000 = 10% | Base is the weight given: 100/900 = 11.11% |
| 7 | **Buy-a-get-b: wrong base** | Buy 10 get 2 ⇒ 2/10 = 20% | Base is total received: 2/12 = 16.67% |
| 8 | **"m = n" direction flipped** | CP of 15 = SP of 12 ⇒ (15−12)/15 | Denominator is *n*: (15−12)/12 = 25% |
| 9 | **Weighted profit averaged unweighted** | 40% at +20%, 60% at +10% ⇒ 15% | Weight it: 0.4(20) + 0.6(10) = 14% |
| 10 | **Answering the wrong quantity** | Asked for MP, gave SP | Re-read the final clause |
| 11 | **Ignoring overheads** | "Bought for ₹500, spent ₹50 on repairs" | CP includes repairs: CP = ₹550 |
| 12 | **Compounding markup with discount linearly** | 50% markup − 20% discount = 30% profit | 1.50 × 0.80 = 1.20 ⇒ 20% profit |

---

## Practice Answer Key

| Q | Ans | Q | Ans | Q | Ans | Q | Ans | Q | Ans |
|---|---|---|---|---|---|---|---|---|---|
| 1 | b | 11 | c | 21 | b | 31 | c | 41 | b |
| 2 | b | 12 | c | 22 | c | 32 | c | 42 | b |
| 3 | c | 13 | c | 23 | b | 33 | c | 43 | b |
| 4 | c | 14 | b | 24 | b | 34 | c | 44 | c |
| 5 | b | 15 | b | 25 | c | 35 | b | 45 | d |
| 6 | c | 16 | c | 26 | c | 36 | c | 46 | b |
| 7 | b | 17 | b | 27 | c | 37 | d | 47 | c |
| 8 | c | 18 | b | 28 | c | 38 | b | 48 | c |
| 9 | c | 19 | c | 29 | b | 39 | b | 49 | a |
| 10 | b | 20 | c | 30 | c | 40 | c | 50 | c |

**Scoring guide:** 45+/50 → strong. 35–44 → solid; revise markup–discount chains and false weights. Below 35 → re-read Sections 2.5–2.9 and redo the Medium set.

---

**⬅️ Back:** [Topic 1 — Percentages](01-percentages.md) · **➡️ Next:** [Topic 3 — Ratio, Proportion & Partnership](03-ratio-proportion-partnership.md)
