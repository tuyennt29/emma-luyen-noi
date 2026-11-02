# Emma Luyện Nói

Gia sư nói tiếng Anh chạy bằng giọng nói, dùng được khi lái xe.

Mỗi ngày Emma soạn một đoạn 6–8 câu ngắn về chính bạn (trình độ A2–B1). Buổi luyện có 4 bước, chạy hoàn toàn bằng giọng nói:

1. **Nghe**: Emma đọc mẫu cả đoạn.
2. **Nói theo**: nói theo từng câu sau tiếng bíp. Emma chấm điểm và chỉ ra những từ còn thiếu.
3. **Kể lại**: kể lại cả đoạn. Claude nhận xét tối đa 3 lỗi và đưa câu sửa mẫu.
4. **Hỏi đáp**: trả lời 3 câu hỏi, sau đó nói theo câu trả lời hay hơn.

**Tự chọn chủ đề:** bấm nút *Tự chọn chủ đề*, nói yêu cầu bằng tiếng Việt hoặc tiếng Anh (ví dụ "họp với khách hàng Nhật"). Emma soạn bài ngay và chạy đủ 4 bước như trên.

Khẩu lệnh: `repeat` · `next` · `slower` · `stop` (hoặc "lặp lại", "tiếp", "chậm", "dừng").

## Cách dùng
- Mở bằng Chrome (Android, máy tính) hoặc Safari (iPhone), rồi cho phép dùng micro.
- Vào **Cài đặt**, dán API key:
  - **Gemini (miễn phí):** lấy tại aistudio.google.com, mục *Get API key* (key bắt đầu bằng `AIza`).
  - **Claude:** lấy tại console.anthropic.com (key bắt đầu bằng `sk-ant-`).
  - App tự nhận loại key. Key chỉ lưu trên thiết bị của bạn.
- Thêm vào màn hình chính để mở như một ứng dụng.

## Công nghệ
Chỉ gồm một file HTML tĩnh, không cần máy chủ. Nhận giọng nói và đọc dùng Web Speech API. AI: Gemini Flash (tự chọn bản mới nhất) hoặc Claude (`claude-sonnet-5-5` soạn bài, `claude-haiku-5-5` chấm bài), gọi thẳng từ trình duyệt. Lịch sử luyện tập lưu trong localStorage.

## Triển khai
Dùng GitHub Pages: Settings → Pages → Deploy from branch → `main` / root.
