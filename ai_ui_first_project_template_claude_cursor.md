# AI UI‑First Project Template

**GitHub Starter Repository**\
Claude `ui-designer` + Cursor

> This repository is intended to be used as a **GitHub Template Repo**.
> Click **“Use this template”** to start a new project.

This template is a **repeatable, design‑first project structure** for beginners using **Claude’s ****************************************************************************`ui-designer`**************************************************************************** skill inside Cursor**.

Use this **at the start of every new project** to avoid inconsistent UI, vague requirements, and premature coding.

---

## How to Use This Template (Every New Project)

1. Copy this entire folder structure
2. Fill in files **top to bottom**
3. Do **not** skip steps
4. Do **not** write code until Step 6

This ensures AI behaves like a **designer → product manager → developer** (in that order).

---

## Repository Structure (Starter)

```
ai-ui-first-template/
├── reference-images/
│   └── app-inspiration/
│       └── .gitkeep
├── documents/
│   ├── designs/
│   │   └── .gitkeep
│   ├── prd/
│   │   └── .gitkeep
│   └── ux-design/
│       └── .gitkeep
├── project-idea.md
├── README.md
├── .gitignore
├── LICENSE
└── .github/
    └── ISSUE_TEMPLATE/
```

> `.gitkeep` files allow empty folders to exist in GitHub.
> These are meant to be replaced as the project progresses.

---

## STEP 1 — Add UI Reference Images (Design Input)

**Purpose:** Give AI visual context before it thinks or builds.

### Rules

- 3–10 screenshots max
- Same general product category
- Similar visual style

### Folder

```
reference-images/app-inspiration/
```

**Good Sources:**

- SaaS dashboards
- Mobile app UIs
- Landing pages
- Internal products you admire

---

## STEP 2 — Write the Project Idea (Plain English)

**File:** `project-idea.md`

### Template

```md
# Project Idea

## What is this product?
(Describe in simple terms.)

## Who is it for?
(Non-technical description.)

## What problem does it solve?
(One or two sentences.)

## Desired tone and feeling
- Professional / Friendly / Calm / Bold
- Trust level
- Simplicity vs power
```

✱ Do **not** include technical details.

---

## STEP 3 — Run Claude `ui-designer` Skill (MANDATORY FIRST AI STEP)

**This step extracts a design system from images.**

### Cursor Prompt (Copy Exactly)

```
Use the ui-designer skill.

Reference images are located in:
reference-images/app-inspiration/

Extract a complete design system including:
- Color palette (with hex values)
- Typography (font families, sizes, weights)
- Button, card, input styles
- Spacing system
- Visual hierarchy rules
- Notable patterns across screens
- Animation techniques

Output a complete markdown design system.
```

### Save Output

**Location:**

```
documents/designs/app-inspiration_design_system.md
```

This file becomes your **design authority**.

---

## STEP 4 — Generate MVP PRD (Product Thinking)

**Goal:** Turn idea → structure.

### Claude Prompt

```
Using project-idea.md, generate an MVP PRD including:

- Elevator pitch
- Problem statement
- Target audience
- MVP feature list
- UX/UI considerations

Ask clarifying questions if necessary.
```

### Save Output

```
documents/prd/mvp_prd.md
```

---

## STEP 5 — Create the Final UI Implementation Prompt

**This is the most important artifact.**

It combines **design rules + product requirements** into a build‑ready instruction set.

### Claude Prompt

```
Combine the following into a single implementation-ready UI prompt:

1. Design system from:
documents/designs/app-inspiration_design_system.md

2. MVP PRD from:
documents/prd/mvp_prd.md

The output should:
- Define visual principles
- Specify colors, typography, spacing
- Describe app screens and components
- Be suitable for building a web app

Output only the final prompt.
```

### Save Output

```
documents/ux-design/final_ui_prompt.md
```

---

## STEP 6 — (ONLY NOW) Begin UI Development

At this point you may:

- Create a React project
- Use Cursor IDE to generate components
- Feed `final_ui_prompt.md` into Claude

### Rule

❌ No design decisions outside this file
✅ All UI must follow this prompt

---

## README.md (Repository Root)

```md
# AI UI‑First Project

This project uses a **design‑first AI workflow** powered by Claude’s `ui-designer` skill and Cursor.

## How to Start a New Project

1. Click **Use this template** on GitHub
2. Rename the repository
3. Add UI screenshots to `reference-images/app-inspiration/`
4. Fill out `project-idea.md`
5. Run the Claude workflow in order (see below)

## Required Workflow Order

1. UI reference images
2. Design system extraction (Claude ui-designer)
3. MVP PRD generation
4. Final UI implementation prompt
5. Front‑end development

❗ **Do not write code before Step 4 is complete.**

## Source of Truth

All UI decisions must follow:
```

documents/ux-design/final\_ui\_prompt.md

```

## Recommended Tech Stack (After Step 4)
- Next.js / React
- Tailwind CSS
- shadCN UI
- Lucide Icons
- Rive / GSAP / Unicorn Studio (optional)
```

md

# Project Name

This project follows the AI UI‑First workflow.

## Workflow

1. Visual references
2. Design system extraction
3. MVP PRD generation
4. Unified UI implementation prompt
5. Front-end development: use Next.js, React,
   shadCN, TailwindCSS, Rive, GreenSock for animations, Unicorn Studio,

## Source of Truth

See: documents/ux-design/final\_ui\_prompt.md

````

---

## Why This Template Works

- Prevents premature coding
- Forces consistency
- Makes AI predictable
- Scales to teams
- Easy to restart or revise

This is a **design‑led, AI‑assisted product system**, not a prompt experiment.

---

## Recommended Reuse

For every new project:

1. Duplicate this folder
2. Replace images
3. Rewrite `project-idea.md`
4. Re-run steps 3–5

No exceptions.

---

## Optional Extensions (Advanced)

- Add `/branding/` for logos
- Add `/tokens/` for design tokens
- Add `/components/` docs
- Version prompts with timestamps

---

## .gitignore (Recommended)

```gitignore
node_modules
.next
.env
.env.local
.DS_Store
````

## LICENSE

Use **MIT License** for maximum reuse and flexibility.

---

## How to Publish This as a GitHub Template Repo

1. Create a new GitHub repository
2. Name it:
   `ai-ui-first-template`
3. Push this folder structure
4. Go to **Repo Settings → Template Repository**
5. Enable **“Template repository”**

Users can now click **Use this template** to start instantly.

---

## When to Fork vs Template

- **Template:** New product ideas
- **Fork:** Evolving the workflow itself

---

**This repository is intentionally strict.**

Constraints are what make AI useful.

