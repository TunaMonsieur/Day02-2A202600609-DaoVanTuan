Case ví dụ: Thực tập/ New hire khi onboard cần hỏi thông tin và set up cho môi trường làm việc mới từ mentor
# 01 - Individual Problem Scan

Use this template to list 5+ problems from your experience and prepare top 3 Problem Cards.

## Instructions
- Scan at least 5 problems using the four lenses (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác).
- For each problem, note actor and evidence (how often, time lost, number of people affected).
- Select top 3 and fill Problem Card template below for each.

## Problem Bank (fill at least 5)
| # | Lăng kính | Problem quan sát được | Ai đang đau? | Dấu hiệu thật |
|---|---|---|---|---|
| 1 |  Lặp lại | Onboarding docs rời rạc, thiếu bước cụ thể (dev setup, access) | Intern / new hire | Mất nhiều thời gian setup: 4–16 giờ tuần đầu, hỏi mentor nhiều lần |
| 2 | Pain từ người khác | Không rõ owner cho task cụ thể (ai chịu trách nhiệm) | New hire / PM | Nhiều lần bị chuyển tiếp, chậm xử lý task, email/Slack ping lặp lại |
| 3 | Tốn thời gian | Viết update hàng tuần (status update) không biết lấy info từ đâu | Junior PM / Intern | Mất 30–90 phút mỗi tuần, thiếu consistency giữa tuần, nhiều follow-up |
| 4 | AI có thể tốt hơn | Hiểu task từ nhiều Slack/thread/tài liệu gây thiếu bối cảnh | Developer / Designer | Mất 15–60 phút để tìm/ghép context, dễ làm sai yêu cầu |
| 5 | Tốn thời gian | Quyền truy cập (repo, tools, cloud) bị delay do approval/permission | New hire | Delay 1–3 ngày chờ access, block công việc ban đầu |

## Top 3 — Problem Cards

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Onboarding documentation rời rạc và thiếu hướng dẫn cụ thể cho dev/engineer khiến new hire tốn nhiều thời gian cho setup và hỏi mentor lặp lại. | Workflow rõ, tốn nhiều thời gian, ảnh hưởng TFMC | Có nên cho AI đọc internal docs/org chart? Privacy limits? |
| 2 | Khi nhận task, người thực hiện phải tìm context từ nhiều Slack/thread và tài liệu, mất thời gian ghép bối cảnh và dễ làm sai yêu cầu. | Thông tin phân tán, gây rework và delay | Chất lượng tóm tắt AI đo thế nào? Ai verify? |
| 3 | Khi cần biết ai chịu trách nhiệm một tác vụ hay tài nguyên, team thường bị chuyển tiếp nhiều lần, delay assign và execution. | Nhiều người bị ảnh hưởng, gây chuyển tiếp và delay | Data access & owner registry governance? |

Repeat the card template three times and fill for each chosen problem.

### Problem Card #1 — Onboarding docs & setup
Problem 1 câu:
Onboarding documentation rời rạc và thiếu hướng dẫn cụ thể cho dev/engineer khiến new hire tốn nhiều thời gian cho setup và hỏi mentor lặp lại.

Actor:
Intern / New hire và mentor.

Thời điểm / bối cảnh:
Ngày đầu / tuần đầu làm việc, khi cần thiết lập môi trường dev và truy cập công cụ.

Current workflow 5 bước:
1. Nhận link onboarding (Google Doc, repo README)
2. Thử theo hướng dẫn, gặp lỗi setup
3. Search Slack/intranet cho giải pháp
4. Ping mentor/owner và chờ trả lời
5. Mentor hướng dẫn thủ công hoặc cập nhật doc

Bottleneck:
Docs thiếu bước cụ thể và outdated; thiếu checklist quyền truy cập; mentor phải giải thích lặp.

Impact:
Mất 4–16 giờ trong tuần đầu cho new hire; mentor tốn thời gian trả lời; chậm TFMC (time-to-first-meaningful-contribution).

Success metric:
Giảm TFMC 50% (ví dụ từ 16h → 8h); giảm số lần hỏi lặp lại trong 2 tuần đầu ≥ 50%.

Non-AI alternative:
Chuẩn hóa onboarding hub + checklist, assign buddy, pre-provision access theo role.

AI hypothesis:
AI Q&A internal (được cấp quyền đọc docs và org chart) có thể trả lời nhanh câu hỏi onboarding, gợi link tới step chính xác và owner; giảm thời gian tìm hiểu ban đầu.

Quick gut:
- [ ] No AI / process fix
- [x] Rule
- [x] Workflow
- [x] Agent
- [ ] Chưa biết

Draft current workflow (ASCII):
[Access docs: 0.5-2h] → [Attempt setup: 1-4h] → [Search Slack: 0.5-2h] → [Ask mentor: wait 0.5-8h] → [Complete setup]

Draft future workflow (ASCII):
[Onboarding hub + pre-provision (rule): 0.5h] → [AI-assisted Q&A + link to step: 0.5-5'] → [User verify with buddy: 10-30'] → [Done]

Fallback:
Nếu AI trả sai owner/step → user verify with buddy/mentor; AI only suggests links, not final authority.

Question I want the group to challenge me on:
Should we allow AI read access to internal docs/org chart? What privacy limits are needed?

### Problem Card #2 — Hiểu task từ nhiều Slack/thread/tài liệu
Problem 1 câu:
Khi nhận task, người thực hiện phải tìm context từ nhiều Slack/thread và tài liệu, mất thời gian ghép bối cảnh và dễ làm sai yêu cầu.

Actor:
Intern/ New hire.

Thời điểm / bối cảnh:
Khi bắt đầu task hoặc xử lý ticket yêu cầu xác nhận scope/requirements.

Current workflow 4 bước:
1. Đọc task/ticket brief
2. Search liên quan trên Slack, Google Docs, Confluence
3. Mở nhiều thread và đọc để ghép context
4. Nếu không rõ, hỏi product owner hoặc requester

Bottleneck:
Thông tin phân tán, search không precise, thread dài.

Impact:
Mất 15–60 phút để lấy đủ context; nếu sai hiểu yêu cầu → rework và delay.

Success metric:
Giảm thời gian chuẩn bị context xuống <10 phút; giảm rework do hiểu sai ≥ 30%.

Non-AI alternative:
Better triage template, require requester fill required context fields, maintain decision log.

AI hypothesis:
AI assistant có thể tổng hợp các nguồn liên quan thành summary ngắn kèm trích dẫn link, giúp người thực hiện nhanh nắm context.

Quick gut:
- [ ] No AI
- [x] Rule
- [x] Workflow
- [x] Agent
- [ ] Chưa biết

Draft current workflow (ASCII):
[Read brief: 2'] → [Search Slack/docs: 10-40'] → [Read threads/docs: 5-20'] → [Ask clarifying question: 10-240'+ wait]

Draft future workflow (ASCII):
[AI gather + summary + links: 1-5'] → [User skim & confirm: 2-10'] → [Ask specific clarifying question if needed]

Fallback:
If AI hallucinate → user checks source links and flags issue; keep human-in-loop for approval.

Question I want the group to challenge me on:
How to measure quality of AI summaries? Who verifies them in team? 

### Problem Card #3 — Không rõ owner / tìm người phụ trách đúng việc
Problem 1 câu:
Khi cần biết ai chịu trách nhiệm một tác vụ hay tài nguyên, team thường bị chuyển tiếp nhiều lần, delay assign và execution.

Actor:
New hire / PM / Requester.

Thời điểm / bối cảnh:
Khi cần approval, access, hoặc assigned owner cho task mới.

Current workflow 4 bước:
1. Search org chart / team pages
2. Ping channel hoặc từng người
3. Người nhận chuyển tiếp nếu không phải owner
4. Khi có owner, task bắt đầu

Bottleneck:
Org chart không cập nhật; không có responsibility registry; communication vòng.

Impact:
Delay 0.5–48 giờ; accountability mơ hồ; tasks bị trễ.

Success metric:
Giảm thời gian tìm owner xuống <2 giờ; giảm số lần chuyển tiếp xuống <1 lần trung bình.

Non-AI alternative:
Maintain up-to-date owner registry, include owner field khi tạo ticket.

AI hypothesis:
AI internal search (read-only) có thể trả về candidate owners with confidence score and link to org chart/profile; requester still verifies.

Quick gut:
- [ ] No AI
- [x] Rule
- [x] Workflow
- [x] Agent
- [ ] Chưa biết

Draft current workflow (ASCII):
[Search org chart: 5-20'] → [Ping person/channel: wait 0.5-24h] → [Follow-up: wait] → [Assign]

Draft future workflow (ASCII):
[Owner registry + AI candidate suggestions: 1-5'] → [Requester choose/confirm: 5-30'] → [Assign]

Fallback:
If AI suggests wrong owner → manual verification via org chart or PM.



---
Guidance: see example in `02-deliverable-example.md` for a completed model.