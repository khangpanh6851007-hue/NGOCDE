# ULTRA V8 MEGA — Thế Kỷ 22

Website giao diện tiếng Việt theo phong cách thiên giới – công nghệ tương lai. Dự án được đóng gói dưới dạng **một tệp `index.html` duy nhất**, không cần cài Node.js, không cần build và có thể triển khai bằng GitHub Pages.

## Tính năng chính

- Màn hình loading 0–100% trước khi vào trang; thanh tiến trình tăng từ từ và có thời gian hiển thị tối thiểu khoảng 9 giây.
- Giao diện responsive cho điện thoại và máy tính, hiệu ứng nền sao, cung điện và các thẻ chức năng.
- Đồng hồ, lịch và các khu vực/chức năng quản lý nội dung tích hợp trong trang.
- Lưu dữ liệu phía trình duyệt bằng `localStorage` và phiên làm việc bằng `sessionStorage`.
- Có chức năng xuất/nhập dữ liệu sao lưu JSON trong giao diện.
- Khu vực mô hình 3D sử dụng Three.js tải từ CDN khi mở tính năng 3D; cần kết nối Internet để tải thư viện.

## Chạy thử trên máy

1. Tải hoặc clone repository.
2. Mở `index.html` bằng trình duyệt hiện đại.
3. Để kiểm tra giống môi trường GitHub Pages, có thể chạy bằng máy chủ tĩnh cục bộ; không cần bước build.

## Triển khai GitHub Pages

Workflow nằm tại `.github/workflows/deploy.yml`.

1. Đưa `index.html`, `README.md` và thư mục `.github/workflows/` lên repository GitHub.
2. Chọn **Settings → Pages**.
3. Trong **Build and deployment**, đặt **Source** là **GitHub Actions**.
4. Push lên nhánh `main` (hoặc `master`) hoặc chạy workflow thủ công ở tab **Actions**.
5. Sau khi workflow hoàn tất, mở URL GitHub Pages được hiển thị trong **Settings → Pages**.

Không cần khai báo framework hay lệnh build vì website là HTML tĩnh.

## Cấu trúc repository

```text
.
├── index.html
├── README.md
└── .github/
    └── workflows/
        └── deploy.yml
```

## Lưu ý về dữ liệu và bảo mật

- Dữ liệu lưu trong `localStorage` thuộc trình duyệt và thiết bị hiện tại. Xóa dữ liệu website/trình duyệt hoặc đổi trình duyệt có thể làm mất dữ liệu; hãy xuất bản sao lưu JSON định kỳ.
- Đăng nhập và phân quyền hiện tại là cơ chế chạy ở phía trình duyệt, **không phải xác thực máy chủ**. Không dùng để bảo vệ dữ liệu nhạy cảm hoặc làm hệ thống nhiều người dùng có yêu cầu bảo mật thực tế.
- Một số chức năng 3D tải Three.js từ jsDelivr nên cần Internet. Các phần HTML/CSS/JS chính được gói trực tiếp trong `index.html`.
- Tệp HTML hiện có tham chiếu tùy chọn tới `manifest.webmanifest` và đăng ký `sw.js` nếu có trên máy chủ HTTPS. Hai tệp phụ này không nằm trong gói một-file hiện tại; website chính vẫn có thể chạy như trang HTML tĩnh, còn PWA/offline service worker sẽ chưa được kích hoạt.

## Phiên bản

**ULTRA V8 MEGA — định hướng giao diện tương lai thế kỷ 22 / 2027.**
