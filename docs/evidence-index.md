# Bảng minh chứng Rubric A3 - Phiên bản v3

Thông tin sản phẩm: **Website Trang Trại Gà Quang Linh (QL FARM)**  
Sinh viên: **Đàm Quang Linh - 2071020117**  
Lớp / Ngành: **CNTT 20-04 / Công nghệ thông tin**  
Giảng viên hướng dẫn: **ThS. Lê Thái Bảo**

## Ma trận đối chiếu 12 tiêu chí

| Mã tiêu chí | Nội dung tuyên bố | Phép thử / Cách kiểm chứng | Vị trí tệp / Minh chứng | Phiên bản |
|---|---|---|---|---|
| A3.TC1a | Sử dụng cấu trúc HTML5 Semantic. | Mở DevTools Elements; xác nhận `header`, `nav`, `main`, `section`, `footer`. | [index.html](../index.html), [ket-qua.html](../ket-qua.html) | v3 |
| A3.TC1b | Chia nội dung rõ ràng bằng heading và khu vực semantic. | Kiểm tra thứ tự h1/h2/h3; kiểm tra anchor trỏ đến các `id`. | [index.html](../index.html) | v3 |
| A3.TC2a | Trình bày đủ ba Card sản phẩm. | Đếm ba `article.card`, kiểm tra ba ảnh và liên kết đặt mua. | [index.html](../index.html), [assets/images/](../assets/images/) | v3 |
| A3.TC2b | Tất cả hình ảnh có mô tả thay thế. | Tìm thẻ `img`; xác nhận thuộc tính `alt`, `width`, `height` hợp lệ và tải được. | [index.html](../index.html) | v3 |
| A3.TC3a | Hiển thị bảng giá bằng Semantic Table. | Kiểm tra `table`, `thead`, `tbody`, `th scope`, ba dòng dữ liệu. | [index.html](../index.html) | v3 |
| A3.TC3b | Bảng không làm vỡ bố cục trên màn hình hẹp. | DevTools đặt 320px; kiểm tra vùng `.table-wrapper` cho phép cuộn ngang. | [css/style.css](../css/style.css) | v3 |
| A3.TC4a | Giao diện responsive Mobile-First. | Kiểm tra bố cục 320px, 640px và 960px; không có tràn ngang ngoài vùng bảng dự kiến. | [css/style.css](../css/style.css) | v3 |
| A3.TC4b | Menu, Grid/Card chống vỡ ở 320px. | Kiểm tra `.site-nav` wrap; `.product-grid` dùng `minmax(0, 1fr)` và Card có `min-width: 0`. | [css/style.css](../css/style.css) | v3 |
| A3.TC5 | Form có HTML5 Validation đầy đủ. | Test rỗng/sai/đúng: `required`, `email`, `minlength`, `maxlength`; xác nhận không gửi khi dữ liệu không hợp lệ. | [index.html](../index.html) | v3 |
| A3.TC6 | Trường form có label và mô tả hỗ trợ. | Kiểm tra `label[for]` khớp `input/textarea[id]`; kiểm tra `aria-describedby` trỏ tới help text. | [index.html](../index.html) | v3 |
| A3.TC7a | Form mô phỏng luồng gửi GET đến trang kết quả. | Gửi dữ liệu hợp lệ; xác nhận URL chứa `fullname`, `email`, `message` và tải `ket-qua.html`. | [index.html](../index.html), [ket-qua.html](../ket-qua.html) | v3 |
| A3.TC7b | Bàn giao có truy xuất tệp/hướng dẫn và khai báo giới hạn. | Mở README và các tệp hồ sơ; kiểm tra liên kết tương đối, vòng đời v1/v2/v3, hạn chế tĩnh và log AI. | [README.md](../README.md), [CHANGELOG.md](../CHANGELOG.md), [RELEASE_NOTES.md](../RELEASE_NOTES.md), [AI_LOG.md](../AI_LOG.md) | v3 |

## Checklist Local - Repository - GitHub Pages

| Hạng mục | Local | Repository | GitHub Pages |
|---|---|---|---|
| Tên và chủ sở hữu dự án | Hiển thị đúng tên, mã sinh viên và giảng viên trong hồ sơ | Đồng bộ trong README và tài liệu v3 | Cần xác nhận nội dung sau khi triển khai |
| Tệp `index.html` | Mở `http://localhost:8080/index.html` | Tồn tại tại thư mục gốc nhánh `main` | URL trỏ tới trang chủ nếu Pages đã bật |
| Tệp `ket-qua.html` | Mở trực tiếp và nhận tham số GET hợp lệ | Tồn tại tại thư mục gốc nhánh `main` | URL `/ket-qua.html` khi Pages hoạt động |
| CSS và ảnh | `css/style.css`, 4 ảnh tải không lỗi | Đường dẫn hoa/thường khớp hệ thống | Kiểm tra Network không có 404 tài nguyên |
| Responsive 320/640/960 | DevTools không phát hiện tràn bố cục ngoài bảng | Mã CSS đã có breakpoint và Grid an toàn | Kiểm tra lại sau publish |
| Tab/focus | Dùng Tab và xác nhận focus-visible | CSS và HTML đã chứa trạng thái tương ứng | Xác nhận trên trình duyệt công khai |
| Form rỗng/sai/đúng | Chạy ba trường hợp validation | Mã HTML lưu đúng các thuộc tính | Chạy lại URL công khai |
| Liên kết tài liệu `.md` | Mở từng liên kết tương đối trong workspace | Tên tệp khớp chính xác | Tài liệu Markdown hiển thị từ repository |
| Trang RELEASE/CHANGELOG/AI_LOG | Đọc đủ nội dung v1/v2/v3 | Tất cả tệp ở thư mục gốc | Minh chứng có thể truy cập qua GitHub |
