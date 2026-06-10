# Mục tiêu

Xây dựng một trang Web Hệ thống Tài liệu (Help Center) mới, hiện đại và tích hợp sẵn một Chatbot AI sử dụng công nghệ RAG (Retrieval-Augmented Generation). Chatbot sẽ dùng nguồn kiến thức chính xác từ repository GitHub chứa dữ liệu Markdown bạn vừa tạo để trả lời câu hỏi của người dùng.

## Cấu trúc Hệ thống Đề xuất (Tech Stack)

Để hệ thống hoạt động mượt mà, dễ quản lý nội dung và dễ dàng triển khai, tôi đề xuất sử dụng bộ công nghệ sau:

1. **Frontend & Docs Framework**: 
   - **Next.js (Pages Router)** kết hợp **Nextra**: Cung cấp cấu trúc website tài liệu tối ưu nhất hiện nay. Tương thích 100% với file `_meta.json` và hỗ trợ SSG để load trang cực nhanh.
   - **Tailwind CSS & Lucide Icons**: Tailwind giúp tùy biến giao diện nhanh gọn (đổi màu sắc chuẩn FireAnt), còn Lucide Icons cung cấp bộ icon hiện đại, nhẹ nhàng thay thế cho các thư viện cũ.
   - **Lưu ý**: Tạm thời chưa dùng Framer Motion ở Phase 1 để tập trung tối ưu tốc độ tải trang, chỉ sử dụng CSS transitions cơ bản.
2. **Hệ thống quản lý nội dung (CMS) cho Non-Tech User**:
   - **TinaCMS (Gói Cloud Free - tối đa 2 users)**: Cung cấp giao diện soạn thảo trực quan (Visual Editing) cho team nội dung. Người viết chỉ cần thao tác trên web (`/admin`), TinaCMS sẽ tự động sinh file Markdown và push lên repo GitHub `fireant-help-db`. Khắc phục triệt để rào cản kỹ thuật về Git/Markdown cho người viết.
2. **AI & RAG Pipeline**:
   - **Vercel AI SDK**: Thư viện giúp tạo giao diện Chatbot trả lời theo thời gian thực (Streaming) cực mượt.
   - **LLM & Embedding**: OpenAI (GPT-4o-mini hoặc GPT-4o) + `text-embedding-3-small`. Hoặc có thể dùng Google Gemini.
3. **Vector Database**:
   - **Pinecone** hoặc **Supabase (pgvector)**: Nơi lưu trữ phiên bản số hoá (Vector) của toàn bộ bài viết, tốc độ tìm kiếm siêu nhanh và có gói Miễn phí tốt.

---

## Lộ trình Triển khai (3 Giai đoạn)

### Giai đoạn 1: Dựng trang Web Docs cơ bản
- Khởi tạo dự án Next.js (Pages Router) + Nextra mới.
- Tích hợp **Tailwind CSS** và **Lucide Icons** để thiết kế giao diện: Thêm logo, tùy chỉnh màu sắc chủ đạo chuẩn bộ nhận diện của FireAnt.
- Cài đặt và cấu hình **TinaCMS**. Liên kết TinaCMS với repo GitHub `fireant-help-db` của bạn.
- Thiết lập quy trình xuất bản nội dung: Content team viết bài qua trang `/admin` (TinaCMS) → TinaCMS tự động commit lên Git → Hệ thống (Nextra) tự động nhận diện file Markdown để hiển thị lên website với đầy đủ cấu trúc Sidebar.

### Giai đoạn 2: Số hoá dữ liệu (Vectorization)
- Mở tài khoản Pinecone hoặc Supabase.
- Viết một script bằng TypeScript/Python để: Quét toàn bộ thư mục `fireant-help-output` → Bóc tách nội dung Text từ Markdown → Chia nhỏ các đoạn văn (Chunking) → Tạo Embeddings → Đẩy vào Vector DB kèm siêu dữ liệu (đường dẫn gốc làm nguồn trích dẫn).

### Giai đoạn 3: Tích hợp Giao diện Chatbot & RAG API
- Thiết kế một UI Chatbot (Nút Chat ở góc màn hình mở ra khung chat).
- Viết API `/api/chat` xử lý quy trình RAG:
  1. Nhận câu hỏi từ User.
  2. Tạo embedding cho câu hỏi đó.
  3. Tìm kiếm (Similarity Search) lấy ra 5 đoạn văn bản liên quan nhất từ Vector DB.
  4. Nạp 5 đoạn này vào Prompt cho LLM để LLM có dữ liệu trả lời chính xác.
  5. Trả luồng dữ liệu (Stream) từng chữ về UI Chatbot.

---

## Mời bạn duyệt kế hoạch
Trước khi tôi bắt đầu gõ code, tôi cần bạn chốt một số lựa chọn sau:

1. **LLM Provider**: Bạn muốn dùng **OpenAI** hay **Google Gemini** để cung cấp sức mạnh cho Chatbot?
2. **Vector DB**: Bạn đã dùng dịch vụ Vector Database nào chưa, hay tôi sẽ hướng dẫn bạn tạo tài khoản **Pinecone** (miễn phí và dễ dùng nhất)?
3. **Nơi lưu code mới**: Chúng ta nên tạo một thư mục hoàn toàn mới trên máy của bạn (vd: `C:\Users\ADMIN\Documents\Github\fireant-help-web`) để chứa code Website này nhé? Tránh để lẫn lộn với code cào dữ liệu cũ.
