# Trang Trại Gà Quang Linh

## Tác giả

- Tên sản phẩm: Trang Trại Gà Quang Linh
- Tác giả/owner repository: **linhdam208-hash**
- Hồ sơ GitHub: https://github.com/linhdam208-hash

## Mô tả

Website giới thiệu trang trại bằng HTML/CSS tĩnh. Sản phẩm trình bày giới thiệu trại, ba nhóm sản phẩm, quy trình chăn nuôi 4 bước, bảng giá tham khảo, và form liên hệ đặt hàng. Form gửi dữ liệu bằng `GET` đến trang `ket-qua.html`; sản phẩm không lưu dữ liệu trên máy chủ.

## Liên kết sản phẩm

- Repository: https://github.com/linhdam208-hash/trang-trai-ga
- GitHub Pages dự kiến: https://linhdam208-hash.github.io/trang-trai-ga/
- Trạng thái ngày 18/11/2026: URL Pages đã thử nhưng nhận phản hồi 404; cần bật GitHub Pages cho nhánh `main` và thư mục gốc (`/(root)`).
- Commit bàn giao: https://github.com/linhdam208-hash/trang-trai-ga/commit/a124134c57c6eec4326bbe1b88ba80fd8978305e

## Cấu trúc thư mục

```text
trang-trai-ga/
├── index.html          # Trang chủ và form liên hệ
├── ket-qua.html        # Trang thông báo sau khi form hợp lệ
├── css/
│   └── style.css       # Giao diện và bố cục
├── assets/
│   └── images/         # Hình ảnh trang trại và sản phẩm
├── README.md           # Hướng dẫn sử dụng và kiểm tra
├── AI_LOG.md           # Ghi lại quyết định sử dụng AI
└── RELEASE_NOTES.md    # Ghi chú phiên bản bàn giao
```

## Chạy local

Yêu cầu: Git và Python 3 (hoặc công cụ server tĩnh tương đương).

```powershell
git clone https://github.com/linhdam208-hash/trang-trai-ga.git
cd trang-trai-ga
python -m http.server 8080
```

Mở `http://localhost:8080/index.html` trong trình duyệt. Có thể mở trực tiếp `index.html`, nhưng chạy bằng server giúp kiểm tra URL tương đối và luồng form ổn định hơn.

## Cách kiểm tra chức năng chính

1. Mở trang chủ và kiểm tra thanh điều hướng dẫn đến `Giới thiệu`, `Sản phẩm`, `Quy trình`, `Bảng giá`, `Đặt hàng`.
2. Kiểm tra ba thẻ gốc và ba ảnh trong thư mục `assets/images/` đều hiển thị.
3. Cuộn tới `Bảng giá`, xác nhận ba dòng sản phẩm.
4. Tại form đặt hàng:
   - Không nhập dữ liệu rồi bấm gửi: trình duyệt phải báo trường bắt buộc.
   - Nhập họ tên dưới 2 ký tự: trường họ tên phải không hợp lệ.
   - Nhập email sai định dạng: trường email phải không hợp lệ.
   - Nhập nội dung đặt hàng dưới 10 ký tự: trường nội dung phải không hợp lệ.
   - Nhập đủ dữ liệu hợp lệ và bấm `Kiểm tra & Gửi yêu cầu`: URL chuyển sang `ket-qua.html` kèm tham số `fullname`, `email`, `message`.
5. Kiểm tra nút `Quay về trang chủ` hoặc liên kết brand để trở lại `index.html`.
6. Thử ở kích thước màn hình điện thoại để kiểm tra menu, lưới sản phẩm và bảng giá không bị tràn.

## Nguồn xuất bản

- Mã nguồn: nhánh `main` trên GitHub repository nêu trên.
- Phương thức dự kiến: GitHub Pages, xuất bản thư mục gốc của nhánh `main`.
- Tài liệu bàn giao: `RELEASE_NOTES.md`.
- Minh chứng mã: [commit a124134c](https://github.com/linhdam208-hash/trang-trai-ga/commit/a124134c57c6eec4326bbe1b88ba80fd8978305e).
- Kết quả kiểm tra/hồ sơ sử dụng AI: `AI_LOG.md`.
