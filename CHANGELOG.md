# Nhat Ky Thay Doi (Changelog)

Tat ca cac thay doi va ban cap nhat dang chu y cua du an **SaveVault** duoc ghi lai tai tai lieu nay.

## [v1.1.0] - 2026-09-29
- 🚀 Phát hành phiên bản SaveVault v1.1.0 với nhiều tính năng và cải tiến vượt trội:
- ☁️ Sao Lưu & Khôi Phục Database Lên Cloud: Hỗ trợ sao lưu toàn bộ cơ sở dữ liệu SQLite (danh mục game, lịch sử sao lưu) lên Google Drive & OneDrive bằng công nghệ VACUUM INTO an toàn, không khóa bảng.
- 🛡️ Chính Sách Lưu Trữ Database Thông Minh (Retention Policy): Giữ tối đa 5 bản sao lưu database gần nhất, tự động xóa các bản cũ trên đám mây và làm sạch lịch sử.
- 🔄 Nâng Cấp Hệ Thống Auto-Update: Thêm cơ chế tự động Rollback hoàn tác khi gặp sự cố, cửa sổ console trực quan theo dõi tiến trình nâng cấp và độ trễ an toàn khi tắt app.
- 🎯 Cải Thiện Trải Nghiệm Giao Diện: Bổ sung hộp thoại xác nhận trước khi sao lưu/khôi phục database với màu sắc và nhãn nút chuyên biệt; sửa lỗi đè lớp z-index giữa các modal.
- ✨ Đồng Bộ Giao Diện Nút Bấm: Chuẩn hóa kích thước nút Primary trên các modal Cài đặt và Auto-Update cho trải nghiệm mượt mà, nhất quán.

## [v1.0.0] - 2026-09-28
- 🚀 Phát hành chính thức phiên bản SaveVault v1.0.0.
- 🎮 Tự động quét & tìm kiếm save game: Tích hợp thư viện offline Ludusavi 12.000+ tựa game và PCGamingWiki MediaWiki API trực tuyến.
- 💾 Sao lưu & Khôi phục 1-Click: Hỗ trợ tạo snapshot theo thời gian, nén file zip và khôi phục nguyên vẹn về thư mục gốc chỉ với 1 click.
- ☁️ Đồng bộ đám mây (Cloud Sync): Hỗ trợ Google Drive & Microsoft OneDrive qua giao thức OAuth 2.0 PKCE bảo mật.
- 🎨 Giao diện Dark Glassmorphism hiện đại: Xây dựng trên nền tảng .NET 10 & Photino Blazor siêu nhẹ và mượt mà.
- 🔄 Hệ thống Auto-Update thông minh: Tự động kiểm tra bản cập nhật, tải ngầm an toàn với cơ chế bắt lỗi toàn diện và tự khởi động lại app.

