# RELEASE_NOTES - Bản phát hành chính thức v3

## Thông tin phiên bản

- Tên/Mã phiên bản: **Website Trang Trại Gà Quang Linh (QL FARM) - v3**
- Phiên bản: **v3 (Bản hoàn thiện bàn giao A3)**
- Ngày cập nhật: **2026-11-19**
- Sinh viên: **Đàm Quang Linh - 2071020117**
- Lớp / Ngành: **CNTT 20-04 / Công nghệ thông tin**
- Giảng viên hướng dẫn: **ThS. Lê Thái Bảo**
- Nhánh phát hành: `main`
- Repository: https://github.com/linhdam208-hash/trang-trai-ga

## Tóm tắt nâng cấp

Từ `v2` sang `v3`, dự án chuyển sang giai đoạn hoàn thiện hồ sơ bàn giao A3: bổ sung `CHANGELOG.md` và `docs/evidence-index.md`, đồng bộ toàn bộ thông tin chủ sở hữu, chuẩn hóa liên kết tương đối và rà soát chéo mã nguồn với 12 tiêu chí Rubric A3.

## Tính năng hoàn thiện

- HTML5 Semantic và cấu trúc nhiều section rõ ràng.
- Giao diện Mobile-First, breakpoint 640px và 960px.
- Ba sản phẩm dạng Card kèm hình ảnh có thuộc tính `alt`.
- Bảng giá Semantic Table với tiêu đề cột và hàng.
- Form đặt hàng có `required`, ràng buộc độ dài, `email`, `label` gắn với `id` và gửi `GET` sang `ket-qua.html`.
- Trạng thái focus bằng `:focus-visible` cho điều hướng và form.

## Lỗi giao diện/responsive đã khắc phục

- Thanh điều hướng cho phép `flex-wrap: wrap`, giúp menu không cố gắng giữ thành một dòng duy nhất ở 320px.
- Lưới Card sử dụng `repeat(..., minmax(0, 1fr))` và Card đặt `min-width: 0`.
- Lưới quy trình/bảng giá dùng `minmax(0, 1fr)` và các khối con đặt `min-width: 0`; vùng bảng còn có cuộn ngang an toàn.
- CSS hình ảnh dùng `max-width: 100%` và `height: auto` để tránh tràn ngang.

## Hạn chế còn lại

- Đây là website tĩnh; không có CSDL và không có backend.
- Form chỉ mô phỏng gửi dữ liệu bằng phương thức `GET` tới `ket-qua.html`; dữ liệu không được lưu.
- Trang kết quả không hiển thị lại tham số đã nhập.
- GitHub Pages chỉ hoạt động sau khi được cấu hình xuất bản nhánh `main`, thư mục `/ (root)`.
- Chưa có bộ test tự động; phần bàn giao dùng checklist thủ công và DevTools.

## Hướng dẫn kiểm tra bàn giao

1. Chạy `python -m http.server 8080` tại thư mục gốc.
2. Kiểm tra `index.html`, các neo điều hướng, ba Card, bảng giá và ba ảnh.
3. Kiểm tra form rỗng/sai/đúng bằng trình duyệt.
4. Kiểm tra responsive tại 320px, 640px và 960px; kiểm tra Tab, focus và không tràn ngang.
5. Kiểm tra `ket-qua.html` sau khi form hợp lệ và liên kết trở về trang chủ.
6. Đối chiếu tại [docs/evidence-index.md](docs/evidence-index.md).

## Tài liệu liên quan

- [README.md](README.md)
- [CHANGELOG.md](CHANGELOG.md)
- [AI_LOG.md](AI_LOG.md)
- [Bảng minh chứng A3](docs/evidence-index.md)
