# BUSINESS REQUIREMENTS DOCUMENT (BRD)

# WEBSITE HỌC VÀ ÔN TẬP TỪ VỰNG TIẾNG ANH

**Phiên bản:** 1.0  
**Trạng thái:** Draft  
**Mục đích:** Mô tả yêu cầu nghiệp vụ cho nền tảng hỗ trợ người dùng học và ôn tập từ vựng tiếng Anh.

---

## 1. TỔNG QUAN DỰ ÁN

### 1.1. Bối cảnh

Người học tiếng Anh thường có thể ghi nhớ một từ trong thời gian ngắn nhưng dễ quên nếu không được ôn tập thường xuyên và theo nhiều hình thức khác nhau.

Website được xây dựng nhằm hỗ trợ người dùng:

- Học từ vựng mới.
- Ôn lại các từ đã học.
- Kiểm tra khả năng ghi nhớ từ theo nhiều cách.
- Luyện khả năng nhận biết nghĩa, nhớ từ tiếng Anh và sử dụng từ trong câu.
- Luyện phát âm từ vựng.
- Theo dõi quá trình học tập và mức độ ghi nhớ.

### 1.2. Tầm nhìn

Xây dựng một nền tảng học từ vựng tiếng Anh đơn giản, dễ sử dụng và tập trung vào việc giúp người học **nhớ từ lâu hơn thông qua việc chủ động truy xuất kiến thức**, thay vì chỉ đọc và ghi nhớ thụ động.

### 1.3. Mục tiêu kinh doanh/sản phẩm

Hệ thống cần hướng đến các mục tiêu:

1. Giúp người dùng duy trì thói quen học từ vựng.
2. Tăng khả năng ghi nhớ từ thông qua nhiều dạng bài tập.
3. Cho phép người dùng tự tạo và tổ chức danh sách từ vựng theo chủ đề.
4. Tự động hỗ trợ người dùng xác định những từ cần ôn tập.
5. Cung cấp thông tin tiến độ để người dùng biết mình đang học tốt ở mức nào.

---

## 2. PHẠM VI SẢN PHẨM

### 2.1. Trong phạm vi

Phiên bản đầu tiên của hệ thống bao gồm:

- Đăng ký và đăng nhập tài khoản.
- Quản lý hồ sơ người dùng.
- Tạo và quản lý danh sách/chủ đề từ vựng.
- Thêm, chỉnh sửa, xóa từ vựng.
- Hiển thị thông tin chi tiết của từ.
- Học từ mới.
- Ôn tập từ đã học.
- Lật thẻ từ vựng.
- Câu hỏi trắc nghiệm về nghĩa của từ.
- Nhập từ tiếng Anh dựa trên nghĩa tiếng Việt.
- Dịch câu ví dụ từ tiếng Việt sang tiếng Anh.
- Luyện phát âm từ.
- Ghi nhận kết quả học tập.
- Theo dõi tiến độ và trạng thái ghi nhớ từ.

### 2.2. Ngoài phạm vi của phiên bản đầu tiên

Các nội dung sau chưa phải yêu cầu bắt buộc của phiên bản đầu:

- Khóa học video hoàn chỉnh.
- Lớp học trực tuyến với giáo viên.
- Mạng xã hội cho người học.
- Hệ thống thi/chứng chỉ tiếng Anh.
- Thanh toán và gói thuê bao.
- Ứng dụng mobile native.

Những chức năng trên có thể được xem xét ở các phiên bản sau.

---

## 3. ĐỐI TƯỢNG SỬ DỤNG VÀ VAI TRÒ

### 3.1. Người học

Người học là đối tượng sử dụng chính của hệ thống.

Người học có thể:

- Quản lý tài khoản cá nhân.
- Tạo danh sách từ vựng.
- Học từ mới.
- Ôn tập từ đã học.
- Làm các dạng bài kiểm tra.
- Luyện phát âm.
- Xem kết quả và tiến độ học tập.

### 3.2. Quản trị viên

Quản trị viên chịu trách nhiệm quản lý nội dung và vận hành hệ thống.

Quản trị viên có thể:

- Quản lý người dùng.
- Quản lý nội dung từ vựng dùng chung của hệ thống.
- Quản lý chủ đề từ vựng dùng chung.
- Theo dõi các thông tin vận hành cần thiết.
- Xử lý nội dung không phù hợp hoặc dữ liệu sai.

---

## 4. YÊU CẦU CHỨC NĂNG CHÍNH

## 4.1. Quản lý tài khoản

Hệ thống phải cho phép người dùng:

- Đăng ký tài khoản.
- Đăng nhập.
- Đăng xuất.
- Quản lý thông tin cá nhân.
- Thay đổi mật khẩu.
- Khôi phục mật khẩu khi quên.
- Xóa tài khoản theo quy định của hệ thống.

---

## 4.2. Quản lý danh sách/chủ đề từ vựng

Người dùng có thể tạo các danh sách từ vựng theo mục đích học tập, ví dụ:

- Công việc.
- Du lịch.
- Công nghệ.
- Giao tiếp hằng ngày.
- TOEIC.
- IELTS.
- Chủ đề tự tạo.

Mỗi danh sách có thể chứa nhiều từ vựng.

Người dùng có thể:

- Tạo danh sách.
- Đổi tên danh sách.
- Xóa danh sách.
- Xem danh sách.
- Thêm từ vào danh sách.
- Xóa từ khỏi danh sách.

---

## 4.3. Quản lý từ vựng

Mỗi từ vựng có thể bao gồm các thông tin nghiệp vụ sau:

- Từ tiếng Anh.
- Nghĩa tiếng Việt.
- Từ loại.
- Câu ví dụ tiếng Anh.
- Câu ví dụ tiếng Việt.
- Phiên âm.
- Phát âm tiếng Anh.
- Các thông tin bổ sung liên quan đến từ.

Người dùng có thể:

- Thêm từ mới.
- Chỉnh sửa thông tin từ.
- Xóa từ.
- Xem chi tiết từ.
- Tra cứu từ trong danh sách học.

---

## 4.4. Học từ mới

Hệ thống cung cấp chế độ học từ mới giúp người dùng làm quen với từ trước khi bước vào phần ôn tập.

Một màn hình học từ có thể hiển thị:

- Từ tiếng Anh.
- Nghĩa tiếng Việt.
- Từ loại.
- Phiên âm.
- Câu ví dụ.
- Nút nghe phát âm.
- Thông tin bổ sung nếu có.

Người dùng có thể chuyển sang từ tiếp theo trong danh sách.

---

## 4.5. Ôn tập bằng lật thẻ

Đây là một hình thức ôn tập cơ bản.

Mặt trước của thẻ có thể hiển thị:

> `abandon`

Người dùng chọn **Lật thẻ** để xem:

> `từ bỏ, từ bỏ một thứ gì đó`

Sau khi xem đáp án, người dùng đánh giá mức độ nhớ của bản thân, ví dụ:

- Nhớ.
- Không nhớ.
- Khó nhớ.

Kết quả này được ghi nhận để phục vụ việc theo dõi tiến độ và lựa chọn từ cần ôn lại.

---

## 4.6. Trắc nghiệm nghĩa của từ

Hệ thống đưa ra một từ tiếng Anh và nhiều phương án trả lời bằng tiếng Việt.

Ví dụ:

**What does "rapid" mean?**

A. Chậm  
B. Nhanh  
C. Yếu  
D. Im lặng

Người dùng chọn một đáp án.

Hệ thống phải:

- Xác định câu trả lời đúng/sai.
- Hiển thị đáp án đúng sau khi trả lời.
- Ghi nhận kết quả.
- Cập nhật tiến độ học từ.

---

## 4.7. Dịch nghĩa tiếng Việt sang từ tiếng Anh

Hệ thống hiển thị nghĩa tiếng Việt và yêu cầu người dùng nhập từ tiếng Anh tương ứng.

Ví dụ:

> **Nghĩa:** từ bỏ

Người dùng nhập:

> `abandon`

Hệ thống kiểm tra câu trả lời và xác định người dùng trả lời đúng hay sai.

Đây là hình thức kiểm tra khả năng **tự nhớ từ tiếng Anh**, thay vì chỉ nhận diện đáp án.

---

## 4.8. Dịch câu tiếng Việt sang tiếng Anh

Hệ thống sử dụng một câu tiếng Việt gắn với từ vựng đang học.

Ví dụ:

> **Tiếng Việt:** Tôi quyết định từ bỏ kế hoạch đó.

Người dùng nhập câu trả lời bằng tiếng Anh.

Hệ thống hỗ trợ người dùng kiểm tra khả năng sử dụng từ trong ngữ cảnh.

Yêu cầu nghiệp vụ:

- Câu hỏi phải liên quan đến từ vựng đang được ôn tập.
- Hệ thống cần cung cấp câu trả lời tham khảo.
- Có thể đánh giá mức độ đúng của câu trả lời.
- Kết quả phải được ghi nhận vào tiến độ học.

Ở phiên bản đầu, việc đánh giá có thể tập trung vào việc người dùng có sử dụng đúng từ mục tiêu hay không. Cách chấm điểm chi tiết hơn có thể được mở rộng trong tương lai.

---

## 4.9. Luyện phát âm

Người dùng có thể nghe cách phát âm chuẩn của từ tiếng Anh.

Hệ thống cung cấp:

- Nút phát âm.
- Âm thanh phát âm của từ.
- Phiên âm để người dùng tham khảo.

Mục tiêu của chức năng là giúp người dùng nghe và bắt chước cách phát âm của từ.

Trong các phiên bản tương lai, hệ thống có thể mở rộng thành chức năng ghi âm giọng nói của người dùng và đánh giá mức độ tương đồng với cách phát âm mẫu.

---

## 4.10. Chế độ ôn tập tổng hợp

Ngoài việc chọn từng loại bài tập riêng lẻ, hệ thống có thể cung cấp một phiên ôn tập tổng hợp.

Một phiên có thể kết hợp:

1. Lật thẻ.
2. Trắc nghiệm nghĩa.
3. Việt → Anh.
4. Dịch câu Việt → Anh.
5. Luyện phát âm.

Hệ thống ưu tiên đưa những từ mà người dùng chưa nhớ tốt hoặc cần ôn tập lại.

---

## 5. HỆ THỐNG GHI NHẬN VÀ TIẾN ĐỘ HỌC

Hệ thống phải ghi nhận kết quả của người dùng trong quá trình học.

### 5.1. Thông tin có thể theo dõi

- Số từ đã học.
- Số từ đang học.
- Số từ đã ghi nhớ tốt.
- Số lần ôn tập.
- Số câu trả lời đúng.
- Số câu trả lời sai.
- Điểm hoặc tỷ lệ chính xác.
- Thời điểm ôn tập gần nhất.
- Thời điểm dự kiến cần ôn lại.

### 5.2. Trạng thái từ vựng

Một từ có thể được phân loại theo các trạng thái như:

- **New:** Chưa học.
- **Learning:** Đang học.
- **Review:** Đang trong quá trình ôn tập.
- **Mastered:** Đã ghi nhớ tốt.

Việc phân loại trạng thái giúp hệ thống xác định cách tiếp tục hỗ trợ người dùng.

### 5.3. Ôn tập theo mức độ ghi nhớ

Hệ thống nên ưu tiên những từ:

- Người dùng trả lời sai nhiều lần.
- Người dùng đánh giá là khó nhớ.
- Đã lâu chưa được ôn tập.
- Vừa học nhưng chưa đạt mức ghi nhớ mong muốn.

Mục tiêu là tránh việc người dùng phải ôn lại tất cả các từ với tần suất giống nhau.

---

## 6. LUỒNG SỬ DỤNG CHÍNH

### 6.1. Luồng học từ mới

```text
Đăng nhập
   ↓
Chọn danh sách từ vựng
   ↓
Chọn "Học từ mới"
   ↓
Xem từ + nghĩa + ví dụ + phát âm
   ↓
Chuyển sang từ tiếp theo
```

### 6.2. Luồng ôn tập

```text
Đăng nhập
   ↓
Chọn "Ôn tập"
   ↓
Hệ thống xác định các từ cần ôn
   ↓
Chọn dạng bài tập
   ↓
Người dùng trả lời
   ↓
Hệ thống kiểm tra kết quả
   ↓
Cập nhật tiến độ
   ↓
Chuyển sang câu tiếp theo
```

### 6.3. Luồng ôn tập tổng hợp

```text
Chọn danh sách
   ↓
Bắt đầu ôn tập
   ↓
Hệ thống chọn từ cần ôn
   ↓
Lật thẻ / Trắc nghiệm / Việt → Anh
/ Dịch câu / Phát âm
   ↓
Ghi nhận kết quả
   ↓
Cập nhật trạng thái từ
   ↓
Hoàn thành phiên ôn tập
   ↓
Hiển thị kết quả
```

---

## 7. DASHBOARD VÀ BÁO CÁO HỌC TẬP

Sau khi đăng nhập, người dùng có thể xem tổng quan quá trình học.

Dashboard nên hiển thị:

- Tổng số từ đã học.
- Số từ cần ôn hôm nay.
- Số từ đã ghi nhớ.
- Tiến độ theo từng danh sách/chủ đề.
- Điểm hoặc tỷ lệ chính xác gần đây.
- Số ngày duy trì việc học.
- Kết quả của các phiên ôn tập gần nhất.

Mục tiêu của Dashboard là giúp người dùng dễ dàng biết:

> **Hôm nay cần học gì, cần ôn gì và mình đang tiến bộ như thế nào.**

---

## 8. YÊU CẦU NGHIỆP VỤ VÀ QUY TẮC

### 8.1. Quy tắc tạo câu hỏi

Mỗi câu hỏi ôn tập phải liên quan đến từ vựng đang được kiểm tra.

Đối với câu hỏi trắc nghiệm:

- Chỉ có một đáp án đúng.
- Các phương án còn lại phải hợp lý nhưng không được gây hiểu nhầm.
- Không sử dụng cùng một đáp án đúng liên tục nếu hệ thống có thể kiểm soát việc phân bố đáp án.

### 8.2. Quy tắc đánh giá

Sau mỗi câu hỏi, hệ thống phải xác định kết quả của người dùng.

Kết quả có thể được sử dụng để:

- Cập nhật số lần đúng.
- Cập nhật số lần sai.
- Cập nhật điểm.
- Cập nhật trạng thái ghi nhớ.
- Xác định thời điểm ôn tập tiếp theo.

### 8.3. Quy tắc phát âm

Mỗi từ có phát âm tương ứng để người dùng có thể nghe.

Hệ thống nên hỗ trợ tối thiểu phát âm tiếng Anh theo một chuẩn thống nhất, đồng thời có thể mở rộng nhiều giọng phát âm trong tương lai.

### 8.4. Quy tắc phiên ôn tập

Mỗi phiên ôn tập cần:

- Xác định danh sách/tập từ được ôn.
- Tạo các câu hỏi tương ứng.
- Ghi nhận kết quả từng câu.
- Tổng hợp kết quả khi kết thúc phiên.
- Cập nhật tiến độ của các từ đã ôn.

---

## 9. YÊU CẦU TRẢI NGHIỆM NGƯỜI DÙNG

Website cần hướng đến trải nghiệm đơn giản và tập trung vào việc học.

Các nguyên tắc chính:

- Giao diện dễ hiểu đối với người mới.
- Người dùng có thể bắt đầu học trong ít bước.
- Mỗi màn hình học tập tập trung vào một nhiệm vụ.
- Phản hồi đúng/sai phải rõ ràng.
- Người dùng dễ dàng chuyển sang từ hoặc câu tiếp theo.
- Có thể sử dụng thuận tiện trên máy tính và thiết bị di động.
- Không làm người dùng mất tập trung bởi các chức năng không cần thiết.

---

## 10. TIÊU CHÍ THÀNH CÔNG VÀ ĐỊNH HƯỚNG PHÁT TRIỂN

### 10.1. Tiêu chí thành công của phiên bản đầu

Sản phẩm được xem là đáp ứng mục tiêu khi người dùng có thể:

1. Tạo hoặc chọn một danh sách từ vựng.
2. Học các từ trong danh sách.
3. Ôn từ bằng nhiều hình thức khác nhau.
4. Nghe phát âm của từ.
5. Nhận biết được từ mình nhớ tốt và từ còn yếu.
6. Nhìn thấy tiến độ học tập của bản thân.
7. Quay lại hệ thống và tiếp tục ôn những từ cần thiết.

### 10.2. Định hướng phát triển tương lai

Các phiên bản sau có thể mở rộng:

- Thuật toán Spaced Repetition nâng cao.
- Ghi âm giọng nói của người dùng.
- AI đánh giá phát âm.
- AI đánh giá câu dịch tiếng Việt → tiếng Anh.
- Sinh tự động câu ví dụ và câu hỏi.
- Gợi ý từ vựng phù hợp với trình độ.
- Phân tích điểm mạnh và điểm yếu của người học.
- Gamification: điểm, cấp độ, streak, huy hiệu.
- Bảng xếp hạng.
- Ứng dụng mobile.
- Nội dung học theo mục tiêu TOEIC, IELTS, giao tiếp và chuyên ngành.

---

# PHỤ LỤC A — TỔNG HỢP CHỨC NĂNG

| Nhóm chức năng | Chức năng | Người sử dụng |
|---|---|---|
| Tài khoản | Đăng ký | Người học |
| Tài khoản | Đăng nhập/Đăng xuất | Người học |
| Tài khoản | Quản lý hồ sơ | Người học |
| Từ vựng | Tạo danh sách | Người học |
| Từ vựng | Quản lý từ | Người học |
| Học tập | Học từ mới | Người học |
| Ôn tập | Lật thẻ | Người học |
| Ôn tập | Trắc nghiệm nghĩa | Người học |
| Ôn tập | Việt → Anh | Người học |
| Ôn tập | Dịch câu Việt → Anh | Người học |
| Phát âm | Nghe phát âm | Người học |
| Tiến độ | Theo dõi kết quả | Người học |
| Tiến độ | Xác định từ cần ôn | Hệ thống |
| Quản trị | Quản lý người dùng | Quản trị viên |
| Quản trị | Quản lý nội dung dùng chung | Quản trị viên |

---

# PHỤ LỤC B — NGUYÊN TẮC CỐT LÕI CỦA SẢN PHẨM

Sản phẩm được xây dựng dựa trên 4 nguyên tắc:

**Learn → Recall → Practice → Review**

- **Learn:** Làm quen và hiểu từ mới.
- **Recall:** Chủ động nhớ lại từ và nghĩa.
- **Practice:** Sử dụng từ trong câu và luyện phát âm.
- **Review:** Ôn lại đúng thời điểm để củng cố khả năng ghi nhớ.

Mục tiêu cuối cùng không chỉ là giúp người dùng **nhận ra một từ**, mà là giúp người dùng có thể **tự nhớ, hiểu và sử dụng từ đó trong ngữ cảnh thực tế**.
