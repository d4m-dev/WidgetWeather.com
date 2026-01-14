🌤️ Weather Widget Pro

Widget dự báo thời tiết hiện đại, tự động nhận diện vị trí và hiển thị dự báo 5 ngày. Thiết kế Responsive, đẹp mắt trên cả máy tính và điện thoại.

🚀 Demo

Xem trực tiếp tại: https://d4m-dev.github.io/WidgetWeather.com/

📦 Cách nhúng vào Website

Bạn có thể nhúng widget này vào bất kỳ trang web nào (WordPress, Blogspot, Landing Page...) chỉ với 1 dòng code.

Cách 1: Sử dụng Server của d4m-dev (Khuyên dùng)

Copy dòng mã sau và dán vào nơi bạn muốn hiển thị widget trên trang web của bạn:

<script src="[https://d4m-dev.github.io/WidgetWeather.com/widget-loader.js](https://d4m-dev.github.io/WidgetWeather.com/widget-loader.js)"></script>


Cách 2: Tự Host (Nâng cao)

Nếu bạn muốn tải code về và tự upload lên host của mình:

Tải toàn bộ source code về.

Đổi tên file widget chính thành weather.html (hoặc giữ nguyên index.html).

Sửa file widget-loader.js, thay đổi biến defaultUrl thành đường dẫn đến file html của bạn.

Nhúng file .js vào trang web đích.

✨ Tính năng chính

📍 Tự động định vị (Geolocation):

Hỏi quyền truy cập vị trí người dùng để hiển thị thời tiết chính xác tại nơi họ đang đứng.

Nếu người dùng từ chối, tự động chuyển về vị trí mặc định (Hồ Chí Minh).

📅 Dự báo 5 ngày:

Hiển thị chi tiết nhiệt độ, icon thời tiết cho 5 ngày tiếp theo.

Giao diện: Dạng cột dọc bên phải (Desktop) hoặc danh sách dọc phía dưới (Mobile).

📱 Responsive (Tương thích di động):

PC: Hiển thị dạng thẻ ngang (Card), kích thước gọn gàng.

Mobile: Tự động chuyển sang dạng dọc, tối ưu cho màn hình cảm ứng.

🛡️ Fallback thông minh:

Nếu API Key hết hạn hoặc lỗi mạng, widget sẽ tự động chuyển sang hiển thị Dữ liệu mẫu (Sample Data) thay vì bị vỡ giao diện.

🛠️ Cấu trúc thư mục

index.html (hoặc weather.html): File giao diện chính.

widget-loader.js: Script giúp nhúng widget vào trang web khác (tạo iframe, auto-resize).

README.md: Tài liệu hướng dẫn.

⚙️ Tùy chỉnh API

Mặc định widget sử dụng API Key miễn phí từ OpenWeatherMap. Để ổn định hơn, bạn nên thay bằng key của riêng mình:

Mở file index.html.

Tìm dòng const API_KEY = '...'.

Thay thế bằng Key của bạn.
