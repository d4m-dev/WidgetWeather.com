# 🌤️ Widget Weather

**Widget Weather** là một tiện ích hiển thị thời tiết thời gian thực với thiết kế tối giản (minimalist), hiện đại. Công cụ này được tối ưu hóa để nhúng vào Notion, Obsidian, GitHub Profile hoặc bất kỳ trang web cá nhân nào.



## ✨ Tính năng chính

* **Dữ liệu thời gian thực:** Cập nhật nhiệt độ, tình trạng thời tiết và độ ẩm chính xác.
* **Thiết kế Responsive:** Tự động điều chỉnh kích thước để phù hợp với mọi bố cục (sidebar, full-width).
* **Tùy biến cao:** Hỗ trợ thay đổi giao diện (Dark/Light mode) và ngôn ngữ.
* **Siêu nhẹ:** Tải nhanh, không gây ảnh hưởng đến hiệu suất trang web chính.

---

## 🚀 Hướng dẫn Nhúng (Integration)

Bạn có thể nhúng widget này thông qua `iframe` vào bất kỳ nền tảng nào hỗ trợ HTML.

### 1. Nhúng vào HTML / Website cá nhân

Copy đoạn mã dưới đây và dán vào nơi bạn muốn hiển thị widget:

```html
<iframe 
  src="[https://widgetweather.com/?city=Hanoi&lang=vi&theme=dark](https://widgetweather.com/?city=Hanoi&lang=vi&theme=dark)"
  width="100%" 
  height="200" 
  frameborder="0" 
  scrolling="no"
  style="border-radius: 12px; box-shadow: 0 4px 14px rgba(0,0,0,0.1);">
</iframe>
```

### 2. Nhúng vào Notion / Obsidian

Để widget hiển thị đẹp nhất trên các công cụ ghi chú này, hãy làm theo các bước sau:

1.  **Sao chép URL widget** với các tham số bạn muốn (ví dụ: thành phố Đà Nẵng, ngôn ngữ tiếng Việt):
    `https://widgetweather.com/?city=DaNang&lang=vi&theme=auto`
2.  **Dán (Paste)** đường dẫn vừa copy vào trang Notion hoặc Obsidian.
3.  Chọn tùy chọn **"Create Embed"** (Tạo bản nhúng) trong menu hiện ra.
4.  **Điều chỉnh kích thước:** Kéo các cạnh của khung widget để mở rộng chiều ngang hoặc chiều dọc cho phù hợp với giao diện của bạn.

---

## ⚙️ Bảng tham số tùy chỉnh (Configuration)

Bạn có thể tùy biến widget bằng cách thêm các tham số vào sau đường dẫn URL gốc (Query Parameters). Dưới đây là danh sách đầy đủ các tham số được hỗ trợ:

| Tham số | Mô tả | Giá trị mặc định | Ví dụ |
| :--- | :--- | :--- | :--- |
| `city` | Tên thành phố bạn muốn xem thời tiết (Viết liền, không dấu). | `Hanoi` | `?city=HoChiMinh` |
| `lang` | Ngôn ngữ hiển thị thông tin. | `en` | `?lang=vi` (Tiếng Việt) |
| `theme` | Chế độ màu sắc giao diện. | `auto` | `?theme=dark` hoặc `?theme=light` |
| `units` | Đơn vị đo nhiệt độ. | `metric` | `?units=metric` (°C) hoặc `?units=imperial` (°F) |
| `bg` | Màu nền tuỳ chỉnh (Mã Hex, bỏ dấu #). | `transparent` | `?bg=000000` |

### 💡 Mẹo cấu hình (Pro Tips)
* **URL kết hợp:** Để có một widget hoàn chỉnh cho người Việt, hãy dùng chuỗi sau:
    > `https://widgetweather.com/?city=Hanoi&lang=vi&units=metric&theme=dark`
* **Nền trong suốt:** Mặc định widget có nền trong suốt để hòa vào màu nền website của bạn. Nếu muốn đặt màu riêng, hãy dùng tham số `bg`.

---

## 🛠️ Đóng góp & Hỗ trợ (Support)

Dự án này được phát triển mã nguồn mở. Chúng tôi rất hoan nghênh mọi ý kiến đóng góp từ cộng đồng.

* **Báo lỗi (Bug Report):** Nếu widget không hiển thị hoặc sai thông tin, vui lòng mở một [Issue mới](https://github.com/d4m-dev/WidgetWeather.com/issues).
* **Đóng góp tính năng:** Hãy Fork dự án và gửi Pull Request.

**Credits:**
Developed with ❤️ by [d4m-dev](https://github.com/d4m-dev).
