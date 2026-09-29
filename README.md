# 🛡️ SaveVault - Game Save Manager & Cloud Vault (Portable)

<div align="center">

![SaveVault Badge](https://img.shields.io/badge/SaveVault-v1.0.0-06b6d4?style=for-the-badge&logo=shield)
![Platform](https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011%20x64-blue?style=for-the-badge&logo=windows)
![Type](https://img.shields.io/badge/Type-Portable%20--%20No%20Install-emerald?style=for-the-badge)
![Cloud](https://img.shields.io/badge/Cloud-Google%20Drive%20%7C%20OneDrive-f59e0b?style=for-the-badge)

**Ứng dụng tự động quản lý, sao lưu và đồng bộ Save Game PC lên Đám mây hàng đầu.**  
*Bảo vệ thành quả cày cuốc của bạn an toàn tuyệt đối — Chạy ngay không cần cài đặt!*

[Tải Về & Khởi Chạy](#-tải-về--khởi-chạy-cực-nhanh) • [Tính Năng Chính](#-tính-năng-nổi-bật) • [Hướng Dẫn Sử Dụng](#-hướng-dẫn-sử-dụng-nhanh) • [Đồng Bộ Đám Mây](#-đồng-bộ-đám-mây-google-drive--onedrive) • [Câu Hỏi Thường Gặp (FAQ)](#-câu-hỏi-thường-gặp--xử-lý-sự-cố-faq)

</div>

---

## ⚡ Tải Về & Khởi Chạy Cực Nhanh

SaveVault được đóng gói ở định dạng **Portable Self-Contained**, bạn **không cần cài đặt**, không cần cài thêm .NET Runtime hay phần mềm phụ trợ.

1. **Tải về**:
   - Tải file nén mới nhất tại mục [Releases](https://github.com/tuannguyen01101995/SaveVault-Publish/releases) hoặc bấm nút xanh **Code > Download ZIP**.
2. **Giải nén**:
   - Giải nén file `.zip` vào thư mục bất kỳ trên máy tính của bạn (Khuyên dùng: `D:\SaveVault` hoặc `C:\SaveVault`).
   - *Lưu ý: Tránh đặt trong thư mục `C:\Program Files` để ứng dụng có toàn quyền ghi file dữ liệu cấu hình portable mượt mà nhất.*
3. **Khởi chạy**:
   - Nhấp đúp chuột vào file **`SaveVault.exe`** ở thư mục gốc để mở ứng dụng ngay!

---

## 🎮 Tính Năng Nổi Bật

| Tính năng | Mô tả chi tiết |
| :--- | :--- |
| 🔍 **Dò tìm 12.000+ tựa game** | Tích hợp cơ sở dữ liệu offline Ludusavi khổng lồ và PCGamingWiki API, tự nhận diện vị trí lưu save của hầu hết các game Steam, Epic Games, GOG, Game Pass và game độc lập. |
| 💾 **Sao lưu 1-Click** | 1 chạm để sao lưu toàn bộ dữ liệu save vào thư mục riêng biệt. Hỗ trợ tạo mốc chơi thời gian (**Snapshot**) và nén file **ZIP** siêu tiết kiệm dung lượng. |
| 🔄 **Khôi phục an toàn (Restore)** | Phục hồi dữ liệu save ngược lại vị trí gốc của game chỉ với 1 click. Tự động tạo điểm hoàn tác dự phòng trước khi khôi phục để tránh mất mát dữ liệu. |
| ☁️ **Đồng bộ Đám mây độc lập** | Kết nối trực tiếp tài khoản **Google Drive** và **OneDrive** qua giao thức OAuth 2.0 PKCE bảo mật. Không cần cài đặt phần mềm Google Drive hay OneDrive trên máy tính. |
| 🎨 **Giao diện Dark Glassmorphism** | Thiết kế hiệu ứng kính mờ sang trọng, chuyển động vi mô mượt mà, tối ưu tài nguyên phần cứng (tiêu tốn cực ít RAM, chỉ ~40MB). |
| 🚀 **Tự động cập nhật (Auto-Update)** | Tự động kiểm tra bản cập nhật mới từ GitHub, hiển thị tiến trình tải trực quan và nâng cấp an toàn chỉ với 1 thao tác. |

---

## 📁 Cấu Trúc Thư Mục Phát Hành

Khi giải nén gói SaveVault, bạn sẽ thấy cấu trúc thư mục được tổ chức rất gọn gàng:

```text
SaveVault/
├── 🚀 SaveVault.exe                # File chạy ứng dụng (Chỉ cần nhấp đúp vào đây)
├── 📖 README.md                    # Tài liệu hướng dẫn sử dụng nhanh này
├── 📝 CHANGELOG.md                 # Nhật ký thay đổi và các điểm mới của phiên bản
├── ⚙️ version.json                 # Thông tin phiên bản phục vụ tự động cập nhật
├── ⚙️ changelogs.json              # Dữ liệu nhật ký phiên bản dùng trong ứng dụng
├── 📁 app/                         # Nhân ứng dụng và giao diện người dùng
│   └── 📖 GoogleDrive_Setup_Guide.html  # Hướng dẫn kết nối Google Drive kèm ảnh minh họa
├── 📁 data/                        # Nơi lưu trữ 100% dữ liệu của ứng dụng (Chuẩn Portable)
│   ├── backups/                    # Nơi cất giữ tất cả các bản sao lưu save game
│   ├── config/                     # Cấu hình cá nhân hóa & Token OAuth (mã hóa AES-256)
│   ├── covers/                     # Ảnh bìa game tự động tải
│   ├── database/                   # CSDL SQLite (save_backup.db) & manifest.yaml
│   ├── logs/                       # Nhật ký hoạt động hàng tháng (JSON)
│   ├── reverts/                    # Điểm hoàn tác an toàn trước khi khôi phục
│   └── temp/                       # Thư mục tạm dùng chung
│       └── auto_update/            # Gói tải về, runner script phục vụ Auto-Update
```

---

## 📖 Hướng Dẫn Sử Dụng Nhanh

### 1. Dò Tìm & Sao Lưu Save Game
1. Mở SaveVault, tại ô tìm kiếm ở màn hình chính, gõ tên tựa game bạn muốn sao lưu (Ví dụ: `Elden Ring`, `Cyberpunk 2077`, `Black Myth: Wukong`...).
2. SaveVault sẽ tự động quét ổ đĩa và hiển thị đường dẫn thư mục save thực tế trên máy của bạn kèm số lượng file và dung lượng.
3. Bấm nút **"Sao Lưu Ngay"**:
   - Bản sao lưu sẽ được tạo trong thư mục `Backups/<Tên Game>/`.
   - Bạn có thể bật tùy chọn nén `.zip` hoặc tạo snapshot mốc thời gian tại màn hình hoặc trong tab Cài Đặt.

### 2. Khôi Phục Save Game (Restore)
1. Chuyển sang tab **"Lịch Sử"**.
2. Tìm game cần khôi phục trong danh sách.
3. Nhấp vào bản sao lưu bạn muốn quay lại, sau đó bấm nút **"Khôi Phục"**.
4. SaveVault sẽ tự động giải nén và đưa toàn bộ file save về chính xác thư mục gốc của game.

---

## ☁️ Đồng Bộ Đám Mây (Google Drive & OneDrive)

Lưu trữ save game trên đám mây giúp bạn yên tâm tuyệt đối khi cài lại Windows hoặc chơi game trên nhiều máy tính khác nhau:

1. Chuyển sang tab **"Cài Đặt"** > Chọn mục **"Đồng Bộ Đám Mây"**.
2. **Với Google Drive**:
   - Nhập **Client ID** của bạn (Tạo miễn phí trên Google Cloud Console theo chuẩn Desktop App).
   - Bấm **"Kết Nối Google Drive"** -> Trình duyệt sẽ mở ra để bạn đăng nhập và cấp quyền bảo mật.
   - 📖 *Xem hướng dẫn từng bước kèm hình ảnh minh họa bằng cách mở file `app/GoogleDrive_Setup_Guide.html` hoặc bấm nút xem hướng dẫn trực tiếp trong ứng dụng.*
3. **Với OneDrive**:
   - Nhập **Client ID** từ Azure Portal cá nhân.
   - Bấm **"Kết Nối OneDrive"** và xác nhận đăng nhập tài khoản Microsoft.
4. Sau khi kết nối, tại mỗi bản sao lưu bạn có thể bấm **"Tải Lên Đám Mây"** hoặc tải xuống bất cứ lúc nào.

---

## ❓ Câu Hỏi Thường Gặp & Xử Lý Sự Cố (FAQ)

### ❓ 1. Windows SmartScreen báo *"Windows protected your PC"* khi mở `SaveVault.exe`?
- **Nguyên nhân**: SaveVault là phần mềm nguồn mở miễn phí, chưa đăng ký chứng chỉ số doanh nghiệp có phí hàng năm của Microsoft.
- **Cách xử lý**: Nhấp vào chữ **"More info"** (Thông tin khác) > Bấm nút **"Run anyway"** (Vẫn chạy). Ứng dụng hoàn toàn sạch sẽ, không chứa mã độc.

### ❓ 2. Ứng dụng có tự nhận diện game crack / repack không?
- **Có!** SaveVault hỗ trợ cơ chế phân giải đường dẫn thông minh, tự động quét các thư mục `%APPDATA%`, `%LOCALAPPDATA%`, `Saved Games`, `Documents` và các thư mục giả lập Steam phổ biến (Goldberg, CODEX, FLT, RUNE...).

### ❓ 3. Dữ liệu tài khoản đám mây của tôi có an toàn không?
- **Tuyệt đối an toàn!** SaveVault hoạt động theo cơ chế Client-Side thuần túy (không gửi bất kỳ thông tin nào về máy chủ trung gian). Mã truy cập đám mây được mã hóa chuẩn **AES-256** và chỉ lưu trên chính máy tính của bạn trong tệp `data/config/app_config.json`.

### ❓ 4. Làm thế nào để cập nhật phiên bản mới?
- Mỗi khi khởi động, nếu có bản cập nhật mới trên GitHub, SaveVault sẽ hiển thị thông báo. Bạn chỉ cần nhấn **"Cập Nhật Ngay"**, ứng dụng sẽ tự động tải gói cập nhật, kiểm tra tính toàn vẹn và nâng cấp mà không làm mất dữ liệu save hay cấu hình cũ của bạn.

---

## 💬 Hỗ Trợ & Đóng Góp Ý Kiến

- Nếu bạn gặp lỗi hoặc muốn đề xuất tựa game mới, vui lòng tạo [GitHub Issue](https://github.com/tuannguyen01101995/SaveVault-Publish/issues).
- Xem nhật ký các bản cập nhật tại [CHANGELOG.md](file:///c:/Users/TuanNguyen/Desktop/New%20folder%20%289%29/SaveVault/CHANGELOG.md).

<div align="center">

**SaveVault** — Được phát triển với niềm đam mê dành cho cộng đồng game thủ PC.  
*Chúc bạn có những giờ phút chơi game vui vẻ và an tâm trọn vẹn!*

</div>
