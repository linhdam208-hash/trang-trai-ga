# AI_LOG - Quyết định của sinh viên

## 1. Hiện tượng và dữ kiện ban đầu

- Repository đã có `index.html`, `ket-qua.html`, `css/style.css` và ảnh sản phẩm.
- `README.md` chỉ còn một tiêu đề và hai dòng giới thiệu ngắn.
- Repository chưa có `AI_LOG.md` và `RELEASE_NOTES.md`.
- Website là trang tĩnh: form dùng `action="ket-qua.html"` và `method="get"`; chưa có xử lý/lưu dữ liệu phía máy chủ.
- GitHub repository tồn tại; URL GitHub Pages dự kiến được kiểm tra trong phiên làm việc và trả HTTP 404 vào ngày 18/11/2026.
- Commit đang bàn giao: `a124134c57c6eec4326bbe1b88ba80fd8978305e` trên nhánh `main`.

## 2. Nhận định trước khi dùng AI

Tài liệu bàn giao cần mô tả đúng trang có sẵn, không được suy đoán chức năng backend hoặc mô tả Pages đã hoạt động khi hiện tại chưa chứng minh được. URL, commit, cấu trúc thư mục và cách kiểm tra phải lấy trực tiếp từ repository.

## 3. Công cụ, prompt và phản hồi mẫu

- Công cụ: GitHub Copilot SDK trong VS Code, Gemini
- Prompt của sinh viên: yêu cầu tạo/sửa `README.md`, `AI_LOG.md` và `RELEASE_NOTES.md` theo các mục nội dung; không yêu cầu thay đổi giao diện hoặc chức năng sản phẩm.
- AI đề xuất: kiểm tra repository, xác minh remote và commit, đối chiếu `index.html`/`ket-qua.html`, ghi rõ Pages đang 404, và tạo ba tài liệu theo đúng tên tệp.

## 4. Gợi ý của AI

AI đề xuất:

- Trình bày `linhdam208-hash` là tác giả/owner theo dữ liệu Git và GitHub vì tên đầy đủ của sinh viên không có trong repository.
- Liên kết trực tiếp repository, hồ sơ GitHub và commit thay cho ghi thông tin không thể xác minh.
- Mô tả form là luồng tĩnh bằng `GET`, không tuyên bố dữ liệu được gửi hoặc lưu.
- Ghi hạn chế Pages thay vì giả định Pages đã bật.
- Đưa ra bộ kiểm tra có thể tự chạy local.

## 5. Quyết định của sinh viên

Sinh viên chấp nhận gợi ý đối chiếu repository và ghi đúng trạng thái thực tế. Sinh viên giữ nguyên `index.html`, `ket-qua.html`, `css/style.css` và toàn bộ tài nguyên ảnh; chỉ tạo/cập nhật tài liệu. Sinh viên chọn mã phiên bản `v1.0.0` cho bản bàn giao do đây là mốc phát hành đầu tiên hiện có trong repository.

Quyết định không kích hoạt hoặc giả lập GitHub Pages trong tài liệu vì không có quyền cấu hình nguồn xuất bản được xác nhận ngoài repository; thay vào đó ghi URL dự kiến và trạng thái kiểm tra 404.

## 6. Phần sửa đã thực hiện

- Cập nhật `README.md` bằng mô tả sản phẩm, tác giả/owner, cấu trúc thư mục, hướng dẫn local, URL Pages, nguồn xuất bản, cách kiểm tra và liên kết minh chứng.
- Tạo `AI_LOG.md` này để ghi hiện tượng, định hướng, gợi ý, quyết định và cách thử lại.
- Tạo `RELEASE_NOTES.md` theo phiên bản `v1.0.0`.
- Không sửa mã HTML, CSS hay ảnh.

## 7. Cách thử lại và kết quả

1. Chạy `git status` và `git log` để xác nhận nhánh `main`, remote, tác giả commit và mã commit.
2. Kiểm tra bằng HTTP HEAD:
   - Repository: HTTP 200.
   - Hồ sơ GitHub: HTTP 200.
   - URL Pages dự kiến: HTTP 404.
3. Đối chiếu nội dung trang chủ, trang kết quả, form và CSS trực tiếp trong repository.
4. Sau khi tài liệu được lưu, kiểm tra lại các tệp bằng git diff và URL Markdown của commit.

Kết quả: tài liệu đã được viết theo trạng thái thực tế của sản phẩm và commit hiện có. Chức năng website không thay đổi trong phiên làm việc này; việc Pages hiển thị vẫn phụ thuộc cấu hình GitHub Pages trên repository.
