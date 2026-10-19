# Self-assessment report

Project: **Ví minh chứng ĐRL (ĐRL Evidence Wallet)**

Course: **CSC13008 — Web Application Development** · Class: **24KTPM1**

Assignment: **PA#1 — Idea and Wireframe**

Team: Lê Nguyễn Quốc Học (24127044), Thái Quang Huy (24127177), and Trần Hoàng Phúc (24127505).

This assessment follows the five criteria in the supplied PA#1 rubric (pages 1-3). Evidence refers to the current proposal, original-size PNG mockups, and AI usage log. Static mockups are explicitly accepted; clickable interactions and working application code are not required for this milestone.

## Criteria, scores, and evidence

| Criterion | Max points | Self-assessed points | Evidence and justification |
| --- | ---: | ---: | --- |
| The problem and the users | 20 | 20 | [The Problem](PROPOSAL.md#2-the-problem) is one paragraph describing the difficulty of organizing activity evidence before an appeal window. It contains neither "platform" nor "ecosystem". [Users](PROPOSAL.md#3-users) names HCMUS students and explains their job: organize activity records by item, check completeness, and retrieve evidence when needed. This meets the 17-20 band. |
| Scope, with a Not building list | 15 | 14 | [Scope](PROPOSAL.md#5-scope) has eight Building bullets and nine concrete Not building exclusions, including score calculation, school integration, OCR, certificate verification, and native mobile apps. One role, one seeded semester, and fixed rules limit the work. This meets the 13-15 band; one point is reserved because authentication, private uploads, CRUD, and the additional counted/missing workflow still create a substantial workload for three people in eight weeks, without a detailed delivery plan. |
| Three screens of the main flow | 35 | 35 | [Screen 1](wireframes/screen-1.png), [Screen 2](wireframes/screen-2.png), and [Screen 3](wireframes/screen-3.png) follow item selection, activity entry, and checking in order. The app-specific sample activity and date error are consistent. Text is readable in the individual PNGs at their submitted size. The [flow diagram](wireframes/flow.png) shows add, save-and-check, cancel, edit, and completion paths; [Screens](PROPOSAL.md#6-screens) also explains group expansion, other Add evidence buttons, form selections, and the file picker. This meets the 30-35 band. |
| Each screen explained | 15 | 15 | [Screens](PROPOSAL.md#6-screens) explains what the student is trying to do on every screen and where each action leads. It describes cancellation without saving, editing with retained values, and returning to the checklist with the saved record's status and updated counts. The descriptions match the illustrated activity and explain that checking is based on app rules rather than official university acceptance. This meets the 13-15 band. |
| AI-LOG.md | 15 | 14 | [AI usage log](AI-LOG.md) has ten tasks attributed to team members: three from Quoc Hoc, three from Hoang Phuc, and four from Quang Huy. Each records Tool, Asked for, Kept, Changed, Rejected, and By hand. Specific rejection reasons include unsupported demand claims, a Word template instead of Markdown, and a failed arrow-generation script. This meets the 13-15 band; one point is reserved because some entries describe rejected features or ideas generically instead of identifying concrete suggestions and their reasons. No TODO fields remain. |
| **Total** | **100** | **98** | **20 + 14 + 35 + 15 + 14 = 98.** |

## What we did not manage

- We have not validated demand through user interviews. The problem is a proposal supported by the described workflow, not a claim of measured demand; interviews are not required by this rubric.
- Some AI-log entries remain generic about rejected suggestions. The setup entry also acknowledges that file-by-file acceptance and manual contributions were not recorded in detail.
- The additional sign-in and counted/missing workflows are described but not drawn. The three submitted screens cover the selected core activity-recording flow.
- Some mockup labels, including the certificate check and appeal-readiness wording, are broader than the metadata checks the app can perform. The proposal clarifies these limits, but the PNG wording has not been revised.

The artifacts are static mockups, an accepted PA#1 format. Authentication, persistent storage, access control, uploads, and rule execution are planned for later assignments and have not been implemented or tested.

## Submission total

The team's proposed total is **98/100**. Following the rubric's ascending-ID naming rule, the submission ZIP should be named **24127044-24127177-24127505_98.zip** and contain the proposal, three screen images, AI log, and this report. Preserve the relative image paths; include the supplementary flow diagram because the proposal links to it.

This is a self-assessment, not a confirmed instructor grade. The rubric's honesty adjustment applies to the difference between the claimed total and the awarded mark.
