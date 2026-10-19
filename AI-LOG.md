# AI usage log

## 2026-10-17 - Repository setup

- **Logged by:** Lê Nguyễn Quốc Học
- **Tool:** OpenAI Codex.
- **Asked for:** Create a minimal PA#1 repository skeleton, keep wireframes as `.gitkeep`, and use concise English documentation.
- **Kept:** The minimal repository structure for the PA#1 Markdown deliverables and the wireframes directory. Which generated file contents were accepted unchanged was not recorded.
- **Changed:** Documentation was translated into English and the AI log shortened and reformatted at the user's request.
- **Rejected:** Unnecessary features outside the PA#1 scope.
- **By hand:** No manual writing or edits were reported for this setup step; this does not establish that none occurred.

## 2026-10-17 — Research Web project ideas

- **Logged by:** Lê Nguyễn Quốc Học
- **Tool:** ChatGPT with web search and PDF reading.
- **Asked for:** Compare solution gaps, product value, feasibility, and alignment with the PA#1 rubric.
- **Kept:** Research summary and comparison of ProofLock, ThesisGate, and FundFlow.
- **Changed:** Shortened the AI log for submission.
- **Rejected:** Claims of unique features already offered by competitors, and scopes too large for the course.
- **By hand:** No manual edits or independent verification were reported.

## 2026-10-17 — Compare research recommendations

- **Logged by:** Lê Nguyễn Quốc Học
- **Tool:** ChatGPT with PDF reading.
- **Asked for:** Compare the earlier project research with the PA#1 Deep Research report.
- **Kept:** The report’s DRL Evidence Wallet recommendation as an alternative to ProofLock and ThesisGate.
- **Changed:** Distinguished documented workflows from assumptions about user needs.
- **Rejected:** Treating either report’s ranking as proof of demand; neither included user interviews.
- **By hand:** No manual changes or independent validation were reported.

## 2026-10-17 — Understanding the brief and the ĐRL rules

- **Logged by:** Trần Hoàng Phúc.
- **Tool:** Claude (claude.ai, Claude Opus 5.5) with web search.
- **Asked for:** explain the rubric and slides; review the two idea reports a teammate made with ChatGPT and compare them by complexity and fit with the course; check how ĐRL works at HCMUS; write a project overview (PROJECT_OVERVIEW.md) as shared context for the team.
- **Kept:** the recommendation to build the ĐRL evidence idea instead of ProofLock or ThesisGate (one role, a clear three-step flow, fits CRUD + JWT + upload in PA#4); the split of ĐRL items into "activities with evidence" (the app's focus), "recorded by the school" and "personal circumstances" (not built); the evidence check rules (activity period, certificate for off-campus activities, online interactions not counted, item-specific fields such as hours for volunteering, original paper for blood donation); the Not building list.
- **Changed:** Claude's first suggestions used "phúc khảo", semester dates and made-up criterion names; after it read the school's 2025–2026 ĐRL notices we switched to "khiếu nại" and the activity period. Claude could only find the old 2016 regulation online, so I downloaded the current one (QĐ 1028/2020, amended by QĐ 2739/2023) and had it checked: the groups, maximum points and item numbers had all changed (e.g. volunteering is now 4.3 and scored by hours, and the old "max 2 times per semester" limit no longer exists). We updated the overview, the wireframes and the Screens text to match.
- **Rejected:** a Word report template (the brief asks for .md files); any feature that predicts the final ĐRL score.
- **By hand:** found and downloaded the current ĐRL regulation; made the final topic decision together with my teammates after comparing the options.

## 2026-10-17 — Three wireframes

- **Logged by:** Trần Hoàng Phúc.
- **Tool:** Claude Design, with prompts drafted together with Claude.
- **Asked for:** a mobile-width web mockup of the three main-flow screens, in Vietnamese, with arrows labelled by the button that triggers each step.
- **Kept:** layout, colours, wording, the example activity used across all three screens.
- **Changed:** across several rounds: the summary count was wrong (our prompt's mistake); the chosen item first showed "needs more evidence", which made adding a new activity look odd, so it now starts with no evidence; equal-height phone frames cut off the file upload, so we went back to full-page screens; long URLs overflowed and were shortened. After we got the current ĐRL regulation, we regenerated the screens with its six groups, moved the example to item 4.3 and added an hours field, then fixed a truncated file name and buttons that wrapped onto two lines.
- **Rejected:** the generated script that measured elements to draw arrows (it crashed with "Cannot read properties of null (reading 'offsetWidth')"); replaced with fixed SVG arrows. Also rejected a desktop version: we keep mobile width because students save evidence on their phones, and the app stays a responsive web app, not a native app.
- **By hand:** checked every version against the regulation and the Screens text, including that each button in the drawings is explained; exported the images and renamed them to screen-1.png, screen-2.png, screen-3.png and flow.png.

## 2026-10-17 – 18 — Screens section, review of `PROPOSAL.md`, and this log

- **Logged by:** Trần Hoàng Phúc.
- **Tool:** Claude.
- **Asked for:** a draft of the Screens section (one paragraph per screen, matching our final wireframes); a review of the whole `PROPOSAL.md` once the team had written it; a draft of my entries in this log.
- **Kept:** the three screen paragraphs, including the explanation of buttons that have no arrow in the drawings (expanding a collapsed group, "Thêm minh chứng" on item 4.2, the file picker) and the note that the screens are a full-page mockup at mobile width; the review's fixes for consistency: screen and button names in Vietnamese as in the drawings, status names in Scope matching the screens, "ĐRL item" instead of "DRL criterion", a rewritten Main flow that adds the first and last steps, the matching Building line for marking activities as counted or missing, and fixed image links.
- **Changed:** we added to the Screens text that the activity period and appeal window are reference data stored for the semester and not live-synced with HCMUS systems, and that the check is "complete according to the app's predefined checklist" rather than an official result; in the log, the separate "Not verified" line was merged into "Changed" because the course template has no such field.
- **Rejected:** the first log draft, because it also covered my teammate's ChatGPT research, which they log themselves.
- **By hand:** the Team, Problem, Users and Scope sections were first written by my teammates; I chose which parts of the work to log and checked every draft against what we actually did.

## 2026-10-17 — Project Idea Research
- **Logged by:** Thái Quang Huy — 24127177
- **Tool:** ChatGPT (GPT-6) + Deep Research
- **Asked for:** Research and compare suitable web application ideas based on the PA#1 requirements and rubric.
- **Kept:** The DRL Evidence Wallet idea, including its problem, users, scope, and main flow.
- **Changed:** Focused on a smaller, student-side evidence preparation application.
- **Rejected:** The other 14 ideas in ChatGPT's report, including its two runners-up, Move-in Condition Record (93/100) and Lab Help Queue (92/100); I judged the DRL idea (94/100 in the report) to be the best of them, so we chose it.
- **By hand:** Shared the research report with the team. The team discussed the options and selected DRL.

## 2026-10-17 — Scope Review
- **Logged by:** Thái Quang Huy — 24127177
- **Tool:** ChatGPT (GPT-6)
- **Asked for:** Evaluate the proposed DRL scope and suggest improvements for an 8-week project.
- **Kept:** Predefined criteria, evidence uploads, and rule-based completeness checks.
- **Changed:** Clarified that checklist completion does not guarantee official acceptance.
- **Rejected:** Unnecessary features and overly broad claims about appeal readiness.
- **By hand:** Reviewed the AI feedback and discussed the scope with the team.

## 2026-10-17 — Proposal Drafting
- **Logged by:** Thái Quang Huy — 24127177
- **Tool:** ChatGPT (GPT-6)
- **Asked for:** Complete the PA#1 proposal using project context prepared by a team member.
- **Kept:** The agreed problem, primary user, main flow, and scope.
- **Changed:** Refined the wording and clarified the application's limitations.
- **Rejected:** Claims implying official HCMUS integration or guaranteed evidence acceptance.
- **By hand:** Provided the project context and reviewed the completed proposal.

## 2026-10-17 — Screens Review
- **Logged by:** Thái Quang Huy — 24127177
- **Tool:** ChatGPT (GPT-6)
- **Asked for:** Review Section 6 and the wireframes created by a team member against the PA#1 rubric.
- **Kept:** The existing three-screen flow and wireframe designs.
- **Changed:** Clarified checklist-based status and predefined reference dates in the screen descriptions.
- **Rejected:** Wording implying that the app officially validates appeal evidence.
- **By hand:** Reviewed the AI feedback and requested corrections. The wireframes were created by a team member.

## 2026-10-19 — Documentation polish (commit 80b323f)
- **Logged by:** Lê Nguyễn Quốc Học
- **Tool:** None. No AI tool was used for this commit.
- **Asked for:** Not applicable.
- **Kept:** Not applicable.
- **Changed:** Not applicable.
- **Rejected:** Not applicable.
- **By hand:** Commit 80b323f "Polish PA#1 submission documentation" was made by hand and changed AI-LOG.md, PROPOSAL.md, README.md and SELF_ASSESSMENT_REPORT.md.

## 2026-10-19 — Final review against the rubric (Claude Code)
- **Logged by:** Thái Quang Huy — 24127177
- **Tool:** Claude Code (Claude Sonnet 5.5).
- **Asked for:** A final review of PA#1 against the rubric, and a list of edits: shorten the three screen paragraphs in PROPOSAL.md Section 6, rewrite the self-assessment in the course template, add questions to the thin AI-LOG entries, tidy README.md, and build the submission zip.
- **Kept:** Which edits the team accepted unchanged was not recorded.
- **Changed:** Claude Code rewrote the three Screens paragraphs, moved the limitations into one Notes paragraph, moved the counted/missing bullet under "Last priority" in Scope, marked step 5 of the main flow as last priority, rewrote the self-assessment with a total of 93 (the number given in the request), removed the "Before submission" section from README.md, and added placeholder questions to this log that were later resolved. It did not change the images, the Vietnamese labels, the screen names, or the project scope.
- **Rejected:** Nothing was rejected during the session itself; any later rejection by the team was not reported.
- **By hand:** No manual writing or checking was reported for this step; this does not establish that none occurred.
