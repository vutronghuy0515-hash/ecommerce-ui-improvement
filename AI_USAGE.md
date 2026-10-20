# AI Usage Log

## 1. Công cụ AI

- **ChatGPT (OpenAI):** Hỗ trợ phân tích website, đề xuất phương án cải tiến giao diện và giải thích kiến thức HTML/CSS.
- **Claude Code (Anthropic) trong Visual Studio Code:** Hỗ trợ xây dựng mã nguồn và giao diện mẫu bằng HTML5/CSS3 theo phương án đã lựa chọn.

## 2. Mục đích sử dụng

Sử dụng AI để hỗ trợ khảo sát giao diện website **Nhà Sách Phương Nam** (https://nhasachphuongnam.com/), phân tích năm khu vực gồm trang chủ, danh mục sản phẩm, chi tiết sản phẩm, tìm kiếm và giỏ hàng. Từ kết quả khảo sát, lựa chọn cải tiến **Danh mục Văn Phòng Phẩm** bằng cách tổ chức các nhóm danh mục và bộ lọc theo dạng có thể thu gọn hoặc mở rộng. AI cũng được sử dụng để đề xuất bố cục, hỗ trợ viết HTML5/CSS3 và giải thích các thành phần mã nguồn.

## 3. Prompt đã sử dụng

### Prompt 1 – Phân tích website (ChatGPT)

> Bạn là chuyên gia phân tích nghiệp vụ và thiết kế trải nghiệm người dùng cho website thương mại điện tử.
>
> Tôi đang khảo sát website: Nhà sách Phương Nam https://nhasachphuongnam.com/
>
> Hãy giúp tôi lập bảng phân tích các khu vực:
> 1. Trang chủ.
> 2. Danh mục sản phẩm.
> 3. Chi tiết sản phẩm.
> 4. Tìm kiếm.
> 5. Giỏ hàng.
>
> Với mỗi khu vực, hãy nêu:
> - Mục đích của chức năng.
> - Thành phần giao diện cần có.
> - Điểm thuận tiện đối với khách hàng.
> - Một vấn đề có thể phát sinh.
> - Một đề xuất cải tiến.
>
> Không khẳng định những tính năng chưa được kiểm chứng.
> Phân biệt rõ nhận xét dựa trên quan sát và đề xuất của AI.

### Prompt 2 – Đề xuất giao diện (ChatGPT)

> Tôi đang thực hiện bài tập phát triển giao diện website thương mại điện tử bằng HTML5 và CSS3.
>
> Tôi muốn cải tiến khu vực: Danh mục sản phẩm.
>
> Đối tượng sử dụng: khách hàng mua sắm trực tuyến tại Việt Nam.
>
> Hãy đề xuất:
> 1. Bố cục giao diện
> 2. Các thành phần HTML cần sử dụng.
> 3. Cách tổ chức CSS.
> 4. Cách hiển thị trên máy tính và điện thoại.
> 5. Những điểm cần kiểm tra về khả năng sử dụng.
>
> Trước tiên, hãy giải thích phương án thiết kế. Chưa tạo toàn bộ mã nguồn cho đến khi tôi yêu cầu.

### Prompt 3 – Yêu cầu tạo mã nguồn (nội dung ghi trong báo cáo Nhiệm vụ 3)

> Dựa trên phương án đã thống nhất, hãy tạo một trang giao diện thương mại điện tử bằng HTML5 và CSS3.
>
> Yêu cầu:
> - Giao diện có tiêu đề và khu vực sản phẩm.
> - Có tối thiểu 4 sản phẩm mẫu.
> - Mỗi sản phẩm có hình ảnh, tên, giá và nút thao tác.
> - Bố cục phù hợp với màn hình máy tính và điện thoại.
> - Mã HTML có cấu trúc rõ ràng.
> - CSS được tách thành file riêng.
> - Không sử dụng backend hoặc cơ sở dữ liệu.
> - Không đưa thư viện hoặc thành phần không cần thiết vào dự án.
>
> Giải thích cách chạy trang web và những phần tôi cần kiểm tra.

**Lưu ý về bản ghi prompt:** Prompt 3 được chép theo nội dung đang có trong báo cáo. Nếu prompt chi tiết thực tế đã gửi Claude Code khác với đoạn trên, cần bổ sung nguyên văn từ lịch sử trò chuyện Claude trước khi nộp để phản ánh đúng quá trình sử dụng AI.

## 4. Kết quả AI đề xuất

ChatGPT đề xuất chia giao diện danh mục thành hai khu vực: thanh danh mục/bộ lọc bên trái và danh sách sản phẩm bên phải. Các nhóm danh mục sử dụng HTML `<details>` và `<summary>` để mở hoặc thu gọn. CSS Grid được đề xuất để bố trí danh sách sản phẩm; CSS được tách riêng và thiết kế để hiển thị phù hợp với màn hình máy tính và điện thoại.

Dựa trên phương án đã chọn, Claude Code hỗ trợ xây dựng trang mẫu **Góc Văn Phòng Phẩm** với 8 sản phẩm minh họa, gồm hình ảnh, tên, giá và nút xem thông tin. Trang được xây dựng bằng HTML5/CSS3, không có backend, cơ sở dữ liệu hoặc chức năng thanh toán thực tế. Bộ lọc giá, thương hiệu và sắp xếp chủ yếu mang tính minh họa giao diện, không xử lý lọc dữ liệu thực.

## 5. Kiểm tra và điều chỉnh

Sau khi nhận kết quả phân tích từ AI, em đã đối chiếu với website Nhà Sách Phương Nam qua việc quan sát và chụp màn hình các khu vực. Em điều chỉnh nhận xét về trang chủ vì website đã có khu vực truy cập nhanh theo danh mục; đồng thời phát hiện thông tin **thương hiệu** và **nhà cung cấp** ở một số trang chi tiết sản phẩm chưa được trình bày thống nhất. Ở khu vực tìm kiếm, em quan sát trang kết quả khi nhập từ khóa “hay”; ở giỏ hàng, em kiểm tra cách hiển thị sản phẩm và tổng tiền. Những nhận xét không phù hợp với trải nghiệm quan sát được đã được loại bỏ hoặc thay đổi.

Đối với trang giao diện tự xây dựng, em đã mở bằng Google Chrome, sử dụng **Chrome DevTools** để xem bố cục ở kích thước máy tính và điện thoại, kiểm tra hình ảnh và nội dung. Em cũng tự tinh chỉnh **kiểu chữ, một số thông tin văn bản và kích thước bố cục** để trang rõ ràng và cân đối hơn. Chrome DevTools là công cụ dùng để kiểm tra giao diện, không phải công nghệ viết mã nguồn.

## 6. Phần em hiểu và có thể giải thích

- **`index.html` và HTML5:** Tổ chức các phần như tiêu đề, thanh danh mục, bộ lọc, danh sách và thông tin sản phẩm. Việc chỉnh sửa nội dung HTML giúp thông tin hiển thị rõ ràng, đúng mục đích.
- **`<aside>`:** Chứa thanh danh mục và khu vực bộ lọc ở bên trái.
- **`<details>` và `<summary>`:** Cho phép mở/thu gọn nhóm danh mục bằng chức năng có sẵn của HTML, không cần JavaScript.
- **`<article>` và `<img>`:** Tổ chức từng thẻ sản phẩm và hiển thị hình minh họa sản phẩm.
- **`css/style.css` và CSS3:** Quy định kiểu chữ, màu sắc, khoảng cách, kích thước và cách bố trí các thành phần. Các thay đổi về kiểu chữ và kích thước bố cục được thực hiện thông qua CSS.
- **CSS Grid:** Sắp xếp thanh danh mục và khu vực sản phẩm thành các cột; bố trí các thẻ sản phẩm theo dạng lưới.
- **Responsive và Chrome DevTools:** CSS quyết định cách bố cục thay đổi theo kích thước màn hình; Chrome DevTools giúp em mô phỏng và kiểm tra kết quả trên máy tính, điện thoại. Việc kiểm tra bằng DevTools khác với việc trực tiếp viết hoặc chỉnh sửa quy tắc `@media` trong CSS.

Qua quá trình thực hiện, AI được sử dụng để hỗ trợ phân tích và tạo mã nguồn ban đầu; các nội dung khảo sát, đánh giá và điều chỉnh được kiểm tra lại trước khi đưa vào bài tập.
