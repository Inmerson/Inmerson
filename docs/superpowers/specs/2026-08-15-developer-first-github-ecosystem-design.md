# Developer-First GitHub Ecosystem Design

## Goal

Make the public GitHub presence feel like it is maintained by one real developer over time: technically serious, concise, a little personal, and consistent without looking templated.

The personal profile remains minimal. The two organizations become the main entry points. Public repositories keep a shared baseline for clarity, but each README should sound like it belongs to that specific project rather than being generated from one master template.

## Scope

This work is split into three related tracks so each can be implemented and reviewed independently:

1. Organization profiles
2. Public repository READMEs
3. Repository metadata, pinning, and final profile cleanup

The tracks share the same writing rules but do not require identical layouts.

## Voice and visual direction

The overall style is developer-first rather than academic-marketing or startup-marketing.

- Use short, concrete sentences.
- Prefer plain technical language over polished corporate phrases.
- Describe what exists now before describing what may exist later.
- Do not oversell foundation-stage projects.
- Avoid repeated phrases across repositories.
- Avoid slogans, manifesto sections, large badge walls, typing animations, visitor counters, and decorative statistics.
- Keep headings useful rather than ornamental.
- Keep repository-specific details specific: architecture projects should talk about systems, Java should talk about programming practice, calculus should talk about mathematical exploration, and biotechnology projects should use careful scientific language.

The writing should not pretend that every project has the same maturity or the same purpose.

## Track 1 — Organization profiles

### Inmersion-CS

The organization README should become a compact developer hub.

It should explain that the organization contains software and learning projects around computer science and related university subjects. It should not list every repository in a large table.

Recommended structure:

1. `# Inmersion-CS`
2. Two short introductory paragraphs
3. `## Areas` with a compact line or short list covering:
   - Computer systems
   - Programming
   - Mathematics
   - Information systems
   - Supporting university subjects
4. `## Projects` with only a small set of representative public repositories, not the whole inventory
5. One short note that individual repositories describe their own current status and roadmap

The tone should be technical and direct. Avoid phrases such as “source of truth,” “production-quality foundation,” “deliberate practice,” or repeated references to engineering principles unless they are needed for a specific project.

### Inmersion-Biotech

This organization should use the same level of simplicity but a different voice.

Recommended structure:

1. `# Inmersion-Biotech`
2. Short introduction explaining that the organization contains biotechnology-related software and learning projects
3. `## Areas` covering:
   - Biotechnology
   - Quantitative learning
   - Scientific visualization
   - Botany / plant science
   - Organic chemistry where relevant
4. `## Projects` only if there are enough public repositories to make the section useful; otherwise omit it rather than forcing a one-item showcase
5. Short note that some work remains private while it is being developed

Do not make one mathematics repository the identity of the whole biotechnology organization.

## Track 2 — Public repository README standard

There is a shared baseline, not a fixed template.

Every public repository should answer these questions somewhere near the top:

- What is this project?
- What actually works today?
- What is still planned?
- How do I run it locally?
- Where do contribution and license details live?

Recommended common elements:

- Project title
- One-sentence description
- Honest status note when the project is early-stage
- Project-specific explanation or learning scope
- Current functionality
- Local development commands
- Roadmap only when useful
- Contributing / license links when present

The order may change by project.

### Project-specific treatment

**Architecture** should emphasize computer architecture, data representation, system state, CPU/memory concepts, and future simulation work. It does not need generic language about “making complex ideas observable” in every section.

**Calculus** should focus on mathematical exploration, explanation, visual reasoning, and practice. It can keep a broader learning narrative because that fits the project.

**Java** should sound more like a programming project: practice, reading code, writing code, debugging, program flow, objects, and future browser-based exercises.

**InfoSystems** should focus on requirements, process/data modeling, systems thinking, and realistic cases.

Other Inmersion-CS repositories should keep their own subject vocabulary rather than receiving copied versions of the same introduction.

**Math-Biotech-Project** may remain public inside Inmersion-Biotech, but it should be presented as one project inside the organization rather than as the organization’s identity. Its README should preserve careful distinctions between implemented features, experimental features, and planned work.

## Writing patterns to reduce

Across the current READMEs, some phrases are technically reasonable but become artificial when repeated too often. Reduce or vary phrases such as:

- “production-quality foundation”
- “source of truth”
- “design cycle”
- “carefully designed digital tools”
- “deliberate practice” when it is not central to the project
- repeated long lists of CI, accessibility, governance, and build tooling in the opening sections

Keep those details where they matter, especially in development or contributing sections, but do not make every README read like a project charter.

## Track 3 — Repository metadata, pinning, and profile cleanup

### Repository descriptions

GitHub repository descriptions should be one natural sentence and should describe the project, not its process.

Examples of the intended style:

- Architecture — `Learning project for computer architecture, data representation, and system behavior.`
- Calculus — `Interactive web project for learning calculus through explanation, practice, and visualization.`
- Java — `Web-based Java learning project focused on programming practice and debugging.`
- InfoSystems — `Learning project for requirements, process modeling, data modeling, and systems thinking.`

Descriptions for other repositories should follow the same principle without forcing the same sentence shape.

### Pinning

The personal profile should stay minimal and organization-first.

Pin representative repositories at the organization level where GitHub allows it. Do not pin every repository. For Inmersion-CS, prefer the projects that best represent technical depth and subject range. A likely first set is:

- Architecture
- Java
- Calculus
- InfoSystems

The final order should reflect actual maturity after the README audit.

For Inmersion-Biotech, do not force multiple pins when there is only one public repository worth presenting. The organization profile itself should carry the identity until more work becomes public.

### Personal profile

Keep the personal README focused on:

- Name and short identity line
- Inmersion-CS
- Inmersion-Biotech
- One concise About / Focus paragraph

Do not bring back individual project cards, GitHub stats, technology walls, or a long product catalog.

### Public planning artifacts

Internal planning documents should not become part of the public-facing story. After the redesign is verified, review `docs/superpowers/` in the public profile repository and remove planning artifacts that no longer provide value to visitors. Do not remove project documentation that is actually useful to users or contributors.

## Safety and accuracy rules

- Do not claim features that do not exist.
- Do not change a repository from private to public.
- Do not add licenses where the licensing decision has not been made.
- Do not describe the user as an expert, researcher, senior engineer, or other unsupported professional status.
- Preserve security, accessibility, and privacy notes when they are materially relevant, but keep them proportional to the project.
- Scientific repositories should distinguish observation, modeling, calculation, and interpretation carefully.

## Success criteria

A visitor should get three impressions:

1. The account belongs to a real developer who organizes work deliberately.
2. The repositories are related but not clones of one template.
3. Current capabilities and project maturity are easy to understand without marketing language.

The finished GitHub presence should look maintained, coherent, and technically credible without looking over-designed.