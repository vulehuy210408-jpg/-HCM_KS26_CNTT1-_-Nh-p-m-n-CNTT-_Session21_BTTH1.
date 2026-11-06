# BÀI TẬP TỔNG HỢP BUỔI 21: NHẬP MÔN CÔNG NGHỆ THÔNG TIN
## Hành Trình Xử Lý 1 Lỗi Cài Đặt Thật (Node.js & npm)

* **Họ và tên học viên:** Vũ Lê Huy
* **Mã sinh viên:** N26DTCN046
* **Lớp học:** IT108-K26

---

## PHẦN 1 – GOOGLING ĐÚNG CÁCH

### 1. Vì sao câu hỏi "văn nói" kém chất lượng?
* Chứa nhiều từ thừa, đại từ nhân xưng, thiếu từ khóa kỹ thuật cốt lõi khiến thuật toán Google không khớp được mã lỗi chuẩn trên các diễn đàn chuyên môn.

### 2. Bóc tách lỗi theo 3 thành phần cốt lõi
| Thành phần | Nội dung bóc tách |
| :--- | :--- |
| **Tên phần mềm / Hệ điều hành** | Node.js / npm trên Windows 11 |
| **Mã lỗi nguyên văn** | `'npm' is not recognized as an internal or external command, operable program or batch file.` |
| **Thao tác đang làm** | Mở Terminal trong VS Code và gõ lệnh `npm -v` |

### 3. Ba câu truy vấn Google tối ưu
* **Giới hạn trong StackOverflow (`site:`):**
  
  site:stackoverflow.com "npm is not recognized as an internal or external command" windows 11


---

## PHẦN 2 – THẨM ĐỊNH STACKOVERFLOW

### 1. So sánh Câu trả lời A và B
| Tiêu chí | Câu trả lời A | Câu trả lời B |
| :--- | :--- | :--- |
| **Vote & Tích xanh** | +186 Upvotes, có tích xanh (Accepted Answer) | +2 Upvotes, không có tích xanh |
| **Thời gian đăng bài** | 2 năm trước | 9 năm trước |
| **Tags hệ điều hành/phần mềm** | `[node.js]`, `[windows]`, `[npm]` (Khớp hoàn toàn) | `[node.js]`, `[windows-xp]` (Lệch hệ điều hành) |

### 2. Kết luận lựa chọn và Cảnh báo bẫy
* **Lựa chọn:** Áp dụng **Câu trả lời A** (*Thêm đường dẫn cài đặt Node.js vào biến môi trường PATH*).
* **Bẫy nguy hiểm:** Câu trả lời B khuyên *gỡ Node.js, cài lại driver mạng cho Windows XP* — đây là bẫy cực kỳ nguy hiểm vì dùng cho hệ điều hành cũ (Windows XP) không khớp với Windows 11 hiện đại, làm lệch hướng xử lý và có thể làm hỏng cấu hình mạng máy tính.

### 3. Quy trình 30 giây đọc lướt StackOverflow
1. **Bước 1:** Kiểm tra tiêu đề và mã lỗi xem có khớp hoàn toàn với lỗi của mình không.
2. **Bước 2:** Cuộn thẳng xuống câu trả lời có tích xanh (Accepted Answer) và lượng Upvotes cao nhất.
3. **Bước 3:** Đọc nhanh đoạn lệnh giải pháp xem có trực quan và an toàn không trước khi thao tác.



## PHẦN 3 – HỎI AI ĐÚNG CÁCH VÀ NHẬN DIỆN RỦI RO

### 1. Prompt hoàn chỉnh theo Công thức 3 Thành phần

[Context - Ngữ cảnh]: Tôi đang cài đặt Node.js trên máy tính Windows 11 mới. Tôi đã thử thêm đường dẫn C:\Program Files\nodejs\ vào biến môi trường PATH theo hướng dẫn nhưng lỗi vẫn tiếp tục xảy ra khi mở Terminal mới.

[Raw Error - Lỗi nguyên văn]:
'npm' is not recognized as an internal or external command, operable program or batch file.

[Instruction - Yêu cầu]: Với tư cách là chuyên gia hỗ trợ kỹ thuật, hãy phân tích nguyên nhân tại sao việc cấu hình PATH ở trên có thể chưa có hiệu lực và cung cấp các bước kiểm tra nâng cao để khắc phục triệt để lỗi nhận diện lệnh npm trên Windows 11.
## PHẦN 4: VIẾT BUG REPORT CHUẨN ĐỂ NHỜ HỖ TRỢ
## Bài tập tổng hợp: Hành Trình Xử Lý 1 Lỗi Cài Đặt Thật (Buổi 21)

## 1. Tin nhắn kiểu "Kém" (Mù mờ, thiếu ngữ cảnh)
> *"Thầy ơi, máy em bị lỗi npm không chạy được, sửa kiểu gì ạ?"*

---

## 2. Tin nhắn chuẩn theo Bug Reporting Framework 4 mảnh ghép
| Mảnh ghép | Nội dung trong tin nhắn của bạn |
| :--- | :--- |
| **Context (Ngữ cảnh)** | Cài đặt Node.js trên laptop Windows 11 mới, đang mở Terminal trong VS Code để kiểm tra môi trường học tập. |
| **Expected (Kỳ vọng)** | Khi gõ lệnh `npm -v`, Terminal phải trả về số phiên bản của npm (ví dụ: `10.x.x`). |
| **Actual (Thực tế)** | Terminal báo lỗi không nhận diện lệnh: `'npm' is not recognized as an internal or external command, operable program or batch file.` |
| **Log & Screenshot (Nhật ký & Ảnh chụp)** | Đã kiểm tra và thêm đường dẫn `C:\Program Files\nodejs\` vào biến môi trường PATH nhưng vẫn bị lỗi. <br>*(Kèm ảnh chụp màn hình Terminal thông báo lỗi và ảnh cấu hình biến môi trường PATH)*. |

---

## 3. Phím tắt chụp màn hình & Lưu ý bảo mật
* **Phím tắt chụp màn hình trên Windows:** Sử dụng tổ hợp phím **`Windows + Shift + S`** để mở công cụ chụp ảnh màn hình nhanh (Snipping Tool).
* **Lưu ý bảo mật:** Trước khi gửi ảnh lên không gian công cộng hoặc nhờ trợ giảng hỗ trợ, phải kiểm tra kỹ để **che mờ các thông tin nhạy cảm** (như email cá nhân, tên người dùng máy tính, mã token, hoặc đường dẫn thư mục cá nhân) nhằm tránh rò rỉ dữ liệu riêng tư.