# GitHub Profile Organizations-First Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Replace the current profile README with a minimal organizations-first presentation centered on `Inmersion-CS` and `Inmersion-Biotech`, without featuring individual repositories.

**Architecture:** This is a single-file rewrite of `README.md`. The page will use a centered hero, two prominent organization descriptions, one short About / Focus paragraph, and a restrained closing line. No project showcase, statistics wall, product catalog, or long technology section will remain.

**Tech Stack:** GitHub Markdown, inline HTML supported by GitHub README rendering, Shields.io badges.

## Global Constraints

- English copy only.
- Dark-theme friendly and readable in GitHub light mode.
- No `Selected Work` section.
- Do not feature or highlight `Math-CS`.
- Do not feature or highlight `Math-Biotech-Project` or `Math & Biotech Lab`.
- No individual repository cards.
- No typing animation, trophy wall, visitor counter, or GitHub statistics section.
- No Inmerse product catalog.
- No engineering-principles list.
- Keep the page visually calm and concise.
- Avoid unsupported labels such as `expert`, `researcher`, `senior engineer`, or `AI expert`.

---

### Task 1: Replace the profile with an organizations-first README

**Files:**
- Modify: `README.md`

**Interfaces:**
- Consumes: approved organizations-first design spec and the public organization URLs.
- Produces: final profile README.

- [ ] **Step 1: Replace the current hero**

Use this structure:

```html
<div align="center">

# Halil İbrahim Öztürk

### Biotechnology · Software · AI-Assisted Learning Systems

I build careful digital systems for **learning, science, and understanding complex information**.

[![Computer Science](https://img.shields.io/badge/Inmersion--CS-Computer%20Science-0969da?logo=github&logoColor=white)](https://github.com/Inmersion-CS)
[![Biotechnology](https://img.shields.io/badge/Inmersion--Biotech-Biotechnology-2da44e?logo=github&logoColor=white)](https://github.com/Inmersion-Biotech)

</div>
```

- [ ] **Step 2: Add the organization section directly below the hero**

Use:

```markdown
---

## Organizations

### [Inmersion-CS](https://github.com/Inmersion-CS)

A computer-science learning and software organization for focused environments across computing, mathematics, information systems, and related subjects.

### [Inmersion-Biotech](https://github.com/Inmersion-Biotech)

A biotechnology-focused software and learning organization connecting scientific concepts with structured learning, visualization, and carefully designed digital tools.
```

- [ ] **Step 3: Add one concise About / Focus paragraph**

Use:

```markdown
## About / Focus

I study in **Poland** and work at the intersection of biotechnology, software, learning systems, privacy-aware design, and responsible AI. My public work is organized through the two organizations above so each field can remain focused and easier to explore.
```

- [ ] **Step 4: Add a restrained closing line**

Use:

```html
---

<div align="center">

**Science with care. Software with clarity.**

</div>
```

- [ ] **Step 5: Remove all excluded content**

Confirm the README contains none of the following as featured content or sections:

```text
Selected Work
Math-CS
Math & Biotech Lab
Math-Biotech-Project
Technology
Inmerse ecosystem
Engineering principles
Activity
GitHub statistics
Most used languages
```

- [ ] **Step 6: Verify exact section order**

The final README must be:

```text
Hero
Organizations
About / Focus
Closing line
```

- [ ] **Step 7: Verify primary links**

Confirm these URLs are present exactly:

```text
https://github.com/Inmersion-CS
https://github.com/Inmersion-Biotech
```

- [ ] **Step 8: Read back the final README from GitHub**

Fetch `Inmerson/Inmerson` → `README.md` and confirm there are no duplicate sections, malformed HTML tags, stale project descriptions, or truncated content.

- [ ] **Step 9: Commit**

Use commit message:

```text
feat: simplify profile around organizations
```
