# Hướng dẫn cấu hình và chạy ứng dụng

## 1. Cấu hình kết nối Database

Ứng dụng sử dụng file `src/config/config.json` để cấu hình kết nối đến cơ sở dữ liệu (MongoDB).

### Ví dụ cấu hình:

```json
{
  "development": {
    "username": "<tên người dùng mongo>",
    "password": "<mật khẩu mongo>",
    "database": "<tên database>",
    "host": "localhost",
    "dialect": "mongodb"
  }
}
```

**Lưu ý:**

- Thay thế `<tên người dùng mongo>`, `<mật khẩu mongo>`, `<tên database>` bằng thông tin thực tế của bạn.
- Nếu MongoDB không yêu cầu username/password, có thể để trống 2 trường này.

## 2. Cài đặt package

Chạy lệnh sau trong thư mục gốc của project:

```powershell
npm install
```

## 3. Khởi động ứng dụng

Chạy lệnh:

```powershell
npm run dev
```


## 4. Truy cập ứng dụng

Sau khi khởi động thành công, mở trình duyệt và truy cập:

```
http://localhost:3000
```

Bạn có thể thay đổi port trong file `server.js` nếu muốn.

---

Nếu gặp lỗi kết nối database, kiểm tra lại thông tin trong `src/config/config.json` và đảm bảo MongoDB đang chạy trên máy của bạn.
