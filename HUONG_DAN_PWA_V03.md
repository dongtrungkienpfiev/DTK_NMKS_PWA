# DTK_NMKS PWA v0.3 — đồng bộ Android v0.6

## Cập nhật trực tiếp trên GitHub (trình duyệt, không cần GitHub Desktop)

Repository: https://github.com/dongtrungkienpfiev/DTK_NMKS_PWA

1. Trước khi cập nhật, tải ZIP mã nguồn repo về máy để dự phòng.
2. Mở repo, chọn **Add file → Upload files** trên nhánh **main**.
3. Từ thư mục ZIP đã giải nén, kéo **các tệp và thư mục bên trong** vào màn hình upload, không kéo file ZIP. Danh sách đúng ở gốc repo gồm `index.html`, `app.js`, `style.css`, `sw.js`, `questions.json`, `manifest.webmanifest`, thư mục `icons/`. Không được tạo lồng thêm thư mục.
4. Chọn **Commit directly to main → Commit changes**.
5. Kiểm tra trong **Actions** hoặc **Settings → Pages** xem GitHub Pages triển khai xong.
6. Mở https://dongtrungkienpfiev.github.io/DTK_NMKS_PWA/ trên điện thoại khi có Internet. Đóng/mở lại ứng dụng (nếu cần tải lại trang một lần) để cập nhật cache. **Không xóa dữ liệu trang web, không gỡ PWA cũ** khi đang cần giữ tiến độ.

## Chức năng

- 423 câu, 7 nhóm: giữ nguyên dữ liệu gốc; luyện tập tự do hoặc tuần tự; sai thử lại ngay, không có thời gian chờ.
- “Xem kết quả”: danh sách toàn nhóm, chọn bất kỳ câu; thấy lựa chọn đã chọn gần nhất, biết hoàn thành/chưa hoàn thành; có nút trả lời lại câu chưa đúng.
- Mở lại ứng dụng: khôi phục nhóm/câu đang làm hoặc câu chưa hoàn thành gần nhất.
- Củng cố: sau khi hoàn thành toàn bộ câu của một nhóm, mở 10 câu ngẫu nhiên; xáo trộn phương án; chỉ ghi nhận lần chọn đầu tiên trong một lượt; đạt ≥70% được cộng 2/7 điểm; không làm mất điểm đã đạt; cho thực hiện lượt mới.
- Điểm luyện tập: 8 × số câu hoàn thành/423; điểm củng cố: 2 × số nhóm đã đạt/7.
- PDF báo cáo tiếp tục hoạt động offline.

## Giới hạn và an toàn dữ liệu

- Lưu trong `localStorage` của trình duyệt. Xóa dữ liệu Safari/Chrome hoặc gỡ PWA có thể xóa kết quả.
- Những câu từng hoàn thành ở phiên bản cũ có thể không lưu được phương án đã chọn; hiển thị ghi chú, không giả định đáp án cũ.
- Các khoản điểm củng cố đã đạt ở phiên bản cũ được giữ nguyên. Câu hỏi củng cố mới chỉ ghi nhận lần chọn đầu tiên.
- Chưa kiểm thử thực tế trên nhiều thiết bị; nên chạy thử trên máy không có dữ liệu học quan trọng trước khi cập nhật cho toàn lớp.
- Báo cáo PDF do thiết bị tự lập, chưa có chữ ký xác thực của máy chủ.
