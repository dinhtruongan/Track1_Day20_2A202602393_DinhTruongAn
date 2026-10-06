# Track 1 · Day 20 — Product Metrics Lab

- **Họ tên:** Đinh Trường An
- **MHV:** 2A202602393
- **Dự án đã được học viên chọn:** AI-07 Explainable Course Recommender
- **Bối cảnh dự án:** Bài tập lớn ở trường, độc lập với Vin và khóa học trên VLearn.
- **Tiến độ:** Đang phát triển tại [SE2026-AI/ai-07-explainable-course-recommender](https://github.com/SE2026-AI/ai-07-explainable-course-recommender).
- **Metrics Pack:** [Bản trình bày đầy đủ 00–06](./metrics-pack.html)
- **AI Support Log:** [Nhật ký hỗ trợ](./ai-support-log.md)
- **Trạng thái:** Bản đề xuất chi tiết do AI soạn để học viên rà soát. Chưa phải bài hoàn tất đã được học viên chốt và chưa nộp.

## Phạm vi của bản đề xuất

Metrics Pack này là bài lab VLearn áp dụng framework product metrics lên bài tập lớn ở trường đang được thực hiện. Nguồn gốc dự án và nơi giao bài lab là hai bối cảnh riêng biệt; các tính năng/metric đề xuất phục vụ định hướng phát triển AI-07, chưa phải kết quả vận hành thực tế.

Use case: sinh viên lập kế hoạch môn học cho học kỳ sắp tới bằng gợi ý có giải thích.

Core action đề xuất: sinh viên xác nhận và lưu một kế hoạch học kỳ chứa ít nhất một môn được gợi ý sau khi xem giải thích, đạt các ràng buộc kiểm tra được và được sinh viên xác nhận phù hợp.

Nhịp đề xuất: theo chu kỳ đăng ký thực tế. Retention chính là sinh viên có qualified plan ở chu kỳ kế tiếp khi họ vẫn còn nhu cầu/đủ điều kiện chọn môn.

Mô tả repo xác nhận định hướng API-first recommendations với explanations cho Web/Mobile đối tác; việc lưu plan, kiểm tra chất lượng và events là yêu cầu thiết kế đề xuất, chưa được xác nhận đã triển khai.

## Nội dung Metrics Pack

| Mục | Nội dung |
|---|---|
| 00 | Dự án, persona, core job, use case và các giả định cần xác minh |
| 01 | Phân biệt job/action/value/event, Core Action Card, đánh giá năm tiêu chí |
| 02 | Action Nature Card và câu mẫu cadence có lý do |
| 03 | Activation có công thức/mẫu số/window; hai góc engagement; NSM; ba leading indicators; counter-metrics |
| 04 | Retention đủ sáu thành phần, công thức, eligibility và cohort maturity |
| 05 | Loop hai chu kỳ, hypothesis đề xuất, phép kiểm chứng và điều kiện bác bỏ |
| 06 | Tám events map metric, identity/properties, năm acceptance criteria, tự rà bảy lỗi |

## Nội dung có thể áp dụng cho dự án thật — AI đề xuất

Ứng dụng đối tác cần quan sát quyết định của sinh viên sau khi nhận gợi ý: xem giải thích, chọn môn và xác nhận kế hoạch. Số request API hoặc số kết quả AI tạo ra tự nó chưa đo được giá trị hỗ trợ quyết định.

Cần nối student identity, recommendation, plan, term và cycle; định nghĩa quality threshold trước khi tính North Star và retention. Chu kỳ đăng ký quyết định window, thay vì mặc định dùng DAU hoặc D7.

Các ý trên là gợi ý để học viên tự phản ánh, chưa được ghi như trải nghiệm hay kết luận cá nhân của người nộp.

## Hoàn thiện trước khi nộp

Học viên cần tự xác nhận/sửa core action, cadence, metric hypothesis và viết rationale/reflection bằng nhận định của mình. Rà lại khả năng thực tế của sản phẩm, dữ liệu lịch đăng ký và tracking ở đối tác. AI Support Log phải giữ đúng mức hỗ trợ thực tế.

Link ở đầu README hiện trỏ tới tệp trong thư mục. Khi có bản công khai hoặc tệp đã cấp quyền xem, cập nhật link Metrics Pack sang địa chỉ có thể xem trực tiếp. Repository GitHub: [Track1_Day20_2A202602393_DinhTruongAn](https://github.com/dinhtruongan/Track1_Day20_2A202602393_DinhTruongAn). Metrics Pack hiện là tệp HTML trong repo; chưa có trang trình bày được host hoặc hành động nộp VLearn.

## Nguồn

- [Brief Day 20 trên VLearn](https://vlearn.dev/course/k04-l34-p2-t1/reader?day=D08&part=lab-961eda13-s02-doc)
- [AI-07 repository](https://github.com/SE2026-AI/ai-07-explainable-course-recommender)



