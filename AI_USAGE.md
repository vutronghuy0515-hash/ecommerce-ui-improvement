# AI Usage Log

> **Phạm vi:** Mục 1–7 là nhật ký của **Buổi 1**. Mục 8 trở đi ghi lại **Buổi 2**, tiếp tục trên cùng website. Những đánh giá kiểm thử ở giai đoạn Buổi 1 là thông tin lịch sử, không tự động đồng nghĩa với đã kiểm thử toàn bộ bản Buổi 2.

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


---

## 8. Nhật ký dùng AI – Bài tập cá nhân Buổi 2 (theo báo cáo thực hành)

**Dữ liệu gốc:** Bản báo cáo Buổi 2 với tám prompt, kết quả Bước 1–8 và câu trả lời Mục 9 do sinh viên cung cấp. Các đoạn prompt sau chép lại từ **phần Prompt trong báo cáo** (các nhãn `[HTML - Buổi 2]`, `[CSS - Buổi 2]` là nhãn tài liệu trong báo cáo, không phải đường dẫn file mới). Không khẳng định từng ký tự trùng với lịch sử chat Claude Code nếu hai bản khác nhau.

### 8.1. Prompt Bước 1 – Rà soát mã nguồn hiện có

**Prompt ghi trong báo cáo:**

> Tôi đang làm bài tập cá nhân môn Phát triển ứng dụng thương mại điện tử. Trong Buổi 1, tôi đã khảo sát một website TMĐT và tạo một giao diện cải tiến bằng HTML/CSS.
> Đây là mã HTML hiện tại: [HTML Buổi 1]
> Đây là mã CSS hiện tại: [CSS - Buổi 1]
> Hãy giúp tôi:
> 1. Xác định những thành phần HTML đã có.
> 2. Chỉ ra các thành phần HTML còn thiếu hoặc chưa hợp lý.
> 3. Nêu ba vấn đề về cấu trúc HTML hoặc trình bày.
> 4. Đề xuất cách cải thiện bằng kiến thức HTML5 và CSS3 cơ bản.
> 5. Giải thích thứ tự nên thực hiện các cải tiến.
> Chưa viết lại toàn bộ mã nguồn.
> Không tạo website mới. Hãy giúp tôi hiểu mã hiện tại trước khi sửa.

**Kết quả và xử lý của sinh viên:** Chọn `section.products` và xác định ba vấn đề: kích thước hình ảnh, tên/giá/nút và thanh sắp xếp. Chưa viết lại trang.

### 8.2. Prompt Bước 2 – Củng cố HTML5 ngữ nghĩa

**Prompt ghi trong báo cáo:**

> Tôi đang học HTML5 và muốn cải thiện cấu trúc HTML của bài tập Buổi 1.
> Đây là mã HTML hiện tại: [HTML Buổi 1]
> Hãy hướng dẫn tôi:
> 1. Xác định các phần tử HTML đang được sử dụng.
> 2. Kiểm tra cách sử dụng header, nav, main, section, article và footer nếu có.
> 3. Kiểm tra thứ bậc tiêu đề h1, h2, h3.
> 4. Kiểm tra cách sử dụng img, alt và a.
> 5. Phát hiện các thẻ chưa đóng hoặc lồng nhau chưa hợp lý.
> 6. Đề xuất cách sửa phù hợp với nội dung hiện tại.
> Hãy phân biệt lỗi cần sửa và đề xuất cải thiện. Không thêm phần tử HTML chỉ để làm mã nguồn dài hơn. Không viết lại toàn bộ website. Giải thích lý do của từng thay đổi.

**Kết quả và xử lý của sinh viên:** Rà soát các thẻ; theo mã HTML Buổi 2, toolbar là `header.products-toolbar` và `section.products` dùng `aria-labelledby` trỏ đến `h2#tieu-de-san-pham`. Giữ tám sản phẩm.

### 8.3. Prompt Bước 3 – Kiểm tra liên kết CSS

**Prompt ghi trong báo cáo:**

> Tôi đang thực hiện Bài tập cá nhân Buổi 2 – Bước 3: Tạo và liên kết tệp CSS, môn Phát triển ứng dụng WEB/TMĐT tại UEH.
> Tôi đang tiếp tục cải tiến website Góc Văn Phòng Phẩm từ Buổi 1, sử dụng repository ecommerce-ui-improvement.
> Các bước Buổi 2 phải liên tục trên cùng dự án.
> Ở Bước 1, tôi chọn khu vực danh sách sản phẩm, với ba vấn đề:
> - Hình ảnh sản phẩm còn nhỏ so với khung ảnh.
> - Tên, giá và nút thao tác còn tương đối nhỏ.
> - Thanh sắp xếp chưa nổi bật, khoảng cách chưa cân đối.
> Ở Bước 2, tôi đã củng cố cấu trúc HTML5 của section.products và header.products-toolbar, đồng thời liên kết khu vực sản phẩm với tiêu đề h2 bằng aria-labelledby.
> BƯỚC 3 – YÊU CẦU KIỂM TRA CSS HIỆN CÓ
> Hãy đọc trực tiếp index.html và css/style.css hiện tại trong workspace.
> Kiểm tra cấu trúc thư mục dự án và xác nhận css/style.css đã tồn tại.
> Kiểm tra thẻ <link rel="stylesheet" href="css/style.css"> trong phần <head> của index.html.
> Kiểm tra các quy tắc CSS định dạng font chữ, màu chữ, màu nền và margin của body.
> Kiểm tra quy tắc áp dụng cho hình ảnh img, đặc biệt max-width và height, giải thích vì sao hình ảnh không vượt quá khung chứa.
> Chỉ ra các CSS selector hiện có liên quan đến .products, .products-toolbar, .product-grid, .product-card, .product-image, .product-info và .sort-box.
> Đối chiếu với nội dung Bước 3 của giảng viên và xác định những yêu cầu nào đã hoàn thành từ Buổi 1, những yêu cầu nào cần kiểm tra thêm.
> Hướng dẫn tôi dùng Chrome DevTools để xác nhận CSS đang được áp dụng và kiểm tra lỗi đường dẫn.
> QUY ĐỊNH QUAN TRỌNG
> Đây là dự án kế thừa từ Buổi 1, không phải website mới.
> Không tạo lại css/style.css nếu file đã tồn tại.
> Không thay thế CSS hiện tại bằng CSS ví dụ đơn giản trong đề.
> Không sửa thiết kế, màu sắc, kích thước, hình ảnh hoặc bố cục.
> Không sửa HTML đã hoàn thành ở Bước 2.
> Không dùng JavaScript, Bootstrap hay Tailwind CSS.
> Không commit hoặc push GitHub.
> Chỉ phân tích và giải thích mã nguồn thực tế; nếu phát hiện lỗi liên kết CSS, báo cho tôi trước khi sửa.
> Không tự nhận đã kiểm thử bằng Chrome nếu thực tế không có quyền truy cập trình duyệt.
> Kết quả trả về:
> Cấu trúc thư mục thực tế.
> Vị trí dòng liên kết CSS trong HTML.
> Các quy tắc font chữ, màu chữ, nền và margin đang dùng, kèm vị trí trong CSS.
> Quy tắc dành cho hình ảnh.
> Bảng đối chiếu yêu cầu Bước 3 với tình trạng hiện tại.
> Giải thích đơn giản để tôi hiểu và có thể trình bày trước giảng viên.
> Kết luận có cần sửa bất kỳ mã nguồn nào ở Bước 3 hay không, kèm lý do.
> Không tạo website mới và không tự chỉnh sửa bất kỳ file nào.

**Kết quả và xử lý của sinh viên:** Kiểm tra `css/style.css` và `<link rel="stylesheet" href="css/style.css">`; không cần tạo mới hay đổi thiết kế.

### 8.4. Prompt Bước 4 – CSS Selector và Box Model

**Prompt ghi trong báo cáo:**

> Tôi muốn thực hành CSS selector và Box Model trên một thẻ sản phẩm trong website của
> mình.
> HTML hiện tại: [HTML - Buổi 2].
> Hãy hướng dẫn tôi:
> 1. Sử dụng element selector và class selector.
> 2. Sử dụng descendant selector khi phù hợp.
> 3. Điều chỉnh margin, padding và border.
> 4. Sử dụng border-radius để bo góc.
> 5. Định dạng tên và giá sản phẩm.
> 6. Định dạng liên kết thành nút thao tác đơn giản.
> Hãy giải thích sự khác nhau giữa margin và padding.
> Giải thích tác dụng của box-sizing: border-box.
> Chỉ đưa ra phần CSS cần thiết.
> Không thay đổi nội dung hoặc tạo lại toàn bộ HTML.

**Kết quả và xử lý của sinh viên:** Claude hỗ trợ sửa 5 selector/6 khai báo: giảm padding ảnh 18→14px; tăng chữ tên/giá/nút và chỉnh padding vùng thông tin/nút. Giữ `box-sizing: border-box` và `object-fit: contain`.

### 8.5. Prompt Bước 5 – Flexbox thanh công cụ

**Prompt ghi trong báo cáo:**

> Tôi đang học CSS3 và muốn thực hành Flexbox trên một khu vực của website thương
> mại điện tử.
> Đây là HTML hiện tại: [HTML - Buổi 2].
> Hãy hướng dẫn tôi:
> 1. Xác định phần tử cha cần sử dụng display: flex.
> 2. Căn chỉnh các phần tử bằng justify-content.
> 3. Căn chỉnh theo trục còn lại bằng align-items.
> 4. Tạo khoảng cách bằng gap.
> 5. So sánh kết quả khi thay đổi các giá trị của justify-content.
> Hãy đưa ra một đoạn CSS ngắn phù hợp với HTML.
> Giải thích từng thuộc tính và kết quả mong đợi.
> Không sử dụng framework CSS.
> Không viết lại toàn bộ giao diện.

**Kết quả và xử lý của sinh viên:** Thử `justify-content: flex-start` nhưng quan sát trên Chrome thấy chưa cân đối; chọn `space-between`, `align-items: center`, `gap: 20px`, làm rõ `.sort-box` bằng nền/viền/padding.

### 8.6. Prompt Bước 6 – Grid danh sách sản phẩm

**Prompt ghi trong báo cáo:**

> Tôi đã có một danh sách sản phẩm bằng HTML.
> Đây là mã HTML hiện tại: [HTML - Buổi 2].
> Hãy hướng dẫn tôi sử dụng CSS Grid để:
> 1. Bố trí danh sách thành hai cột.
> 2. Điều chỉnh khoảng cách giữa các sản phẩm.
> 3. Giữ hình ảnh hiển thị đúng tỷ lệ.
> 4. Thay đổi số cột và quan sát kết quả.
> 5. Giải thích grid-template-columns, repeat và gap.
> 6. Giải thích tác dụng của object-fit: cover.
> Chỉ viết CSS cần thiết cho danh sách hiện có.
> Không sử dụng Bootstrap hoặc Tailwind CSS.
> Giải thích cách kiểm tra kết quả trên trình duyệt.

**Kết quả và xử lý của sinh viên:** Trên Chrome DevTools thử 2/3 cột, `gap: 16px` và `24px`; giữ `gap: 20px` và Grid tự động trong CSS gốc, không lưu thay đổi thử nghiệm.

### 8.7. Prompt Bước 7 – Hover và Focus

**Prompt ghi trong báo cáo:**

> Tôi muốn bổ sung hiệu ứng hover và focus cho một nút bấm hoặc liên kết trong website.
> Đây là HTML hiện tại: [HTML - Buổi 2].
> Đây là CSS hiện tại: [CSS - Buổi 2].
> Hãy hướng dẫn tôi:
> 1. Tạo hiệu ứng hover nhẹ.
> 2. Sử dụng transition để tạo chuyển đổi mượt.
> 3. Bổ sung focus-visible để hỗ trợ điều hướng bằng bàn phím.
> 4. Đảm bảo màu chữ và màu nền dễ nhìn.
> 5. Không làm thay đổi bố cục quá nhiều.
> Hãy chỉ đưa ra phần CSS cần thêm hoặc sửa.
> Giải thích từng thuộc tính và cách kiểm tra.

**Kết quả và xử lý của sinh viên:** Claude hỗ trợ bổ sung Hover/transition cho card, ảnh và nút; dùng media query phù hợp thiết bị và giảm chuyển động. `summary:focus-visible` đã có sẵn nên không nhận là thêm mới.

### 8.8. Prompt Bước 8 – AI hỗ trợ kiểm tra thay đổi độc lập

**Prompt ghi trong báo cáo:**

> Tôi đã hoàn thành một phần giao diện website TMĐT bằng HTML5 và CSS3.
> Đây là mã nguồn:
> HTML hiện tại: [HTML - Buổi 2].
> CSS hiện tại: [CSS - Buổi 2 - New].
> Tôi nhận thấy vấn đề sau:
> Khi kiểm tra giao diện ở chiều rộng 390px bằng Chrome DevTools, tôi nhận thấy hình ảnh sản phẩm trong các thẻ khá nhỏ, chưa thực sự nổi bật.
> Hãy giúp tôi:
> 1. Xác định nguyên nhân có thể gây ra lỗi.
> 2. Chỉ ra thuộc tính hoặc phần tử cần kiểm tra.
> 3. Đề xuất cách sửa ít thay đổi nhất.
> 4. Giải thích vì sao cách sửa có thể giải quyết vấn đề.
> 5. Đề xuất cách kiểm tra sau khi sửa.
> Không viết lại toàn bộ mã nguồn.
> Phân biệt nguyên nhân đã xác định và giả thuyết cần kiểm tra.

**Kết quả và xử lý của sinh viên:** Sinh viên tự thêm `@media (max-width: 390px) { .product-image { padding: 5px; } }` (từ 14px), giữ hai cột. Claude chỉ xem CSS và phân tích cascade/box model, không chỉnh sửa thêm. Kiểm tra trực quan sau sửa và bàn phím/chuột chưa được chứng thực đầy đủ trong báo cáo.

## 9. Những đề xuất AI đã được kiểm tra hoặc điều chỉnh

| Bước | Nội dung AI hỗ trợ | Phần sinh viên kiểm tra/quyết định |
|---|---|---|
| 2–4 | Kiểm tra cấu trúc HTML và đề xuất điều chỉnh kích thước vùng ảnh, thông tin | Giữ nguyên nội dung tám sản phẩm; chỉ tiếp tục chỉnh khu vực đã chọn |
| 5 | Đề xuất/thử phương án căn Flexbox | Thử `flex-start` trên Chrome nhưng không chọn; dùng `space-between` vì cân đối hơn |
| 6 | Hướng dẫn thử Grid hai/ba cột, các giá trị `gap` | Tự thao tác trên DevTools, quan sát rồi **không lưu** CSS thử nghiệm |
| 7 | Claude bổ sung hiệu ứng Hover | Giữ lại quy tắc Focus-visible đã có, không thêm thừa |
| 8 | Claude phân tích đề xuất tự sửa vùng ảnh | Sinh viên **tự** giảm padding 14→5px tại ≤390px; Claude kiểm tra mã nguồn và không sửa lại |

**Phân biệt kiểm tra:** Phân tích quy tắc CSS không tương đương với việc kiểm tra trực tiếp trên Chrome. Bản báo cáo vẫn ghi **Chưa xác minh** đối với chất lượng hình ảnh sau sửa, thao tác liên kết/chi tiết và Hover/Focus nếu chưa có kiểm thử trực tiếp. Không ghi các chức năng tìm kiếm, lọc, sắp xếp là xử lý dữ liệu thật.

## 10. Prompt 9 – Hỗ trợ cập nhật README để nộp Buổi 2

**Mục đích yêu cầu:** Giữ nguyên lịch sử Buổi 1; cập nhật README ngắn gọn theo bảy mục của giảng viên: giới thiệu bài tập; website/khu vực tham khảo; kỹ thuật HTML5/CSS3; cách chạy; các thay đổi Buổi 2; AI và cách kiểm tra; liên kết repository/Pages.

**Kết quả:** Tạo lại README và nhật ký AI dựa trên báo cáo Buổi 2; không sửa `index.html`, `css/style.css`, không thay đường dẫn ảnh, không tự commit hoặc push. Việc cập nhật GitHub cần thực hiện và xác nhận riêng.
