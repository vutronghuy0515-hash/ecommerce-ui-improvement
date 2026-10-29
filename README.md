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

### 6.1. Vấn đề ban đầu

Ở bước khảo sát Nhà Sách Phương Nam, danh sách nhóm sản phẩm và bộ lọc ở thanh bên trái khá dài, khiến khách hàng có thể phải cuộn nhiều để tìm nội dung cần thiết. Giải pháp đã chọn: tổ chức danh mục theo nhóm có thể thu gọn/mở rộng bằng HTML `<details>`/`<summary>`, giữ sidebar bên trái và danh sách sản phẩm bên phải.

Khi rà soát lại mã nguồn của bản dựng đầu tiên, còn phát hiện thêm một số điểm chưa nhất quán: tên thương hiệu trong logo không khớp tên dự án ở các nơi khác trong trang; hai loại nhóm trong sidebar (Danh Mục và Bộ Lọc) dùng chung màu sắc nên khó phân biệt; nội dung trang bị giới hạn trong khung `max-width: 1200px` nên trên màn hình rộng có khoảng trống lớn hai bên; phần đầu trang (logo, menu, banner) gộp chung trong một khối nền xanh, không có breadcrumb hay ô tìm kiếm; và 8 ảnh SVG sản phẩm có một hình nền pastel cố định khác màu nhau bên trong từng file, khiến các thẻ sản phẩm trông thiếu đồng nhất.

### 6.2. Các nhóm cải tiến đã thực hiện

| Khu vực | Vấn đề | Cải tiến đã làm | Trạng thái |
|---|---|---|---|
| Header, thanh điều hướng, breadcrumb, banner | Logo, menu và banner gộp chung một khối nền xanh (gradient), không có breadcrumb, không có ô tìm kiếm | Tách thành 4 phần: header xanh (logo + ô tìm kiếm), thanh điều hướng nền trắng, breadcrumb "Trang chủ / Danh mục / Văn Phòng Phẩm", banner giới thiệu danh mục nền xanh nhạt | Đã triển khai trong `index.html`/`css/style.css` |
| Sidebar – Danh Mục và Bộ Lọc | Hai loại nhóm dùng chung màu mũi tên/nền hover xanh dương, khó phân biệt; các dòng checkbox/radio không có hiệu ứng hover | Nhóm Bộ Lọc đổi sang tông cam (`--color-accent`), nhóm Danh Mục giữ tông xanh dương; thêm hover/con trỏ rõ ràng cho từng dòng checkbox/radio | Đã triển khai, vẫn dùng `<details>`/`<summary>` thuần HTML, không JavaScript |
| Chiều rộng nội dung (container) | `max-width: 1200px` khiến nội dung bị bó hẹp trên màn hình lớn | Thêm biến `--container-max: 1680px`, áp dụng cho header, nav, breadcrumb, banner và layout chính | Đã triển khai |
| Lưới sản phẩm | Lưới dùng 1 mốc cỡ ô tối thiểu cố định, chưa tối ưu cho màn hình rộng | `grid-template-columns: repeat(auto-fill, minmax(260px, 1fr))` ở desktop (ra 4 cột khi đủ chỗ); tự co giãn còn ít cột hơn ở tablet (≤1024px, cỡ ô tối thiểu 220px) và mobile (≤640px, cỡ ô tối thiểu 150px) | Đã triển khai |
| Product card | Ảnh sát mép khung nền pastel; nhãn giảm giá màu cam dễ nhầm với các màu nhấn khác trên trang | Nền khung ảnh đổi sang trắng và có đệm quanh ảnh; nhãn giảm giá đổi sang nền đỏ nhạt/chữ đỏ đậm (`--color-sale-bg`/`--color-sale-text`); bo góc card dùng biến riêng `--radius-card: 8px` | Đã triển khai |
| 8 file SVG sản phẩm | Mỗi file có sẵn 1 hình chữ nhật nền pastel khác màu (ví dụ `#eaf2fb`, `#eafbf1`, `#fff6e8`...) đóng cứng bên trong, khiến 8 thẻ sản phẩm có 8 tông nền khác nhau dù CSS đã quy định nền chung | Xoá dòng `<rect>` nền pastel trong cả 8 file, giữ nguyên toàn bộ hình vẽ và `viewBox="0 0 300 300"` gốc | Đã triển khai; đã kiểm tra lại cả 8 file vẫn có cấu trúc `<svg>...</svg>` hợp lệ |
| Tên thương hiệu | Logo ghi "Nhà sách Phương Nam", không khớp tên dự án ở `<title>`, footer, README | Đổi logo thành "Góc Văn Phòng Phẩm" | Đã triển khai |

### 6.3. Phân biệt chức năng thật và chức năng minh hoạ

Các phần sau **chỉ mang tính minh hoạ giao diện, chưa xử lý dữ liệu thực**, có ghi chú rõ ràng trên trang:
- Ô tìm kiếm ở header (không có `<form>`/submit, placeholder và `title` ghi rõ "minh hoạ").
- Ô "Sắp xếp theo" ở khu vực sản phẩm (có chữ "(minh hoạ)" hiển thị trực tiếp cạnh nhãn, không chỉ trong `aria-label`).
- Bộ lọc Thương Hiệu/Khoảng Giá ở sidebar (có ghi chú "* Bộ lọc ở trên chỉ mang tính minh hoạ giao diện").
- Các liên kết menu "Sách", "Quà Tặng", "Liên Hệ" và danh mục con trong sidebar (có `title` báo chưa có trang tương ứng).

Các phần **có hoạt động thật**, chỉ bằng HTML/CSS, không cần JavaScript:
- Mở/đóng từng nhóm danh mục và bộ lọc bằng `<details>`/`<summary>`.
- Mở mô tả ngắn sản phẩm qua nút "Xem chi tiết" (cũng là `<details>`/`<summary>`).
- Liên kết menu "Văn Phòng Phẩm" trỏ tới điểm neo thật `#danh-sach-san-pham` ngay trong trang.

### 6.4. Giữ nguyên, không thay đổi

8 sản phẩm mẫu (tên, giá, mô tả), bảng màu chủ đạo xanh dương – trắng, font hệ thống (Segoe UI), footer, và cơ chế `<details>`/`<summary>` cho toàn bộ sidebar và nút "Xem chi tiết".

### 6.5. Kiểm tra sau khi sửa

Đã kiểm tra bằng dòng lệnh sau mỗi lần sửa: còn đủ 8 sản phẩm, 8 ảnh, 16 cặp thẻ `<details>/<summary>` cân bằng, 8 file SVG còn hợp lệ. Giao diện desktop đã được xem trực tiếp qua ảnh chụp màn hình thực tế trong quá trình làm việc và được xác nhận chấp nhận. Việc kiểm tra riêng ở kích thước tablet (768px)/mobile (390px) bằng Chrome DevTools **chưa được xác nhận cụ thể** tại thời điểm viết tài liệu này — cần tự kiểm tra trước khi coi là hoàn tất.

## 7. Hỗ trợ từ AI

- **ChatGPT:** Hỗ trợ phân tích website tham khảo, đề xuất hướng cải tiến và giải thích HTML/CSS.
- **Claude trong VS Code:** Hỗ trợ tạo mã nguồn HTML/CSS và hình minh họa dựa trên phương án đã chọn.
- **Phần em thực hiện:** Đối chiếu kết quả AI với ảnh khảo sát thực tế, kiểm tra trang web trên Chrome bằng **Chrome DevTools**, tự chỉnh sửa kiểu chữ, văn bản và bố cục; tìm hiểu vai trò của HTML `<details>`/`<summary>` và CSS trong thiết kế.

Các prompt chính, kết quả AI và quá trình kiểm tra/điều chỉnh cần được ghi riêng trong file **`AI_USAGE.md`** theo yêu cầu bài tập.
