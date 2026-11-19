# AI_LOG - Nhật ký sử dụng AI

## 1. Hiện tượng và dữ kiện ban đầu

- Dự án có `index.html`, `ket-qua.html`, `css/style.css` và thư mục `assets/images/`.
- Mã nguồn tách HTML/CSS; form dùng `action="ket-qua.html"` và `method="get"`, không có CSDL/backend.
- Các phiên bản thực tế: `v1` tại commit `a124134`, `v2` tại commit `90f9742` (tag `v2.0`) và trạng thái chuyển sang `v3`.
- Trước phiên bản v3, tài liệu chưa có `CHANGELOG.md` và `docs/evidence-index.md`; README/các ghi chú cần đồng bộ chủ sở hữu và liên kết.
- Tên chủ sở là **Đàm Quang Linh - 2071020117 - CNTT 20-04 / Công nghệ thông tin - ThS. Lê Thái Bảo**.

## 2. Nhận định của sinh viên trước khi dùng AI

Sinh viên cần lưu giữ dữ kiện thực tế thay vì suy đoán. Cấu trúc, tên tệp và đường dẫn phải lấy từ workspace; trạng thái GitHub Pages chỉ được ghi theo kết quả kiểm chứng, không mặc định là đã hoạt động.

Với giai đoạn v3, tài liệu phải đủ cấu trúc, 100% liên kết chéo đúng tên tệp và HTML/CSS cần rà lại thuộc tính truy cập cơ bản, responsive 320px/640px/960px.

## 3. Công cụ AI sử dụng và tóm tắt gợi ý

- **Gemini:** hỗ trợ giai đoạn v2 đề xuất khung nội dung README, AI_LOG và RELEASE_NOTES; sinh viên yêu cầu tóm tắt, đối chiếu repository và không sao chép hội thoại dài.
- **GitHub Copilot SDK trong VS Code:** hỗ trợ giai đoạn v3 rà workspace, thống nhất tài liệu, tạo bảng minh chứng và ghi nhận các lỗi CSS/HTML có thể phát hiện.

Gợi ý AI cho v3 gồm:
- Viết README theo đúng 8 mục và tên sản phẩm “Website Trang Trại Gà Quang Linh (QL FARM)”.
- Viết CHANGELOG theo ba mốc v1/v2/v3.
- Dùng `minmax(0, 1fr)` và `min-width: 0` cho Grid.
- Tạo mục minh chứng và checklist Local – Repository – GitHub Pages.
- Kiểm tra các liên kết `href/src/action` và thuộc tính `alt`/`label`.

## 4. Quyết định của sinh viên

- **Chấp nhận:** cấu trúc tài liệu 8 mục/6 mục, bảng minh chứng, checklist, cách kiểm tra trình duyệt và ghi rõ giới hạn website tĩnh.
- **Chấp nhận có điều chỉnh:** gộp tên chủ sở hữu và thông tin giảng viên vào mọi tài liệu bắt buộc; giữ tên tệp thực tế thay vì dùng tên viết tắt.
- **Chấp nhận cho mã nguồn:** bổ sung `min-width: 0` cho khối split layout và đổi `grid-template-columns` sang `minmax(0, 1fr)`, vì hai thuộc tính làm giảm nguy cơ tràn cột mà không đổi bố cục.
- **Bác bỏ:** không cho phép AI tuyên bố backend, CSDL hoặc GitHub Pages đã hoạt động nếu không có bằng chứng trực tiếp.
- **Bác bỏ:** không ghi commit/URL mẫu thay cho dữ kiện repository thực tế.

## 5. Phần tự chỉnh sửa và kiểm chứng thực tế

Sinh viên tự chịu trách nhiệm quyết định cuối, kiểm tra workspace và đối chiếu bằng trình duyệt/DevTools:

- Kiểm tra ba ảnh trong `assets/images/`, đường dẫn stylesheet và hai trang HTML.
- Xác nhận mọi thẻ `img` có `alt` và mọi trường form có `<label for>` tương ứng.
- Xác nhận menu dùng `flex-wrap: wrap`, Grid Card dùng `minmax(0, 1fr)`, và vùng bảng có `overflow-x: auto`.
- Rà lại form rỗng/sai/đúng: `required`, `minlength`, `maxlength` và `type="email"`.
- Kiểm tra liên kết Markdown bằng cách đối chiếu tên tệp thực tế trong thư mục gốc và `docs/`.
- Cập nhật CSS split layout sau khi rà soát để phòng tràn ở thiết bị hẹp.

Hướng dẫn kiểm chứng trên DevTools: đặt Responsive Mode ở 320px, 640px và 960px; dùng Tab để kiểm tra focus; kiểm tra Console và Network không có lỗi tài nguyên; gửi form hợp lệ và xác nhận URL chuyển sang `ket-qua.html?fullname=...&email=...&message=...`.

## 6. Cam kết bảo mật

Hồ sơ không chứa token, mật khẩu, khóa API, cookie hoặc dữ liệu đăng nhập nhạy cảm. Sinh viên cam kết không đưa thông tin cá nhân bí mật hoặc bí mật repository vào mã nguồn và tài liệu bàn giao.
