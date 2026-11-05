# Traffic Light README Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Add a friendly Indonesian README that helps beginners understand and run the traffic-light simulator.

**Architecture:** Add one Markdown file at the repository root. Describe the existing standalone HTML/JavaScript project without changing its behavior or adding setup requirements.

**Tech Stack:** Markdown, HTML, and vanilla JavaScript.

**Spec:** `docs/superpowers/specs/2026-11-04-traffic-light-readme-design.md`

## Global Constraints

- Write in Indonesian with a casual, clear tone for beginners.
- State that opening `index.html` in a browser is sufficient.
- Describe only behavior confirmed by the current files.
- Do not add features, dependencies, or setup tooling.

## Review Focus

- The open/run instructions must match the standalone project and not imply dependencies.
- The described red/yellow/green sequence and one-second yellow delay must match `app.js`.
- The filenames and file roles must match the repository.
- README formatting and headings must render as valid Markdown.
- Keep all content beginner-friendly and in Indonesian.

---

### Task 1: Writing the beginner README

**Files:**
- Create: `README.md`

**Interfaces:**
- Consumes: Current behavior in `index.html` and `app.js`.
- Produces: An Indonesian README with project overview, file guide, run instructions, and simulator behavior.

- [ ] **Step 1: Write `README.md`**

Include a short friendly introduction; list `index.html` and `app.js` with their roles; explain that the user can open `index.html` directly in a browser; describe clicking “Switch Traffic Light,” the one-second yellow light, and the alternating red/green state.

- [ ] **Step 2: Verify the documentation**

Run: `git diff --check`
Expected: No whitespace errors. Confirm the README's filenames, opening instructions, and timing against `index.html` and `app.js`.
