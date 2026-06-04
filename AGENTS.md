# Project Constraints & Workflow

- **Task:** Read content exclusively from `source.md` in this directory and generate a fully responsive, clean, static single-page website (`index.html` or a structured `dist/` folder with separate HTML, CSS, and JS).

- **Core Requirement:** Do NOT generate arbitrary placeholder text. Parse the Markdown hierarchy, code blocks, and lists from `source.md` and translate them into (semantic) HTML elements.


# Model Restrictions

- **Enforced Models Only:** You must strictly use Google Gemini models for all background operations, code writing, and structural layouts. 

- **Primary Agent (Coding & Architecture):** `gemini-3.1-pro`

- **Subagents (Asset Generation & Quick Fixes):** `gemini-3.5-flash`

- *Restriction:* Under no circumstances should you invoke or route tasks to Claude or GPT-OSS models for this workspace.


# Design & Aesthetic Guidelines

You must build the UI around a modern, editorial reading experience reminiscent of high-end literary or research platforms. Stick strictly to these visual properties:


- **Background:** Clean, warm off-white with a subtle yellowish/brownish parchment undertone (`#fdfbf7` or `#faf6ee`). Avoid clinical pure white (`#ffffff`).

# Typography & Fonts

- **Google Fonts Import:** Include `<link href="https://fonts.googleapis.com/css2?family=Newsreader:ital,opsz,wght@0,6..72,400..700;1,6..72,400..700&display=swap" rel="stylesheet">` in the HTML head.

- **CSS Font Stack:** 
  - Headings: `font-family: "Newsreader", "Georgia", serif;`
  - Body text: `font-family: "Google Sans", sans-serif;`

- **Typography Sizing:** 

  - Body text: `1.15rem` to `1.25rem` for an effortless reading feel.

  - Line Height: `1.65` or `1.7` to give the text breathing room over the warm background.

  - Text Alignment: Normalize text from right and left (`text-align: justify;` with `hyphens: auto;`) for a clean editorial block feel.

  - Headings: Use slightly heavier weights (`600` or `700`) of the heading font to keep the design cohesive.

- **Color Palette:**

  - **Primary Text / Solids:** Deep soft black (`#1a1a1a` or `#222222`)

  - **Secondary Accents / Borders:** Rich walnut brown (`#4a3525` or `#5c4a3c`)

  - **Highlights / Active Elements / Callouts:** Striking clean terracotta or deep crimson red (`#a62626` or `#b81d24`)


# Dynamic Updates & Pedagogical Patterns

- **Fonts:** Replaced Google Sans with Adwaita Sans for body text.
- **Code Blocks:** `font-weight` set to medium (500) for better readability on parchment background.
- **Code Comments:** PrismJS integrated. Comments inside code blocks are specifically styled as translucent italics (`opacity: 0.6`).
- **Anatomie Pattern:** Complex code files (Jenkinsfile, Dockerfile, docker-compose, K8s Pods/Deployments) are broken down into logical steps using `<div class="anatomie-step theme-X">`. Each theme uses a distinct CSS border/heading color.
- **Blockquotes:** Used extensively to define core concepts (Volumes, PV/PVC, ConfigMap, Secret) directly before their associated code listings.
