# 📌 Hướng Dẫn Khôi Phục Database và Kết Nối Với ASP.NET

## 📋 Yêu Cầu
✅ **SQL Server Management Studio 19** (SSMS 19) - Phiên bản bắt buộc để đảm bảo tương thích.
✅ **SQL Server** đã được cài đặt và chạy trên hệ thống của bạn.
✅ **ASP.NET Project** sẵn sàng để kết nối với database.

---

## 🛠️ Hướng Dẫn Khôi Phục Database
1. 📥 **Tải file database backup** (`.bak`) từ repository này.
2. 🔍 **Mở SQL Server Management Studio 19** và kết nối với server của bạn.
3. 🏗️ **Tạo một database mới** (hoặc sử dụng database có sẵn nếu phù hợp).
4. 🔄 **Thực hiện khôi phục database**:
   - Nhấp chuột phải vào **Databases** > **Restore Database**.
   - Chọn **Device** > **Browse...** và tìm đến file `.bak` đã tải về.
   - Nhấn **OK** và kiểm tra lại thông tin trước khi khôi phục.
   - Nhấn **OK** để bắt đầu quá trình restore.

---

## 🔗 Kết Nối Database Với ASP.NET
1. ✍️ **Cập nhật chuỗi kết nối** trong `appsettings.json` hoặc `Web.config`:
   ```json
   "ConnectionStrings": {
       "DefaultConnection": "Server=YOUR_SERVER;Database=YOUR_DATABASE;User Id=YOUR_USERNAME;Password=YOUR_PASSWORD;"
   }
   ```
   Hoặc sử dụng Windows Authentication:
   ```json
   "ConnectionStrings": {
       "DefaultConnection": "Server=YOUR_SERVER;Database=YOUR_DATABASE;Trusted_Connection=True;"
   }
   ```
2. ▶️ **Chạy ứng dụng ASP.NET** và kiểm tra kết nối database.

---

💡 Nếu gặp lỗi hoặc cần hỗ trợ, vui lòng mở một issue trên repository này. 🚀

