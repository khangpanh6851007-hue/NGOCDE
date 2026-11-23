# Cung Trời Hóa Lạc Ultra 2027 — V5 LOCAL

Website tĩnh chạy trực tiếp trên trình duyệt, gồm 18 điện chức năng, khu vực Thiên Đình 3D, tài khoản nhiều cấp và lưu trữ cục bộ.

## 1. Tệp triển khai

- `index.html`: trang web chính (dùng bản `index_ultra2027_v5_local.html` đổi tên thành `index.html`).
- `manifest.webmanifest`: cấu hình PWA.
- `sw.js`: service worker.
- `.github/workflows/deploy.yml`: tự động triển khai lên GitHub Pages.

## 2. Đưa mã nguồn lên GitHub

1. Tạo một repository trên GitHub.
2. Tải các tệp nêu trên lên thư mục gốc repository.
3. Đổi tên `index_ultra2027_v5_local.html` thành `index.html`.
4. Tạo thư mục `.github/workflows/` và đặt `deploy.yml` vào trong đó.
5. Vào **Settings → Pages** và chọn **GitHub Actions** làm Build and deployment source.
6. Đẩy commit lên nhánh `main` (hoặc `master`). Workflow sẽ tự chạy và xuất bản website.

## 3. Lưu ý quan trọng

- Đây là bản **LOCAL**: dữ liệu, tài khoản và hoạt động lưu trong `localStorage` của trình duyệt/thiết bị. Dữ liệu không tự đồng bộ giữa các thiết bị và không có máy chủ/backend.
- Xóa dữ liệu trình duyệt hoặc đổi trình duyệt có thể làm mất dữ liệu. Hãy dùng chức năng **Điện Sao Lưu** để xuất JSON định kỳ.
- Cơ chế băm SHA-256 chạy ở phía trình duyệt không phải xác thực an toàn phía máy chủ. Không dùng để lưu dữ liệu nhạy cảm hoặc làm hệ thống quản trị công khai.
- Mô hình 3D tải Three.js và OrbitControls từ CDN, vì vậy cần kết nối internet để tải thư viện.
- PWA cần được phục vụ qua HTTPS (GitHub Pages đáp ứng điều kiện này).
- Không đưa mật khẩu, token hoặc khóa bí mật vào repository.

## 4. Triển khai thủ công

Nếu không dùng GitHub Actions, bật GitHub Pages cho nhánh và thư mục chứa `index.html`, `manifest.webmanifest`, `sw.js`.

## 5. Phiên bản

**V5 LOCAL — Ultra 2027**  
Bản này giữ dữ liệu trên thiết bị hiện tại; không có Cloud Sync.
