# Hồ sơ số Trường Mầm non

> **Triển khai cho:** Trường Mầm non Diễn Thịnh — Nghệ An
> 🌐 https://schoolrecords.github.io/mamnondienthinh

Website quản lý hồ sơ số cho trường mầm non.
Dữ liệu đồng bộ tự động từ Google Sheet qua Google Apps Script.

## Tính năng

- 6 nhóm Hồ sơ số với liên kết tới Google Drive
- Quản lý CBGV, danh sách trẻ, lớp học
- Hệ thống KĐCL - TĐG: 5 Tiêu chuẩn × 22 Tiêu chí (theo TT 22/2024)
- Báo cáo Tự đánh giá theo 7 bước (CV 5942/BGDĐT-QLCL)
- Trang quản trị: cập nhật cấu hình, mật khẩu, dữ liệu trực tiếp trên web
- Responsive cho cả máy tính và điện thoại

## Cấu trúc 4 file

- `index.html` — Giao diện + dữ liệu seed (tiêu chuẩn, tiêu chí, minh chứng)
- `style.css` — Style (responsive desktop + mobile)
- `app.js` — Logic frontend (render, CRUD, gọi API)
- `README.md` — Tài liệu này

## Triển khai cho 1 trường mới

1. Copy 4 file của template sang repository riêng của trường
2. Tạo Google Sheet từ template, nhập thông tin trường
3. Triển khai Google Apps Script (`Code.gs`) → lấy URL Web App `/exec`
4. Dán URL vào hằng `API_URL` ở gần cuối `index.html`
5. Bật GitHub Pages cho repository → web hoạt động

## Cấu hình ban đầu

Vào trang Admin (nút ⚙ Admin trên thanh điều hướng):

- Cập nhật tên trường, địa chỉ, điện thoại, email, hiệu trưởng, bản đồ
- Đổi mật khẩu Admin (mặc định `admin@2026`)
- Bổ sung link Google Drive cho từng đầu mục hồ sơ

## Căn cứ pháp lý

- Thông tư 19/2018/TT-BGDĐT (sửa đổi bởi TT 22/2024/TT-BGDĐT)
- Công văn 5942/BGDĐT-QLCL ngày 28/12/2018
- Nghị định 13/2023/NĐ-CP (bảo vệ dữ liệu cá nhân)
- Nghị định 30/2020/NĐ-CP (định dạng văn bản hành chính)

## Tác giả

Thiết kế bởi **Chung Trần**
