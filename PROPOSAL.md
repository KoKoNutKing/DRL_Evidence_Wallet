# PA#1 – Idea and Wireframe: Ví minh chứng ĐRL (ĐRL Evidence Wallet)

Course: Web Application Development (CSC13008) · Class: 24KTPM1

## 1. Team

| No. | Full name          | Student ID |
| --- | ------------------ | ---------- |
| 1   | Lê Nguyễn Quốc Học | 24127044   |
| 2   | Thái Quang Huy     | 24127177   |
| 3   | Trần Hoàng Phúc    | 24127505   |

## 2. The Problem

Every semester, HCMUS students take part in volunteer work, competitions, seminars, and club activities that may count toward their training points (Điểm rèn luyện, ĐRL). Some activities require evidence such as certificates or organizer confirmations, which students may keep in different places such as phone galleries, downloads, email, and chat. When the school publishes the preliminary ĐRL result and students have about two weeks to appeal missing items, they may discover too late that the evidence is missing, that the activity falls outside the counted period, or that they cannot tell which ĐRL item it belongs to. The problem is keeping each activity and its evidence organized under the correct ĐRL item, and knowing early whether the record has everything it needs.

## 3. Users

| User          | What they are trying to get done                                                                                                                                                                                                               |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| HCMUS student | Record each activity with its evidence under the correct ĐRL item, check early whether the record is complete according to the app's checklist, and have the evidence ready when the preliminary result comes out and the appeal window opens. |

## 4. Main flow

Main job: turn an activity the student has just taken part in into a saved record, under the right ĐRL item, with evidence checked for completeness according to the app's predefined checklist.

1. The student signs in and opens the current semester; its activity period and appeal window are already stored. *(not drawn)*
2. On "Danh sách minh chứng học kỳ" (Semester evidence checklist), the student finds the ĐRL item the activity belongs to and taps "Thêm minh chứng" (Add evidence). *(Screen 1)*
3. On "Thêm minh chứng" (Add evidence), the student enters the activity details and any field the item needs (for example the hours taken part, for item 4.3), attaches the certificate or confirmation file, and taps "Lưu và kiểm tra" (Save and check). *(Screen 2)*
4. On "Kiểm tra minh chứng" (Evidence check), the app checks the record against the item's rules and shows "Đủ minh chứng" (Enough evidence) or "Cần chỉnh sửa" (Needs changes), with exactly what is missing. The student either fixes it with "Sửa lại" (Edit) or keeps it with "Hoàn tất" (Done) and returns to the checklist, where the item's status is updated. *(Screen 3)*
5. When the school publishes the preliminary ĐRL result, the student marks each saved activity as counted or missing, and uses the list of missing activities, each with its evidence, to file appeals through the school's own appeal process before the appeal window closes. *(last priority, not drawn; the appeal itself is filed outside the app)*

## 5. Scope

### Building

- Student registration and login with email and password.
- One predefined semester (activity period and appeal window) and the ĐRL groups and items of the current HCMUS regulation, seeded in the database; no admin page for managing them.
- Create, view, edit, and delete activity records: activity name, date, organizer, location (on-campus or off-campus), ĐRL item, item-specific fields such as hours for item 4.3, and an optional note.
- One or more evidence files (image or PDF) per activity, each with an evidence type chosen by the student (certificate, participation confirmation, or photo); only the owner can open them.
- A small set of fixed rules checked for each record: required fields are filled, the date is within the activity period, at least one evidence file exists, an off-campus activity has an attached file labelled by the student as a certificate or participation confirmation, and item-specific fields are filled.
- Each record is shown as **"Đủ minh chứng" (Enough evidence)** or **"Cần chỉnh sửa" (Needs changes)**, with the missing requirements listed. On the checklist, each item shows "Đủ minh chứng", "Cần bổ sung" (Needs more evidence) or "Chưa có minh chứng" (No evidence yet); items recorded by the school are labelled "Trường tự ghi nhận".
- A responsive, mobile-first interface.

The summary counts saved activities, not ĐRL items. For supported items, show "Chưa có minh chứng" when no activity is saved, "Cần bổ sung" when any saved activity fails a checklist check, and "Đủ minh chứng" when at least one activity is saved and all saved activities pass. These statuses describe checklist completeness, not university acceptance.

Last priority, only if time allows: after the preliminary result, the student marks each activity as counted or missing and sees the list of missing activities to appeal, with their evidence.

### Not building

- No ĐRL score calculation or prediction.
- No automatic appeal submission and no integration with Shub, hcmus.drl.vn, or other HCMUS systems.
- No HCMUS SSO.
- No AI/OCR for reading certificates or evidence files.
- No certificate authenticity verification.
- No administrator interface for editing ĐRL items and no automatic scraping or updating of ĐRL regulations.
- No storage of personal-circumstance data (items 5.7–5.11, such as orphan or low-income household status).
- No native mobile app.
- No email, SMS, or push notifications.

## 6. Screens

The three screens below follow one another in the main flow. They are a mockup (colours and sample content) rather than a grey-box wireframe; only the flow is meant to be assessed. They are shown as full pages at mobile width (390 px): it is a responsive web app opened in the phone's browser, and on a phone the user scrolls down to see the rest of the page. Screen names and button labels are kept in Vietnamese, exactly as they appear in the drawings, with an English translation in brackets.

The whole flow, with arrows from each button to the screen it opens:

![Main flow](wireframes/flow.png)

### Screen 1 – "Danh sách minh chứng học kỳ" (Semester evidence checklist)

![Screen 1](wireframes/screen-1.png)

The student has signed in and wants to see which saved activities already have enough evidence, then pick the ĐRL item a new activity belongs to. The top shows the activity period, the appeal window and a summary: 5 saved activities, 4 with enough evidence and 1 needing more. Tapping a collapsed group card (1, 2, 3, 5 or 6) expands it to show its items. Items marked "Trường tự ghi nhận" (recorded by the school) have no button. Every other item has "Thêm minh chứng" (Add evidence), which opens Screen 2 for that item, for example 4.2 "Hiến máu tình nguyện". In the drawing the student taps it on item 4.3 "Hoạt động tình nguyện vì cộng đồng", which has no evidence yet.

### Screen 2 – "Thêm minh chứng" (Add evidence)

![Screen 2](wireframes/screen-2.png)

The student has chosen item 4.3 and now records the activity and its proof. The card at the top repeats the item's rule: volunteering is scored by hours taken part, and an off-campus activity needs a certificate or participation confirmation. The student enters the activity name, date, organizer and hours, chooses "Ngoài trường" (off-campus) and "Giấy chứng nhận" (certificate), may add a note, and taps the upload area, which opens the device's file picker (PDF, JPG or PNG). "Hủy" (Cancel) returns to Screen 1 without saving anything. "Lưu và kiểm tra" (Save and check) saves the activity and opens Screen 3.

### Screen 3 – "Kiểm tra minh chứng" (Evidence check)

![Screen 3](wireframes/screen-3.png)

The student has just saved the activity and wants to know whether the record is complete. The banner shows "Cần chỉnh sửa" (Needs changes) because the date 28/02/2026 is outside the activity period 02/03 – 13/09/2026; the other checks pass (details filled, 6 hours, file attached, certificate for an off-campus activity). "Sửa lại" (Edit) returns to Screen 2 with all fields still filled, so the student can correct the date. "Hoàn tất" (Done) keeps the record and returns to Screen 1, where item 4.3 shows "Cần bổ sung" (Needs more evidence) and the summary is 6 saved, 4 with enough evidence, 2 needing more. If every check passes, the banner and the item show "Đủ minh chứng" (Enough evidence).

**Notes.** The checks use the evidence type the student selected, not the contents of the file. The activity period and appeal window are stored reference data for the semester, not live-synced with HCMUS. Results are for reference only; the official ĐRL result comes from the school.
