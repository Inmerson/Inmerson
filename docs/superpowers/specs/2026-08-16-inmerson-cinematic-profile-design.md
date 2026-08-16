# Inmerson Cinematic GitHub Profile Design

## Goal

Redesign the personal GitHub profile so it feels distinctive, calm, technical, and recognizably Inmerson.

The new profile should borrow the visual rhythm of the reference video—dark/minimal presentation, strong typography, terminal-like spacing, and a cinematic first impression—without copying the original profile or turning the page into a badge/statistics wall.

## Direction chosen

Three broad directions were considered:

1. **Ultra-minimal organization hub** — very clean and professional, but visually too close to the current profile.
2. **Stats-heavy developer profile** — visually active, but dependent on decorative widgets and third-party services.
3. **Cinematic Inmerson profile** — strong identity, restrained visual styling, native GitHub compatibility, and enough technical detail without clutter.

The chosen direction is **Cinematic Inmerson profile**.

## Visual language

- Dark/minimal composition that works naturally in GitHub dark mode and remains readable in light mode.
- Centered hero section with `INMERSON` as the primary identity.
- Secondary identity: `Halil İbrahim Öztürk`.
- Compact field line: `Biotechnology · Software · AI-Assisted Learning Systems`.
- Short motif: `observe · understand · build`.
- Monospace/terminal-inspired spacing using Markdown and safe HTML only.
- No animated typing effects.
- No visitor counters.
- No large badge collections.
- No third-party activity/statistics cards that create unnecessary external dependencies or tracking.

## Page structure

### 1. Hero

The top of the README should immediately establish the Inmerson identity.

Suggested hierarchy:

- `INMERSON`
- `observe · understand · build`
- `Halil İbrahim Öztürk`
- `Biotechnology · Software · AI-Assisted Learning Systems`

A small ASCII/terminal-style visual may be included if it remains readable on mobile and does not overwhelm the page.

### 2. Focus

A concise paragraph explaining that the work sits at the intersection of biotechnology, software, learning systems, scientific visualization, privacy-aware design, and responsible AI.

The tone should remain careful and factual. It should not present the user as an expert, researcher, senior engineer, or other unsupported professional role.

### 3. Two main branches

The two public organizations remain the primary navigation model:

- **Inmersion-CS** — computing, mathematics, information systems, and software learning projects.
- **Inmersion-Biotech** — biotechnology-related software, scientific learning, visualization, and quantitative work.

These should look like two deliberate branches of one broader Inmerson identity rather than unrelated links.

### 4. Selected work

The personal profile should not expose the full private repository inventory.

Only public work that is useful to visitors should be referenced. Private repositories remain private and are not described in a way that reveals internal details.

The profile may point visitors toward the organizations instead of maintaining a large project catalog.

### 5. Native GitHub activity

Do not embed third-party GitHub stats cards. GitHub's native contribution/activity surfaces already appear on the profile and should remain the main activity signal.

This preserves the cinematic simplicity and avoids unnecessary external image services.

### 6. Closing line

Use one restrained closing line, preferably:

`Science with care. Software with clarity.`

It should function as a quiet signature rather than a marketing slogan.

## Implementation boundaries

- Primary implementation target: `README.md` in `Inmerson/Inmerson`.
- Do not modify any other repository as part of this profile pass.
- Do not change repository visibility.
- Do not expose private repository names or internal project details in the public README.
- Preserve the public organization links.
- Avoid remote scripts; GitHub README-compatible Markdown and safe HTML only.
- External images should be avoided unless they materially improve the design and are hosted in a controlled repository location.

## Mobile/readability requirements

- The hero must remain readable on a narrow mobile viewport.
- ASCII art, if used, must be compact enough not to require horizontal scrolling.
- Important information must remain understandable even if GitHub strips or changes decorative HTML behavior.
- The profile should still make sense in light mode.

## Success criteria

A visitor should quickly understand that:

1. `Inmerson` is the unifying identity.
2. The account combines biotechnology, software, and AI-assisted learning work.
3. Inmersion-CS and Inmersion-Biotech are the two main public branches.
4. The page feels intentional and visually memorable without looking noisy or template-generated.
5. The design is technically simple enough to remain stable on GitHub and does not rely on third-party statistics widgets.

## Relationship to the previous design

This design intentionally revises the earlier ultra-minimal personal-profile rule. The previous organization-first structure is preserved, but the personal profile is allowed a stronger hero and more distinctive visual identity. The earlier guidance against badge walls, visitor counters, exaggerated claims, and decorative statistics remains in force.
