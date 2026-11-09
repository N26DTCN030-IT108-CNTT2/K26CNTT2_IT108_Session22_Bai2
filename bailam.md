# [D26TXCN02-N]_IT108_[Session 22]_[Bài 2]
**Bài tập: Xử lý lỗi thư viện mã nguồn mở bằng GitHub Issues**

**Thông tin sinh viên:**
- **Họ và tên:** Lê Hồ Thanh Thảo
- **Mã sinh viên:** N26DTCN030
- **Lớp:** D26TXCN02-N
- **Môn học:** Nhập môn Công nghệ Thông tin

---

## 1. Tiêu chí ưu tiên khi đọc bình luận trên GitHub Issues

Trong một luồng thảo luận (Issue) trạng thái **OPEN** với quá nhiều bình luận trái chiều, việc lọc ra câu trả lời chất lượng là rất quan trọng. Ta nên ưu tiên đọc các bình luận có đặc điểm sau:

* **Tương tác tích cực cao (High Positive Reactions):** Ưu tiên các bình luận sở hữu nhiều biểu tượng **Thumbs Up (👍)**, **Heart (❤️)**, hoặc **Hooray (🎉)**. Đây là sự "bình chọn" trực tiếp từ cộng đồng lập trình viên — những người đã thử nghiệm giải pháp đó và xác nhận thành công.
* **Bình luận được tác giả/Maintainer ghim (Pinned Comment):** Những giải pháp được đội ngũ phát triển dự án ghim lên đầu hoặc thả tim xác nhận.
* **Đoạn mã rõ ràng, kèm giải thích ngắn gọn:** Bình luận chỉ ra rõ nguyên nhân gốc rễ (Root Cause) và cung cấp đoạn mã chỉnh sửa cụ thể thay vì chỉ đưa ra lời khuyên chung chung như "xóa đi cài lại".

---

## 2. Phân tích khái niệm "Workaround" và lý do không nên đợi bản cập nhật chính thức

### Khái niệm Workaround
**Workaround** (Giải pháp tạm thời / Đường vòng) là một phương pháp hoặc đoạn mã được áp dụng để khắc phục/bỏ qua sự cố của phần mềm ngay lập tức mà không cần sửa lỗi tận gốc trong bộ mã nguồn chính của thư viện.

### Lý do không nên đợi bản cập nhật chính thức (Official Release) ngay lúc đó:
1. **Tiến độ dự án (Deadline):** Quy trình phát hành bản sửa lỗi chính thức (Hotfix/Patch release) từ nhà sản xuất đòi hỏi nhiều thời gian: duyệt PR, chạy kiểm thử tự động (CI/CD), kiểm thử thủ công và đưa lên trình quản lý gói (NPM, PyPI,...). Đợi bản cập nhật sẽ làm gián đoạn công việc hiện tại.
2. **Duy trì luồng phát triển (Unblock Workflow):** Áp dụng Workaround giúp ứng dụng tiếp tục chạy ổn định trong môi trường phát triển (Development environment), giúp lập trình viên tiếp tục hoàn thiện các tính năng khác.
3. **Chủ động trong lập trình:** Lập trình viên chuyên nghiệp luôn cần linh hoạt tìm kiếm các phương án dự phòng thay vì bị động phụ thuộc vào nhà sản xuất mã nguồn mở.