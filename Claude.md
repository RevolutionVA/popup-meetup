# CLAUDE.md

This file provides context for AI-assisted work on the RevolutionVA Pop-up Meetups repository.

## Project Overview

Pop-up Meetups is a community initiative by [RevolutionVA](https://revolutionva.org), a 501(c)(3) nonprofit uniting developers in Hampton Roads and Virginia. The initiative enables community members to propose informal tech talks at local venues — coffee shops, libraries, coworking spaces — across the 757 area.

This repository manages the proposal and approval workflow entirely through GitHub Issues and GitHub Actions. It does not contain application code.

## Organization Context

- **RevolutionVA** (revolutionva.org) — Parent organization. President: Kevin Griffin. VP: Linda Nichols.
- **757tech.org** — Hampton Roads tech community hub, maintained by Kevin Griffin, supported by RevolutionVA. Pop-up Meetup events should be listed here.
- **757 Developers on Meetup** (meetup.com/757dev) — The Meetup group where Pop-up events are published. ~2,000 members.
- **757 Tech Newsletter** (757tech.org) — Weekly newsletter covering Hampton Roads tech events. Good channel for promoting approved talks.
- **RevolutionVA GitHub org** (github.com/revolutionva) — This repo lives here alongside other RevolutionVA open source work.

## Repository Structure

```
popup-meetups/
├── CLAUDE.md                          # This file
├── README.md                          # Public-facing overview and speaker instructions
├── CODE_OF_CONDUCT.md                 # Adapted from RevolutionVA's existing CoC
├── SPEAKER_GUIDE.md                   # Post-approval instructions for speakers
├── REVIEWER_GUIDE.md                  # Internal guide for RevolutionVA team reviewers
├── plans/
│   └── plan.md                        # Initiative roadmap and decision log
└── .github/
    ├── ISSUE_TEMPLATE/
    │   ├── talk-proposal.yml          # Structured form for talk submissions
    │   └── venue-submission.yml       # Structured form for venue submissions
    └── workflows/
        └── triage.yml                 # GitHub Actions: auto-comment on new issues
```

## Workflow Summary

1. Speaker opens an issue using the **Talk Proposal** template.
2. GitHub Actions posts an automatic acknowledgment comment.
3. RevolutionVA team triages the issue (labels: `needs-review` → `in-review` → `approved`). Declined issues will be closed with comment.
4. Approved talks are scheduled with a venue; label advances to `scheduled`.
5. Event is listed on Meetup (757dev group) and 757tech.org.
6. Issue is closed after the event occurs.

Venue proposals follow the same flow using the **Venue Submission** template and the `venue-submission` label.

## Labels to Create

These labels must be created manually in the GitHub repo settings — they are not auto-created:

| Label | Color (suggested) | Purpose |
|---|---|---|
| `needs-review` | `#e4e669` | Newly submitted, awaiting triage |
| `in-review` | `#0075ca` | Actively being evaluated |
| `approved` | `#0e8a16` | Approved, scheduling in progress |
| `scheduled` | `#006b75` | Date and venue confirmed |
| `changes-requested` | `#e99695` | Feedback sent, waiting on speaker |
| `declined` | `#b60205` | Not a fit, issue closed |
| `venue-submission` | `#d876e3` | Venue proposal (not a talk) |

## GitHub Actions Setup

The `triage.yml` workflow requires **write permissions for issues**. Enable this at:
Settings > Actions > General > Workflow permissions > Read and write permissions

## Code of Conduct

`CODE_OF_CONDUCT.md` is adapted from the existing RevolutionVA CoCs in the [RevolutionVA/code-of-conduct](https://github.com/RevolutionVA/code-of-conduct) repository. If the source CoC is updated, this file should be reviewed for consistency.

Contact for CoC reports: team@revolutionva.org

## Tone and Voice

When drafting or editing content in this repo, match the existing RevolutionVA voice:
- Friendly and accessible, not corporate
- Welcoming to first-time speakers and newcomers to the community
- Concise — avoid filler language
- Hampton Roads community-specific where relevant (reference 757, local cities, local groups)
- No em dashes

## Related Repositories

- [RevolutionVA/code-of-conduct](https://github.com/RevolutionVA/code-of-conduct) — Source CoC documents
- [RevolutionVA/757-community-site-public](https://github.com/RevolutionVA/757-community-site-public) — 757tech.org source (open for contributions; Pop-up Meetups may warrant a dedicated section)
- [github.com/revolutionva](https://github.com/revolutionva) — Full RevolutionVA GitHub org