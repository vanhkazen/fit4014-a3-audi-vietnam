# AI_LOG – Nhật ký sử dụng và đối chiếu AI (Phiên bản v3)

**Sinh viên thực hiện:** Trần Việt Anh – MSV: `2071020020` – Lớp: `CNTT 20-04`  
**Dự án:** Website Showroom Trực Tuyến Audi Việt Nam (`fit4014-a3-audi-vietnam`)  
**Công cụ AI tham khảo:** Gemini và GitHub Copilot (VS Code)

---

## 1. Bảng theo dõi quá trình sử dụng AI (Chuẩn Lab 8)

| Ngày           | Dùng AI làm gì                                                                                                                               | Em sửa lại gì                                                                                                                                                                                                                                                                                                                       |
| :------------- | :------------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **18/11/2026** | Rà soát lỗi Semantic HTML5 và bố cục CSS theo Rubric A3                                                                                      | Giữ gợi ý đưa trang về duy nhất 1 thẻ `<h1>` tại Hero (đổi thương hiệu trên header thành `<span>`) và viết lại CSS theo tư duy Mobile-First (`min-width: 640px`, `992px`). **Bác bỏ** gợi ý dùng `z-index` để giữ nhãn đè ảnh `.car-badge` — tự tay xóa bỏ hoàn toàn nhãn này để giữ bố cục thẻ xe phẳng, bám sát kiến thức đã học. |
| **18/11/2026** | Hỗ trợ khởi tạo khung bộ tài liệu bàn giao cho mốc `v2`                                                                                      | AI viết theo góc nhìn bên thứ ba và chèn ghi chú nhắc nhở chung chung; tôi tự biên tập lại toàn bộ câu chữ cho khớp với quá trình làm bài thực tế và tổ chức lại thư mục `css/styles.css`.                                                                                                                                          |
| **19/11/2026** | Tổng hợp thông số kỹ thuật mẫu xe Audi RS7 Performance 2025 từ bài đánh giá MotorTrend và rà soát liên kết `css/styles.css` cho mốc nộp `v3` | Tự đối chiếu từng thông số thực tế (`621 HP`, `0–96 km/h trong 3,0 giây`, `850 Nm`, `Quattro`) vào `index.html`; dọn dẹp tệp CSS thừa ở thư mục gốc để giữ duy nhất `css/styles.css`; trực tiếp chạy kiểm thử trên Chrome DevTools và URL GitHub Pages ẩn danh rồi ghi nhận kết quả thật vào `docs/evidence-index.md`.              |

---

## 2. Chi tiết các quyết định kỹ thuật quan trọng

### 2.1. Chuẩn hóa Semantic HTML5 & Trợ năng Form

- **Vấn đề ban đầu:** Trang có 2 thẻ `<h1>` (ở logo header và tiêu đề Hero); biểu mẫu đăng ký lái thử thiếu thẻ `<label>` liên kết tường minh.
- **Quyết định của sinh viên:** Chấp nhận phương án chỉ giữ 1 thẻ `<h1>` duy nhất ở khu vực Hero Banner; bổ sung đầy đủ `<label for="...">`, gợi ý `<p class="help">` gắn `aria-describedby` và trạng thái `:user-invalid`, `:focus-visible` trong `css/styles.css`.
- **Kiểm chứng thực tế:** Mở DevTools (`F12 -> Elements`) xác nhận DOM chỉ có 1 thẻ `<h1>`; nhấn phím `Tab` thấy viền focus đỏ rõ nét; gửi form rỗng bị trình duyệt chặn lại đúng quy chuẩn.

### 2.2. Tái cấu trúc CSS Mobile-First và Quy hoạch thư mục `css/`

- **Vấn đề ban đầu:** CSS viết theo hướng Desktop-First (`max-width`) và chiều cao ảnh cố định `430px` gây tràn khung ngang trên màn hình hẹp 320px.
- **Quyết định của sinh viên:** Quy hoạch mã định dạng vào `css/styles.css`, viết CSS cơ sở 1 cột cho 320px, mở rộng lên 2 cột ở `640px` và 3 cột ở `992px`, dùng `aspect-ratio: 16 / 10` cho khung ảnh.
- **Kiểm chứng thực tế:** Chạy thử trên Chrome DevTools ở độ rộng `320px` và `375px` (iPhone SE), lệnh Console `document.body.scrollWidth > window.innerWidth` trả về `false` (không xuất hiện thanh cuộn ngang).

### 2.3. Kiểm soát và đối chiếu kết quả trên môi trường triển khai thật

- Toàn bộ nội dung mã nguồn và tài liệu bàn giao (`README.md`, `CHANGELOG.md`, `docs/evidence-index.md`, `docs/AI_LOG.md`) đều đã được kiểm tra chéo đường dẫn tương đối (`css/styles.css`, `assets/audi-logo.png`, `ket-qua.html`) và xác minh hoạt động công khai trên GitHub Pages tại `https://vanhkazen.github.io/fit4014-a3-audi-vietnam/` trước khi gắn tag `v3`.
- Ảnh minh chứng được lưu trong `docs/evidence/`: [06-pages-public.png](../docs/evidence/06-pages-public.png) và [after-320.png](../docs/evidence/after-320.png).
