# E-link Web Controller

Giao diện **v2** gọn, dễ dùng — đầy đủ chức năng từ [XLY95/xly95.github.io](https://github.com/XLY95/xly95.github.io).

## Tính năng

| Tab | Mô tả |
|-----|--------|
| **Trang chủ** | Kết nối BLE, đồng bộ giờ, đổi đồng hồ/lịch, cài đặt nâng cao (gập) |
| **Đếm ngược** | Chọn ngày, nhập chữ, gửi lên màn hình |
| **Ảnh** | Tải ảnh, dithering, gửi E-Paper |
| **Thiết kế** | Canvas thiết kế mẫu |

## Cấu trúc

```
elink-web/
  index.html          # Giao diện v2
  css.css             # Style mới (+ legacy cho tab ảnh/thiết kế)
  app.js              # Logic BLE & xử lý ảnh
  legacy-styles.css   # Style nền cho editor/ảnh
  index-haiau-backup.html  # Bản giao diện cũ (haiau)
```

## Chạy local

```bash
cd elink-web
python -m http.server 8080
```

Mở http://localhost:8080 — **Ctrl+F5** sau khi cập nhật.

## Lưu ý

- Chrome/Edge trên máy tính; iOS dùng **Bluefy**
- Thiết bị `DLG-CLOCK-*`
- Múi giờ **0** nếu máy đúng giờ Việt Nam
