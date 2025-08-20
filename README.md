# Hướng dẫn cấu hình và chạy ứng dụng

## 1. Cấu hình kết nối Database

Ứng dụng sử dụng file `src/config/config.json` để cấu hình kết nối đến cơ sở dữ liệu **MySQL**.

### Ví dụ cấu hình:

```json
{
  "development": {
    "username": "root",
    "password": "<mật khẩu mysql>",
    "database": "<tên database>",
    "host": "127.0.0.1",
    "port": 3306,
    "dialect": "mysql",
    "logging": false
  }
}
```

**Lưu ý:**

- Thay thế `<mật khẩu mysql>`, `<tên database>` bằng thông tin thực tế của bạn.
- Đảm bảo MySQL đã được cài đặt và đang chạy trên máy tính của bạn.

## 2. Cài đặt package

Chạy lệnh sau trong thư mục gốc của project:

```powershell
npm install
```

## 3. Khởi động ứng dụng

Chạy lệnh:

```powershell
npm start
```

Hoặc:

```powershell
node server.js
```

## 4. Truy cập ứng dụng

Sau khi khởi động thành công, mở trình duyệt và truy cập:

```
http://localhost:3000
```

Bạn có thể thay đổi port trong file `server.js` nếu muốn.

---

Nếu gặp lỗi kết nối database, kiểm tra lại thông tin trong `src/config/config.json` và đảm bảo MySQL đang chạy trên máy của bạn.
