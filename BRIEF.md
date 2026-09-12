# Mã Biểu Tượng — brief nội dung & sản phẩm

Tài liệu tổng hợp yêu cầu cho phiên bản 2 của trang giải mã giấc mơ, dùng làm tham chiếu khi chỉnh sửa sau này.

## Thương hiệu
- Tên sản phẩm: **Mã Biểu Tượng**, chữ ký "by Thanh Hoà" ở logo/chân trang.
- Không hiển thị tên UCM Centre, Francis L. Kaya, hay bất kỳ thương hiệu/tổ chức nguồn nào trên giao diện hoặc trong prompt gửi Claude.
- Chỉ nhắc đến tên phương pháp **DSSI** (không giải thích nó là của ai).

## Hook chính
"Giải mã các biểu tượng trong đời sống của bạn." — mở rộng khỏi phạm vi "giấc mơ" sang "biểu tượng trong đời sống" nói chung.

## Input (đầu vào của người dùng)
1. **Thiên Thần đồng hành** — người dùng chọn 1 trong 72 Thiên Thần (danh sách "Tên — đặc điểm ngắn", có ô tìm kiếm lọc theo tên). Không bắt buộc — có thể bỏ qua nếu chưa xác định. Danh sách 72 tên dùng bộ tên truyền thống Shem HaMephorash (kiến thức phổ thông, không thuộc bản quyền riêng của UCM); phần mô tả đặc điểm do Thanh Hoà/trang tự viết lại, không copy nguyên văn từ bất kỳ nguồn nào.
2. **Mô tả giấc mơ/biểu tượng theo 3 trục** (thay cho 1 ô textarea lớn, để thân thiện hơn):
   - Ở đâu (Where) — bối cảnh
   - Ai xuất hiện (Who) — nhân vật
   - Điều gì đã diễn ra (What) — sự việc/hành động/biểu tượng chính (có sẵn "chip" gợi ý nhanh: con rắn, răng rụng, bay lên, bị đuổi, nước dâng...)

## Output (kết quả giải mã) — mỗi lần giải mã cần có
1. **Tóm tắt** ngắn gọn.
2. **Biểu tượng chính**: tên biểu tượng + **đặc điểm/đặc tính tự nhiên vốn có** của nó (nếu là con vật: tập tính; nếu là cây/thiên nhiên: đặc tính sinh học) — điểm cộng suy ra từ đặc tính được biểu hiện trọn vẹn, điểm trừ suy ra từ đặc tính bị biến dạng/thiếu hụt. Ví dụ mẫu: cây tán rộng vốn có đặc tính che chở cây khác → điểm cộng là "che chở", điểm trừ là "mất khả năng che chở/cô lập".
3. **3 trục Where / Who / What**: mỗi trục có điểm cộng và điểm trừ riêng.
4. **Ngũ Hành cộng hưởng**: xác định 1 trong 5 nguyên tố (Kim/Mộc/Thuỷ/Hoả/Thổ) cộng hưởng với giấc mơ, kèm biểu hiện tích cực và mất cân bằng của nguyên tố đó trong bối cảnh giấc mơ.
5. **Liên hệ Thiên Thần** (chỉ khi người dùng có chọn): 1-2 câu nối thông điệp giấc mơ với hành trình cùng Thiên Thần đã chọn.
6. **Thông điệp tổng hợp** từ vô thức.
7. **Câu hỏi phản tư** (2-3 câu) để người dùng tự chiêm nghiệm thêm.

## Định hướng thiết kế (vibe tham chiếu người dùng gửi)
Ba ảnh tham chiếu đều là collage nền giấy màu kem/be ấm, có các ô vuông viền/khối xanh cobalt chứa hình ảnh/hoạ tiết khoa học-tự nhiên (DNA, biểu đồ, dữ liệu nhị phân, bản đồ/la bàn), xen giữa các hoạ tiết vẽ tay nhỏ (dấu sao, dấu cộng/trừ, đường lượn sóng, chấm màu cam-đỏ) rải quanh một hình khối trung tâm lớn (bàn tay / viên nang / các đường tam giác hoá). Bảng màu cảm hứng: nền kem/be ấm + xanh cobalt làm màu cấu trúc chính + xanh ngọc làm màu tích cực + cam-đỏ trầm làm màu tiêu cực. Vì Artifact không tải được ảnh ngoài (CSP), toàn bộ phần "collage" trong bản HTML được vẽ lại bằng SVG/CSS gốc (DNA, la bàn, lông vũ, lưới toạ độ, ngũ hành) thay vì dùng ảnh thật, giữ đúng tinh thần "khoa học gặp huyền học" nhưng không vi phạm bản quyền ảnh.

## Ghi chú kỹ thuật
- Phân tích chạy qua khả năng `sample` của Claude Artifact (`claude.use("sample")`) — chỉ hoạt động khi xem trong Artifact trên claude.ai, không chạy trên bản tĩnh GitHub Pages.
- Lịch sử giải mã ("Sổ tay") lưu trong `localStorage`, riêng theo từng trình duyệt, không đồng bộ.
- Nguồn tư liệu gốc (bài giảng dài về "Giấc mơ là hiện thực" do người dùng gửi) chỉ dùng làm tài liệu tham khảo nội bộ để hiểu tinh thần phương pháp — không được trích dẫn nguyên văn hoặc xuất bản lại trên trang vì lý do bản quyền; mọi câu chữ hiển thị trên site đều được viết lại bằng lời văn riêng.
