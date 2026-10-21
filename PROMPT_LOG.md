# NHẬT KÝ PROMPT ENGINEERING (VIBE CODING LOG)
- **Họ và tên:** Lương Duy Thuận
- **MSSV:** 125000352
- **Tên đề tài Website:** Landing Page giới thiệu Game "Black Myth: Wukong"
- **Công cụ AI đã sử dụng:** Gemini, ChatGPT (Codex)
## 1. Yêu cầu ban đầu (System/Initial Prompt)
> *Ghi lại prompt tổng quan ban đầu bạn dùng để khởi tạo khung website.*

Bạn là một Senior Front-end Developer chuyên thiết kế các Landing Page game hoành tráng, hiện đại và chuẩn SEO. Hãy viết mã nguồn cho một Landing Page giới thiệu game "Black Myth: Wukong" bao gồm 2 file riêng biệt: index.html và style.css (External CSS) tuân thủ chặt chẽ các quy chuẩn kỹ thuật sau:

1. Cấu trúc HTML (Semantic HTML5):
Sử dụng đầy đủ và chuẩn xác tối thiểu 5 thành phần Semantic HTML5:

<header>: Chứa logo game, khẩu hiệu (tagline) và thanh điều hướng.

<nav>: Thanh điều hướng nằm trong header chứa các link liên kết (Trang chủ, Cốt truyện, Tính năng, Thư viện ảnh, Mua ngay).

<main>: Khu vực nội dung chính chứa các section bên dưới.

<section> / <article>: Chia rõ ràng các khối nội dung (Hero Section, About Section, Features Section, Gallery Section).

<footer>: Chân trang chứa thông tin bản quyền (Copyright), liên kết mạng xã hội và thông tin nhà phát hành.

2. CSS & Styling (style.css - External CSS):

Liên kết bên ngoài qua thẻ <link rel="stylesheet" href="style.css">.

CSS Variables: Khai báo và sử dụng hệ thống biến tại :root để quản lý đồng bộ màu sắc mang phong cách mộng mị, cổ phong huyền bí của Wukong (--primary-color, --bg-color, --text-color, --accent-color), font chữ, spacing và transition.

Bố cục (Layout): Sử dụng kết hợp CSS Flexbox và CSS Grid để căn chỉnh responsive cơ bản trên Desktop và Mobile.

## 2. Quá trình tinh chỉnh & Giải quyết sự cố (Iteration Iterations)
### Lần 1: Dựng khung Semantic HTML & CSS Variable
- **Prompt đã dùng:**

Role: Bạn là một Senior Front-end Developer chuyên thiết kế các Landing Page game hoành tráng, hiện đại và chuẩn SEO.
Nhiệm vụ: Hãy viết mã nguồn cho một Landing Page giới thiệu game "Black Myth: Wukong" bao gồm 2 file riêng biệt: index.html và style.css (External CSS) tuân thủ chặt chẽ các quy chuẩn kỹ thuật sau:
1. Yêu cầu Cấu trúc HTML (Semantic HTML5):
File index.html phải sử dụng đầy đủ và chuẩn xác tối thiểu 5 thành phần Semantic HTML5:
- <header>: Chứa logo game, khẩu hiệu (tagline) và thanh điều hướng.
- <nav>: Thanh điều hướng nằm trong header chứa các link liên kết (Trang chủ, Cốt truyện, Tính năng, Thư viện ảnh, Mua ngay).
- <main>: Khu vực nội dung chính chứa các section bên dưới.
- <section> / <article>: Chia rõ ràng các khối nội dung:
  - Hero Section: Banner hoành tráng giới thiệu tên game, nút Call-to-Action (CTA) "Đặt Hàng Ngay" / "Xem Trailer".
  - About Section (<article>): Giới thiệu cốt truyện và cảm hứng từ Tây Du Ký.
  - Features Section: Danh sách tính năng nổi bật (Đồ họa Unreal Engine 5, Hệ thống chiến đấu linh hoạt, Boss hoành tráng) trình bày dạng thẻ (Card layout).
  - Gallery Section: Lưới hình ảnh/video demo game.
- <footer>: Chân trang chứa thông tin bản quyền (Copyright), các liên kết mạng xã hội và thông tin liên hệ/nhà phát hành (Game Science).
2. Yêu cầu CSS & Styling (style.css - External CSS):
- File CSS được liên kết bên ngoài qua thẻ <link rel="stylesheet" href="style.css">.
- CSS Variables: Khai báo và sử dụng hệ thống biến tại :root để quản lý đồng bộ:
  - Màu sắc mang phong cách mộng mị, cổ phong huyền bí của Wukong (Ví dụ: --primary-color vàng kim/đồng, --bg-color tối/đen xám, --text-color trắng/xám sáng, --accent-color đỏ thẫm/cam lửa).
  - Font chữ (Google Fonts phong cách mạnh mẽ/cổ điển).
  - Spacing & Transition (Khoảng cách padding, margin, thời gian hiệu ứng ứng mượt mà).
- Bố cục (Layout): Sử dụng kết hợp CSS Flexbox (cho Header, Navigation, Footer) và CSS Grid (cho Features Card và Gallery) để giao diện căn chỉnh responsive cơ bản trên Desktop và Mobile.
- Hiệu ứng: Có hiệu ứng hover chuyển màu/phóng to nhẹ cho các nút CTA, thẻ tính năng và ảnh gallery.
Đầu ra mong muốn:
1. Trả về mã nguồn file index.html đầy đủ, chuẩn chỉnh.
2. Trả về mã nguồn file style.css riêng biệt, chỉn chu, có chú thích rõ ràng.

- **Kết quả AI tạo ra:** ...
- **Nhận xét & Tinh chỉnh của SV:** (Ví dụ: AI xài thẻ <div> nhiều quá, đã
nhắc AI sửa lại thành <main> và <section>).
### Lần 2: Tích hợp thư viện Animate.css & AOS
- **Prompt đã dùng:**

ROLE & MỤC TIÊU: Bạn là một Senior Front-end Developer. Hãy cập nhật và mở rộng mã nguồn dự án Landing Page game "Black Myth: Wukong" (bao gồm file index.html và style.css) bằng cách bổ sung các thư viện tương tác, hiệu ứng cuộn trang và hiệu ứng phản hồi người dùng (micro-interactions) theo đúng các yêu cầu kỹ thuật chi tiết dưới đây.
TƯƠNG TÁC & HIỆU ỨNG (LIBRARIES & CSS EFFECTS)
A. Tích hợp Animate.css (Hiệu ứng xuất hiện ngay khi tải trang):
1. Nhúng thư viện: Bổ sung đường link CDN bản mới nhất của Animate.css vào bên trong thẻ <head> của file index.html.
2. Áp dụng hiệu ứng: Gắn các class tương ứng của Animate.css vào các thành phần quan trọng trong Hero Section:
   - Tiêu đề chính (Main Title - "Black Myth: Wukong"): Sử dụng hiệu ứng animate__animated animate__fadeInDown hoặc animate__backInDown để tiêu đề xuất hiện ấn tượng từ trên xuống.
   - Đoạn mô tả / Tagline: Sử dụng animate__animated animate__fadeIn với khoảng hoãn nhẹ để hiển thị mượt mà sau tiêu đề.
   - Nút bấm Call-to-Action (CTA): Sử dụng animate__animated animate__zoomIn kết hợp với hiệu ứng nhịp đập lặp lại animate__pulse animate__infinite (hoặc hiệu ứng thu hút chú ý tương tự) giúp kích thích người dùng click "Đặt Hàng Ngay" hoặc "Xem Trailer".
B. Tích hợp AOS - Animate On Scroll (Hiệu ứng khi cuộn trang):
1. Nhúng thư viện:
   - Thêm link CDN CSS của AOS (Animate On Scroll) vào thẻ <head>.
   - Thêm link CDN JS của AOS ngay trước thẻ đóng </body>.
   - Thêm đoạn mã JavaScript khởi tạo ở cuối trang:
     HTML
     <script>
       AOS.init({
         duration: 1000, // Thời gian chạy hiệu ứng (ms)
         once: true,     // Hiệu ứng chỉ chạy 1 lần khi cuộn qua
         offset: 120     // Khoảng cách bắt đầu kích hoạt hiệu ứng
       });
     </script>
2. Gắn hiệu ứng vào các Section:
   - About Section (<article>): Áp dụng data-aos="fade-right" cho khối hình ảnh và data-aos="fade-left" cho khối nội dung văn bản cốt truyện.
   - Features Section (Danh sách tính năng): Gắn data-aos="fade-up" cho các thẻ bài viết (Feature Cards). Sử dụng thuộc tính data-aos-delay="100", data-aos-delay="200", data-aos-delay="300" cho từng thẻ nối tiếp để tạo hiệu ứng xuất hiện gợn sóng (staggered animation) sinh động.
   - Gallery Section (Thư viện hình ảnh/video): Gắn data-aos="zoom-in" hoặc data-aos="flip-left" cho từng khung ảnh demo.
   - Footer: Gắn data-aos="fade-up" để chân trang xuất hiện êm ái khi cuộn đến cuối.
C. Hiệu ứng :hover & :focus tự viết bằng External CSS (style.css):
1. Nút bấm (Buttons / CTA):
   - Trạng thái :hover:
     - Thay đổi màu nền (background-color) sang tông màu sáng hơn hoặc chuyển sắc (gradient).
     - Thêm dải hiệu ứng phát sáng mộc mạc/huyền bí xung quanh nút bằng box-shadow (ví dụ: box-shadow: 0 0 15px var(--accent-color)).
     - Dịch chuyển nhẹ nút lên trên với transform: translateY(-3px).
     - Đảm bảo có thuộc tính transition: all 0.3s ease; để chuyển động mịn màng.
   - Trạng thái :focus / :focus-visible:
     - Hiển thị viền outline rõ ràng (ví dụ: outline: 2px solid var(--primary-color); outline-offset: 4px;) nhằm hỗ trợ tốt nhất cho người dùng điều hướng bằng phím Tab (Accessibility/a11y).
2. Các thẻ bài viết & Khung hình ảnh (Cards & Gallery Items):
   - Trạng thái :hover:
     - Khung thẻ nhẹ nhàng nâng lên (transform: translateY(-8px) hoặc scale(1.03)).
     - Đổi màu viền (border-color) sang màu kim loại vàng/đồng (var(--primary-color)).
     - Đổ bóng phần chân thẻ (box-shadow: 0 10px 20px rgba(0,0,0,0.5)).
     - Nếu thẻ có chứa hình ảnh, hình ảnh bên trong sẽ phóng to nhẹ (transform: scale(1.1)) nhờ thuộc tính overflow: hidden trên khung chứa.
ĐẦU RA MONG PHẢI ĐẠT ĐƯỢC:
1. File index.html hoàn chỉnh: Đã liên kết đầy đủ các CDN (Animate.css, AOS CSS, AOS JS), thẻ Semantic HTML5 giữ nguyên, các thuộc tính data-aos và class Animate.css được đặt chính xác vào đúng các vị trí.
2. File style.css hoàn chỉnh: Chứa đầy đủ biến :root, bố cục Flexbox/Grid và các quy tắc CSS tùy chỉnh chi tiết cho hiệu ứng :hover, :focus, :active cũng như hiệu ứng hình ảnh mượt mà.

- **Thách thức gặp phải:** (Ví dụ: AOS không chạy khi cuộn trang).
- **Cách sửa prompt (Debug prompt):** ...
## 3. Đánh giá cá nhân về quá trình Vibe Coding
- AI đã giúp bạn tiết kiệm thời gian ở phần nào nhất?
=> Viết mã nguồn thô (Boilerplate Code): AI giúp khởi tạo cực kỳ nhanh cấu trúc khung trang HTML5, khai báo đầy đủ các thẻ Semantic (<header>, <nav>, <main>, <section>, <footer>) và tạo sẵn danh sách biến CSS Variables (:root) chỉ trong vài giây.

- Bài học rút ra khi đặt câu hỏi (Prompt) cho AI trong thiết kế web?
=> Càng chi tiết, kết quả càng chính xác: Đặt prompt mang tính chiến lược theo quy trình từng bước (Step-by-step) thay vì viết một yêu cầu chung chung. Phân chia rõ ràng giữa cấu trúc HTML, styling CSS và các hiệu ứng JS/Thư viện sẽ giúp AI sinh code chuẩn xác ngay từ đầu.
