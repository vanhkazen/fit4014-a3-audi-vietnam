# Chỉ mục kiểm chứng

| Em thử gì | Kết quả | Ảnh/link (nếu có) |
|---|---|---|
| Mở URL Pages công khai và kiểm tra tài nguyên | Trang Pages trả HTTP 200. CSS, ảnh Audi RS7 và CSS Google Fonts trả HTTP 200; ảnh trong trang đã tải và hai font Plus Jakarta Sans, JetBrains Mono được trình duyệt xác nhận đã nạp. Bản đang công khai vẫn là nội dung trước cập nhật v3. | [Trang Pages](https://vanhkazen.github.io/fit4014-a3-audi-vietnam/), [ảnh chụp trang Pages](../docs/evidence/06-pages-public.png) |
| Bấm lần lượt 5 mục trên thanh menu điều hướng | Đã bấm đủ **Trang chủ**, **Dòng xe**, **Công nghệ**, **Về Audi**, **Đăng ký lái thử** trên bản local; từng liên kết đổi đúng hash và có khu vực đích tương ứng. | `index.html` |
| Xem ở bề rộng di động `320px` và `375px` (iPhone SE) bằng giả lập viewport | Ở cả hai kích thước `document.body.scrollWidth > window.innerWidth` trả về `false`; nội dung không tràn ngang. Đây là kiểm tra giả lập, không phải iPhone thật. | [Ảnh chụp ở 320px](../docs/evidence/after-320.png) |
| Kiểm tra co giãn qua điểm ngắt `640px` và `992px` | Trên bản local, danh mục xe và công nghệ có 1 cột ở `320px`/`375px`, 2 cột từ `640px` và 3 cột từ `992px`; không tràn ngang tại các kích thước đã thử. | [`css/styles.css`](../css/styles.css) |
| Kiểm thử biểu mẫu đăng ký lái thử (`#contact`) | Trên bản local, biểu mẫu trống bị chặn theo kiểm tra hợp lệ của trình duyệt và trường họ tên khớp `:user-invalid`; sau khi điền dữ liệu thử hợp lệ, GET chuyển tới `ket-qua.html` và hiện tiêu đề xác nhận thành công. | [ket-qua.html](../ket-qua.html) |

Các thao tác menu, kích thước màn hình và biểu mẫu được kiểm thử trên bản local; chưa thể xác nhận những kết quả này trên Pages vì bản v3 chưa được xuất bản. Ảnh trang Pages ghi nhận đúng phiên bản cũ đang công khai, còn ảnh `after-320.png` là bản v3 local.
