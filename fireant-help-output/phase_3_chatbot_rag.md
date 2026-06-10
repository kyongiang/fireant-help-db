# Giai đoạn 3: Tích hợp Giao diện Chatbot & RAG API

- Thiết kế một UI Chatbot (Nút Chat ở góc màn hình mở ra khung chat).
- Viết API `/api/chat` xử lý quy trình RAG:
  1. Nhận câu hỏi từ User.
  2. Tạo embedding cho câu hỏi đó.
  3. Tìm kiếm (Similarity Search) lấy ra 5 đoạn văn bản liên quan nhất từ Vector DB.
  4. Nạp 5 đoạn này vào Prompt cho LLM để LLM có dữ liệu trả lời chính xác.
  5. Trả luồng dữ liệu (Stream) từng chữ về UI Chatbot.
