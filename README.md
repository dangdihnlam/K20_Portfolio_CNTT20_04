# Portfolio thực hành Lab 5

## Thông tin sản phẩm

- **Tên sản phẩm:** FIT / Portfolio V5 – Portfolio thực hành HTML5 và CSS3.
- **Tác giả:** Lâm (theo nội dung trang chủ; cập nhật nếu đây là tên mẫu).
- **Mô tả:** Website portfolio tĩnh giới thiệu cá nhân, kỹ năng, dự án và lộ trình học tập. Có bố cục responsive, điều hướng bằng liên kết trong trang, hiệu ứng focus/hover và form kiểm tra dữ liệu ở trình duyệt. Form chỉ mô phỏng; không gửi email và không lưu dữ liệu.
- **Hồ sơ tác giả:** Chưa có URL hồ sơ trong dự án. Bổ sung liên kết hồ sơ cá nhân tại đây trước khi phát hành.
- **Repository:** Chưa cấu hình/cung cấp URL repository. Bổ sung URL GitHub thực tế tại đây.
- **URL GitHub Pages:** Chưa cấu hình/cung cấp URL Pages. Bổ sung URL sau khi bật GitHub Pages.

## Cấu trúc thư mục

```text
K20_Portfolio_CNTT20_04/
├── index.html          # Trang portfolio chính
├── ket-qua.html        # Trang kết quả mô phỏng của form
├── css/
│   └── style.css       # Giao diện, responsive và trạng thái tương tác
├── kiem-tra-lab5.txt   # Mẫu ghi kết quả kiểm thử/minh chứng
├── AI_LOG.md           # Nhật ký sử dụng AI
└── README.md           # Hướng dẫn dự án
```

## Chạy local

1. Mở terminal tại thư mục `K20_Portfolio_CNTT20_04` (thư mục chứa `index.html`).
2. Chạy máy chủ tĩnh bằng Python:

   ```powershell
   py -m http.server 8000
   ```

   Nếu lệnh `py` không có, thử `python -m http.server 8000`.
3. Mở `http://localhost:8000/` trên trình duyệt. Dừng máy chủ bằng `Ctrl+C`.

Cũng có thể mở trực tiếp `index.html`, nhưng chạy máy chủ local giúp kiểm tra các đường dẫn trang và hành vi giống môi trường xuất bản hơn. Nếu gặp 404, kiểm tra terminal đang ở đúng thư mục chứa `index.html`.

## Nguồn và cách xuất bản

- **Mã nguồn:** các file HTML/CSS trong repository của dự án; repository URL cần được bổ sung sau khi tạo hoặc xác nhận repository.
- **Nguồn xuất bản dự kiến:** GitHub Pages từ repository này. Pages chưa được xác nhận đã bật; sau khi cấu hình, điền URL Pages thực tế ở phần Thông tin sản phẩm.
- Với cấu hình Pages xuất bản từ thư mục gốc của nhánh đã chọn, `index.html` là trang vào; giữ nguyên `css/style.css` và `ket-qua.html` cùng cấu trúc tương đối để tránh lỗi đường dẫn/404.

## Kiểm tra trang và chức năng chính

1. **Trang chủ (`index.html`):** xác nhận tiêu đề “Xin chào, tôi là An”, nội dung giới thiệu và các mục Giới thiệu, Kỹ năng, Dự án, Lộ trình, Liên hệ hiển thị.
2. **Điều hướng:** bấm từng liên kết trên menu và các nút/liên kết trong thẻ dự án; trang cần cuộn tới đúng mục tương ứng.
3. **Responsive:** thử cửa sổ hẹp và rộng; các thẻ dự án cần chuyển từ một cột sang hai cột ở `48rem`, rồi ba cột ở `64rem`.
4. **Bàn phím và tương tác:** dùng `Tab`/`Shift+Tab` để đi qua liên kết, ô nhập và nút; kiểm tra dấu focus nhìn rõ. Thử hover menu, nút và thẻ dự án; nhấn giữ nút để thấy trạng thái active.
5. **Kiểm tra form:** để trống trường bắt buộc hoặc nhập email không hợp lệ để xác nhận trình duyệt báo lỗi; thử tên dưới 2 ký tự và tin nhắn dưới 10 ký tự; sau đó nhập dữ liệu giả hợp lệ và gửi. Trang `ket-qua.html` phải mở và có liên kết quay lại form. Dữ liệu gửi bằng GET sẽ xuất hiện trên URL; không nhập thông tin thật.
6. **Đường dẫn và trang kết quả:** xác nhận CSS tải được ở cả hai trang và liên kết quay lại tới `index.html#lien-he` hoạt động. Khi kiểm tra trên Pages, mở trực tiếp trang chủ và thử gửi form để phát hiện lỗi 404.

## Hồ sơ và minh chứng

- **Hồ sơ cá nhân trực tuyến:** chưa được cung cấp; thêm URL hồ sơ tác giả tại đây.
- **Minh chứng kiểm thử:** [mẫu ghi kết quả Lab 5](./kiem-tra-lab5.txt). Điền kết quả thực tế, ảnh chụp màn hình hoặc URL minh chứng sau khi chạy các bước kiểm tra ở trên.
- **Nhật ký AI:** [AI_LOG.md](./AI_LOG.md).
