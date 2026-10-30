# RELEASE_NOTES — Portfolio thực hành Lab 5

## Bản bàn giao

- **Tên sản phẩm:** FIT / Portfolio V5 – Portfolio thực hành HTML5 và CSS3
- **Mã phiên bản bàn giao:** v7
- **Ngày cập nhật:** 2026-10-30
- **Mã nguồn của bản này:** working tree trong thư mục dự án, đặc biệt là [trang portfolio](./index.html), [trang kết quả form](./ket-qua.html) và [stylesheet](./css/style.css). Các liên kết này trỏ tới đúng các tệp được bàn giao cùng bản ghi chú.

## Thay đổi chính

- Hoàn thiện CSS tương tác cho trạng thái focus bàn phím, hover menu, button và project card; giữ nguyên các breakpoint responsive hiện có.
- Hoàn thiện kiểu dáng trường form và đồng bộ font, giới hạn chiều rộng/resize textarea.
- Đổi nhãn trường textarea từ “Mật khẩu” thành “Nội dung tin nhắn”, phù hợp với mục đích form liên hệ mô phỏng.
- Bổ sung hướng dẫn sản phẩm và chạy/kiểm tra trong [README](./README.md), cùng nhật ký sử dụng AI tại [AI_LOG.md](./AI_LOG.md).

## Lỗi đã sửa

- Các khai báo CSS Lab 5 còn placeholder/không hoàn chỉnh đã được thay bằng giá trị CSS cụ thể để stylesheet áp dụng được.
- Nhãn “Mật khẩu” không khớp với dữ liệu thực tế của textarea đã được sửa.
- Đã bổ sung hướng dẫn kiểm tra đường dẫn trang chủ, stylesheet và trang đích form nhằm hỗ trợ xử lý lỗi 404. Người dùng có báo đã sửa được lỗi đường dẫn/404; lỗi không được tái hiện độc lập trong lần bàn giao này.

## Commit liên quan

- **Commit gần nhất được quan sát:** `79d7142` (`AI`).
- Đây là commit nền trong repository, không xác nhận là commit chứa toàn bộ thay đổi v7. Các thay đổi bàn giao hiện chưa có commit v7 riêng; không có hash commit phát hành để dẫn.

## Hạn chế còn lại

- Portfolio hiện không tham chiếu ảnh; do đó chưa có ảnh để kiểm tra tải/hiển thị.
- Form chỉ dùng GET để mô phỏng điều hướng tới `ket-qua.html`. Không gửi email, không lưu dữ liệu; dữ liệu mẫu xuất hiện trong URL.
- URL repository, GitHub Pages và hồ sơ tác giả thực tế chưa được cung cấp/xác nhận trong README.
- Lỗi 404 đã được người dùng báo là đã sửa, nhưng chưa có URL Pages hoặc minh chứng kiểm tra trực tiếp để xác nhận trạng thái xuất bản.

## Tiếp tục kiểm tra và bàn giao

1. Mở [README](./README.md) và làm theo phần **Chạy local** để chạy từ đúng thư mục chứa `index.html`.
2. Kiểm tra liên kết điều hướng, bố cục ở kích thước hẹp/rộng, trạng thái focus/hover, validation của form, điều hướng tới `ket-qua.html` và liên kết quay lại.
3. Nếu có 404, kiểm tra thư mục gốc đang phục vụ có `index.html`, `ket-qua.html`, `css/style.css`, đồng thời kiểm tra Console/Network của trình duyệt.
4. Trước khi phát hành công khai, điền URL repository, URL Pages và hồ sơ tác giả vào README; thử lại trang chủ và form bằng URL Pages thực tế.
5. Tạo commit/tag v7 riêng sau khi chốt nội dung và xác nhận các bước kiểm tra. Ghi hash commit/tag phát hành tại đây để liên kết chính xác với bản mã đã nộp.