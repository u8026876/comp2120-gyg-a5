# COMP2120 A4 presentation kit

This is the group's approved warm visual style. Give this folder to Codex or Claude so each member's slides can be assembled into one consistent presentation. A Google account is not required: the PPTX and reference PDF are in this repository.

## Kyubin's final handoff: three main slides

Use these three files, in this order, for Kyubin's main contribution. These numbers identify this handoff; the group may assign different positions in the assembled presentation.

| Order | File | Topic |
| --- | --- | --- |
| 1 | [final-draft-slide-1.pptx](final-draft-slide-1.pptx) | Q1: project choice |
| 2 | [final-draft-slide-2.pptx](final-draft-slide-2.pptx) | Q2: issue choice |
| 3 | [final-draft-slide-3.pptx](final-draft-slide-3.pptx) | Challenges: defining correct behavior |

[Preview slide 3](final-draft-slide-3-preview.png). Speaking scripts and sources are in the PPTX notes.

The two earlier TIKA-4431 technical slides are optional backups for questions, outside the three-slide main handoff:

- [Problem and before/after behavior](backup-TIKA-4431-problem.pptx)
- [Fix, compatibility boundary and test evidence](backup-TIKA-4431-fix-and-evidence.pptx)

Other Kyubin section files in this folder are source packages or earlier variants. Use the three numbered files above for the main contribution to avoid duplicate slides.

## Start here

1. Read [AGENTS.md](AGENTS.md) and [design-tokens.json](design-tokens.json).
2. Open or import [the editable PowerPoint template](COMP2120-A4-warm-template.pptx). Duplicate a suitable slide and replace its prompts; keep the native text and layout.
3. Use [the PDF](COMP2120-A4-warm-template.pdf) and [preview](preview.png) to check appearance. [The TIKA-4431 example](example-tika-4431.png) shows a completed problem slide; it is Kyubin's work, not a contribution for other members to claim.
4. Return your editable section as `<name>-<issue>-section.pptx`, with a PDF or PNG preview and source-bearing speaker notes. Aim for roughly 55 seconds; coordinate any extra time or slides with the group.
5. Reply to the template announcement with your name, issue/contribution and chosen layout so we can coordinate the final assembly.

The template is a layout library, not a finished seven-slide talk. Keep only the slides your section needs. The last guide slide is deliberately skipped.

## Layouts

| Template slide | Use | Background |
| --- | --- | --- |
| 1 | Cover or contribution introduction | Forest |
| 2 | Problem: one large input with before/after interpretation | Forest hero + warm paper comparison |
| 3 | Decision: alternative, chosen rule, boundary, trade-off | Warm paper |
| 4 | Evidence: regression, exact scope/result, lesson | Forest |
| 5 | Explanation beside code, screenshot or diagram | Warm paper |
| 6 | Demonstration: one input and one visible result | Forest |
| 7 | Guide for using the kit | Sage; skip in presentation |

The completed group draft has separate teammate slots, Kyubin's section and technical backups. This kit contains clean prompts and does not supply anyone's results.

## Approved design

- Canvas: 16:9, 960 by 540 points.
- Forest `#203B34`; warm paper `#F0E8D9`; light terracotta `#D99575` on dark backgrounds; rust `#A14F37` on light backgrounds; sage `#B8C7AB`; sage background `#D8DFCE`.
- Use Manrope for headings and prose; Roboto Mono for code, filenames and small technical labels. Preserve the existing font sizes and geometry. Typical title: 32–36 pt; body: about 20 pt; hero code: 48 pt.
- Use color to explain the issue: terracotta for the character or interpretation that causes the problem; forest/paper for the main content. Keep layouts flat and avoid adding repeated cards, pill labels, shadows or unrelated decoration.
- If a font is missing, report it before choosing a substitute. Do not silently re-theme the section.
- Shorten text or choose another supplied layout before reducing the type. Keep meaningful screenshots fully visible and preserve their proportions.

## Content and evidence

Explain the trigger, why the issue mattered, the decision, one piece of evidence and what you learned. Keep detailed commands, revisions, sources and a timed speaking script in speaker notes. State the limits that affect your conclusion on the slide as well.

Use your actual work and current links. Distinguish local checks, human review, a group PR, an upstream PR and a merge. Do not invent test results, dates, approvals, authorship or understanding. Disclose AI and other assistance accurately.

The public A4 brief sets a maximum ten-minute group presentation plus a separate 3–5 minute Q&A: https://comp.anu.edu.au/courses/comp2120/assignments/assignment4/

## Prompt to give Codex or Claude

```text
Prepare my COMP2120 A4 contribution slides using the presentation/ folder in
u8026876/comp2120-gyg-a5.

Read presentation/AGENTS.md, presentation/README.md and
presentation/design-tokens.json. Reuse native slides from
presentation/COMP2120-A4-warm-template.pptx; inspect the reference PDF and
preview first. Follow the supplied forest / warm paper / terracotta style,
fonts, spacing and hierarchy. Do not design a new theme.

My name and GitHub username:
My issue or contribution:
My actual work, decisions and evidence:
My issue / commit / PR links:
My collaborators and AI assistance:

Ask me for missing facts; do not invent them. Explain my trigger, decision,
evidence and lesson in about 55 seconds. Put source links and a suggested
script in speaker notes. Return editable PPTX slides plus a rendered PDF or
PNG preview, and inspect for overflow, clipping and font substitution.
```

## Scope

These files are COMP2120 group coordination assets. Keep the entire `presentation/` folder out of patches and PRs intended for Apache Tika. Publishing this kit does not submit anything to Canvas.

Prepared with Codex at Kyubin Park's request, 21 October 2026.
