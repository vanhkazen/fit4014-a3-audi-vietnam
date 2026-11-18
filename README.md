# Showroom Trực Tuyến Audi Việt Nam

## Sản phẩm này là gì?

Website giới thiệu thương hiệu Audi, tập trung vào Audi RS7 Performance 2025, các dòng xe và công nghệ của hãng. Khách hàng yêu thích xe sang có thể xem thông tin và dùng biểu mẫu đăng ký lái thử.

## Demo

https://vanhkazen.github.io/fit4014-a3-audi-vietnam/

## Tính năng

- Thanh menu điều hướng tới **Trang chủ**, **Dòng xe**, **Công nghệ**, **Về Audi** và **Đăng ký lái thử**.
- Hero giới thiệu Audi RS7 Performance 2025 cùng bốn thông số nổi bật; các mục Dòng xe, Công nghệ và Về Audi cung cấp thêm thông tin.
- Biểu mẫu lái thử có kiểm tra dữ liệu bắt buộc ở trình duyệt; gửi biểu mẫu hợp lệ bằng GET tới `ket-qua.html`.

## Cách mở

1. Mở URL ở mục [Demo](https://vanhkazen.github.io/fit4014-a3-audi-vietnam/) trên trình duyệt.
2. Bấm các mục **Trang chủ**, **Dòng xe**, **Công nghệ**, **Về Audi** hoặc **Đăng ký lái thử** trên thanh menu để cuộn tới từng phần.
3. Bấm nút **Khám phá các dòng xe** để xem danh mục, hoặc điền biểu mẫu ở cuối trang và bấm **Gửi yêu cầu ngay**.

## Cấu trúc thư mục

```text
.
├── index.html
├── ket-qua.html
├── css/
│   └── styles.css
├── assets/
├── docs/
│   ├── AI_LOG.md
│   ├── evidence-index.md
│   └── evidence/
│       ├── 06-pages-public.png
│       └── after-320.png
```

## Đã kiểm tra

Kết quả và phạm vi kiểm tra được ghi tại [docs/evidence-index.md](docs/evidence-index.md). URL GitHub Pages mở công khai được; bản đang phục vụ tại thời điểm kiểm tra vẫn là nội dung RS7 trước khi cập nhật v3. Bản v3 trong workspace cần được xuất bản trước khi xác nhận lại thông số và giao diện trên Pages. Ảnh minh chứng: [06-pages-public.png](docs/evidence/06-pages-public.png), [after-320.png](docs/evidence/after-320.png).

## Hạn chế / Chưa kiểm tra

- Biểu mẫu đăng ký là biểu mẫu tĩnh dùng GET để chuyển sang `ket-qua.html`; chưa có backend hoặc cơ sở dữ liệu để lưu thông tin và không gửi email.
- Chưa kiểm tra trực tiếp trên thiết bị iPhone vật lý; các kiểm tra kích thước hẹp được thực hiện bằng trình duyệt giả lập.
- Tính năng Google Fonts và ảnh showroom ngoài repository cần kết nối Internet.

## Khai báo AI

Nhật ký sử dụng AI và phần tự chỉnh sửa được ghi trong [docs/AI_LOG.md](docs/AI_LOG.md).
