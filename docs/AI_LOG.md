# Nhật ký sử dụng AI

## Hiện tượng và dữ kiện ban đầu

- Người dùng báo: “không hiện ảnh”, “không đúng đường dẫn”, trang lỗi và máy chủ trả 404.
- Dự án là website tĩnh gồm `index.html`, `ket-qua.html` và `css/style.css`. Tại thời điểm xem mã, HTML không có thẻ ảnh hoặc đường dẫn ảnh; CSS được liên kết tương đối bằng `css/style.css`, form gửi tới `ket-qua.html`.
- Chưa có ảnh chụp lỗi, URL đang truy cập hoặc thông tin cấu hình máy chủ để xác định chính xác nguyên nhân 404.

## Nhận định trước khi dùng AI

Các lỗi có thể liên quan tới đường dẫn tương đối hoặc việc mở/chạy dự án từ sai thư mục. Tuy nhiên, vì không có URL và dữ liệu lỗi cụ thể, chưa thể kết luận đây là nguyên nhân. Việc không thấy ảnh cũng phù hợp với mã hiện tại vì trang chưa tham chiếu file ảnh nào.

## Công cụ và trao đổi mẫu

- **Công cụ:** trợ lý AI trong VS Code; xem nội dung HTML/CSS và các tệp hướng dẫn dự án.
- **Yêu cầu ban đầu (tóm tắt):** hỗ trợ với tình trạng không hiện ảnh, sai đường dẫn, lỗi trang và 404.
- **Phản hồi AI liên quan (tóm tắt):** hoàn thiện một số chỗ CSS còn thiếu và thay nhãn form gây nhầm lẫn; nêu rằng dự án chưa có ảnh được tham chiếu và gợi ý kiểm tra thư mục/đường dẫn mở trang.

## Gợi ý, quyết định và lý do

- Gợi ý kiểm tra thư mục gốc đang chạy có chứa `index.html`, giữ nguyên đường dẫn tương đối `css/style.css` và `ket-qua.html`, và không coi việc tải trang thành công là bằng chứng ảnh đã được cấu hình.
- Chấp nhận các sửa đổi CSS/form vì chúng hoàn thiện các phần còn khuyết và làm nhãn form khớp với nội dung tin nhắn. Không tự thêm ảnh hoặc URL ảnh vì chưa có tài nguyên và nguồn ảnh được cung cấp.
- Không kết luận nguyên nhân gốc của 404 khi thiếu URL, cấu hình xuất bản và ảnh chụp lỗi.

## Phần đã sửa

- AI đã đề xuất và cập nhật trạng thái focus/hover, transition cho nút và thẻ, cùng kiểu dáng và kích thước trường form trong `css/style.css`.
- Nhãn textarea trong `index.html` được đổi từ “Mật khẩu” thành “Nội dung tin nhắn”, phù hợp với form liên hệ mô phỏng.
- README được bổ sung hướng dẫn chạy local và kiểm tra đường dẫn. Nhật ký này không ghi nhận thay đổi đường dẫn ảnh, vì dự án chưa có ảnh được tham chiếu.

## Cách thử lại và kết quả

- Hướng dẫn thử: chạy máy chủ tĩnh tại thư mục chứa `index.html`, mở trang chủ, xác nhận CSS tải được; gửi form bằng dữ liệu giả để mở `ket-qua.html`; kiểm tra Console/Network nếu vẫn gặp 404.
- Người dùng đã báo “Đã sửa được lỗi”, nhưng không cung cấp bước tái hiện, URL, ảnh chụp hoặc kết quả kiểm tra cụ thể. Vì vậy, đây là báo cáo của người dùng, không phải kết quả kiểm chứng độc lập; chưa xác nhận riêng việc hiển thị ảnh hay xuất bản trên Pages.
