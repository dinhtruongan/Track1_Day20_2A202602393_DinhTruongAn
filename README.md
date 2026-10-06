# Track 1 · Day 20 — Product Metrics

- **Họ tên:** Đinh Trường An
- **MHV:** 2A202602393
- **Dự án:** [AI-07 — Explainable Course Recommender](https://github.com/SE2026-AI/ai-07-explainable-course-recommender), bài tập lớn ở trường đang phát triển.
- **Metrics Pack:** [Xem bài trình bày](https://dinhtruongan.github.io/Track1_Day20_2A202602393_DinhTruongAn/metrics-pack.html)

## Cấu trúc nộp bài

```text
Track1_Day20_2A202602393_DinhTruongAn/
├── README.md
└── ai-support-log.md
```

## Điều mang về áp dụng cho dự án thật

Đo giá trị AI-07 qua việc sinh viên chọn và lưu kế hoạch môn học phù hợp, thay vì chỉ đếm số lần hệ thống trả gợi ý. Nhịp đo đi theo chu kỳ đăng ký; lưu lại nhiều lần trong cùng kỳ chưa chắc tạo thêm giá trị.

Kế hoạch hiện lưu trên trình duyệt, nên event thành công cần được ghi sau khi lưu thực sự hoàn tất và khử trùng cùng hành vi. Để đo retention xuyên kỳ, dự án cần identity ổn định, lịch chu kỳ và khả năng khôi phục kế hoạch. Các dữ liệu demo không được dùng như số liệu người dùng thật.
