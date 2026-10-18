# Self-assessment report

Project: **Ví minh chứng ĐRL (ĐRL Evidence Wallet)**

Course: **CSC13008 — Web Application Development** · Class: **24KTPM1**

Assignment: **PA#1 — Idea and Wireframe**

Team: Lê Nguyễn Quốc Học (24127044), Thái Quang Huy (24127177), and Trần Hoàng Phúc (24127505).

This assessment covers the proposal and mockups currently in the repository. It uses the five criteria and maximum scores from the existing assessment template. The original rubric PDF is not included in the repository, so the team should confirm the scoring criteria and accepted mockup format before submission.

## Criteria, scores, and evidence

| Criterion | Max points | Self-assessed points | Evidence and justification |
| --- | ---: | ---: | --- |
| Problem and users | 20 | 20 | [Problem](PROPOSAL.md#2-the-problem) and [Users](PROPOSAL.md#3-users) identify HCMUS students, scattered evidence, and the need to prepare records before the appeal window closes. The goal is concrete: organize each activity under its ĐRL item and identify incomplete records early. |
| Scope and Not building | 15 | 15 | [Scope](PROPOSAL.md#5-scope) defines a single student role, one predefined semester, activity CRUD, owner-only evidence access, fixed checks, and counted/missing tracking. Nine explicit exclusions constrain the project, including score prediction, automatic appeals, school integration, OCR, and certificate verification. |
| Three screens of main flow | 35 | 35 | [Screen 1](wireframes/screen-1.png), [Screen 2](wireframes/screen-2.png), and [Screen 3](wireframes/screen-3.png) follow one activity from item selection through entry to a checklist result. The [flow diagram](wireframes/flow.png) labels forward, cancel, edit, and completion paths. The example consistently uses item 4.3 and demonstrates an out-of-period date error. These are static PNG mockups. |
| Each screen explained | 15 | 15 | [Screens](PROPOSAL.md#6-screens) explains each screen's purpose, displayed information, actions, and destinations. It covers group expansion, the file picker, cancellation, retaining form values on edit, and the checklist update after completion. It also explains the difference between reference checks and official school results. |
| AI-LOG | 15 | 13 | [AI usage log](AI-LOG.md) attributes all six entries through Logged by and describes tools, requests, accepted output, changes, rejected suggestions, and manual work. Entries explain corrections to terminology, rules, and mockups. Two repository-setup fields still contain TODOs, so this criterion is not assessed at full marks. |

## Total score

**98 / 100** = 20 + 15 + 35 + 15 + 13.

This is a proposed self-assessment based on the available artifacts. Full points for the screen criterion assume that static mockups with a labelled flow diagram meet the official submission requirements.

## What we did not manage

- The repository-setup entry in AI-LOG still needs confirmation of which generated files were accepted and which parts the team wrote by hand.
- The project idea has not been validated through user interviews, as noted in the research comparison log. The problem and workflow are a proposal rather than demonstrated user demand.
- The supplied screen artifacts are static images. They illustrate navigation and validation results but do not provide clickable interactions or working file uploads.

Application implementation is planned for later assignments. Login, persistent storage, evidence access control, and automatic rule checks have not been implemented or tested. The proposal describes sign-in and the later counted/missing workflow, but those steps are outside the three-screen mockup.

## Final review before submission

- Confirm the criteria, point weights, mockup format, and packaging requirements against the official rubric.
- Complete the remaining AI-log fields with the actual team decisions and review the final self-assessed score.
- Verify that the submitted package preserves the relative paths between the proposal and all four PNG files.
