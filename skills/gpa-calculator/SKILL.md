---
name: gpa-calculator
description: Calculate or estimate current and projected cumulative GPA, course-level GPA impact, quality points, GPA credits, and retake effects using institution-configurable rules.
---

# Purpose

Help the user calculate or estimate how GPA-bearing coursework affects a student's cumulative GPA. Produce transparent, auditable calculations and identify missing, invalid, or ambiguous inputs.

This skill is an estimating aid. It does not determine or certify an official institutional GPA.

# Configuration required before use

Replace or complete the bracketed values in the supporting references:

- `[institution name]`
- `[approved academic-record source]`
- `[current institutional grade scale]`
- `[retake treatment]`
- `[rounding rule]`
- `[institutional GPA verification statement]`

Do not rely on this skill until the institution has verified these inputs against current authoritative policy.

# Activation

Activate when the user's primary intent is to calculate, estimate, project, compare, or understand the numerical effect of GPA-bearing coursework on GPA.

Recognize requests about a current or cumulative GPA, a future GPA, course or grade scenarios, repeated courses, retakes, or transcript-based calculations.

Do not activate for general GPA definitions, academic-standard questions, general course planning, or repeat-policy questions without a calculation request.

# Required inputs

For a cumulative or projected GPA calculation, collect or identify:

1. Current cumulative GPA.
2. Current cumulative quality credits.
3. For each planned or in-progress course: course name or identifier, expected or actual grade, and course credits.
4. For each retake: confirmation that it is a retake, previous grade, and previous course credits.

Read `references/input-reference-guide.md` when the user needs help identifying baseline GPA and quality-credit fields from an academic-history report or unofficial transcript.

# Workflow

1. Confirm the requested calculation and whether it includes planned courses, in-progress courses, retakes, or scenario comparisons.
2. Collect and validate the required baseline and course inputs.
3. Read `references/grade-scale.md` when converting letter grades to grade points.
4. Read `references/calculation-rules.md` when performing a projected calculation, handling retakes, or explaining the calculation.
5. Calculate the result using the documented formulas. Keep intermediate values visible enough for the user to audit.
6. Report the result using the output format below.
7. State assumptions, incomplete entries, policy dependencies, and limitations. Never present an estimate as an official GPA.

# Validation and uncertainty

- Accept only grades in the configured approved grade scale unless the user supplies an authoritative institutional mapping.
- Require numeric GPA and credit values. Do not silently convert unclear text into numbers.
- Require positive course credits for courses being added or removed.
- Do not calculate a retake without both the previous grade and previous course credits.
- Do not calculate a cumulative GPA when the required baseline is missing or when projected GPA credits would be zero or negative.
- If values conflict between sources, identify the conflict and ask which authoritative value to use.
- Do not invent institutional repeat, forgiveness, replacement, rounding, exclusion, or residency rules.

# Output format

For a complete calculation, provide:

- Current GPA and baseline quality credits
- Projected GPA, when applicable
- GPA change, when applicable
- Projected quality points and quality credits, when applicable
- A course-by-course table with course, grade, credits, retake status, points added, points removed, and net GPA credits
- A short list of assumptions or unresolved inputs
- `[institutional GPA verification statement]`

For incomplete inputs, do not fabricate a result. Identify the missing fields and ask for them in a compact format.

# Guardrails

- Keep the student or advisor central; the calculation supports advising and does not replace institutional records or policy interpretation.
- Treat the grade scale and calculation rules in the supporting references as configurable rules represented by the institution's supplied GPA calculator model.
- Do not edit, overwrite, or claim to have updated an original spreadsheet unless a compatible spreadsheet tool and explicit user authorization are available.
- Protect personally identifiable student information. Use only the information needed for the requested calculation.
