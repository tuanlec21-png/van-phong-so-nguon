# Lỗi giao diện và câu chữ trên vmarketingpro.com

Dò ngày 25/11/2026 trên trang chủ đang chạy (https://vmarketingpro.com, trang giới thiệu OPC), ở cỡ 1440×900 và 390×844. Chỉ dò trang chủ; chưa dò các trang sau đăng nhập, form đăng ký, khung chat và trang Chính sách bảo mật.

Cách dùng: mở Claude Code trong thư mục mã nguồn của trang, dán file này vào và yêu cầu sửa. Nếu đã cài skill unslop thì gõ `/unslop trang chủ` rồi đưa file này làm danh sách lỗi đã dò sẵn.

## Yêu cầu chung khi sửa

- Giữ nguyên sản phẩm, các mục và thứ tự: video đầu trang, phần giới thiệu, Thị trường (`#xu-huong`), Chi phí (`#chi-phi`), Cho ai (`#cho-ai`), Nền tảng (`#mo-hinh`), Hợp tác (`#hop-tac`), phần kêu gọi cuối trang, chân trang.
- Không đổi số liệu, nguồn, tên sản phẩm hay ý nghĩa câu chữ, trừ các mục ghi rõ ở phần "Câu chữ và nội dung".
- Không thay hiệu ứng bị gỡ bằng hiệu ứng trang trí khác (kính mờ, nhiễu hạt, neon, lưới bento).
- Sau khi sửa, dựng lại trang ở 1440px và 390px để kiểm tra.

## Phần kỹ thuật đang ổn, không cần sửa

- Trang tải được, không có lỗi script hay tài nguyên hỏng.
- Không cuộn ngang ở 390px.
- Các phép tính trên trang đúng: 6 × 5.310.000 × 1,215 ≈ 38,7 triệu; từ 9 lên 29 USD là tăng 222%; 182.000 trong 10 tháng ≈ 600 mỗi ngày.

## Lỗi giao diện

### Màu và bề mặt

1. Chữ gradient tím sang xanh ngọc trên logo "OPC", trên phần "trên một nền tảng" của tiêu đề chính, và trên cả bốn con số ở mục Thị trường (39 tỷ USD, 10%, −80.000, 29 USD). Đổi về màu chữ đặc.
2. Trang có 51 phần tử dùng gradient. Chỉ giữ gradient khi là chuyển sắc nhẹ trong cùng một màu trung tính.
3. Bóng màu phát sáng trên nút "Đăng ký" (đầu trang và trong phần giới thiệu) và trên nút nổi "Hỏi OPC". Bỏ bóng màu.
4. Quầng màu tím toả sau nội dung ở phần giới thiệu và đầu các mục, cùng lưới ô mờ trên nền. Bỏ, dùng một nền trung tính.
5. Viền màu xanh ngọc quanh thẻ sản phẩm ở phần giới thiệu và ô "AI local model". Đổi về viền mảnh trung tính.
6. Các gạch chân gradient dưới sáu ô Marketing, Nhân sự, Kế toán, Sale, Quản trị, Chăm sóc khách hàng. Bỏ hoặc dùng một màu.
7. Chỉ dùng một màu nhấn, cho hành động chính và một hai chỗ thật sự cần nổi.

### Kiểu chữ

8. Nhãn in hoa giãn chữ ở 13 chỗ: "THỊ TRƯỜNG", "CHI PHÍ", "CHO AI", "NỀN TẢNG", "HỢP TÁC", "MỚI LÀ MỨC SÀN CHO 6 VỊ TRÍ", "DOANH NGHIỆP TRẢ", "AI LÀM VIỆC", "PHÙ HỢP KHI", "RỦI RO", "ÁP DỤNG KHI"… Đổi về chữ thường viết hoa đầu câu, không giãn chữ.
9. Chữ quá đậm: 45 phần tử ở độ đậm 700 đến 900 (22 ở 700, 6 ở 800, 16 ở 850, 1 ở 900). Đưa về 400 và 500, tối đa 600 cho chỗ cần nhấn; phân cấp bằng cỡ chữ và màu.
10. Các con số thống kê dùng chữ số đều cột (`tabular-nums`).

### Icon và ký tự

11. Emoji 💬 trên nút nổi "Hỏi OPC". Đổi sang icon nét cùng bộ với các icon khác, hoặc bỏ.
12. Ký tự ▾ cạnh "Đăng nhập". Đổi sang icon mũi tên vẽ bằng nét.
13. Ký tự ↗ và ∞ đứng thay con số ở mục Nền tảng. Xem mục 22.
14. Bốn icon trong ô vuông tím ở mục Cho ai. Icon lấy màu chữ phụ, bỏ ô nền màu.

### Thành phần và bố cục

15. Nhãn viên thuốc "OPC · ONE PERSON COMPANY" phía trên tiêu đề chính. Bỏ, hoặc đổi thành một dòng chữ thường.
16. Bốn thẻ bằng nhau xếp một hàng ở mục Thị trường và mục Cho ai. Tạo nhịp: một thẻ chính lớn hơn, các thẻ còn lại gọn hơn.
17. Nút "Hỏi OPC" xuất hiện ba lần: trong phần giới thiệu, ở phần kêu gọi cuối trang, và nút nổi. Giữ nút nổi hoặc hai nút trong trang, không giữ cả ba.
18. Trên điện thoại nút nổi "Hỏi OPC" che lên nội dung. Thêm khoảng đệm dưới trang hoặc thu nhỏ nút.
19. Trên điện thoại không có menu tới các mục Thị trường, Chi phí, Cho ai, Nền tảng, Hợp tác. Thêm một nút menu.
20. Nút "Đăng ký" và "Đăng nhập" trên thanh điều hướng: một nút chính là đủ, "Đăng nhập" để dạng link chữ.

### Hình ảnh

21. Video đầu trang là cảnh vũ trụ với hạt sáng và vòng neon, không cho thấy sản phẩm. Cân nhắc thay bằng hình sản phẩm thật (màn hình OPC với dữ liệu hợp lý) hoặc giữ video nhưng đặt sau phần giới thiệu. Đây là quyết định của chủ trang, hỏi trước khi đổi.

## Câu chữ và nội dung

22. Ba tuyên bố ở mục Nền tảng không kiểm chứng được: "80% Giảm chi phí vận hành", "↗ Tăng doanh thu", "∞ Tiềm năng mở rộng không giới hạn". Hỏi chủ trang: con số 80% có nguồn hoặc cách tính không. Nếu không có thì bỏ cả ba, hoặc viết lại thành câu cụ thể không kèm con số.
23. Số 29 USD ở mục Thị trường viết "người bán online lỗ trung bình cho mỗi khách hàng mới", nhưng nguồn (SimplicityDX, 2022, qua Marketing Dive) là về các thương hiệu ở Mỹ. Ghi rõ phạm vi, ví dụ "thương hiệu bán online ở Mỹ lỗ trung bình…".
24. Nhãn "MỚI LÀ MỨC SÀN CHO 6 VỊ TRÍ" đọc trúc trắc. Gợi ý: "Mức tối thiểu cho 6 vị trí".
25. "Sale" đổi thành "Bán hàng" ở mọi chỗ (phần giới thiệu, mục Nền tảng, phần mô tả meta), cho thống nhất với phần còn lại viết tiếng Việt.
26. "AI local model" đổi thành cách nói tiếng Việt, ví dụ "AI chạy trên máy chủ riêng". Hiện cụm này và câu giải thích tiếng Việt đứng cạnh nhau, lặp ý.
27. "SaaR — Software as a Result": thuật ngữ không phổ biến, dễ bị đọc thành gõ nhầm "SaaS". Cân nhắc đặt tên tiếng Việt làm chính ("Chia sẻ lợi nhuận") và để "SaaR" làm chú thích.
28. Menu "Đăng nhập" có mục "Marketing Pro (bản cũ)" dẫn tới app.vmarketingpro.com. Hỏi chủ trang có nên để mục này trên trang giới thiệu không.
29. Dấu gạch ngang dài dùng nhiều trong tiêu đề ("Bán hàng online tăng nhanh — chi phí marketing còn tăng nhanh hơn", "Mô hình chuẩn của một công ty — tất cả trên một nền tảng", "SaaS hay SaaR — hai cách hợp tác"). Viết lại bằng dấu phẩy hoặc tách câu.
30. Tiêu đề và nhãn ngắn không kết thúc bằng dấu chấm; chỉ đoạn nhiều câu mới giữ dấu chấm. Soát lại các thẻ ở mục Cho ai và mục Hợp tác.

## Chia sẻ và tìm kiếm

31. Trang không khai báo `og:image`, nên dán link lên Zalo hay Facebook không hiện ảnh xem trước. Thêm `og:image`, `og:title`, `og:description`.

## Chưa kiểm tra

- Các trang đăng nhập: office.vmarketingpro.com/dang-nhap/, office.vmarketingpro.com/quan-tri-he-thong/, app.vmarketingpro.com.
- Form đăng ký, khung chat "Hỏi OPC", trang /chinh-sach-bao-mat.
- Tám link nguồn ở mục Thị trường và Chi phí còn mở được và còn đúng số liệu hay không.
- Giao diện ở chế độ sáng, nếu trang có.
