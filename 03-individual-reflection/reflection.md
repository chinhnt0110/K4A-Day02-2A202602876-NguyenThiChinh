# 03 — Individual Reflection

> Viết bằng lời của bạn (Phase 7 trong `01-worksheet.md`). Có thể dùng AI gợi ý câu hỏi tự soi, không dùng AI viết thay. 8-12 câu, có chuyện cụ thể.

## Thông tin cá nhân

- Họ và tên: Nguyễn Thị Chinh
- Mã học viên: 2A202602876
- Nhóm: Bttention
- Candidate problem nhóm chọn: Hệ thống xử lý tự động phản ánh của cư dân Vinhomes

---

## 1. Tôi đã tham gia vào phần nào?

Ghi việc cụ thể + kết quả cụ thể. Không ghi chung chung kiểu "tham gia thảo luận".

| Hoạt động | Tôi đã làm gì? (việc cụ thể) | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| Scan cá nhân | Brainstorm các vấn đề liên quan đến quy trình kiểm tra vận doanh hàng ngày của Green SM: điền form kiểm tra an toàn vận doanh, góc chụp ảnh xe, đối chiếu defect, xe cạn pin, kiểm tra vệ sinh nội thất xe | Đóng góp 5 bài toán có số liệu và trích dẫn nghiên cứu thật vào pool ý tưởng chung của nhóm |
| Pitch Problem Card | Pitch Card #3 (Tài xế giao xe cạn pin ảnh hưởng ca sau) với số liệu mất 80k–120k/ca và 12–16% xe cạn pin | Giúp nhóm hiểu sâu về điểm nghẽn năng lượng trong logistics xe điện fleet |
| Challenge bài của bạn khác | Phản biện bài của các thành viên: chỉ ra thiếu impact đo được, logic giữa các bước trong thực tế, thiếu tính khả thi, thiếu số và bằng chứng, vấn đề dữ liệu bảo mật và khó triển khai thu thập | Thuyết phục nhóm loại bỏ các bài toán rủi ro cao, chưa đủ chặt chẽ (cuộc gọi lừa đảo, bệnh gia súc) |
| Gom trùng / cluster | Đề xuất phân loại 15 ý tưởng của nhóm thành 4 cụm: Vinhomes, Fleet Ops, Video Stream/CV, Giám sát chuyên ngành | Giúp nhóm có cấu trúc phân loại khoa học, tránh tranh luận lan man |
| Chọn candidate problem | Cùng nhóm bỏ phiếu thống nhất chọn đề tài "Xử lý phản ánh cư dân Vinhomes" dựa trên tính cấp thiết và khả năng pilot trên 1 tòa nhà | Đạt được sự đồng thuận 100% trong nhóm để bước vào vòng Deep-Dive |
| Validation / research | Research xem đã có giải pháp nào giải quyết vấn đề Vinhomes chưa, các giải pháp đó có ưu nhược điểm gì, xem có research gap không | Làm rõ khoảng trống công nghệ của các chatbot hiện tại khi xử lý các khiếu nại phức tạp của cư dân |
| Workflow nhóm | Đóng góp xây dựng luồng Before (6 bước thủ công) và luồng Future (phân loại 3 cấp độ P1/P2/P3, draft phản hồi và dispatch kỹ thuật) | Làm rõ điểm nghẽn lớn nhất nằm ở bước BQL đọc và nhập liệu ticket thủ công |
| Problem Statement | Viết và hoàn thiện Problem Statement v0 và v1, đặc biệt là thiết lập ranh giới vận hành (Operational Boundary) | Xác lập giới hạn an toàn: AI chỉ soạn nháp, cấm tự ý hứa bồi thường tiền hay tự đóng ticket P1 |
| Rule / Workflow / Agent | Phân tích bảng so sánh 4 cấp độ kỹ thuật, cùng nhóm chọn giải pháp Workflow + LLM Feature cho giai đoạn MVP thay vì Agent tự trị toàn phần | Giữ cho dự án thực tế, kiểm soát rủi ro chi phí API và ảo giác (hallucination) |
| Decision | Cùng nhóm ra quyết định GO có điều kiện: Thử nghiệm pilot giới hạn tại 1 tòa chung cư (S2.05 Smart City) với kịch bản rollback chi tiết | Giúp dự án có lộ trình triển khai an toàn, bảo vệ SLA của Vinhomes |

**Dấu tay rõ nhất của tôi trong artifact cuối (1-2 câu):**

```text
Dấu tay rõ nhất của tôi là phản biện các candidate problems (Mục 3.4 trong group report) và đóng góp phân tích ranh giới an toàn Operational Boundary cho hệ thống phản ánh Vinhomes.
```

---

## 2. Bảng dùng AI (mỗi dòng 1 phase có dùng AI — 2 cột cuối bắt buộc)

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Gợi ý các vấn đề và pain points | Gợi ý nhanh nhiều góc nhìn đa dạng (an toàn xe, kiểm tra ảnh ngoại quan, sạc pin, vệ sinh nội thất) | Đưa ra các mô tả chung chung ("mất nhiều thời gian"), gợi ý dùng camera nhận diện mùi/bụi nội thất thiếu tính khả thi kỹ thuật | Tự tra cứu paper của GAO, nghiên cứu của AFS Group và thông số pin VinFast để đưa số liệu, bằng chứng định lượng thật vào bảng |
| Problem Card | Hỗ trợ dựng khung Before/After workflow và gợi ý công thức tính metric | Giúp cấu trúc nhanh các bước tuần tự 1-2-3-4 theo logic thời gian | AI có xu hướng "tự động hóa 100%", bỏ quên vai trò kiểm tra của con người (HITL) và không có nhánh dự phòng khi AI đoán sai | Bổ sung bước KTV duyệt xác nhận và thiết kế nhánh Fallback rõ ràng (nếu AI tự tin < 80% thì chuyển sang tra cứu thủ công) |
| Workflow | Hỗ trợ dựng khung workflow hiện tại và tương lai, tạo sinh ra mã mermaid | Tự động sinh cú pháp Mermaid trực quan, phân nhánh luồng P1/P2/P3 nhanh chóng | Cho AI tự động dispatch kỹ thuật và tự gửi tin nhắn cho cư dân mà không qua kiểm duyệt của Ban Quản Lý (BQL) | Đặt chốt chặn Lễ tân BQL bắt buộc phải xem và bấm "Duyệt" nội dung phản hồi trước khi gửi tới cư dân |
| Research | Tìm kiếm và trả về các bài báo, giải pháp, và thông tin liên quan đến vấn đề | Tóm tắt nhanh ưu/nhược điểm của các hệ thống quản lý chung cư (BMS) truyền thống | Lan man về vấn đề quản lý bất động sản chung, không phải là xử lý phản ánh của cư dân; tự bịa quotes lý thuyết | Thu hẹp phạm vi vào xử lý phản ánh dịch vụ; thay thế bằng số liệu khảo sát thật từ 8 cư dân Vinhomes và phỏng vấn lễ tân |
| Problem Statement | Soạn thảo nháp các câu văn theo khung chuẩn 6 trường thông tin (v0/v1) | Giúp câu văn gãy gọn, đúng cấu trúc kỹ thuật sản phẩm (Product Framing) | Đặt Success Metric quá viển vông ("giải quyết 100% khiếu nại trong 5s") và không đưa ra ranh giới những việc AI bị cấm làm | Hạ metric xuống thực tế (85% phân loại dưới 15s; giảm thời gian phản hồi từ 45' xuống 5') và siết chặt Boundary (cấm AI tự hứa bồi thường tiền) |
| Rule / Workflow / Agent | Lập bảng so sánh đánh giá ưu nhược điểm giữa Rule, Workflow + LLM, và Agent | Liệt kê đầy đủ các tiêu chí so sánh: chi phí token, độ phức tạp thuật toán, độ trễ (latency) | AI bị thiên vị "solution-first", khuyên nhóm nên làm Full Agentic Loop cho hiện đại dù bài toán chỉ cần Workflow | Kiên quyết cùng nhóm chọn Workflow + LLM Feature để tránh bẫy ảo giác, tiết kiệm chi phí và dễ kiểm soát rủi ro vận hành |
| Decision | Không dùng | Nhóm tự thảo luận vì đây là quyết định trách nhiệm của con người dựa trên năng lực và tính an toàn của dự án | Không áp dụng | Nhóm tự phân tích và thống nhất quyết định |

> Nếu phase nào không dùng AI, ghi `Không dùng` và vì sao tự làm.

---

## 3. Reflection câu hỏi mở

Chọn 3-4 câu trong 6 câu dưới để viết thành đoạn 8-12 câu (không trả lời bullet 1 dòng):
- Tôi học được gì khi nghe top 3 problems của các bạn khác?
- Nhóm có lúc nào bị solution-first, đòi làm Agent cho ngầu không?
- Tôi có thay đổi ý kiến sau khi bị challenge không, vì sao đổi?
- Tôi đóng góp gì thật sự vào artifact cuối, phần nào có dấu tay của tôi?
- Điều khó nhất khi viết Problem Statement là gì, metric hay boundary?
- Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn ở điểm nào?

**Reflection:**

```text
Hầu hết các bạn đều chọn những đề tài mà mình quen thuộc, xuất phát trực tiếp từ pain point của bản thân hoặc gia đình chứ không phải những đề tài fancy hay không nắm rõ workflow hiện tại, không bị mất thời gian vào việc đoán workflow. Nếu làm lại, tôi sẽ challenge nhóm quyết liệt hơn về tính khả thi có làm được trong lab không vì hầu hết các bài đều không có khả năng thu thập dữ liệu. Điều khó nhất khi viết Problem Statement là phần metric vì không những model metric mà còn phải cover cả business metric sao cho đo lường được hiệu quả thực tế của doanh nghiệp. Bên cạnh metric, việc thiết lập Operational Boundary cũng đòi hỏi nhóm phải cân não rất nhiều để tránh việc AI tự hứa bồi thường tài chính gây rủi ro pháp lý. Nhóm tôi ban đầu cũng từng có xu hướng solution-first khi muốn xây dựng Agent tự trị hoàn toàn, nhưng sau khi phân tích kỹ lưỡng giữa Rule, Workflow và Agent, chúng tôi đã đồng thuận chọn kiến trúc Workflow có con người kiểm duyệt (Human-in-the-loop) để đảm bảo độ tin cậy cao nhất. Đóng góp rõ nét nhất của tôi là kiên trì phản biện loại bỏ các bài toán thiếu tính khả thi và giữ vững tính an toàn trong ranh giới vận hành của hệ thống phản ánh cư dân Vinhomes.
```

---

## 4. Tự kiểm cuối bài (check trước khi nộp repo)

- [x] [12đ] Cá nhân có 5+ problems + top 3 Problem Cards
- [x] [12đ] Tôi đã pitch rõ + challenge nhóm đúng trọng tâm (ghi ở bảng mục 1)
- [x] Nhóm có nhật ký hội tụ từ candidates về 1 bài
- [x] [15đ] Nhóm có workflow trước/sau
- [x] [20đ] Nhóm có PS v0/v1 với metric + boundary rõ
- [x] [15đ] Nhóm có so sánh No AI / Rule / Workflow / Agent
- [x] [10đ] Nhóm có Go / Not Yet / No-Go + lý do rõ
- [x] [10đ] Reflection này có vai trò thật + AI giúp/sai ở đâu + điều học được + nếu làm lại đổi gì
- [x] [6đ] Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp AI
