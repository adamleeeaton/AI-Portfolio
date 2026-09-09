# Calculation rules

These rules are configurable. Replace the bracketed fields after confirming the institution's current policy.

## Baseline

```text
Current quality points = current cumulative GPA × current cumulative quality credits
```

Convert each grade to grade points using `grade-scale.md`.

## Standard course

```text
New quality points = course credits × expected-grade points
Net GPA credits = course credits
Points removed = 0
```

## Retake

Use the institution's configured rule: `[retake treatment: replacement, both attempts, exclusion, or other]`.

If the institution uses replacement treatment, the template is:

```text
New quality points = new course credits × expected-grade points
Points removed = previous course credits × previous-grade points
Net GPA credits = new course credits − previous course credits
```

If previous grade or previous credits are missing, mark the row incomplete rather than estimating removed points.

## Projected totals

```text
Projected quality credits = current quality credits + sum(net GPA credits)
Projected quality points = current quality points + sum(new quality points) − sum(points removed)
Projected GPA = projected quality points ÷ projected quality credits
GPA change = projected GPA − current cumulative GPA
```

Do not divide by zero or a negative projected credit total. Report the issue and request correction.

## Rounding

Use `[institutional rounding rule]`. Unless the institution specifies otherwise, retain full precision during calculation and display results to three decimal places. Do not round intermediate values.

## Important limitation

The formulas depend on current institutional policy. Do not apply retake, forgiveness, exclusion, residency, or rounding rules without resolving the policy question.
