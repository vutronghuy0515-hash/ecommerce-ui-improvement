# E-commerce UI Improvement

**Tên dự án:** Góc Văn Phòng Phẩm  
**Học phần:** Phát triển ứng dụng WEB/TMĐT – Bài tập cá nhân Chương 1

## 1. Giới thiệu

Dự án xây dựng trang giao diện mẫu cải tiến **Danh mục Văn Phòng Phẩm** dựa trên website Nhà Sách Phương Nam. Trọng tâm là tổ chức các nhóm danh mục và bộ lọc dài theo dạng **thu gọn/mở rộng**, giúp giao diện gọn gàng và dễ quan sát hơn. Đây là bài tập học tập, không phải website chính thức của Nhà Sách Phương Nam.

## 2. Website tham khảo

- **Tên website:** Nhà Sách Phương Nam.
- **URL:** https://nhasachphuongnam.com/
- **Trang tham khảo trực tiếp:** https://nhasachphuongnam.com/collections/van-phong-pham
- **Khu vực đã khảo sát:** Trang chủ, danh mục sản phẩm, chi tiết sản phẩm, tìm kiếm và giỏ hàng.
- **Khu vực được chọn cải tiến:** Danh mục Văn Phòng Phẩm.

## 3. Chức năng

- Hiển thị danh sách **8 sản phẩm mẫu** với hình ảnh, tên, giá và nút **“Xem chi tiết”**.
- Cho phép mở/đóng các nhóm danh mục bằng HTML `<details>` và `<summary>`.
- Hiển thị mô tả ngắn khi chọn **“Xem chi tiết”** trên thẻ sản phẩm.
- Bố cục sản phẩm phù hợp với màn hình máy tính và điện thoại.

**Lưu ý:** Giá bán chỉ mang tính minh họa, ảnh sản phẩm là hình SVG minh họa. Các chức năng lọc/sắp xếp (nếu có hiển thị) chưa xử lý dữ liệu thực tế; không có đăng nhập, giỏ hàng hoặc thanh toán thật.

## 4. Công nghệ

- **HTML5:** Xây dựng cấu trúc trang, danh mục, thông tin và thẻ sản phẩm.
- **CSS3:** Định dạng màu sắc, kiểu chữ, khoảng cách; sử dụng Grid/Flexbox và Media Queries để bố trí giao diện phù hợp với các kích thước màn hình.

Dự án không sử dụng JavaScript, backend, cơ sở dữ liệu hoặc thư viện giao diện.

## 5. Cách chạy

1. Mở thư mục dự án trong **Visual Studio Code**.
2. Mở file `index.html` bằng **Google Chrome** (hoặc dùng **Live Server** nếu đã cài).
3. Nhấn vào các nhóm danh mục để thử mở/đóng; thử nút **“Xem chi tiết”**.
4. Nhấn `F12` trong Chrome, bật **Toggle device toolbar** (`Ctrl + Shift + M` trên Windows) để kiểm tra giao diện máy tính và điện thoại.

Cần giữ đúng vị trí file `index.html`, `css/style.css` và thư mục `images/` để hình ảnh, định dạng hiển thị đầy đủ.

## 6. Cải tiến đã thực hiện

**Vấn đề ban đầu:** Danh sách nhóm sản phẩm và bộ lọc ở thanh bên trái trang tham khảo khá dài, khiến khách hàng có thể phải cuộn nhiều để tìm nội dung cần thiết.

**Giải pháp:** Tổ chức nhóm danh mục theo dạng thu gọn/mở rộng; sắp xếp khu vực danh mục và lưới sản phẩm rõ ràng hơn; điều chỉnh bố cục cho máy tính và điện thoại.

**Phần em tự điều chỉnh:** Sau khi mở website trên Chrome, em đã tinh chỉnh kiểu chữ, một số nội dung văn bản và kích thước bố cục nhằm giúp giao diện cân đối, dễ đọc và dễ quan sát hơn.

## 7. Hỗ trợ từ AI

- **ChatGPT:** Hỗ trợ phân tích website tham khảo, đề xuất hướng cải tiến và giải thích HTML/CSS.
- **Claude trong VS Code:** Hỗ trợ tạo mã nguồn HTML/CSS và hình minh họa dựa trên phương án đã chọn.
- **Phần em thực hiện:** Đối chiếu kết quả AI với ảnh khảo sát thực tế, kiểm tra trang web trên Chrome bằng **Chrome DevTools**, tự chỉnh sửa kiểu chữ, văn bản và bố cục; tìm hiểu vai trò của HTML `<details>`/`<summary>` và CSS trong thiết kế.

Các prompt chính, kết quả AI và quá trình kiểm tra/điều chỉnh cần được ghi riêng trong file **`AI_USAGE.md`** theo yêu cầu bài tập.
