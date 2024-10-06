# Summary of Famous Discrete Distributions

## 1. Bernoulli Distribution

**Random Variable**:
- **X**: Number of successes in a single trial.
- **Possible values**: 0 (failure), 1 (success).

**Probability Mass Function (PMF)**:
\[
P(X = x) = p^x (1 - p)^{1 - x}
\]
where \( p \) is the probability of success.

**Expectation (Mean)**:
\[
E[X] = p
\]

**Variance**:
\[
\operatorname{Var}(X) = p(1 - p)
\]

---

## 2. Binomial Distribution

**Random Variable**:
- **X**: Number of successes in \( n \) independent Bernoulli trials.
- **Possible values**: \( 0, 1, 2, \dots, n \).

**Probability Mass Function (PMF)**:
\[
P(X = k) = \binom{n}{k} p^k (1 - p)^{n - k}
\]
where \( p \) is the probability of success, and \( \binom{n}{k} \) is the binomial coefficient.

**Expectation (Mean)**:
\[
E[X] = np
\]

**Variance**:
\[
\operatorname{Var}(X) = np(1 - p)
\]

---

## 3. Geometric Distribution

**Random Variable**:
- **X**: Number of trials until the first success.
- **Possible values**: \( 1, 2, 3, \dots \).

**Probability Mass Function (PMF)**:
\[
P(X = k) = p(1 - p)^{k - 1}
\]
where \( p \) is the probability of success.

**Expectation (Mean)**:
\[
E[X] = \frac{1}{p}
\]

**Variance**:
\[
\operatorname{Var}(X) = \frac{1 - p}{p^2}
\]

---

## 4. Negative Binomial Distribution

**Random Variable**:
- **X**: Number of trials needed to achieve \( r \) successes.
- **Possible values**: \( r, r + 1, r + 2, \dots \).

**Probability Mass Function (PMF)**:
\[
P(X = k) = \binom{k - 1}{r - 1} p^r (1 - p)^{k - r}
\]
where \( p \) is the probability of success.

**Expectation (Mean)**:
\[
E[X] = \frac{r}{p}
\]

**Variance**:
\[
\operatorname{Var}(X) = \frac{r(1 - p)}{p^2}
\]

---

## 5. Hypergeometric Distribution

**Random Variable**:
- **X**: Number of successes in the sample.
- **Possible values**: \( \max(0, n - (N - K)) \) to \( \min(n, K) \).

**Probability Mass Function (PMF)**:
\[
P(X = k) = \frac{\binom{K}{k} \binom{N - K}{n - k}}{\binom{N}{n}}
\]
where:
- \( N \) is the population size,
- \( K \) is the number of successes in the population,
- \( n \) is the sample size,
- \( k \) is the number of successes in the sample.

**Expectation (Mean)**:
\[
E[X] = n \left( \frac{K}{N} \right)
\]

**Variance**:
\[
\operatorname{Var}(X) = n \left( \frac{K}{N} \right) \left( \frac{N - K}{N} \right) \left( \frac{N - n}{N - 1} \right)
\]

---

## 6. Poisson Distribution

**Random Variable**:
- **X**: Number of events in a fixed interval.
- **Possible values**: \( 0, 1, 2, \dots \).

**Probability Mass Function (PMF)**:
\[
P(X = k) = \frac{e^{-\lambda} \lambda^k}{k!}
\]
where \( \lambda \) is the average rate of occurrence.

**Expectation (Mean)**:
\[
E[X] = \lambda
\]

**Variance**:
\[
\operatorname{Var}(X) = \lambda
\]

---

## 7. Discrete Uniform Distribution

**Random Variable**:
- **X**: An integer value from \( a \) to \( b \).
- **Possible values**: \( a, a + 1, \dots, b \).

**Probability Mass Function (PMF)**:
\[
P(X = k) = \frac{1}{N}
\]
where \( N = b - a + 1 \).

**Expectation (Mean)**:
\[
E[X] = \frac{a + b}{2}
\]

**Variance**:
\[
\operatorname{Var}(X) = \frac{(N^2 - 1)}{12}
\]

---

## 8. Multinomial Distribution

**Random Variable**:
- **X₁, X₂, ..., Xₖ**: Counts of occurrences for each of \( k \) categories.
- **Possible values**: Each \( Xᵢ \geq 0 \), with \( \sum Xᵢ = n \).

**Probability Mass Function (PMF)**:
\[
P(X_1 = x_1, \dots, X_k = x_k) = \frac{n!}{x_1! x_2! \dots x_k!} p_1^{x_1} p_2^{x_2} \dots p_k^{x_k}
\]
where \( p_i \) is the probability of category \( i \).

**Expectation (Mean)**:
For each category \( i \):
\[
E[X_i] = n p_i
\]

**Variance**:
For each category \( i \):
\[
\operatorname{Var}(X_i) = n p_i (1 - p_i)
\]
For \( i \neq j \):
\[
\operatorname{Cov}(X_i, X_j) = - n p_i p_j
\]

---

## 9. Negative Hypergeometric Distribution

**Random Variable**:
- **X**: Number of trials needed to get \( r \) successes.
- **Possible values**: \( r, r + 1, \dots, N \).

**Probability Mass Function (PMF)**:
\[
P(X = k) = \frac{\binom{k - 1}{r - 1} \binom{N - k}{K - r}}{\binom{N}{K}}
\]

**Expectation (Mean)**:
\[
E[X] = \frac{r(N + 1)}{K + 1}
\]

**Variance**:
\[
\operatorname{Var}(X) = r \frac{(N - K)(N + 1)}{(K + 1)(K + 2)}
\]

---

## 10. Pascal (Negative Binomial Type II) Distribution

**Random Variable**:
- **X**: Number of failures before achieving \( r \) successes.
- **Possible values**: \( 0, 1, 2, \dots \).

**Probability Mass Function (PMF)**:
\[
P(X = k) = \binom{k + r - 1}{k} p^r (1 - p)^k
\]

**Expectation (Mean)**:
\[
E[X] = r \frac{1 - p}{p}
\]

**Variance**:
\[
\operatorname{Var}(X) = r \frac{1 - p}{p^2}
\]
