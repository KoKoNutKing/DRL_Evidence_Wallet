# ĐRL Evidence Wallet — Ví minh chứng ĐRL

A proposed responsive web app that helps HCMUS students organize activity records and supporting evidence by semester and ĐRL item, check whether each record meets a predefined checklist, and prepare evidence for appeals after preliminary training-point results are published.

Course: **Web Application Development (CSC13008)** · Class: **24KTPM1**

Current assignment: **PA#1 — Idea and Wireframe**

## Team

| Full name | Student ID |
| --- | --- |
| Lê Nguyễn Quốc Học | 24127044 |
| Thái Quang Huy | 24127177 |
| Trần Hoàng Phúc | 24127505 |

## The problem

Activity certificates, participation confirmations, and photos often end up scattered across students' phones, downloads, and messages. When an activity is missing from the preliminary ĐRL result, students need to find its evidence and check its date and applicable ĐRL item before the appeal window closes.

The proposed app keeps these records together and identifies missing information early. Its checklist is for reference; the official ĐRL result comes from the school.

## Main flow and mockups

1. Open the semester checklist and choose an ĐRL item.
2. Add an activity, enter its details, and attach evidence.
3. Review the checklist result, correct missing or invalid information, or keep the record and return to the semester checklist.

The example follows an off-campus volunteering activity under item 4.3. Its date, 28/02/2026, is outside the configured activity period of 02/03–13/09/2026, so the result explains why the record needs changes.

![Main flow with labelled navigation arrows](wireframes/flow.png)

| Screen | Purpose | File |
| --- | --- | --- |
| Danh sách minh chứng học kỳ | Review saved evidence and choose an item to add an activity. | [Screen 1](wireframes/screen-1.png) |
| Thêm minh chứng | Enter activity details and attach a certificate, confirmation, or photo. | [Screen 2](wireframes/screen-2.png) |
| Kiểm tra minh chứng | Review the rule checks, edit the record, or return to the checklist. | [Screen 3](wireframes/screen-3.png) |

Open the PNG files directly or view them through the links above. They are static, full-page mockups at mobile width; navigation is shown by the arrows in the flow image. No installation, dependencies, or server are required to review them. The [proposal](PROPOSAL.md#6-screens) explains each screen and its actions.

## Planned scope

- Email and password registration and login.
- One predefined semester, with stored activity dates, an appeal window, and seeded ĐRL groups and items.
- Create, view, edit, and delete personal activity records, including item-specific details such as volunteering hours.
- Attach images or PDFs, with evidence files accessible only to their owner.
- Check required fields, activity dates, evidence presence, off-campus documentation, and item-specific fields using fixed rules.
- Show evidence completeness and missing requirements; after preliminary results, let students mark activities as counted or missing to prepare appeals.
- Provide a responsive interface designed for use on phones.

The scope excludes score calculation or prediction, automatic appeal submission, school-system integration or SSO, AI/OCR, certificate authenticity verification, regulation administration or automatic updates, personal-circumstance records, native mobile apps, and notifications. See the [full scope](PROPOSAL.md#5-scope) for details.

## Current status

This repository contains the project proposal, three screen mockups, a flow diagram, an AI usage log, and a self-assessment. Application implementation and technology selection are pending. Authentication, storage, uploads, and rule checks described above are planned features.

Sign-in and the later counted/missing activity workflow are described in the proposal but are outside the three illustrated screens. Semester dates and the appeal window shown in the mockups are predefined reference data, with no live connection to HCMUS systems.

## Repository guide

```text
README.md                     Project overview and review instructions
PROPOSAL.md                   Team, problem, users, main flow, scope, and screens
AI-LOG.md                     AI use, attribution, and decisions about output
SELF_ASSESSMENT_REPORT.md      Scores, evidence, and remaining work
wireframes/
  flow.png                    Three-screen flow with navigation arrows
  screen-1.png                Semester evidence checklist
  screen-2.png                Add evidence
  screen-3.png                Evidence check
docs/
  README.md                   Placeholder for later development documentation
```

## Before submission

- Confirm the official rubric, accepted mockup format, deadline, and packaging requirements.
- Resolve the remaining repository-setup TODOs in [AI-LOG.md](AI-LOG.md) and review each member's actual AI usage.
- Review the [self-assessment](SELF_ASSESSMENT_REPORT.md) and confirm the team's final scores.
- Check that all linked documents and images remain accessible in the submission package.
