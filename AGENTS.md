# AGENTS.md

## Project Overview
- This project is a self-study website for the `AI Design` class at `Way Maker School`.
- The current implementation lives in `index.html` and teaches AI Design through `the 9 principles of visual design`.
- The site is not a generic course catalog. It is a guided learning experience that helps students `make first, discover principles, and reflect on decisions`.

## Core Educational Position
- The non-negotiable message of this project is: `AI is a tool, and design decisions are made by people.`
- Students should use AI to explore, generate, compare, and revise, but not to replace judgment.
- Every meaningful learning flow should reinforce authorship, critique, and explanation.
- The site should help students answer not only `what they made` but also `why they made it that way`.

## Target Experience
- Audience: students learning independently without constant teacher intervention.
- Tone: clear, encouraging, structured, and concrete.
- Language: default to `Korean` for all student-facing copy unless the user explicitly asks otherwise.
- Writing level: simple enough for students to follow alone, but not childish.
- The experience should feel like a well-designed workbook, not a marketing landing page.

## Learning Framework
- Preserve the learning arc `Make -> Discover -> Reflect`.
- `Make`: students complete a concrete task or mission first.
- `Discover`: students analyze what worked and connect it to a design principle.
- `Reflect`: students explain decisions, revisions, and what they learned.
- Where relevant, include `Analog` work so students also think with hands, paper, sketching, or physical experiments.
- AI use should be scaffolded by level and must always include critical evaluation, not only prompt execution.

## Curriculum Structure Rules
- The homepage should explain the overall course structure, AI-use progression, and roadmap.
- Weekly or module pages should stay easy to scan and should follow a stable pattern.
- The current course spans `20 weeks`, including `2 project weeks`; preserve that assumption unless the user explicitly requests a curriculum change.
- Weeks `1-3` currently function as connected `Step` activities with saved progress and completion gating. Treat them as a special guided flow, not as ordinary static lesson pages.
- For normal lesson pages, prefer this order:
  1. Week hero with title, principle, and AI level
  2. Mission or scenario
  3. Make task
  4. Discover / analysis / principle explanation
  5. Key concepts
  6. Deliverables
  7. Reflection
  8. Analog activity
  9. AI usage guidance
- Project weeks can expand the format, but they should still preserve the same educational logic.
- When adding a new lesson, ensure it has:
  - one concrete output students must produce
  - one explicit design principle or concept focus
  - one reflection prompt
  - one explanation of how AI should be used responsibly

## Content Guidelines
- Keep copy actionable. Prefer `do this`, `compare this`, `revise this`, `explain this`.
- Avoid abstract theory blocks unless they directly support an activity.
- Examples and prompts should be illustrative, not prescriptive. Students must still make choices.
- Reflection prompts should ask for reasoning, not preference only.
- If AI prompt examples are included, they should model good intent and constraints, not encourage copy-paste dependency.
- Avoid overstating AI capability. Do not imply that AI output is correct, final, or sufficient on its own.

## Visual Direction
- Preserve the current editorial classroom aesthetic:
  - warm paper-like background
  - serif display headlines
  - sans-serif Korean body copy
  - mono labels for system/navigation/meta information
  - restrained accent colors mapped to concepts
- The current design language is `structured, academic, tactile, and modern`. Keep that balance.
- Do not redesign toward a generic SaaS dashboard, app-builder template, or flashy AI-product landing page.
- Favor readability and hierarchy over decorative complexity.
- New UI pieces should look like they belong to the existing system: thin borders, compact radius, intentional spacing, muted neutrals with selective accent use.

## Typography And Color
- Respect the existing font roles unless there is a strong reason to change them:
  - `DM Serif Display` for high-emphasis headings
  - `Noto Sans KR` for body text
  - `Space Mono` for labels, metadata, and compact system text
- Reuse existing CSS variables and color semantics when possible.
- If new colors are introduced, they must serve a clear curriculum or UI purpose and harmonize with the existing palette.

## Interaction Rules
- Navigation should remain simple and legible.
- Students must be able to understand where they are in the curriculum at a glance.
- Progress-related behavior should feel stable and forgiving.
- Avoid interactions that hide important learning content behind excessive clicks, hover-only behavior, or fragile animations.
- Motion, if added, should support orientation and emphasis, not spectacle.

## Technical Guidelines
- Prefer keeping the project lightweight and editable as a `single self-contained HTML file` unless the user explicitly wants a larger refactor.
- Use `vanilla HTML, CSS, and JavaScript` unless there is a clear project-level decision to change stack.
- Respect the current render architecture built around home view, week view, and project-week rendering.
- Preserve current behaviors such as:
  - week navigation
  - home/lesson rendering
  - progress persistence
  - import/export flows
- Be careful around the Step 1-3 data model and storage keys; future changes should not silently reset student work.
- Do not introduce build tools, frameworks, or external dependencies casually.
- Keep the site usable as a local file where practical.

## Editing Rules
- Make minimal, intentional changes.
- Preserve existing naming patterns and structural conventions unless a cleanup is part of the requested task.
- If a section pattern already exists, extend that pattern instead of inventing a second one.
- When changing student-facing copy, keep terminology consistent across home, week views, and project views.
- If a request conflicts with the core educational position of the site, preserve the educational position and explain the tradeoff.

## Accessibility And UX
- Maintain strong text contrast and readable font sizes.
- Ensure keyboard-usable controls when editing navigation or forms.
- Preserve responsive behavior for desktop and tablet widths at minimum.
- Student tasks and buttons should be explicit; ambiguous labels are not acceptable.
- Important instructional information should not rely on color alone.

## Quality Bar For Future Work
- Any new feature should answer:
  - Does this help self-study students act, analyze, or reflect more clearly?
  - Does this reinforce that AI supports thinking rather than replaces it?
  - Does this match the current visual and editorial system?
  - Does this keep the page understandable without instructor explanation?
- Prefer coherence over feature growth.
- Prefer curriculum clarity over technical novelty.

## Review Checklist
- Before finishing a change, verify:
  - the page still communicates `AI is a tool; humans make decisions`
  - the modified section matches the `Make -> Discover -> Reflect` logic
  - student-facing Korean copy is natural and consistent
  - layout and spacing still fit the existing design system
  - interactions still work without errors
  - persistence/import/export behavior is not accidentally broken

## Default Assumptions For Future Agents
- If asked to add or revise lesson content, prioritize educational clarity over stylistic experimentation.
- If asked to redesign, evolve the existing visual language instead of replacing it wholesale.
- If asked to add AI-related functionality, keep human judgment visible and required.
- If requirements are underspecified, align decisions to the current site rather than inventing a new product direction.
