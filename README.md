# Track 1 · Day 20 — Product Metrics
**Đinh Trường An · MHV 2A202602393**

## Dự án chọn làm

**AI-07 — Explainable Course Recommender**, bài tập lớn ở trường đang phát triển tại [SE2026-AI/ai-07-explainable-course-recommender](https://github.com/SE2026-AI/ai-07-explainable-course-recommender).

Bài phân tích use case sinh viên chọn môn bằng gợi ý có giải thích và lưu kế hoạch học kỳ. Bối cảnh triển khai được đối chiếu với nhánh [truongan_22001535](https://github.com/SE2026-AI/ai-07-explainable-course-recommender/tree/b587eefb7c5aac86990058fdb981a53cd7931925), commit b587eef.

## Metrics Pack

**[Mở Metrics Pack trực tiếp](https://dinhtruongan.github.io/Track1_Day20_2A202602393_DinhTruongAn/metrics-pack.html)**

Tài liệu có các mục theo brief:

| Mục | Nội dung |
|---|---|
| 00 | Dự án, persona, core job, use case và hiện trạng |
| 01 | Core Action Card; phân biệt job/action/value/event; tự kiểm 5 tiêu chí |
| 02 | Action Nature Card và cadence theo chu kỳ đăng ký |
| 03 | Activation, 2 góc engagement, North Star, 3 leading indicators, counter-metrics |
| 04 | Retention đủ 6 thành phần, công thức và 3 mốc đối chiếu |
| 05 | Project loop 2 chu kỳ và metric hypothesis |
| 06 | 8 events, metric mapping, acceptance criteria và tự soi 7 lỗi |

[Tệp HTML nguồn](./metrics-pack.html) · [AI Support Log](./ai-support-log.md)

## Điều mang về áp dụng cho dự án thật

Giá trị của AI-07 cần được đo ở quyết định của sinh viên: họ chọn và lưu được một kế hoạch có cơ sở, không chỉ ở số lần hệ thống trả gợi ý. Vì nhu cầu chọn môn gắn với kỳ học, nhịp chính nên theo chu kỳ đăng ký; sửa plan nhiều lần trong một kỳ có thể phản ánh khó khăn thay vì engagement tốt.

Đối chiếu code cho thấy kế hoạch hiện được ghi vào localStorage. Vì vậy completion rule của core action phải dựa vào lưu thành công; không mô tả một server confirmation chưa tồn tại. Việc theo dõi retention xuyên kỳ cần stable identity, lịch chu kỳ và phục hồi kế hoạch đã lưu; session demo và dữ liệu giả lập chưa đáp ứng đo người dùng thật.

Các thay đổi có thể mang vào backlog:
- Instrument plan_saved/plan_save_failed sau kết quả ghi storage; khử trùng cùng revision.
- Lưu và khôi phục kế hoạch cùng profile/catalog version để vòng kỳ sau tái sử dụng bối cảnh.
- Phân biệt quality_status=qualified/unknown/invalid; dữ liệu workload thiếu không được tự xem là 0 giờ.
- Thống nhất identity, cycle_id và eligibility trước khi tính retention; tách demo/internal khỏi analytics thật.

Các nội dung trên là kết luận thiết kế được AI hỗ trợ tổng hợp từ brief và code, không phải kết quả phỏng vấn, số liệu vận hành hoặc thử nghiệm retention.

## Revision

Sửa bản đầu từ plan_confirmed trên máy chủ thành plan_saved tại trình duyệt; thay activation window 7 ngày mặc định bằng window của chu kỳ; làm rõ saved-state recovery chưa có trong PlanView. Các lý do và đối chiếu bảy lỗi nằm cuối Metrics Pack.

## Nguồn

- [VLearn · Track 1 Day 20](https://vlearn.dev/course/k04-l34-p2-t1/reader?day=D08&part=lab-961eda13-s12-doc)
- [PlanView tại commit đã đối chiếu](https://github.com/SE2026-AI/ai-07-explainable-course-recommender/blob/b587eefb7c5aac86990058fdb981a53cd7931925/src/web/src/components/PlanView.tsx)
- [Demo session](https://github.com/SE2026-AI/ai-07-explainable-course-recommender/blob/b587eefb7c5aac86990058fdb981a53cd7931925/src/web/src/lib/session.ts)

