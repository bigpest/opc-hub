# Contributing to OPC-Hub

Thanks for wanting to add to OPC-Hub. This is a knowledge base for people running — or trying to run — one-person companies. The best contributions come from people who actually did the thing and can say what it cost them.

## What belongs here

- First-hand stories from solo founders, indie makers and one-person operators.
- Tactics that a single person can execute without hiring: validation, MVPs, pricing, distribution, legal/admin, focus and burnout.
- Playbooks and checklists that someone else can copy today.
- Corrections to existing content.

## What does not belong here

- Ads, affiliate links, referral codes or any form of paid promotion.
- "Thought leadership" with no first-hand experience behind it.
- Links to your product as the main point of the submission. Mentioning your product as context is fine; pitching it is not.
- Content unrelated to one-person companies.
- Private information about other people.

## Ways to contribute

| You want to... | Do this |
|---|---|
| Share a founder story | Open an issue with the **Founder story** template |
| Share a tactic or playbook | Open an issue with the **Tactic or playbook** template |
| Fix a typo or broken link | Open a pull request directly, or use the **Correction** issue template |
| Discuss an idea | Start a thread in Discussions |

## Repository layout

```
.
├── README.md
├── CONTRIBUTING.md
├── .github/
│   ├── ISSUE_TEMPLATE/
│   └── workflows/
├── stories/     # one Markdown file per founder story
├── tactics/     # one Markdown file per tactic
└── playbooks/   # copy-and-use checklists and templates
```

Put new files in the folder that matches the content type. If a piece spans two folders, put it where the reader will look for it first and link to it from the other.

## Story submissions

A story should answer:

1. **Starting point** — what you were doing, what resources you had.
2. **What you tried** — in order, including the things that failed.
3. **What it cost** — time, money and the parts that hurt.
4. **What actually happened** — outcome, with numbers where you have them.
5. **What you would tell someone starting today.**

Keep it honest. Failed stories are as useful as successful ones — arguably more so.

## Tactic and playbook submissions

A tactic should include:

- The problem it solves and who it is for.
- Step-by-step instructions someone can follow.
- Time and money required.
- Pitfalls and edge cases.
- Evidence from your own use, not just theory.

## Style guide

- Write in English, plain and specific. Avoid hype.
- Use Markdown. One H1 per file.
- File names: lowercase, hyphen-separated, descriptive. Examples: `pricing-without-a-sales-team.md`, `story-003-first-100-customers.md`.
- Front matter at the top of every content file:

```markdown
---
title: Pricing without a sales team
author: your-github-handle
date: 2026-10-24
tags: [pricing, solo-founder]
---
```

- Link to other files with relative links, e.g. `../tactics/pricing.md`.
- Use a hosted image URL (or an image host) for screenshots. Do not commit large binaries.
- Translations: keep the English file as the reference and add the translation as `<name>.zh.md`, with a one-line language link under the front matter on both files.
- Anonymize people and companies you do not have permission to name. Remove phone numbers, addresses, emails and anything else identifying.

## Pull request workflow

1. Fork the repository.
2. Create a branch from `main`:
   `git checkout -b docs/add-story-003`
3. Make your change and commit.
4. Push the branch and open a pull request against `main`.
5. Describe what you added and why in the PR description.

Branch names:

- `docs/add-<topic>` for new content
- `fix/<topic>` for corrections
- `chore/<topic>` for structure or tooling

Commit messages:

- `docs: add pricing tactic for solo founders`
- `fix: broken link in founder story 12`
- `feat: add burnout prevention checklist`
- `refactor: reorganize tactics folder`
- `chore: update gitignore`

## Review

Maintainers review pull requests in batches, usually once a week. Small fixes are merged quickly. New stories and longer tactics may sit for a few days to allow comments. If a submission is out of scope we will close it and say why.

## License

OPC-Hub is licensed under Apache-2.0. By submitting a contribution you agree that it is licensed under the same terms.
