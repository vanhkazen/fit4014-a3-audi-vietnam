# AI_LOG - Nhật Ký Sử Dụng AI (Cập nhật bản v2)

## 1. Phạm vi và mục đích sử dụng

Trong giai đoạn chuẩn bị phiên bản **v2**, em sử dụng trợ lý AI để hỗ trợ rà soát bố cục mã nguồn theo Rubric A3 và khởi tạo khung bộ tài liệu bàn giao (`README.md`, `CHANGELOG.md`, `AI_LOG.md`) cho dự án **Website Showroom Audi Việt Nam**.

## 2. Hiện tượng và dữ kiện thực tế của dự án (Mốc v2)

- **Hiện trạng mã nguồn:** Website tĩnh thuần HTML5/CSS3 (`index.html`, `ket-qua.html`, `styles.css`, `assets/`), kế thừa từ commit gốc `1963253b634f311e33798a143649f209be696b5f` trên nhánh `main` của repository `vanhkazen/fit4014-a3-audi-vietnam`.
- **Các điểm đã hoàn thiện ở mã nguồn:**
  - Chuẩn hóa Semantic HTML5: đưa trang về duy nhất 1 thẻ `<h1>` tại Hero Banner, chuyển tên thương hiệu trên header sang `<span>`.
  - Tái cấu trúc CSS sang Mobile-First (1 cột cơ sở ở 320px, mở rộng 2 cột ở 640px và 3 cột ở 992px).
  - Bổ sung `<label>` gắn `for`/`id`, mô tả `<p class="help">` và trạng thái `:user-invalid` cho form đăng ký lái thử.
- **Tình trạng triển khai:** Đang chuẩn bị đẩy bản `v2` lên GitHub để kích hoạt GitHub Pages tại địa chỉ dự kiến `https://vanhkazen.github.io/fit4014-a3-audi-vietnam/`.

## 3. Công cụ AI và nội dung tham khảo

- **Công cụ:** Gemini và GitHub Copilot trong VS Code.
- **Yêu cầu đặt ra cho AI:** Dựa trên cấu trúc tệp thực tế của dự án để viết nháp các tài liệu hướng dẫn vận hành (`README.md`), nhật ký thay đổi (`CHANGELOG.md`) và định dạng biểu mẫu `AI_LOG.md` đúng quy cách môn học.

## 4. Quyết định của sinh viên (Chấp nhận / Chỉnh sửa / Bác bỏ)

- **Bác bỏ phần tử thừa:** Khi AI gợi ý dùng `z-index` để giữ nhãn đè ảnh (`.car-badge`), em quyết định **xóa bỏ hoàn toàn** phần tử này để giữ bố cục phẳng tự nhiên, bám sát nội dung đã học trên lớp.
- **Chỉnh sửa nội dung tài liệu:** AI ban đầu viết tài liệu theo góc nhìn bên thứ ba và chèn các ghi chú nhắc nhở chung chung; em đã tự biên tập lại toàn bộ câu chữ cho khớp với quá trình làm bài thực tế của cá nhân.
- **Giữ nguyên tính trung thực về trạng thái:** Chưa ghi nhận kết quả kiểm thử trực tuyến tại mốc `v2` này vì website cần được đẩy lên GitHub và bật Pages trước, sau đó mới tiến hành kiểm thử thực tế để chốt bản nộp `v3`.

## 5. Bước kiểm chứng tiếp theo (Cho mốc v3)

Sau khi push bản `v2` và kích hoạt thành công GitHub Pages, em sẽ tiến hành chạy kiểm thử trực tiếp trên trình duyệt (độ rộng 320px–1440px, điều hướng phím `Tab`, gửi form thực tế sang `ket-qua.html`), lưu ảnh minh chứng và cập nhật kết quả thật vào bản `v3`.
