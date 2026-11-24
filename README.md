# Cung Trời Hóa Lạc Ultra 2027 — V7 MEGA

Website tĩnh viết bằng HTML, CSS và JavaScript thuần. Phiên bản V7 MEGA có giao diện chủ đề Thiên Đình, các khu chức năng cá nhân và lưu trữ dữ liệu cục bộ trên trình duyệt.

## Tính năng chính

- 24 điện/chức năng được hiển thị trong giao diện.
- Đồng hồ Nhân gian, Thiên giới và lịch âm Việt Nam (UTC+7).
- Nhật ký việc thiện, tâm nguyện, nhiệm vụ, điểm nội bộ và huy hiệu.
- Lịch sự kiện, ghi chú cá nhân, thành tựu và nhắc nhở.
- Tìm kiếm chức năng và dữ liệu ghi chú/sự kiện.
- Giao diện thích ứng cho điện thoại và máy tính.
- Không gian Thiên Đình 3D WebGL; thư viện Three.js cần tải từ CDN khi mở chức năng 3D.
- Xuất/nhập dữ liệu sao lưu JSON (nếu trình duyệt hỗ trợ tải tệp).
- Khu vực đăng nhập/quản lý cục bộ và phân quyền giao diện.
- Các liên kết website liên quan, bao gồm Đức Huỳnh Giáo Chủ.

## Cấu trúc triển khai

Đặt `index.html` ở thư mục gốc của repository. Workflow GitHub Actions cần được lưu đúng đường dẫn:

```text
.
├── index.html
├── README.md
└── .github/
    └── workflows/
        └── deploy.yml
```

## Triển khai lên GitHub Pages

1. Tạo hoặc mở repository GitHub của dự án.
2. Tải phiên bản website muốn phát hành lên repository và đặt tên chính xác là `index.html` ở thư mục gốc.
3. Tạo thư mục `.github/workflows/` nếu chưa có.
4. Đặt workflow tải kèm trong repository tại `.github/workflows/deploy.yml`.
5. Vào **Settings → Pages**.
6. Trong **Build and deployment → Source**, chọn **GitHub Actions**.
7. Commit và push các thay đổi lên nhánh `main`.
8. Mở tab **Actions**, chờ workflow `Deploy to GitHub Pages` chạy thành công.
9. Địa chỉ website được hiển thị tại **Settings → Pages**.

Mỗi lần push thay đổi lên `main`, workflow sẽ tự triển khai lại.

## Chạy thử trên máy

Có thể mở `index.html` trực tiếp trong trình duyệt để xem các chức năng cơ bản. Để kiểm tra gần với môi trường hosting, nên chạy qua máy chủ HTTP cục bộ, ví dụ:

```bash
python -m http.server 8000
```

Sau đó mở `http://localhost:8000`.

## Lưu trữ và giới hạn bảo mật

**Đây là ứng dụng frontend tĩnh.** Dữ liệu người dùng được lưu trong `localStorage`/`sessionStorage` của trình duyệt và thiết bị hiện tại; dữ liệu không tự đồng bộ sang thiết bị khác.

Màn hình đăng nhập và phân quyền trong bản local chỉ phục vụ trải nghiệm/demo phía trình duyệt. Không dùng để bảo vệ dữ liệu nhạy cảm hoặc quản trị website công khai. Muốn có tài khoản thực, xác thực an toàn, phân quyền đáng tin cậy, chat cộng đồng và đồng bộ nhiều thiết bị, cần xây dựng backend/API và cơ sở dữ liệu, đồng thời chuyển việc xác thực sang máy chủ.

Thông báo nhắc việc trên trình duyệt phụ thuộc quyền thông báo và trạng thái hoạt động của trang/trình duyệt; không đảm bảo gửi đúng giờ khi trang đã đóng.

Chức năng 3D cần WebGL và kết nối mạng để tải thư viện Three.js từ CDN. Thiết bị hoặc trình duyệt không hỗ trợ WebGL có thể không hiển thị được cảnh 3D.

## Website liên kết

- Đức Huỳnh Giáo Chủ (Huỳnh Phú Sổ): https://khangpanh6851007-hue.github.io/Duchuynhgiaochuhuynhphuso/

## Phiên bản

- Tên phiên bản giao diện: **V7 MEGA 2027**
- Loại dự án: Website tĩnh (HTML/CSS/JavaScript)
- Triển khai đề xuất: GitHub Pages bằng GitHub Actions

## Giấy phép

Chưa khai báo giấy phép mã nguồn. Nếu muốn cho phép người khác sử dụng, chỉnh sửa hoặc phân phối dự án, hãy bổ sung tệp `LICENSE` với giấy phép phù hợp.
