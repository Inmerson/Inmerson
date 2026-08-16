# Inmerson Cinematic Profile Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Replace the personal GitHub profile README with a distinctive, restrained Inmerson profile inspired by the reference video's cinematic/terminal rhythm while preserving clarity, privacy, and GitHub compatibility.

**Architecture:** Keep the implementation intentionally simple: one public `README.md` using GitHub-compatible Markdown and safe inline HTML. The README will establish the Inmerson identity, retain the two organization links as the main navigation, avoid private-repository disclosure, and rely on GitHub's native profile activity rather than third-party statistics widgets.

**Tech Stack:** GitHub Profile README, Markdown, GitHub-safe HTML.

## Global Constraints

- Primary implementation target: `README.md` in `Inmerson/Inmerson`.
- Do not modify any other repository as part of this profile pass.
- Do not change repository visibility.
- Do not expose private repository names or internal project details in the public README.
- Preserve the public organization links.
- Avoid remote scripts; GitHub README-compatible Markdown and safe HTML only.
- No animated typing effects.
- No visitor counters.
- No large badge collections.
- No third-party activity/statistics cards.
- The hero must remain readable on narrow mobile viewports and in light mode.

---

### Task 1: Replace the profile README

**Files:**
- Modify: `README.md`

**Interfaces:**
- Consumes: the approved cinematic profile design in `docs/superpowers/specs/2026-08-16-inmerson-cinematic-profile-design.md`.
- Produces: the complete public GitHub profile presentation rendered from `README.md`.

- [ ] **Step 1: Fetch the current README and record its blob SHA**

Use GitHub's contents API so the update is based on the current version and does not overwrite an unseen concurrent edit.

- [ ] **Step 2: Replace the README with the approved structure**

Use this content shape:

```markdown
<div align="center">

# INMERSON

`observe · understand · build`

### Halil İbrahim Öztürk

**Biotechnology · Software · AI-Assisted Learning Systems**

</div>

---

## 01 / Focus

A short factual paragraph describing work at the intersection of biotechnology, software, learning systems, scientific visualization, privacy-aware design, and responsible AI.

## 02 / Branches

### Inmersion-CS
Short description and public organization link.

### Inmersion-Biotech
Short description and public organization link.

## 03 / Working principle

A compact terminal-like text block using observation, understanding, and building as the three steps without exaggerated claims.

## 04 / Explore

Two compact links to the public organizations; no private repository catalog.

---

<div align="center">

**Science with care. Software with clarity.**

</div>
```

The actual paragraph copy must remain concise, factual, and readable without decorative assets.

- [ ] **Step 3: Commit the README update**

Commit message:

```text
feat: redesign profile with cinematic Inmerson identity
```

- [ ] **Step 4: Fetch the README after the write**

Verify the returned content contains all of the following exact anchors:

```text
# INMERSON
observe · understand · build
## 01 / Focus
## 02 / Branches
Inmersion-CS
Inmersion-Biotech
## 03 / Working principle
## 04 / Explore
Science with care. Software with clarity.
```

Verify it contains none of these patterns:

```text
github-readme-stats
visitor
typing-svg
private repository names
```

### Task 2: Verify the committed profile change

**Files:**
- Verify: `README.md`

**Interfaces:**
- Consumes: the commit SHA produced by Task 1.
- Produces: evidence that only the intended public profile content changed in the implementation commit.

- [ ] **Step 1: Fetch the implementation commit**

Confirm the commit message is:

```text
feat: redesign profile with cinematic Inmerson identity
```

- [ ] **Step 2: Inspect the commit file list/diff**

Expected implementation change:

```text
README.md
```

The implementation commit must not modify project repositories, visibility settings, or unrelated files.

- [ ] **Step 3: Final content review**

Confirm the page communicates these four facts without unsupported role claims:

1. Inmerson is the unifying identity.
2. Biotechnology, software, and AI-assisted learning are the main fields.
3. Inmersion-CS and Inmersion-Biotech are the two public branches.
4. The presentation is memorable but restrained, with no third-party stats or tracking widgets.
