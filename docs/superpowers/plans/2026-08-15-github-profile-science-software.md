# GitHub Profile Science × Software Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Redesign the `Inmerson/Inmerson` profile README into a visually calm, science-forward portfolio that makes the biotechnology × software identity, strongest public projects, and organization-owned work obvious within a 10–15 second scan.

**Architecture:** This is a single-file content and presentation redesign of `README.md`. The implementation will preserve GitHub-compatible Markdown/HTML, minimize external image dependencies, use a centered hero with restrained badges, present the two strongest public projects first, then explain the Science × Software identity, organization hubs, technology stack, compact Inmerse ecosystem, four engineering principles, and restrained activity cards.

**Tech Stack:** GitHub Markdown, inline HTML supported by GitHub README rendering, Shields.io badges, Skill Icons, GitHub Readme Stats.

## Global Constraints

- English copy only.
- Dark-theme friendly and readable in GitHub light mode.
- No typing animation, trophy wall, visitor counter, or excessive badges.
- Keep external image dependencies minimal.
- Do not use inflated labels such as “expert,” “researcher,” or formal “engineer” status claims.
- Preserve scientific humility and responsible AI language.
- Keep exactly four engineering principles.
- Keep the Inmerse ecosystem visible but secondary.
- Use the established product names: Bird Vision, Fitmers, Biomers, Floramers, Noor, Petmers, Dreamers.

---

### Task 1: Rewrite the profile hero and portfolio hierarchy

**Files:**
- Modify: `README.md`

**Interfaces:**
- Consumes: current profile identity, public repository URLs, organization URLs, and the approved design spec.
- Produces: the final top-level README structure and visual hierarchy used by all later sections.

- [ ] **Step 1: Replace the current hero with a compact Science × Software identity block**

Use this exact structure at the top of `README.md`:

```html
<div align="center">

# Halil İbrahim Öztürk

### Biotechnology · Software Engineering · AI-Assisted Learning Systems

I build thoughtful software that helps people **observe, understand, learn, and organize complex information responsibly**.

[![GitHub](https://img.shields.io/badge/GitHub-Inmerson-181717?logo=github&logoColor=white)](https://github.com/Inmerson)
[![Computer Science](https://img.shields.io/badge/Inmersion--CS-Computer%20Science-0969da?logo=github&logoColor=white)](https://github.com/Inmersion-CS)
[![Biotechnology](https://img.shields.io/badge/Inmersion--Biotech-Biotechnology-2da44e?logo=github&logoColor=white)](https://github.com/Inmersion-Biotech)

</div>
```

- [ ] **Step 2: Add a restrained divider and a Selected Work section immediately after the hero**

Use:

```markdown
---

## Selected work
```

- [ ] **Step 3: Present `Math-CS` as the first featured project**

Use concise copy that explains what the project demonstrates rather than listing every feature:

```markdown
### [Math-CS](https://github.com/Inmerson/Math-CS)

A computational-notebook-style mathematics workspace for computer science, combining mathematical analysis, linear algebra, geometry, visualization, practice, quizzes, and CS-oriented connections.

`React` · `TypeScript` · `Vite` · `Vitest` · `Tailwind CSS` · `Framer Motion` · `KaTeX` · `Capacitor`
```

- [ ] **Step 4: Present `Math & Biotech Lab` as the second featured project**

Use:

```markdown
### [Math & Biotech Lab](https://github.com/Inmersion-Biotech/Math-Biotech-Project)

A mathematics and biotechnology learning laboratory that connects scientific learning with deterministic calculations, biotechnology-oriented examples, 3D visualization, PWA/mobile support, and a versioned REST API.

`React` · `TypeScript` · `Node.js` · `Express` · `Three.js` · `React Three Fiber` · `KaTeX` · `Capacitor`
```

- [ ] **Step 5: Verify the top of the README is scan-friendly**

Read back `README.md` and confirm the first visible sections appear in this exact order:

```text
Hero
Selected work
Math-CS
Math & Biotech Lab
```

Expected result: a visitor can identify the interdisciplinary profile and the two strongest public projects without scrolling through long biography text.

- [ ] **Step 6: Commit the hierarchy rewrite**

Commit message:

```text
feat: redesign profile hero and featured work
```

---

### Task 2: Add the Science × Software identity and organization visibility

**Files:**
- Modify: `README.md`

**Interfaces:**
- Consumes: Task 1 structure.
- Produces: interdisciplinary focus section and clear pathways to organization-owned repositories.

- [ ] **Step 1: Add the Science × Software section below Selected Work**

Use this compact two-column table:

```markdown
## Science × Software

| Science / Biotechnology | Software / Systems |
|---|---|
| Biotechnology learning | Full-stack web and mobile applications |
| Scientific visualization | React / TypeScript architecture |
| Mathematical modeling and quantitative reasoning | Privacy, authorization, and data ownership |
| Careful scientific communication | AI-assisted workflows with human verification |
```

- [ ] **Step 2: Add an Organizations section immediately after it**

Use:

```markdown
## Organizations

### [Inmersion-CS](https://github.com/Inmersion-CS)
Open-source learning environments across computing, mathematics, information systems, language, management, culture, and workplace safety.

### [Inmersion-Biotech](https://github.com/Inmersion-Biotech)
Biotechnology-focused learning and application projects connecting scientific concepts with interactive software, visual models, and deliberate practice.
```

- [ ] **Step 3: Keep the About section concise and secondary**

Use:

```markdown
## About

I study in **Poland** and build software with an emphasis on clear architecture, scientific care, privacy, security, and maintainability. I am especially interested in systems that help people learn, understand, organize, and make better-informed decisions.
```

- [ ] **Step 4: Verify organization discoverability**

Read back `README.md` and confirm both organization links appear above the technology and ecosystem sections.

Expected result: organization-owned work is visible from the personal profile without requiring visitors to infer it from the contribution graph.

- [ ] **Step 5: Commit the identity and organization sections**

Commit message:

```text
feat: clarify science software identity and organizations
```

---

### Task 3: Add compact technology, Inmerse, principles, and activity sections

**Files:**
- Modify: `README.md`

**Interfaces:**
- Consumes: Tasks 1–2 structure.
- Produces: the supporting lower half of the final profile.

- [ ] **Step 1: Add a compact technology section**

Use one centered row only:

```html
## Technology

<div align="center">

<img src="https://skillicons.dev/icons?i=ts,react,vite,nodejs,python,androidstudio,git,github,firebase,figma" alt="Technology icons" />

</div>
```

- [ ] **Step 2: Add the Inmerse ecosystem as a compact secondary section**

Use:

```markdown
## Inmerse ecosystem

**Inmerse** is a private-first family of focused applications currently being developed and refined.

**Bird Vision** · **Fitmers** · **Biomers** · **Floramers** · **Noor** · **Petmers** · **Dreamers**

Shared priorities include privacy, accessibility, clear documentation, security, and responsible AI use.
```

- [ ] **Step 3: Add exactly four engineering principles**

Use:

```markdown
## Engineering principles

- **Scientific care** — communicate scope, uncertainty, and evidence honestly.
- **Privacy by design** — treat security, authorization, and data ownership as product requirements.
- **Clear architecture** — prefer understandable, maintainable systems over unnecessary complexity.
- **Responsible AI** — review and verify AI-assisted output rather than treating it as unquestioned authority.
```

- [ ] **Step 4: Add a restrained activity area at the bottom**

Use at most two transparent-background cards:

```html
## Activity

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=Inmerson&show_icons=true&hide_border=true&bg_color=00000000" alt="GitHub statistics" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Inmerson&layout=compact&hide_border=true&bg_color=00000000" alt="Most used languages" />

</div>
```

- [ ] **Step 5: Finish with one understated closing line**

Use:

```html
---

<div align="center">

**Science with care. Software with clarity.**

</div>
```

- [ ] **Step 6: Verify the final section order**

Read back the complete `README.md` and confirm the order is exactly:

```text
Hero
Selected work
Science × Software
Organizations
About
Technology
Inmerse ecosystem
Engineering principles
Activity
Closing line
```

Expected result: no duplicate About/Technology/Activity sections remain, and the ecosystem does not appear above public work.

- [ ] **Step 7: Commit the lower-half redesign**

Commit message:

```text
feat: polish profile supporting sections
```

---

### Task 4: Final verification and cleanup

**Files:**
- Verify: `README.md`
- Verify: `docs/superpowers/specs/2026-08-15-github-profile-science-software-design.md`

**Interfaces:**
- Consumes: completed README from Tasks 1–3 and the approved design spec.
- Produces: a verified final profile with no stale or contradictory content.

- [ ] **Step 1: Check content against the approved design spec**

Confirm all of the following are true:

```text
Biotechnology × software identity is visible in the hero.
Math-CS is featured first.
Math & Biotech Lab is featured second.
Inmersion-CS and Inmersion-Biotech are directly linked.
Science × Software table is present.
Technology icons appear only once.
Inmerse is compact and secondary.
Exactly four engineering principles are present.
Activity is at the bottom.
No typing animation, trophies, visitor counter, or badge wall exists.
```

- [ ] **Step 2: Check copy for unsupported status claims**

Search the README for these terms and remove them if used as status labels:

```text
expert
researcher
senior engineer
AI expert
```

Expected result: none appear as claims about the profile owner.

- [ ] **Step 3: Verify all primary links**

Confirm these URLs are present exactly:

```text
https://github.com/Inmerson
https://github.com/Inmerson/Math-CS
https://github.com/Inmersion-CS
https://github.com/Inmersion-Biotech
https://github.com/Inmersion-Biotech/Math-Biotech-Project
```

- [ ] **Step 4: Read back the final README from GitHub**

Use the repository file fetch action against `Inmerson/Inmerson` → `README.md` and visually inspect the returned Markdown for duplicate sections, malformed HTML, missing closing tags, or truncated content.

Expected result: the complete README is returned, all `<div>` tags are paired, and all section headings are present once.

- [ ] **Step 5: Commit any verification cleanup**

If cleanup changes are needed, use commit message:

```text
chore: finalize profile README polish
```

If no cleanup is needed, do not create an empty commit.
