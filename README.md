# 🌦️ WidgetWeather.com – Hướng dẫn nhúng & sử dụng

WidgetWeather.com là một **weather widget** (tiện ích thời tiết) gọn nhẹ, dễ nhúng, phù hợp cho blog, landing page, portfolio hoặc website cá nhân.  
Dự án được phát triển và public tại GitHub.

🔗 **Repository:** https://github.com/d4m-dev/WidgetWeather.com/

---

## 📌 Mục lục

- [Giới thiệu](#giới-thiệu)
- [Cách nhúng nhanh (khuyến nghị)](#cách-nhúng-nhanh-khuyến-nghị)
- [Cấu trúc nhúng mẫu](#cấu-trúc-nhúng-mẫu)
- [Các chức năng chính của widget](#các-chức-năng-chính-của-widget)
- [Responsive & tối ưu layout](#responsive--tối-ưu-layout)
- [Xử lý lỗi & dữ liệu mẫu](#xử-lý-lỗi--dữ-liệu-mẫu)
- [Tự host & tuỳ biến nâng cao](#tự-host--tuỳ-biến-nâng-cao)
- [Lưu ý khi đưa vào production](#lưu-ý-khi-đưa-vào-production)
- [License](#license)

---

## 🌍 Giới thiệu

WidgetWeather.com cung cấp một widget hiển thị thông tin thời tiết hiện đại với giao diện dạng **card**, hỗ trợ:

- Hiển thị thời tiết hiện tại
- Thông số môi trường chi tiết
- Dự báo nhiều ngày
- Cơ chế fallback dữ liệu mẫu khi API lỗi

Widget được thiết kế để **chỉ cần 1 dòng script** là có thể sử dụng ngay.

---

## 🚀 Cách nhúng nhanh (khuyến nghị)

Chỉ cần chèn đoạn script sau vào website của bạn:

```html
<script src="https://d4m-dev.github.io/WidgetMusic.com/music-loader.js"></script>
```

👉 Khuyến nghị đặt script **ngay trước thẻ `</body>`** để tránh ảnh hưởng tốc độ render.

---

## 🧱 Cấu trúc nhúng mẫu

Ví dụ HTML đầy đủ:

```html
<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Weather Widget Demo</title>
</head>
<body>

  <h1>Website của tôi</h1>

  <!-- Weather Widget -->
  <script src="https://d4m-dev.github.io/WidgetMusic.com/music-loader.js"></script>

</body>
</html>
```

📌 Widget sẽ tự động render UI sau khi script được load.

---

## ⚙️ Các chức năng chính của widget

### 1️⃣ Thời tiết hiện tại

- 🌡️ Nhiệt độ hiện tại (°C)
- 🤔 Cảm giác như (Feels like)
- 💧 Độ ẩm (%)
- 🌬️ Tốc độ gió (km/h)
- 🔽 Áp suất khí quyển (hPa)

---

### 2️⃣ Dự báo nhiều ngày

- Hiển thị dự báo theo ngày (ví dụ: 5 ngày)
- Mỗi ngày bao gồm:
  - Nhiệt độ
  - Trạng thái thời tiết
  - Icon minh hoạ

---

### 3️⃣ Trạng thái tải & fallback

Widget hỗ trợ các trạng thái:

- ⏳ Đang tải dữ liệu
- ❌ Không thể kết nối API
- 🧪 Hiển thị **dữ liệu mẫu** khi:
  - API key hết hạn
  - Mất kết nối mạng
  - Lỗi từ nhà cung cấp thời tiết

Điều này giúp UI **không bị trống hoặc vỡ layout**.

---

## 📱 Responsive & tối ưu layout

Khuyến nghị bọc widget trong container riêng:

```html
<div class="weather-container">
  <script src="https://d4m-dev.github.io/WidgetMusic.com/music-loader.js"></script>
</div>
```

```css
.weather-container {
  max-width: 520px;
  margin: 0 auto;
  padding: 8px;
}
```

✅ Hiển thị đẹp trên mobile  
✅ Không chạm mép màn hình  
✅ Tránh vỡ layout trong flex/grid

---

## 🧯 Xử lý lỗi & dữ liệu mẫu

Nếu widget hiển thị dữ liệu mẫu hoặc thông báo lỗi:

- Kiểm tra:
  - API key (nếu có cấu hình)
  - Kết nối mạng
  - Console trình duyệt
- Đảm bảo script không bị:
  - Chặn bởi CSP
  - Cache version cũ

---

## 🛠️ Tự host & tuỳ biến nâng cao

Nếu bạn muốn:
- Tuỳ chỉnh giao diện
- Đổi API thời tiết
- Kiểm soát cache & bảo mật

👉 Hãy **fork hoặc clone repo**:

```bash
git clone https://github.com/d4m-dev/WidgetWeather.com.git
```

Sau đó:
- Chỉnh sửa file loader / UI
- Deploy lên GitHub Pages, Vercel, Netlify hoặc server riêng
- Thay URL script bằng domain của bạn

---

## 🔐 Lưu ý khi đưa vào production

- Hạn chế API key theo domain
- Cân nhắc Content Security Policy (CSP)
- Nên version hoá script (`?v=1.0.0`) để tránh cache cũ
- Không commit API key nhạy cảm lên repo public

---

## 📄 License

Vui lòng xem file **LICENSE** trong repository gốc để biết quyền sử dụng, chỉnh sửa và phân phối.

---

💡 *WidgetWeather.com – Gọn nhẹ, đẹp, nhúng nhanh trong 30 giây.*  
Chúc bạn code vui vẻ 🚀
