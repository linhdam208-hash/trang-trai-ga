# Website Trang Trại Gà Quang Linh (QL FARM)

Phiên bản hoàn thiện: **v3 - Bản chốt bàn giao A3**  
Website tĩnh giới thiệu trang trại, ba nhóm sản phẩm, quy trình chăn nuôi, bảng giá và form đặt hàng.

- Sinh viên thực hiện: **Đàm Quang Linh**
- Mã sinh viên: **2071020117**
- Lớp / Ngành: **CNTT 20-04 / Công nghệ thông tin**
- Giảng viên hướng dẫn: **ThS. Lê Thái Bảo**
- Học phần: Thiết kế Web và Triển khai Hệ thống Phần mềm (FIT4014)

## 1. Thông tin sản phẩm

**Website Trang Trại Gà Quang Linh (QL FARM)** được xây dựng bằng HTML5 và CSS3, phù hợp với mục đích giới thiệu sản phẩm nông nghiệp và mô phỏng luồng đặt hàng trên website tĩnh.

## 2. Triển khai GitHub

- GitHub Repository — điền URL: `https://github.com/linhdam208-hash/trang-trai-ga`
- GitHub Pages công khai — điền URL sau khi kích hoạt: `https://linhdam208-hash.github.io/trang-trai-ga/`
- Nguồn xuất bản: nhánh `main`, thư mục `/ (root)`
- Phiên bản: **v3 (Bản chốt bàn giao A3)**
- Trạng thái cấu hình Pages: kiểm tra và cập nhật thực tế trong mục Checklist trước khi nộp.

## 3. Tính năng chính

- HTML5 Semantic: `header`, `nav`, `main`, `section`, `article`, `figure`, `table` và `footer`.
- Responsive Mobile-First tại 320px, 640px và 960px.
- Danh mục 3 sản phẩm dạng Card: gà ta thả vườn, trứng gà ta thảo dược, gà Đông Tảo.
- Bảng giá dùng Semantic `table` với `thead`, `tbody`, `th scope` và khả năng cuộn ngang an toàn.
- Form HTML5 hỗ trợ `required`, `minlength`, `maxlength`, `email` và gửi phương thức `GET` tới `ket-qua.html`.
- Liên kết neo điều hướng theo từng khu vực của trang chủ.
- Trạng thái `:focus-visible` cho liên kết, nút và trường nhập liệu.

## 4. Chạy tại Local

Yêu cầu: Git và Python 3 hoặc server tĩnh tương đương.

```powershell
git clone https://github.com/linhdam208-hash/trang-trai-ga.git
cd trang-trai-ga
python -m http.server 8080
```

Mở `http://localhost:8080/index.html`. Có thể mở trực tiếp tệp HTML nhưng server local giúp kiểm tra đường dẫn tương đối và luồng form chính xác hơn.

## 5. Cây thư mục thực tế

```text
trang-trai-ga/
├── index.html
├── ket-qua.html
├── README.md
├── CHANGELOG.md
├── RELEASE_NOTES.md
├── AI_LOG.md
├── css/
│   └── style.css
├── assets/
│   └── images/
│       ├── ga-dong-tao.jpg
│       ├── ga-tha-vuon.jpg
│       ├── trang-trai.jpg
│       └── trung-ga.jpg
└── docs/
    └── evidence-index.md
```

## 6. Kiểm tra trang và chức năng

- Điều hướng neo: nhấp từng mục trong thanh menu và xác nhận cuộn đúng `id`.
- Responsive: thử 320px, 640px và 960px bằng DevTools; kiểm tra menu wrap, Card và bảng không tràn.
- Tab: dùng phím Tab và xác nhận các liên kết, nút, trường nhập có `focus-visible`.
- Form rỗng: bỏ trống tất cả rồi gửi; trình duyệt phải báo trường bắt buộc.
- Form sai: nhập họ tên dưới 2 ký tự, email sai định dạng hoặc nội dung dưới 10 ký tự; các trường tương ứng phải không hợp lệ.
- Form đúng: nhập dữ liệu hợp lệ, gửi và xác nhận chuyển tới `ket-qua.html` kèm tham số `fullname`, `email`, `message`.
- Liên kết trở lại: kiểm tra brand và nút “Quay về trang chủ” tại trang kết quả.

## 7. Hồ sơ bàn giao và giới hạn kỹ thuật

- [CHANGELOG.md](CHANGELOG.md)
- [RELEASE_NOTES.md](RELEASE_NOTES.md)
- [AI_LOG.md](AI_LOG.md)
- [Bảng minh chứng A3](docs/evidence-index.md)

Giới hạn: đây là website tĩnh; form mô phỏng luồng gửi bằng `GET` tới `ket-qua.html`, không lưu dữ liệu và không có CSDL/backend. Trang kết quả không hiển thị lại dữ liệu đã gửi.

## 8. Nguồn tài nguyên và khai báo AI

- Mã nguồn website: dự án cục bộ và repository GitHub nêu trên.
- Hình ảnh: các tệp trong `assets/images/` do dự án hiện có cung cấp.
- AI hỗ trợ: Gemini và GitHub Copilot được sử dụng để kiểm tra/rà soát tài liệu, đối chiếu mã và đề xuất nội dung. Sinh viên giữ trách nhiệm cuối cùng về tính chính xác, tự kiểm chứng trên trình duyệt/DevTools và không chèn dữ liệu nhạy cảm.
