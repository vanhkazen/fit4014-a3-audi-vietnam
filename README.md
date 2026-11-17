# Audi Việt Nam — Showroom trực tuyến

Website giới thiệu showroom Audi bằng HTML và CSS, thực hiện cho bài tập lớn A3 môn Thiết kế Web & Triển khai HTPM (FIT4014).

## Thông tin

- **Tác giả:** Trần Việt Anh
- **Repository:** [vanhkazen/fit4014-a3-audi-vietnam](https://github.com/vanhkazen/fit4014-a3-audi-vietnam)
- **Hồ sơ tác giả:** [github.com/vanhkazen](https://github.com/vanhkazen)
- **GitHub Pages:** [vanhkazen.github.io/fit4014-a3-audi-vietnam](https://vanhkazen.github.io/fit4014-a3-audi-vietnam/)

> **Trạng thái xuất bản:** URL Pages ở trên là địa chỉ dự kiến theo tên repository. Tại ngày 18/11/2026, cấu hình GitHub Pages của repository chưa được tìm thấy (GitHub Pages API trả về 404), vì vậy chưa xác nhận website đã được triển khai hoặc URL truy cập được. Có thể mở bản local theo hướng dẫn bên dưới.

## Mô tả

Trang chủ giới thiệu Audi RS7 Sportback, bộ sưu tập xe, công nghệ và thông tin thương hiệu. Người xem có thể đi tới biểu mẫu đăng ký lái thử; biểu mẫu kiểm tra các trường bắt buộc ở trình duyệt và chuyển sang trang kết quả mô phỏng. Dữ liệu được gửi bằng GET, không được lưu trên máy chủ và không gửi email.

## Cấu trúc thư mục

```text
.
├── index.html          # Trang showroom và biểu mẫu đăng ký
├── ket-qua.html        # Trang kết quả đăng ký mô phỏng
├── styles.css          # Giao diện và bố cục responsive
├── assets/
│   ├── audi-logo.png
│   ├── audi-etron-gt.jpg
│   ├── audi-q8-etron.jpg
│   ├── audi-rs6-avant.jpg
│   └── audi-rs7-sportback.jpg
├── README.md
├── AI_LOG.md
└── RELEASE_NOTES.md
```

## Chạy local

Không cần cài thư viện hay build:

1. Tải hoặc clone repository.
2. Mở `index.html` trực tiếp bằng trình duyệt; hoặc chạy một máy chủ tĩnh tại thư mục dự án, ví dụ `python -m http.server 8000`, rồi truy cập `http://localhost:8000`.
3. Nếu dùng máy chủ Python, dừng máy chủ bằng `Ctrl+C` sau khi kiểm tra.

## Cách kiểm tra các trang và chức năng

1. Mở trang chủ, kiểm tra logo, ảnh xe và các mục điều hướng.
2. Chọn **Dòng xe**, **Công nghệ**, **Về Audi** trên thanh điều hướng để kiểm tra các phần tương ứng.
3. Tại **Đăng ký lái thử**, gửi thử biểu mẫu thiếu trường hoặc sai định dạng để xem xác thực HTML; sau đó điền đủ họ tên (2–80 ký tự), số điện thoại (10–11 chữ số), email hợp lệ, mẫu xe và ghi chú (10–500 ký tự).
4. Gửi biểu mẫu hợp lệ để tới `ket-qua.html`; kiểm tra liên kết quay lại trang chủ. Trang kết quả chỉ mô phỏng xác nhận, không gửi hay lưu dữ liệu.
5. Thu nhỏ cửa sổ trình duyệt để kiểm tra bố cục trên màn hình nhỏ.

## Nguồn và xuất bản

- Mã nguồn của website được lưu trong repository GitHub nêu trên; dự án là trang tĩnh, không có bước build.
- URL GitHub Pages dự kiến nằm ở phần [Thông tin](#thông-tin), nhưng chưa xác nhận đã bật triển khai.
- Font được tải từ [Google Fonts](https://fonts.google.com/). Ảnh showroom trong phần giới thiệu được nhúng từ [giaxeaudi.com.vn](https://giaxeaudi.com.vn/wp-content/uploads/Audi-Viet-Nam-Co-Bao-Nhieu-Dia-Chi-Showroom-Phan-Phoi-Chinh-Hang.jpg); các ảnh còn lại và logo là tệp trong `assets/`.

## Hồ sơ và minh chứng

- [Hồ sơ GitHub tác giả](https://github.com/vanhkazen)
- [Repository và mã nguồn](https://github.com/vanhkazen/fit4014-a3-audi-vietnam)
- [AI_LOG.md](./AI_LOG.md) — quá trình tham khảo AI và quyết định của sinh viên
- [RELEASE_NOTES.md](./RELEASE_NOTES.md) — ghi chú bàn giao v2
- [Bản mã website tại commit nền 1963253](https://github.com/vanhkazen/fit4014-a3-audi-vietnam/tree/1963253b634f311e33798a143649f209be696b5f)

## Giới hạn

Đây là giao diện minh họa phục vụ học tập, không phải website bán hàng hay đặt lịch thực. Nội dung giá và thông số xe chỉ để tham khảo trong giao diện; biểu mẫu không có backend. Font và ảnh showroom ngoài repository cần kết nối Internet để tải.
