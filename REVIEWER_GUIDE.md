# Reviewer Guide

This guide is for RevolutionVA team members who review Pop-up Meetup proposals.

## Review Timeline

New proposals should receive a response within 7 days of submission. The GitHub Actions workflow automatically posts an acknowledgment comment when a new issue is opened.

## Label Workflow

Move issues through these labels as they progress:

| Step | Label to Apply |
|---|---|
| Issue opened (auto) | `needs-review` |
| Actively being evaluated | `in-review` |
| Revisions requested from speaker | `changes-requested` |
| Approved, scheduling in progress | `approved` |
| Date and venue confirmed | `scheduled` |
| Not a fit, issue closed | `declined` |

## Evaluation Criteria

Review each proposal against these questions:

**Relevance**
- Is this topic useful or interesting to the Hampton Roads developer community?
- Does it fit the spirit of Pop-up Meetups (informal, accessible, community-driven)?

**Clarity**
- Is the abstract clear enough for an attendee to know what they're getting?
- Is the format and duration realistic?

**Feasibility**
- Do we have (or can we find) a venue that fits the format and AV needs?
- Is the speaker's availability workable?

**Inclusivity**
- Is this talk accessible to the stated audience level?
- First-time speakers should be encouraged. If a proposal needs polish, offer feedback rather than declining outright.

## Approving a Proposal

1. Apply the `approved` label and remove `needs-review` / `in-review`.
2. Comment on the issue with:
   - Confirmation of approval
   - Next steps (venue coordination, scheduling)
   - A request for any missing info needed to move forward
3. Begin venue matching. Check the venue list (open issues with the `venue-submission` label) or reach out to known venues.

## Requesting Changes

1. Apply `changes-requested`, remove `in-review`.
2. Comment with specific, actionable feedback. Be encouraging — the goal is to help the speaker improve the proposal, not to gatekeep.
3. Once the speaker updates the issue, re-enter the review loop.

## Declining a Proposal

Declining should be rare. If a proposal isn't a fit:

1. Apply `declined` and close the issue.
2. Comment with a brief, respectful explanation. Where possible, suggest alternatives (a different format, a future submission, another local group that might be a better fit).

## Scheduling Checklist

Once a talk is approved and a venue is confirmed:

- [ ] Date and time agreed with speaker
- [ ] Venue confirmed and contact info on file
- [ ] Meetup event created on [757 Developers](https://www.meetup.com/757dev/)
- [ ] Event listed on 757tech.org (submit to the community site repo or contact Kevin)
- [ ] Announcement drafted for 757 Tech Newsletter and Slack
- [ ] Issue label updated to `scheduled`
- [ ] Speaker sent the [Speaker Guide](SPEAKER_GUIDE.md) link

## Post-Event

- Comment on the issue to close the loop (attendance, any issues, notes for next time)
- Close the issue once the event has occurred
