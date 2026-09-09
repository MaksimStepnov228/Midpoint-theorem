# Rigidity of the Midpoint Mean Value Property on Intervals of Fixed Length

**Status:** submitted to the *National High School Journal of Science*, September 2026.
**Author:** Maksim Stepnov

---

## The question

The mean value theorem guarantees that a point `ξ` exists where `f'(ξ)` equals the average rate of change, but says nothing about where. A classical theorem answers the extreme case: if the **midpoint** is a mean value point of *every* interval, then `f` is a polynomial of degree at most 2.

That hypothesis quantifies over all pairs of endpoints at once, so it is unsurprising that it pins `f` down. This paper keeps only one interval length:

```
f(a + 1) - f(a) = f'(a + 1/2)     for every a in ℝ.          (1)
```

**Must `f` be a quadratic?** Almost everyone I asked said "parabolas again," and so did I at first. The answer is no.

---

## Main results

There is an infinite family of explicit counterexamples, the first being

```
u₁(x) = e^(α₁x) · cos(β₁x),    α₁ = 5.5373565660…,  β₁ = 14.9953525556…
```

a fast-growing oscillation completing one cycle roughly every 0.419 units. The point is not that counterexamples exist, but that they are **expensive**.

**Theorem 2 (Rigidity below the threshold).** If `f` satisfies (1) and `|f(x)| ≤ M·e^(c|x|)` for some `c < α₁`, then `f` is a polynomial of degree at most 2. The constant `α₁` is sharp: `u₁` meets that bound and is not a polynomial.

**Theorem 3 (Expansion theorem).** Every solution of at most exponential growth is a quadratic plus a *finite* combination of explicit exponential-oscillatory modes, one for each `αₖ ≤ c`. The sum is empty precisely when `c < α₁`.

**Section 8.** Some growth hypothesis is unavoidable: there exist solutions of (1) growing faster than any exponential.

---

## Where the constant comes from

Substituting `f(x) = e^(λx)` collapses the problem to

```
λ = 2 sinh(λ/2),    equivalently    sinh z = z,   z = λ/2.
```

Its **triple zero at the origin** is exactly what accounts for the classical solutions `1`, `x`, `x²`; the complex zeros give everything else. `α₁` is twice the smallest positive real part among them.

The root analysis is elementary and self-contained. Separating real and imaginary parts yields a monotone relation `y = Y(x)` together with `tan y / y = tanh x / x`, which localizes every zero to an explicit interval and proves the growth rates `αₖ` are strictly increasing, **with no numerical input**.






Maksim Stepnov · mstepnov29@gmail.com · [github.com/MaksimStepnov228](https://github.com/MaksimStepnov228)
