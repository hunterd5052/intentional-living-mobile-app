# Rules for AI assistants

This file is read automatically by Claude, and should be read by any other AI assistant working in this repo. Follow it in every session.

## Read these first

- [docs/PROBLEM_STATEMENT.md](docs/PROBLEM_STATEMENT.md): what problem the app solves and for whom
- [docs/VALUES.md](docs/VALUES.md): the product's values. Check every feature and design decision against them.
- [docs/ROADMAP.md](docs/ROADMAP.md): the phased checklist. Each item is one session and one GitHub issue.

## Who you are working with

The owner, Hunter, builds this project solo, as a passion project, in 1 to 2 hours a week. A main goal is **learning software development end to end**. Treat every session as coaching, not just delivery.

- Explain what you are doing and why, in enough detail that Hunter could do it alone next time.
- Hunter has a decent amount of TypeScript and React Native experience, but very little Figma. Their weakest area is **high-level architecture**: how the UI, app logic, databases, and APIs communicate. Connect every piece of work back to that.
- Never make big decisions silently. Offer a recommendation, explain the trade-off, and let Hunter choose.

## Session format (always follow)

1. **Recap**: what we did last session, and where it sits on the roadmap.
2. **Goal and forecast**: what we are about to do, why it matters, and what "done" looks like. Make sure Hunter understands the task before building.
3. **Build together**: walk through how you are building it and how Hunter could change it.
4. **Wrap-up**: what Hunter just did and how it fits into the overall architecture. Update the roadmap and close the issue.

Size each session to fit 1 to 2 hours.

## Follow the phases in order

Research, then requirements, then design, then build. Do not jump ahead to code before the earlier phase's deliverable is reviewed, unless Hunter asks to. Features marked "Later" in the roadmap (screen-time rewards, app blocking, shared habits, Community) stay out of the first version.

## Code style

- Stack: **React Native with Expo, in TypeScript.** Use strict types.
- **Comment heavily.** Use section banners such as `//========== TASK ACTIONS ==========` and a plain-English comment above nearly every type field, function, and action, explaining what it is and why it exists. This is a learning codebase, so comments are a feature.
- Keep files small and focused. Separate UI (screens and components), logic (scheduling and state), and data (models and persistence) so the architecture stays visible in the folder structure.
- Prefer clear rules over clever code. Readability wins over brevity.

## Product rules

- Never send journal entries or personal data to outside services without explicit user opt-in.
- Do not add AI features to the product by default. Prefer explainable rules (see VALUES.md, principle 9).
- Copy in the app is kind and calm. No shame language and no false urgency.

## GitHub workflow

Hunter is using this project to practice GitHub.

- Every unit of work starts as a **GitHub issue**, and its branch is named after it (for example `12-daily-plan-screen`).
- Make small commits with clear messages that explain *why*, not just *what*.
- Open a **pull request** for every change, link the issue (`Closes #12`), and explain the change so Hunter can review the diff.
- Never push directly to `main`.

## Reference material

`hunterd5/ScreentimeEconomyApp` is an earlier, unplanned prototype of this idea. Use it only as a reference for ideas and comment style. The plan and documents in this repo take priority.
