# Contributing

Thanks for helping improve this list. The goal is to keep it useful as a research map, not just long as a bibliography.

## What belongs here

- Papers, project pages, code, datasets, hardware guides, or build notes directly about UMI, UMI-style handheld data collection, robot-free manipulation demonstrations, or deployment of UMI-trained policies.
- Closely related background resources when they help readers understand UMI policy learning, data scaling, cross-embodiment deployment, tactile sensing, or contact-rich manipulation.
- Resources with stable public links and enough context for a reader to evaluate them.

## What usually does not belong here

- General robot learning papers with no clear connection to UMI-style data or deployment.
- Marketing pages without technical details, papers, code, data, or reproducible hardware information.
- Duplicate entries in multiple sections. Pick the most important primary category and use a short cross-reference if needed.
- Dead links, private documents, or unpublished internal notes.

## Entry format

Use this format whenever possible:

```markdown
- [Resource Title](https://example.com) - One sentence explaining why it matters for UMI. `label` [project](https://example.com) [code](https://github.com/example/repo) [data](https://example.com/data)
```

Keep descriptions short and specific. Prefer "what this adds to the UMI family" over copying an abstract.

Useful labels:

- `paper`
- `preprint`
- `project`
- `code`
- `data`
- `hardware`
- `survey`

## Categorization

- Put each paper in one primary section.
- If a paper spans multiple themes, choose the theme that best captures its main contribution.
- Use the policy section for methods whose main contribution is learning, representation, or inference-time guidance.
- Use the tactile section for interfaces whose main contribution is sensing, force, compliance, or contact-rich collection.
- Use datasets only for dataset resources or papers whose main contribution is dataset scale.

## Pull request checklist

- The link is public and stable.
- The resource is not already listed under another name.
- The description is one sentence.
- The entry has a label such as `paper`, `preprint`, `code`, `data`, or `hardware`.
- Markdown links work.
- New sections are added only when several resources need them.

## Style

- Use English for the README.
- Keep entries concise and neutral.
- Prefer official project, paper, code, and dataset links over mirrors.
- For arXiv-only work, mark the entry as `preprint`.
- Do not use hype words such as "best", "ultimate", or "state-of-the-art" unless they are part of an official title.
