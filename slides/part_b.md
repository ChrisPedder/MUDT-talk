# Bayes' Theorem in Business
# Part B: Bayes for Business

---

## Learning Objectives

By the end of Part B, you will be able to:

- Understand some ways in which Bayes' theorem is useful in business.
- Give examples of how to apply reasoning under uncertainty in the real world.

---

### Signals are more valuable than customers!

- It's *product-market* fit, not *product-customer* fit.
- Tempting to embellish to sign customers, but sell what you have.
- Most startups shouldn't have sales teams (some B2B only).
- About collecting **data** not revenue (remember priors don't matter)

---

### Reinvention is important.
- Let's say you have two hypotheses about what people will buy.
- Hypothesis A: trained hamsters - 30%.
- Hypothesis B: untrained capybara - 20%.
- You go out and test $H_A$ in the market for 3 months.

<div style="display: flex; justify-content: space-around; align-items: center; margin-top: 20px;">
  <img src="images/hamster.jpeg" alt="Hamster" style="width: 30%; height: auto;">
  <img src="images/capybara.jpeg" alt="Capybara" style="width: 30%; height: auto;">
</div>

---

### Results

After 3 months, you collect evidence E:

 - Only 5% of trial users convert to buying hamsters
 - But 40% of users ask about capybara instead
 - Competitors are gaining traction in your space

 - $P(E | H_A) = 0.15$ possible , but unlikely
 - $P(E | H_B) = 0.70$ evidence suggests the alternate direction

---

### What should you do?
 - $P(H_i | E) = [P(E | H_i) × P(H_i)] / P(E)$
 - $P(E) \approx  P(E | H_A) × P(H_A) + P(E | H_B) × P(H_B)$
 - $P(H_A | E) = (0.15 × 0.30) / 0.185 = 0.045 / 0.185 ≈ 0.24$
 - $P(H_B | E) = (0.70 × 0.20) / 0.185 = 0.14 / 0.185 ≈ 0.76$

 <span class="key-term">The new evidence caused a massive Bayesian update.</span>

---

### Why this matters for startups

- Evidence compounds quickly: Each week of data updates your beliefs.
- Asymmetric likelihood ratios: When evidence fits a pivot hypothesis, the likelihood ratio dramatically shifts probabilities.
- Time is the enemy: Every month spent pursuing H₁ when $P(H_A | E) = 24%$ is a month not spent on H₂ when $P(H_B | E) = 76%$.
- Overconfidence kills: Founders often treat their prior $P(H_A)$ as fixed truth rather than a belief to be updated.

---

### Hiring

**Setup**
 - Hiring a senior software engineer.
 - They score 85/100 on the technical test.
 - What is the probability that they succeed in the company?

---

### Context

 - Base failure rate is 40%, so 60% of engineers meet or exceed expectations after 1 year.
 - Likelihoods - how good is the test?
   - $P(score=85 | Success) = 0.25$
   - $P(score=85 | Failure) = 0.05$
 - $P(Score=85) = 0.15 + 0.02 = 0.17$

---

 ### Outcomes

 - P(Success | Score=85) = (0.25 × 0.60) / 0.17 = 0.88
 - If score = 70,
   - $P(Score=70 | Success) = 0.15$ (below average for successful hires)
   - $P(Score=70 | Failure) = 0.18$ (more common for failed hires)
   - $P(Score=70) = 0.162$
   - $P(Success | Score=70) = (0.15 × 0.60) / 0.162 = 0.56$

---

### More outcomes

- If score = 95,
  - $P(Score=95 | Success) = 0.10$ (rare, but happens for top performers)
  - $P(Score=95 | Failure) = 0.01$ (very unusual)
  - $P(Score=95) = 0.064$
  - $P(Success | Score=95) = (0.10 × 0.60) / 0.064 = 0.94$

---

### Why it matters.

1. Tests are never perfect discriminators. 95 score - 6% chance of failure. Keeps you humble!
2. Low scores are bad. 70 score, indicates the candidate is more likely to fail than our base rate suggests.
3. Context matters enormously - If base success rate is only 30%, $P(Success | Score=85) = 0.68$.

---

### Why it matters.

4. Update based on multiple signals. After the technical test (88% success probability), candidate has an interview.
  - $P(Strong Interview | Success) = 0.70$, and $P(Strong Interview | Failure) = 0.20$.
  - $P(Success) = 0.88$-
  - $P(Success | Strong Interview) = (0.70 × 0.88) / [(0.70 × 0.88) + (0.20 × 0.12)] = 0.96$

---

 ### Use Sherlock Holmes' Principle.

<span class="key-term">Ask yourself regularly "what am I *not* seeing?"</span>"

Sherlock Holmes's Principle, Formalized

1. Elimination phase: Rule out hypotheses that are inconsistent with evidence
2. Improbable remains: What's left might seem unlikely within your current framework
3. Expansion phase (the crucial part): If nothing in your hypothesis space fits, you must expand the space

---

### Bayesian non-parametric version.

 - $P(Data | H₁, H₂, ..., Hₙ) =$ very low.
 - Therefore: $P(Hₙ₊₁ exists | Data)$ is high

---

### Example Blockbuster vs Netflix.

Blockbuster's (implicit) hypothesis space in 2000:

 - H₁: Customers want more store locations
 - H₂: Customers want lower late fees
 - H₃: Customers want better in-store selection
 - H₄: Customers want faster new release availability

They ran tests, collected data, updated beliefs, optimized... and died.

---

### Example Blockbuster vs Netflix.

What they missed was
 - $H_5$: Customers don't want to return tapes, they want streaming.

This wasn't in their hypothesis space. No amount of Bayesian updating within their fixed set of hypotheses would save them.

---

## Key Takeaways: Part B

- Lots of business problems are reasoning under uncertainty.
- Estimating probabilities and using Bayes cuts through the noise.
- Humility and uncertainty is a superpower.

---

## Questions?
