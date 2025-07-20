
# Probability of Getting Heads When 3 Coins Are Tossed

This document explains different approaches to calculate the probability of getting at least one **Head** when three fair coins are tossed simultaneously.

---

## 1. Sample Space Approach

Each coin has 2 outcomes: Head (H) or Tail (T).

**Total outcomes** when 3 coins are tossed:

\[
2^3 = 8
\]

**List of outcomes**:
```
HHH, HHT, HTH, HTT, THH, THT, TTH, TTT
```

Only **TTT** has no Heads.

\[
	ext{Probability of at least 1 Head} = rac{7}{8}
\]

---

## 2. Complementary Approach

Find the probability of getting **no heads (all tails)** and subtract from 1.

\[
P(	ext{All tails}) = rac{1}{2} 	imes rac{1}{2} 	imes rac{1}{2} = rac{1}{8}
\]
\[
P(	ext{At least one head}) = 1 - rac{1}{8} = rac{7}{8}
\]

---

## 3. Binomial Distribution

Let:
- \( n = 3 \)
- \( p = 0.5 \) (probability of Head)

We find:
- \( P(1H) = 3 \cdot 0.5 \cdot 0.25 = 0.375 \)
- \( P(2H) = 3 \cdot 0.25 \cdot 0.5 = 0.375 \)
- \( P(3H) = 1 \cdot 0.125 = 0.125 \)

Total:
\[
0.375 + 0.375 + 0.125 = 0.875 = rac{7}{8}
\]

---

## 4. Tree Diagram

A visual tree showing all outcomes when 3 coins are tossed:

![Probability Tree Diagram](A_probability_tree_diagram_in_a_digital_illustrati.png)

Only one branch leads to all tails (TTT), so:
\[
P(	ext{At least one Head}) = rac{7}{8}
\]

---

## ✅ Final Answer:

> The **probability of getting at least one Head when 3 coins are tossed** = **7/8** or **0.875**
