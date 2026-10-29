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

## 7. Hoàn thiện và tinh chỉnh giao diện (Claude Code trong VS Code)

Phần này ghi lại quá trình dùng Claude Code để rà soát và hoàn thiện tiếp bản dựng ban đầu (mục 1-6 ở trên), vẫn trong phạm vi Bài tập 1 — không phải một bài tập khác.

### 7.1. Vấn đề phát hiện khi rà soát lại mã nguồn

Sinh viên yêu cầu Claude Code đọc lại toàn bộ `index.html`, `css/style.css`, thư mục `images/`, `README.md`, `AI_USAGE.md` và kiểm tra `git status` trước khi sửa gì. AI phát hiện: tên thương hiệu trong logo ("Nhà sách Phương Nam") không khớp tên dự án ở nơi khác; nhóm Danh Mục và nhóm Bộ Lọc trong sidebar dùng chung màu nên khó phân biệt; nội dung trang bị giới hạn `max-width: 1200px`; header/banner gộp chung một khối gradient không có breadcrumb/ô tìm kiếm; 8 file SVG sản phẩm có nền pastel khác màu đóng cứng bên trong. AI cũng tra cứu nhanh 2 trang tham khảo công khai (Thiên Long, Tiki) để đối chiếu nguyên tắc phân cấp thông tin; trang Fahasa trả về lỗi truy cập (HTTP 403) nên AI không khảo sát được và đã báo rõ giới hạn thay vì giả vờ đã xem.

### 7.2. Các yêu cầu đã gửi cho AI (tóm tắt, không chép nguyên văn)

Quá trình diễn ra qua nhiều lượt trao đổi trong cùng một phiên làm việc:

1. **Lượt sửa nhỏ:** yêu cầu sửa các điểm cụ thể đã phát hiện — đổi tên thương hiệu, phân biệt màu nhóm Bộ Lọc/Danh Mục, thêm hover cho checkbox, ghi rõ "(minh hoạ)" cạnh ô sắp xếp, đổi 1 liên kết menu thành điểm neo thật.
2. **Lượt nâng cấp toàn diện:** yêu cầu AI đóng vai Senior Frontend Developer/UI-UX Designer, cải tiến (không thiết kế lại từ đầu) theo chuẩn giao diện danh mục thương mại điện tử chuyên nghiệp — mở rộng chiều rộng nội dung, tách header/nav/breadcrumb/banner, đổi màu nhãn giảm giá, đổi lưới sản phẩm sang 4 cột, xử lý nền pastel trong SVG — kèm yêu cầu không dùng JavaScript/thư viện, không tạo file mới, không tự commit/push.
3. **Lượt tinh chỉnh thêm:** sau khi xem ảnh chụp giao diện, sinh viên phản hồi hình ảnh sản phẩm còn nhỏ/nhiều khoảng trắng và yêu cầu AI xử lý; AI tính toán và thu hẹp `viewBox` của cả 8 file SVG, đồng thời đổi banner sang bố cục 2 cột và tinh chỉnh thêm cỡ chữ/khoảng cách card.
4. **Phản hồi và yêu cầu hoàn tác:** sinh viên xem kết quả của lượt 3 và đánh giá **giao diện xấu đi**, yêu cầu quay lại đúng bản của lượt 2. AI đã hoàn tác toàn bộ thay đổi của lượt 3 (khôi phục `viewBox` gốc `0 0 300 300` của cả 8 SVG, bỏ bố cục banner 2 cột, trả lại cỡ chữ/khoảng cách card như lượt 2).
5. **Lượt hiện tại:** sinh viên xác nhận chỉ đang hoàn thiện Bài tập 1 (chưa sang bài tập mới), yêu cầu rà soát và viết lại `README.md`/`AI_USAGE.md` cho đúng phạm vi, không đổi thêm giao diện.

Nội dung đầy đủ của từng yêu cầu nằm trong lịch sử trò chuyện Claude Code của phiên làm việc; đoạn tóm tắt trên phản ánh đúng các yêu cầu cốt lõi, không phải trích dẫn nguyên văn.

### 7.3. Kết quả thực tế hiện có trong mã nguồn (sau khi đã hoàn tác lượt 3)

- Header tách thành 4 phần: header xanh (logo + ô tìm kiếm minh hoạ), thanh điều hướng nền trắng, breadcrumb, banner giới thiệu danh mục.
- Biến `--container-max: 1680px` thay cho `max-width: 1200px` cũ, áp dụng cho toàn bộ container.
- Sidebar: nhóm Bộ Lọc dùng tông cam (`--color-accent`), nhóm Danh Mục dùng tông xanh dương; hover/con trỏ rõ ràng cho checkbox/radio.
- Lưới sản phẩm 4 cột ở desktop (`minmax(260px, 1fr)`), tự co giãn ở tablet/mobile.
- Product card: nền ảnh trắng, nhãn giảm giá đỏ nhạt/đỏ đậm, bo góc riêng `--radius-card: 8px`.
- Cả 8 file SVG: đã xoá dòng `<rect>` nền pastel, **vẫn giữ `viewBox="0 0 300 300"` gốc** (phần thu hẹp `viewBox` ở lượt 3 đã bị hoàn tác, không còn trong code hiện tại).

### 7.4. Phần sinh viên thực hiện

- Đọc các phân tích/đề xuất của AI và quyết định cho phép áp dụng vào mã nguồn ở từng lượt.
- Xem giao diện qua ảnh chụp màn hình thực tế gửi trong phiên làm việc; trực tiếp đánh giá kết quả lượt 3 là "xấu đi" và yêu cầu AI hoàn tác.
- Xác nhận chấp nhận giao diện ở trạng thái sau lượt 2 (trạng thái hiện tại).
- Quyết định phạm vi và nội dung cần cập nhật trong `README.md`/`AI_USAGE.md`; chưa commit/push lên GitHub.

**Lưu ý trung thực:**
- Sinh viên không tự viết code ở các lượt này — toàn bộ thao tác sửa `index.html`, `css/style.css` và `viewBox` của các file SVG đều do AI thực hiện theo yêu cầu.
- AI không có công cụ trình duyệt để tự chụp ảnh hoặc kiểm thử trực quan; AI chỉ kiểm tra cấu trúc mã nguồn (số lượng sản phẩm, ảnh, số cặp thẻ `<details>/<summary>` cân bằng, cấu trúc `<svg>` hợp lệ) bằng dòng lệnh sau mỗi lần sửa.
- Việc kiểm tra riêng ở từng kích thước màn hình cụ thể (1366px/768px/390px) bằng Chrome DevTools **chưa được xác nhận** trong phiên làm việc này; sinh viên mới xác nhận đã xem giao diện desktop qua ảnh chụp thực tế.
