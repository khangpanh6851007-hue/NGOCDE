# Cung Trời Hóa Lạc Ultra 2027 – Thiên Đình 3D

> README dự án – 2026

Ứng dụng web tiếng Việt mô phỏng không gian Thiên Đình, hỗ trợ ghi nhật ký việc thiện, lưu tâm nguyện, theo dõi điểm hoạt động nội bộ và xem đồng hồ – lịch Song Giới.

## ✨ Tính năng

- **Giao diện Thiên Đình:** phong cách vũ trụ, cung điện, ánh sáng và hiệu ứng chuyển động; bố cục thích ứng máy tính và điện thoại.
- **Đồng hồ Nhân gian:** hiển thị giờ và ngày dương lịch theo múi giờ Việt Nam (UTC+7), cập nhật tự động mỗi giây.
- **Đồng hồ Thiên giới:** hệ quy ước riêng gồm 12 thời thần; mỗi thời thần chia thành 100 thiên khắc và 4 thiên canh. Đây là cách hiển thị giả tưởng của ứng dụng, không phải một chuẩn đo thời gian thiên văn.
- **Lịch Thiên giới:** hiển thị ngày, tháng và năm âm lịch Việt Nam theo múi giờ UTC+7.
- **Điện Công Đức:** ghi lại việc thiện, mô tả và điểm ghi nhận nội bộ.
- **Điện Tâm Nguyện:** lưu các lời nguyện và mục tiêu cá nhân.
- **Bảng Công Đức và Phước Lộc:** tổng hợp hoạt động và huy hiệu tinh thần.
- **Hệ thống liên kết:** giữ các liên kết gốc và cho phép tài khoản quản lý thêm/xóa liên kết tùy chỉnh.
- **Trung tâm quản lý:** giao diện quản lý được mở sau khi đăng nhập tài khoản quản lý cục bộ.

## 📁 Cấu trúc phiên bản một tệp

```text
.
└── index.html   # Giao diện, CSS và JavaScript nằm trong cùng một tệp
```

## 🚀 Chạy ứng dụng

### Chạy trực tiếp

1. Tải `index.html` về máy.
2. Mở tệp bằng trình duyệt hiện đại như Chrome, Edge hoặc Firefox.
3. Cho phép JavaScript hoạt động để đồng hồ, lịch và các chức năng tương tác vận hành.

### Triển khai bằng GitHub Pages

1. Tạo hoặc mở repository trên GitHub.
2. Đưa `index.html` vào thư mục gốc của repository.
3. Đổi tên thành `index.html` nếu tệp đang có tên khác.
4. Mở **Settings → Pages**.
5. Trong **Build and deployment**, chọn **Deploy from a branch**.
6. Chọn nhánh `main` và thư mục `/(root)`, sau đó nhấn **Save**.
7. Chờ GitHub Pages triển khai và mở địa chỉ website được GitHub cung cấp.

## 💾 Dữ liệu và quyền quản lý

- Nhật ký việc thiện, tâm nguyện và liên kết tùy chỉnh được lưu bằng `localStorage` trên trình duyệt hiện tại.
- Trạng thái đăng nhập được lưu trong `sessionStorage` và hết khi phiên trình duyệt kết thúc.
- Dữ liệu cục bộ không tự đồng bộ giữa các thiết bị hoặc trình duyệt. Xóa dữ liệu website của trình duyệt có thể làm mất dữ liệu đã lưu.
- Đăng nhập quản lý trong bản một tệp là cơ chế giao diện phía trình duyệt, **không phải xác thực an toàn phía máy chủ**. Không dùng cơ chế này để bảo vệ dữ liệu nhạy cảm hoặc phân quyền cho hệ thống thực tế.
- Muốn có tài khoản an toàn, dữ liệu dùng chung nhiều thiết bị, sao lưu và phân quyền thật, cần bổ sung backend/API và cơ sở dữ liệu phù hợp.

## 🕰️ Quy ước đồng hồ Song Giới

- Đồng hồ Nhân gian dùng thời gian địa phương theo múi giờ `Asia/Ho_Chi_Minh`.
- Đồng hồ Thiên giới chia ngày thành 12 thời thần, mỗi thời thần 2 giờ; mỗi thời thần chia 100 thiên khắc và 4 thiên canh.
- Lịch âm được tính theo thuật toán lịch âm Việt Nam với múi giờ UTC+7. Nên đối chiếu nguồn lịch chuyên dụng nếu dùng cho nghi lễ hoặc mục đích cần độ chính xác cao.

## 📱 Cài đặt trên điện thoại

Có thể dùng chức năng **Thêm vào màn hình chính** hoặc **Cài đặt ứng dụng** của trình duyệt nếu trình duyệt hỗ trợ. Bản một tệp hiện tại chưa bao gồm manifest và service worker riêng; vì vậy chưa phải gói PWA hoàn chỉnh và không bảo đảm khả năng chạy ngoại tuyến sau khi đóng trình duyệt.

## 🔗 Các liên kết gốc

- [Ngọc Đế](https://khangpanh6851007-hue.github.io/Ngocdecungtroihoalac/)
- [Thiên Đình](https://khangpanh6851007-hue.github.io/ThienDinh/)
- [Làm Việc Thiện Tăng Phước Đức](https://khangpanh6851007-hue.github.io/Lamviecthien/)
- [Chuyển Luân Thánh Vương](https://khangpanh6851007-hue.github.io/ChuyenLuanThanhVuong/)
- [Thượng Ngươn Thánh Đức – Dành Cho Người Hiền Đức](https://khangpanh6851007-hue.github.io/Thuongnguonducthanhdanhchonguoihienduc/)
- [Thời Kỳ Cuối – Màn 3 Đò Chiều Chuyến Cuối](https://khangpanh6851007-hue.github.io/Man3chuyencuoidaithanhloc/)
- [Thanh Lọc Loài Người Và Linh Hồn Tà Ác](https://khangpanh6851007-hue.github.io/Thanhlocloainguoi/)

## ⚖️ Ghi chú

Ứng dụng mang tính cộng đồng và ghi chép cá nhân. Điểm Công Đức là điểm hoạt động nội bộ do ứng dụng quy ước; không xác minh hành động ngoài đời và không đại diện cho giá trị tâm linh hay đánh giá phẩm hạnh.

---

**CUNG TRỜI HÓA LẠC • ULTRA 2027**  
README dự án – 2026
