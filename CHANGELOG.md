# Nhat Ky Thay Doi (Changelog)

Tat ca cac thay doi va ban cap nhat dang chu y cua du an **SaveVault** duoc ghi lai tai tai lieu nay.

## [v1.2.0] - 2026-09-29
- 🚀 Phát hành phiên bản SaveVault v1.2.0 với nhiều tính năng mới và nâng cấp trải nghiệm:
- ℹ️ Bổ Sung Tab Thông Tin & Hỗ Trợ: Thêm tab chuyên biệt ngoài cùng bên phải thanh điều hướng sv-nav-bar, tích hợp cơ chế nạp tĩnh trực tiếp vào mã nguồn lúc build (Zero Disk I/O) giúp mở tức thì không tốn tài nguyên ổ đĩa.
- 📜 Xem Nhật Ký Phiên Bản: Thêm nút tra cứu lịch sử changelog trực tiếp tại card Phiên bản & Cập nhật trong Cài đặt với giao diện timeline trực quan.
- ☁️ Tối Ưu Thanh Dung Lượng Cloud: Sửa triệt để lỗi thanh dung lượng OneDrive bị tràn 100% khi còn trống và bổ sung khả năng nạp hạn mức chính xác cho Google Drive bằng Custom Credentials.
- ⚙️ Tinh Gọn Cấu Hình Google Drive: Lược bỏ chế độ 1-Click rườm rà và nút gạt Dev switch, tập trung trải nghiệm kết nối ổn định với Client ID & Client Secret riêng.
- 🎯 Cải Thiện Giao Diện & Danh Sách Game: Chuẩn hóa kích thước khung danh sách sv-listbox (min 200px - max 300px), khắc phục dứt điểm lỗi tràn layout dropdown gợi ý game.

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
- 🛠️ Bản vá lỗi nóng (Hotfix v1.1.1) khắc phục sự cố Auto-Updater:
- ⚡ Khắc Phục Lỗi Dừng Cửa Sổ Cập Nhật: Sửa triệt để lỗi cú pháp phân tích lệnh batch (update_runner.bat) khiến cửa sổ console dừng lại ở lệnh 'pause' dù cập nhật đã hoàn tất thành công 100% (Exit code: 0).
- 🚀 Tự Động Khởi Chạy Mượt Mà: Cửa sổ cập nhật tự động đóng tức thì sau khi hoàn tất chép đè và khởi động lại SaveVault mà không cần người dùng phải bấm phím thủ công.
- 🛡️ Tối Ưu An Toàn Tiến Trình: Tinh gọn cơ chế kiểm tra mã thoát (Exit code) và bảo toàn tính năng giữ lại cửa sổ để tra cứu lỗi chỉ khi gặp sự cố thực tế.

