# Nhat Ky Thay Doi (Changelog)

Tat ca cac thay doi va ban cap nhat dang chu y cua du an **SaveVault** duoc ghi lai tai tai lieu nay.

## [v1.1.1] - 2026-09-29
- 🛠️ Bản vá lỗi nóng (Hotfix v1.1.1) khắc phục sự cố Auto-Updater:
- ⚡ Khắc Phục Lỗi Dừng Cửa Sổ Cập Nhật: Sửa triệt để lỗi cú pháp phân tích lệnh batch (update_runner.bat) khiến cửa sổ console dừng lại ở lệnh 'pause' dù cập nhật đã hoàn tất thành công 100% (Exit code: 0).
- 🚀 Tự Động Khởi Chạy Mượt Mà: Cửa sổ cập nhật tự động đóng tức thì sau khi hoàn tất chép đè và khởi động lại SaveVault mà không cần người dùng phải bấm phím thủ công.
- 🛡️ Tối Ưu An Toàn Tiến Trình: Tinh gọn cơ chế kiểm tra mã thoát (Exit code) và bảo toàn tính năng giữ lại cửa sổ để tra cứu lỗi chỉ khi gặp sự cố thực tế.

## [v1.1.0] - 2026-09-29
- 🚀 Phát hành phiên bản SaveVault v1.1.0 với nhiều tính năng và cải tiến vượt trội:
- ☁️ Sao Lưu & Khôi Phục Database Lên Cloud: Hỗ trợ sao lưu toàn bộ cơ sở dữ liệu SQLite (danh mục game, lịch sử sao lưu) lên Google Drive & OneDrive bằng công nghệ VACUUM INTO an toàn, không khóa bảng.
- 🛡️ Chính Sách Lưu Trữ Database Thông Minh (Retention Policy): Giữ tối đa 5 bản sao lưu database gần nhất, tự động xóa các bản cũ trên đám mây và làm sạch lịch sử.
- 🔄 Nâng Cấp Hệ Thống Auto-Update: Thêm cơ chế tự động Rollback hoàn tác khi gặp sự cố, cửa sổ console trực quan theo dõi tiến trình nâng cấp và độ trễ an toàn khi tắt app.
- 🎯 Cải Thiện Trải Nghiệm Giao Diện: Bổ sung hộp thoại xác nhận trước khi sao lưu/khôi phục database với màu sắc và nhãn nút chuyên biệt; sửa lỗi đè lớp z-index giữa các modal.
- ✨ Đồng Bộ Giao Diện Nút Bấm: Chuẩn hóa kích thước nút Primary trên các modal Cài đặt và Auto-Update cho trải nghiệm mượt mà, nhất quán.

## [v1.0.0] - 2026-09-29
- 🎉 Phát hành phiên bản khởi đầu SaveVault v1.0.0:
- 📦 Tự động nhận diện và sao lưu file save game từ nhiều nền tảng (Steam, Epic, Ubisoft, GOG,...).
- 🔒 Hỗ trợ nén zip và mã hóa AES-256 an toàn.
- ☁️ Đồng bộ đám mây và giao diện quản lý hiện đại với .NET 10 MAUI Blazor Hybrid.

