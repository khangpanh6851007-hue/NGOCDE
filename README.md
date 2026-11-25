# Cung Trời Hóa Lạc — GitHub Pages

Phiên bản tài liệu triển khai 2026.

## Triển khai GitHub Pages

1. Đưa `index.html` vào thư mục gốc của repository.
2. Đưa thư mục `.github/workflows/` và tệp `deploy.yml` vào repository theo đúng cấu trúc bên dưới.
3. Trên GitHub, mở **Settings → Pages**.
4. Chọn **GitHub Actions** làm nguồn triển khai.
5. Push hoặc merge thay đổi lên nhánh `main`. Workflow sẽ tự động triển khai nội dung trang web.

## Cấu trúc repository

```text
.
├── index.html
├── README.md
└── .github/
    └── workflows/
        └── deploy.yml
```

## Ghi chú

- Gói ZIP này chứa `README.md` và `deploy.yml`.
- Khi giải nén, hãy đặt `deploy.yml` vào `.github/workflows/deploy.yml`.
- Tệp `index.html` của website là tệp riêng, không nằm trong gói ZIP này.
