# Giai đoạn 1: Dựng trang Web Docs cơ bản

- Khởi tạo dự án Next.js (Pages Router) + Nextra mới.
- Tích hợp **Tailwind CSS** và **Lucide Icons** để thiết kế giao diện: Thêm logo, tùy chỉnh màu sắc chủ đạo chuẩn bộ nhận diện của FireAnt. (Chưa dùng Framer Motion ở giai đoạn này để tối ưu tốc độ).
- Cài đặt và cấu hình **TinaCMS** (Sử dụng gói Free cho 2 Users). Liên kết TinaCMS với repo GitHub `fireant-help-db`.
- Thiết lập quy trình xuất bản nội dung: Content team viết bài qua trang `/admin` (TinaCMS) → TinaCMS tự động sinh Markdown và commit lên Git → Hệ thống (Nextra) tự động đọc file Markdown để hiển thị lên website với đầy đủ Menu Sidebar.
