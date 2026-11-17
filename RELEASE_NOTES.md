# Release notes — Audi Việt Nam v2

## Thông tin bản bàn giao

- **Tên:** Audi Việt Nam — Showroom trực tuyến
- **Mã phiên bản:** v2 (bản tài liệu bàn giao)
- **Ngày cập nhật:** 18/11/2026
- **Repository:** [vanhkazen/fit4014-a3-audi-vietnam](https://github.com/vanhkazen/fit4014-a3-audi-vietnam)
- **Bản mã website:** [commit nền `1963253b634f311e33798a143649f209be696b5f`](https://github.com/vanhkazen/fit4014-a3-audi-vietnam/tree/1963253b634f311e33798a143649f209be696b5f)

## Thay đổi chính

- Mở rộng README để người nhận biết cách mở website local, đi qua các phần chính, kiểm tra biểu mẫu và hiểu các giới hạn của bản mô phỏng.
- Thêm nhật ký AI nêu rõ dữ kiện ban đầu, gợi ý, quyết định của sinh viên và phần chưa kiểm thử.
- Thêm ghi chú bàn giao v2 và trạng thái xuất bản.

## Lỗi đã sửa

- Bổ sung các thông tin hướng dẫn bàn giao còn thiếu trong README ban đầu.
- Không có sửa lỗi chức năng trong HTML/CSS ở bản cập nhật tài liệu này.

## Commit liên quan và bản mã nộp

Commit `1963253b634f311e33798a143649f209be696b5f` là commit mã nguồn website đã có trên repository trước khi cập nhật tài liệu. Các thay đổi trong ba tài liệu bàn giao hiện chưa được commit; do đó chưa có commit mới đại diện cho toàn bộ cây thư mục v2. Khi tạo commit nộp, hãy cập nhật mục này bằng liên kết commit mới để trỏ chính xác đến toàn bộ bản bàn giao.

## Hạn chế còn lại

- GitHub Pages chưa được xác nhận bật: truy vấn cấu hình Pages trả về 404. URL dự kiến là [https://vanhkazen.github.io/fit4014-a3-audi-vietnam/](https://vanhkazen.github.io/fit4014-a3-audi-vietnam/), chưa xác nhận truy cập được.
- Website là trang tĩnh; biểu mẫu chỉ chuyển GET sang trang xác nhận, không lưu dữ liệu và không gửi email.
- Chưa thực hiện kiểm thử tương tác trên trình duyệt trong lần cập nhật này.
- Một số ảnh và font tải từ Internet; ảnh showroom được nhúng ngoài repository.

## Tiếp tục kiểm tra và bàn giao

1. Mở `index.html` trực tiếp hoặc chạy `python -m http.server 8000`, rồi làm theo các bước trong [README](./README.md).
2. Nếu cần xuất bản, bật GitHub Pages cho repository với nguồn triển khai phù hợp với trang tĩnh; sau khi hoàn tất, mở URL Pages dự kiến và cập nhật trạng thái trong README.
3. Thực hiện thử biểu mẫu hợp lệ/không hợp lệ trên trình duyệt và ghi nhận kết quả thực tế.
4. Commit ba tài liệu cùng bản mã cần nộp, rồi thay liên kết commit nền ở trên bằng liên kết commit chứa chính xác toàn bộ bản bàn giao.
