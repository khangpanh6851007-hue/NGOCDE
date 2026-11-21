# ✨ Cung Trời Hóa Lạc

Trang web giao diện tối ưu cho thiết bị di động (**Mobile Chuẩn**), tích hợp đồng hồ & lịch thời gian thực, mục **Sấm Truyền Thiên Đình**, danh sách liên kết nhanh đến các phân trang trên GitHub Pages, hiệu ứng nền sao lấp lánh / pháo hoa khi chạm màn hình, màn hình đăng nhập chính và trình quản lý liên kết tùy chỉnh lưu bằng `localStorage`.

---

## 🌟 Tính Năng Chính

* **Màn hình đăng nhập chính:** Khóa truy cập đầu vào với tài khoản mặc định và hỗ trợ đăng xuất (`sessionStorage`).
* **Đồng hồ & Lịch nhân gian:** Cập nhật giờ phút giây và thứ/ngày/tháng/năm tự động mỗi giây.
* **Sấm Truyền Thiên Đình:** Rút ngẫu nhiên câu sấm truyền kèm hiệu ứng chuông âm thanh (khi bật âm thanh).
* **Danh sách liên kết nhanh:** Truy cập trực tiếp các trang liên quan trên GitHub Pages (mở ở tab mới `target="_blank"`):
  * 👑 **Ngọc Đế** — `https://khangpanh6851007-hue.github.io/Ngocdecungtroihoalac/`
  * 🏛️ **Thiên Đình** — `https://khangpanh6851007-hue.github.io/ThienDinh/`
  * 🌱 **Làm Việc Thiện Tăng Phước Đức** — `https://khangpanh6851007-hue.github.io/Lamviecthien/`
  * 🫅 **Chuyển Luân Thánh Vương** — `https://khangpanh6851007-hue.github.io/ChuyenLuanThanhVuong/`
  * ☸️ **Thượng Ngươn Thánh Đức - Dành Cho Người Hiền Đức** — `https://khangpanh6851007-hue.github.io/Thuongnguonducthanhdanhchonguoihienduc/`
  * 🌐 **Thời Kỳ Cuối - Màn 3 Đò Chiều Chuyến Cuối** — `https://khangpanh6851007-hue.github.io/Man3chuyencuoidaithanhloc/`
  * 🔥 **Thanh Lọc Loài Người Và Linh Hồn Tà Ác** — `https://khangpanh6851007-hue.github.io/Thanhlocloainguoi/`
* **Quản lý liên kết tùy chỉnh:** Thêm mới liên kết kèm tên, URL, bảng màu nút và xóa liên kết đã thêm (lưu cục bộ trên trình duyệt qua `localStorage`).
* **Tùy biến giao diện & tương tác:**
  * Chuyển đổi 3 giao diện màu nền (`Mặc định`, `theme-gold`, `theme-teal`).
  * Bật/tắt chuông âm thanh Web Audio API.
  * Chạm vào vùng trống trên màn hình để bắn pháo hoa trên `<canvas>`.

---

## 🛠️ Công Nghệ Sử Dụng

* **HTML5** & **CSS3** (CSS Variables, Flexbox, Glassmorphism, Responsive Mobile)
* **JavaScript (Vanilla JS)** (`sessionStorage`, `localStorage`, Web Audio API, HTML5 Canvas)
* **GitHub Pages** để xuất bản trực tiếp

---

## 🚀 Triển Khai Trên GitHub Pages

1. Tải file `index.html` lên repository GitHub của bạn.
2. Vào **Settings** → **Pages**.
3. Tại mục **Build and deployment** → **Branch**, chọn nhánh chính (thường là `main` hoặc `master`) và thư mục `/ (root)`, sau đó bấm **Save**.
4. Chờ vài phút để GitHub build và truy cập theo đường dẫn GitHub Pages của repository.

---

## ⚠️ Lưu Ý Bảo Mật & Vận Hành

* Vì ứng dụng chạy hoàn toàn ở phía trình duyệt (**client-side**, không có backend/database máy chủ), thông tin đăng nhập và mật khẩu quản lý nằm trong mã nguồn phía client. Chỉ nên dùng để phân luồng/khóa giao diện cơ bản, không dùng cho dữ liệu nhạy cảm cao.
* Các liên kết thêm mới chỉ lưu trên trình duyệt của thiết bị hiện tại (`localStorage`); nếu xóa dữ liệu trình duyệt hoặc đổi máy, danh sách liên kết tùy chỉnh sẽ không tự đồng bộ.

---

## 📝 Ghi Chú Phiên Bản (2026)

* Hoàn thiện vòng lặp vẽ hạt sao và hiệu ứng pháo hoa trên `<canvas>`.
* Bổ sung màn hình đăng nhập chính và nút đăng xuất.
* Thêm liên kết **Thanh Lọc Loài Người Và Linh Hồn Tà Ác**.
