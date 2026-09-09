---
name: knowledge-base-article-builder
description: Create or revise accurate, readable knowledge-base articles from supplied source material or approved organizational sources. Use for article outlines, rewrites, structured content, searchable FAQs, or clean HTML for a knowledge-base platform.
---

# Purpose

Create clear, maintainable knowledge-base content that can be reviewed and published in an organization's chosen knowledge-base platform.

This portfolio version is platform-neutral. Replace bracketed configuration points with the target organization's approved terminology, content hierarchy, publishing rules, source systems, and escalation process before using it operationally.

## When to use

Use this skill when the user requests:

- A knowledge-base article or article revision
- An article outline or content restructuring
- A searchable FAQ or process guide
- Clean HTML or other platform-ready article content
- Help determining where an article belongs in a knowledge-base hierarchy

Do not use this skill for ordinary emails, case notes, calculations, or general policy answers unless article creation or revision is also requested.

## Grounding and source control

Use the supplied source material and, when authorized and available, the organization's approved knowledge sources. Treat authoritative organizational sources as controlling for current policies, procedures, requirements, dates, contacts, links, and exceptions.

- Preserve official terminology, identifiers, requirements, restrictions, dates, validity periods, and source links.
- Do not invent policies, deadlines, contacts, eligibility rules, exceptions, or outcomes.
- If sources conflict, are incomplete, or do not support a proposed statement, identify the issue and mark it for review.
- Keep confidential or personally identifying information out of public examples and portfolio artifacts.
- Keep source attribution separate from the article body unless the user requests attribution in the published content.

## Workflow

1. Identify the requested article type and intended audience.
2. Determine the narrowest appropriate placement in the target knowledge-base hierarchy.
3. Gather and review the supplied source material and approved current sources when needed.
4. Select only the sections supported by the source, such as overview, requirements, steps, important notes, FAQs, and next steps.
5. Preserve important restrictions, exceptions, prerequisites, deadlines, contacts, and links.
6. Apply the target organization's naming, formatting, accessibility, and publishing rules. If none are supplied, use the neutral references in this package.
7. Return the article in the format requested. When HTML is requested, provide one complete HTML code block and keep explanatory text outside it.
8. Perform an accuracy, placement, link, accessibility, privacy, and formatting check before presenting the result.

## Article design rules

- Use the narrowest supported article level: [general], [organization], [department], [program], [specialization], [process], or [FAQ].
- Use a clear title that follows [organization naming convention].
- Use plain language, descriptive headings, and short paragraphs.
- Use numbered lists for ordered procedures and bullets for unordered information.
- Add a FAQ or Common Questions section only when it answers useful questions supported by the source.
- Avoid duplicating information unless repetition materially improves findability or reader clarity.
- Do not create empty headings or unsupported sections.
- Do not silently correct official source material; flag questionable content for review.
- If a process can affect a person's eligibility, safety, privacy, finances, education, employment, or access to services, preserve the required human-review and escalation language: [insert approved safety, referral, or escalation procedure].

## Output rules

When the user does not specify a format, return:

1. Recommended article title
2. One-sentence summary
3. Article content in a clean, reviewable format
4. A short review note listing unresolved source gaps or required local configuration

When the user requests HTML, return a single HTML code block containing only the article content. Use the neutral HTML guidance in `references/html-content-guide.md`, unless the target platform's approved rules are provided.

## Supporting references

- Read [Knowledge-Base Article Standards](references/knowledge-base-article-standards.md) for neutral hierarchy, naming, organization, and quality checks.
- Read [Article Templates](references/article-templates.md) when a starting structure is useful.
- Read [HTML Content Guide](references/html-content-guide.md) when producing or reviewing platform-ready HTML.
