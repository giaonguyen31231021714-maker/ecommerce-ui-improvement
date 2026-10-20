# AI Usage Log

## 1. Công cụ AI
- **Tên công cụ:** Gemini (Google)

## 2. Mục đích sử dụng
- Phân tích nghiệp vụ (BA) và trải nghiệm người dùng (UX) trên website thương mại điện tử thực tế (Hasaki.vn).
- Đề xuất phương án cải tiến bố cục trang chủ nhằm giảm nhiễu thị giác và tối ưu hiển thị Responsive.
- Khởi tạo khung mã nguồn giao diện bằng HTML5 chuẩn ngữ nghĩa, CSS3 (Grid/Flexbox/Variables) và Vanilla JavaScript.


## 3. Prompt đã sử dụng
1. **Prompt 1 (Khảo sát & Phân tích UX):**
   "Tôi đang khảo sát website: Hasaki Beauty & Clinic - https://hasaki.vn/. Hãy giúp tôi lập bảng phân tích các khu vực: Trang chủ, Danh mục sản phẩm, Chi tiết sản phẩm, Tìm kiếm, Giỏ hàng..."
2. **Prompt 2 (Đề xuất phương án cải tiến Trang chủ):**
   "Tôi muốn cải tiến khu vực Trang chủ vì mật độ thông tin/banner quá dày gây nhiễu thị giác... Hãy đề xuất: Bố cục, Thành phần HTML, Cách tổ chức CSS, Cách hiển thị Responsive, Usability checklist..."
3. **Prompt 3 (Sinh mã nguồn HTML/CSS/JS):**
   "Dựa trên phương án đã thống nhất, hãy tạo một trang giao diện thương mại điện tử bằng HTML5 và CSS3... Giải thích cách chạy trang web và những phần tôi cần kiểm tra."*


## 4. Kết quả AI đề xuất
- **Bảng phân tích BA/UX:** Đưa ra cái nhìn tổng quan về mục đích, UI, ưu điểm, hạn chế và đề xuất cụ thể cho 5 khu vực cốt lõi của Hasaki.vn.
- **Phương án kiến trúc bố cục:** Thiết lập nguyên tắc phân cấp thị giác "1 Hero Banner chủ đạo + Quick Links" và giao diện cuộn ngang (Horizontal Scroll) cho di động.
- **Mã nguồn hoàn chỉnh:** Cung cấp file HTML tích hợp CSS3/JS có tính tương tác cao (bộ đếm Flash Sale, chuyển Tab danh mục, Bottom Navigation Bar trên Mobile).

## 5. Kiểm tra và điều chỉnh
- **Kiểm tra (Verification):** 
  - Đã chạy kiểm thử mã nguồn trên trình duyệt Chrome và kiểm tra hiển thị đa thiết bị qua Developer Tools (F12 Mobile Emulation).
  - Xác minh tính chính xác của các thẻ HTML5 Semantic (`<header>`, `<nav>`, `<main>`, `<article>`, v.v.).
- **Điều chỉnh (Adjustments):**
  - Kiểm tra và tinh chỉnh khoảng cách `padding`, `margin` và kích thước nút bấm đạt chuẩn tối thiểu 44x44px trên giao diện Mobile.
  - Chuẩn bị phương án tách đoạn mã CSS từ thẻ `<style>` trong file HTML ra tập tin `style.css` độc lập phục vụ việc nộp bài tập.
- **Điểm không sử dụng:**
  - Không áp dụng các framework/thư viện bên ngoài (như Bootstrap, Tailwind, jQuery) theo đúng yêu cầu tự viết CSS/JS thuần của bài tập.

## 6. Phần tôi hiểu và có thể giải thích
- **HTML5 Semantic:** Giải thích được vai trò của từng thẻ ngữ nghĩa giúp tối ưu SEO và cấu trúc trang web rõ ràng thay vì lạm dụng thẻ `<div>`.
- **CSS Flexbox & CSS Grid:** 
  - Sử dụng `display: grid` kết hợp `grid-template-columns` để chia lưới sản phẩm tự động co giãn.
  - Sử dụng `display: flex` để căn chỉnh thành phần theo hàng ngang/dọc trong Header và Card sản phẩm.
- **Biến CSS (CSS Variables):** Hiểu cách khai báo hệ thống màu sắc và khoảng cách tại khối `:root` để dễ dàng tái sử dụng và quản lý theme.
