# DTK_NMKS – PWA v0.1 (iPhone / Android)

Ứng dụng web cài lên Màn hình chính. Dùng **nguyên vẹn 423 câu hỏi / 7 nhóm** từ bản Android DTK_NMKS v0.3. Không phụ thuộc Apple Developer.

## Đưa lên GitHub Pages

1. Tạo repository mới tên `DTK_NMKS_PWA`, chọn **Public**, không tạo README mặc định. Không dùng repository iOS/Android hiện tại.
2. Giải nén ZIP. Tại trang repository mới chọn **uploading an existing file**. Kéo **toàn bộ nội dung bên trong** thư mục đã giải nén lên GitHub, không tải chính file ZIP. Phải thấy `index.html`, `app.js`, `style.css`, `sw.js`, `questions.json`, `manifest.webmanifest`, thư mục `icons` ở thư mục gốc. Chọn **Commit changes**.
3. GitHub > **Settings** > **Pages** > **Build and deployment** > **Source: Deploy from a branch** > **Branch: main** > **Folder: /(root)** > **Save**.
4. Đường dẫn dự kiến khi Pages được xuất bản: `https://dongtrungkienpfiev.github.io/DTK_NMKS_PWA/` (chỉ hoạt động khi bước 3 triển khai thành công).
5. Mở trên iPhone bằng Safari > **Share** > **Add to Home Screen** > **Add** (trên một số iOS chọn **Open as Web App**).
6. Mở ứng dụng khi có mạng lần đầu để tải đủ 423 câu. Sau đó thử Airplane Mode để xác nhận offline.

## Chức năng

- Định danh: Mã lớp, Mã SV, Họ và tên.
- Học theo nhóm, đáp án sai được thử lại; đúng được đánh dấu hoàn thành.
- 8 điểm cho tỷ lệ câu hoàn thành, 2 điểm cho tỷ lệ nhóm đã củng cố (chỉ mở sau khi làm hết nhóm; 5 câu đầu để củng cố).
- Xuất PDF một trang bằng tính năng offline. Tên `NMKS_MALOP_MASV_HOVATEN.pdf` (họ tên bỏ dấu và khoảng trắng). iPhone có thể hiển thị bảng chia sẻ hoặc lưu file về Tệp.
- Dữ liệu học tập chỉ lưu trên máy trong `localStorage`, không gửi về GitHub.

## Lưu ý quan trọng

- **BẢN THỬ NGHIỆM**: chưa kiểm thử thực tế trên iPhone; cần thử chức năng share PDF và offline trên Safari/iOS.
- GitHub Pages và câu hỏi được công khai; **không đưa mã lớp/sinh viên thực tế hoặc dữ liệu cá nhân lên repo**. Đáp án trong ngân hàng câu hỏi có thể bị người biết kỹ thuật xem; không coi PWA là công cụ thi bảo mật cao.
- Xóa dữ liệu Safari, gỡ ứng dụng hoặc đổi mã lớp/Mã SV có thể làm mất tiến độ cục bộ; nên xuất PDF thường xuyên.
- PDF chỉ là bằng chứng do thiết bị tạo, có khả năng sửa/copy; giảng viên cần đối chiếu trước khi sử dụng chấm chuyên cần.
- Điểm tiến bộ hiện là điểm **ôn tập củng cố**, không phải phép đo tiến bộ độc lập.
- Không mở trực tiếp `index.html` từ ổ cứng để thử offline: PWA cần HTTP localhost hoặc HTTPS.
