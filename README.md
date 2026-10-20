## 1. Giới thiệu
Dự án cải tiến giao diện trang chủ (Homepage) cho website thương mại điện tử chuyên về mỹ phẩm và chăm sóc cá nhân. Mẫu thiết kế tập trung tối ưu hóa trải nghiệm người dùng (UX), nâng cao phân cấp thị giác, giảm tải nhiễu thông tin và đảm bảo tính tương thích cao trên mọi thiết bị di động.

## 2. Website tham khảo
- **Tên website:** Hasaki Beauty & Clinic
- **URL:** https://hasaki.vn/
- **Khu vực đã khảo sát:** Trang chủ (Homepage)

## 3. Chức năng
- **Hiển thị danh sách sản phẩm:** Trình bày sản phẩm dưới dạng lưới (Grid) trên Desktop và cuộn ngang (Horizontal Scroll Snap) trên Mobile cho khu vực Flash Sale.
- **Hiển thị tên và giá sản phẩm:** Cung cấp rõ ràng thông tin tên sản phẩm, thương hiệu, giá bán, giá niêm yết, phần trăm giảm giá và các nhãn cam kết (Badge Giao 2H).
- **Bố cục hỗ trợ nhiều kích thước màn hình:** Tự động co giãn linh hoạt theo độ phân giải màn hình (Desktop $\ge$ 1024px, Tablet 768px - 1023px, Mobile $< 768\text{px}$) kèm thanh Bottom Navigation cố định trên điện thoại.

## 4. Công nghệ
- **HTML5:** Sử dụng đầy đủ các thẻ ngữ nghĩa (Semantic tags) như `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<time>`, `<footer>`.
- **CSS3:** Áp dụng kỹ thuật dàn trang CSS Grid, Flexbox, biến hệ thống (CSS Variables), BEM methodology và Media Queries tối ưu Responsive.
- **JavaScript (Vanilla JS):** Xử lý logic bộ đếm ngược Flash Sale và chuyển đổi dữ liệu tab danh mục không cần tải lại trang.

## 5. Cách chạy
Mở file `index.html` bằng trình duyệt web bất kỳ (Google Chrome, Microsoft Edge, Mozilla Firefox, Safari) hoặc nhấp chuột phải chọn **Open with Live Server** trong Visual Studio Code.

## 6. Cải tiến đã thực hiện
- **Vấn đề ban đầu:** Giao diện trang chủ ban đầu có mật độ banner, hình ảnh và thông tin quảng cáo quá dày đặc, gây rối mắt (Cognitive Overload), khiến người dùng khó nhận diện chương trình ưu đãi chính và thao tác phức tạp khi dùng trên điện thoại.
- **Thay đổi đã thực hiện:**
  - Chỉnh sửa lại bố cục Hero Banner thành dạng "1 Hero Banner chủ đạo + 6 Lối vào nhanh" giúp thu hút khách hàng ngay từ 3 giây đầu.
  - Áp dụng **Card Layout** kết hợp khoảng trống âm (Negative Space) để nhóm rõ ràng từng phân khu thông tin.
  - Chuyển đổi lưới sản phẩm dài trên mobile thành dạng **cuộn ngang (Horizontal Snap Scroll)** cho khối Flash Sale và dạng **Tab điều hướng** cho danh mục gợi ý, giảm bớt chiều dài cuộn trang.
  - Tích hợp thanh điều hướng dưới (**Bottom Navigation Bar**) chuẩn UX Mobile App cho thao tác một tay trên điện thoại.

## 7. Hỗ trợ từ AI
- **Phần AI hỗ trợ:**
  - Phân tích ưu/nhược điểm nghiệp vụ (BA) và trải nghiệm người dùng (UX) trên nền tảng Hasaki.vn.
  - Đề xuất kiến trúc bố cục, cấu trúc danh mục và tiêu chuẩn kiểm tra khả năng sử dụng (Usability Checklist).
  - Tự động sinh mã nguồn khởi tạo bao gồm cấu trúc HTML5 chuẩn ngữ nghĩa, hệ thống biến CSS3 và bộ đếm ngược Flash Sale bằng JavaScript.
- **Phần tôi đã kiểm tra, điều chỉnh hoặc bổ sung:**
  - Kiểm tra và xác nhận tính hợp lý của vị trí hiển thị thanh tìm kiếm, nhãn Giao 2H và khối Flash Sale đối với thói quen mua sắm trực tuyến của người dùng Việt Nam.
  - Rà soát độ tương phản màu sắc (Color Contrast), kích thước vùng chạm nút bấm (Min 44x44px) trên bản di động.
  - Kiểm tra tính tương thích trực tiếp trên các kích thước màn hình thực tế qua công cụ Inspect Elements.