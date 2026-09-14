# SOFTWARE REQUIREMENTS SPECIFICATION (SRS)

# WEBSITE HỌC VÀ ÔN TẬP TỪ VỰNG TIẾNG ANH

**Phiên bản:** 1.0  
**Trạng thái:** Draft for Review  
**Nguồn yêu cầu:** Business Requirements Document (BRD) phiên bản 1.0  
**Vai trò soạn thảo:** Business Analyst  

---

## 1. GIỚI THIỆU

### 1.1. Mục đích tài liệu

Tài liệu Software Requirements Specification (SRS) mô tả các yêu cầu phần mềm cần được đáp ứng để xây dựng website học và ôn tập từ vựng tiếng Anh.

SRS được xây dựng từ BRD do khách hàng cung cấp và chuyển các mục tiêu, phạm vi, quy tắc nghiệp vụ và luồng sử dụng ở cấp độ nghiệp vụ thành các yêu cầu có thể:

- Phân tích và thiết kế.
- Phát triển.
- Kiểm thử và nghiệm thu.
- Theo dõi phạm vi trong quá trình phát triển.

Tài liệu này tập trung vào **hệ thống phải làm gì** và **hệ thống phải đáp ứng điều kiện gì**. Các quyết định triển khai cụ thể như framework, ngôn ngữ lập trình, cơ sở dữ liệu, kiến trúc mã nguồn và hạ tầng có thể được đặc tả trong tài liệu thiết kế kỹ thuật riêng.

### 1.2. Phạm vi hệ thống

Hệ thống là một website hỗ trợ người dùng học, ghi nhớ và ôn tập từ vựng tiếng Anh thông qua nguyên tắc:

> **Learn → Recall → Practice → Review**

Hệ thống cho phép người học quản lý danh sách từ vựng, học từ mới, thực hiện nhiều dạng bài tập, nghe phát âm, theo dõi kết quả và xác định các từ cần ôn tập.

Hệ thống cũng cung cấp khu vực quản trị để quản trị viên quản lý người dùng và nội dung dùng chung.

### 1.3. Đối tượng sử dụng tài liệu

Tài liệu này dành cho:

- Business Analyst.
- Project Manager / Product Owner.
- UI/UX Designer.
- Frontend Developer.
- Backend Developer.
- QA / Tester.
- DevOps / System Administrator khi cần triển khai hệ thống.
- Khách hàng hoặc đại diện nghiệp vụ thực hiện review và nghiệm thu.

### 1.4. Thuật ngữ

| Thuật ngữ | Giải thích |
|---|---|
| User / Người học | Người sử dụng hệ thống để học và ôn tập từ vựng |
| Admin / Quản trị viên | Người quản lý người dùng và nội dung dùng chung |
| Vocabulary | Một mục từ vựng tiếng Anh |
| List / Danh sách | Tập các từ vựng do người dùng tổ chức theo mục đích học |
| Topic / Chủ đề | Chủ đề phân loại từ vựng |
| Review | Hoạt động ôn tập các từ đã học |
| Review Session | Một phiên ôn tập gồm nhiều câu hỏi/bài tập |
| Target Word | Từ vựng mà câu hỏi hiện tại đang kiểm tra |
| Mastered | Trạng thái từ đã ghi nhớ tốt |
| Due for Review | Từ đến thời điểm được hệ thống xác định cần ôn lại |

---

## 2. TỔNG QUAN HỆ THỐNG

### 2.1. Mục tiêu hệ thống

Hệ thống phải hỗ trợ người học:

1. Tạo và tổ chức danh sách từ vựng.
2. Học từ mới theo từng danh sách.
3. Ôn tập bằng nhiều dạng bài tập.
4. Chủ động truy xuất từ thay vì chỉ đọc thông tin.
5. Nghe phát âm chuẩn của từ.
6. Theo dõi kết quả và tiến độ học tập.
7. Xác định các từ còn yếu để ưu tiên ôn tập.

### 2.2. Actor

| Actor | Mô tả | Quyền chính |
|---|---|---|
| Người học | Người dùng chính của hệ thống | Quản lý tài khoản, danh sách, từ vựng; học; ôn tập; luyện phát âm; xem tiến độ |
| Quản trị viên | Quản lý vận hành và nội dung | Quản lý người dùng, nội dung từ vựng dùng chung, chủ đề dùng chung, xử lý dữ liệu không phù hợp/sai |
| Hệ thống | Thành phần tự động thực hiện các quy tắc nghiệp vụ | Chấm câu hỏi, ghi nhận kết quả, cập nhật tiến độ, xác định từ cần ôn, tạo phiên/câu hỏi theo quy tắc |

### 2.3. Phạm vi phiên bản 1.0

#### Trong phạm vi

- Đăng ký.
- Đăng nhập/đăng xuất.
- Quản lý hồ sơ.
- Thay đổi mật khẩu.
- Khôi phục mật khẩu.
- Xóa tài khoản.
- Tạo và quản lý danh sách/chủ đề từ vựng.
- Quản lý từ vựng.
- Học từ mới.
- Ôn tập bằng lật thẻ.
- Trắc nghiệm nghĩa.
- Việt → Anh.
- Dịch câu Việt → Anh.
- Nghe phát âm.
- Ghi nhận kết quả.
- Theo dõi tiến độ.
- Dashboard.
- Xác định từ cần ôn.
- Quản trị người dùng.
- Quản trị nội dung dùng chung.

#### Ngoài phạm vi

- Khóa học video hoàn chỉnh.
- Lớp học trực tuyến với giáo viên.
- Mạng xã hội.
- Hệ thống thi/chứng chỉ.
- Thanh toán/gói thuê bao.
- Mobile native app.
- AI đánh giá phát âm người dùng.
- AI đánh giá câu dịch ở mức nâng cao.
- Các tính năng gamification nâng cao.
- Bảng xếp hạng.

---

## 3. YÊU CẦU CHỨC NĂNG

> Quy ước: **Must** = bắt buộc trong phiên bản 1.0; **Should** = nên có trong phiên bản 1.0 nhưng có thể cần xác nhận ưu tiên; **TBD** = BRD chưa quy định đủ để đặc tả chi tiết.

### 3.1. Quản lý tài khoản

#### FR-AUTH-001 — Đăng ký tài khoản

**Priority:** Must  
**Actor:** Người học

Hệ thống phải cho phép người học tạo tài khoản mới.

**Luồng chính:**
1. Người dùng mở chức năng đăng ký.
2. Người dùng nhập các thông tin bắt buộc.
3. Hệ thống kiểm tra dữ liệu đầu vào.
4. Hệ thống kiểm tra tình trạng tài khoản theo thông tin định danh.
5. Hệ thống tạo tài khoản.
6. Hệ thống thông báo đăng ký thành công hoặc yêu cầu bước xác minh nếu có quy định xác minh.

**Yêu cầu dữ liệu/validation:**

- Trường bắt buộc phải được nhập.
- Email phải có định dạng hợp lệ.
- Thông tin định danh không được trùng với tài khoản đã tồn tại theo chính sách hệ thống.
- Chính sách độ dài/mật khẩu: **TBD**.

**Acceptance Criteria:**

- Đăng ký với dữ liệu hợp lệ tạo được tài khoản.
- Dữ liệu không hợp lệ phải được thông báo lỗi rõ ràng.
- Không tạo tài khoản trùng theo quy tắc định danh.

#### FR-AUTH-002 — Đăng nhập

**Priority:** Must  
**Actor:** Người học, Quản trị viên

Hệ thống phải xác thực người dùng và cho phép truy cập các chức năng phù hợp với vai trò.

**Acceptance Criteria:**

- Thông tin hợp lệ → đăng nhập thành công.
- Thông tin không hợp lệ → không đăng nhập và hiển thị thông báo lỗi.
- Tài khoản không được phép hoạt động → hệ thống từ chối truy cập.

#### FR-AUTH-003 — Đăng xuất

Hệ thống phải cho phép người dùng đăng xuất khỏi phiên đăng nhập hiện tại.

#### FR-AUTH-004 — Quản lý hồ sơ

Người học phải có thể xem và cập nhật thông tin cá nhân mà hệ thống cho phép.

**TBD:** Danh sách trường hồ sơ cụ thể và quy tắc chỉnh sửa.

#### FR-AUTH-005 — Thay đổi mật khẩu

Người học có thể thay đổi mật khẩu sau khi đã xác thực theo chính sách bảo mật của hệ thống.

**TBD:** Chính sách mật khẩu và yêu cầu xác minh lại danh tính.

#### FR-AUTH-006 — Khôi phục mật khẩu

Hệ thống phải hỗ trợ người dùng khôi phục quyền truy cập khi quên mật khẩu.

**TBD:** Cơ chế xác minh, thời hạn mã/liên kết và giới hạn số lần yêu cầu chưa được BRD quy định.

#### FR-AUTH-007 — Xóa tài khoản

Người học phải có thể yêu cầu xóa tài khoản theo quy định của hệ thống.

**TBD:** Cách xử lý dữ liệu lịch sử học tập sau khi xóa tài khoản.

---

### 3.2. Quản lý danh sách/chủ đề

#### FR-LIST-001 — Tạo danh sách

Người học phải có thể tạo một danh sách từ vựng mới.

**Examples:** Công việc, Du lịch, Công nghệ, Giao tiếp hằng ngày, TOEIC, IELTS, chủ đề tự tạo.

**Acceptance Criteria:**

- Tên danh sách hợp lệ → tạo thành công.
- Danh sách mới thuộc quyền sở hữu của người tạo.
- Danh sách có thể được mở để thêm từ.

**TBD:** Độ dài tên, ký tự cho phép, trạng thái trùng tên.

#### FR-LIST-002 — Đổi tên danh sách

Người học có thể đổi tên danh sách mà mình có quyền quản lý.

#### FR-LIST-003 — Xóa danh sách

Người học có thể xóa danh sách của mình.

**Business Rule:** Xóa danh sách không được phép làm ảnh hưởng ngoài phạm vi dữ liệu mà người dùng sở hữu, trừ khi có quy định khác.

**TBD:** Chính sách xóa mềm/xóa vĩnh viễn và xử lý các từ dùng chung trong nhiều danh sách.

#### FR-LIST-004 — Xem danh sách

Người học phải có thể xem các danh sách mình có quyền truy cập.

#### FR-LIST-005 — Thêm từ vào danh sách

Người học có thể thêm từ vựng vào danh sách.

#### FR-LIST-006 — Xóa từ khỏi danh sách

Người học có thể loại bỏ từ khỏi danh sách.

**TBD:** Xóa khỏi danh sách có xóa bản ghi từ vựng hay chỉ xóa liên kết giữa từ và danh sách.

#### FR-LIST-007 — Chủ đề dùng chung

Quản trị viên phải có thể quản lý chủ đề từ vựng dùng chung của hệ thống.

---

### 3.3. Quản lý từ vựng

#### FR-VOC-001 — Thêm từ vựng

Người học phải có thể tạo từ vựng mới trong phạm vi danh sách được phép chỉnh sửa.

**Thông tin có thể bao gồm:**

- Từ tiếng Anh.
- Nghĩa tiếng Việt.
- Từ loại.
- Câu ví dụ tiếng Anh.
- Câu ví dụ tiếng Việt.
- Phiên âm.
- Phát âm tiếng Anh.
- Thông tin bổ sung liên quan.

**Validation:**

- Từ tiếng Anh và nghĩa phải được kiểm tra là dữ liệu hợp lệ.
- Trường bắt buộc cụ thể: **TBD**.

#### FR-VOC-002 — Chỉnh sửa từ vựng

Người học có quyền phải có thể chỉnh sửa thông tin của từ.

#### FR-VOC-003 — Xóa từ vựng

Người học có quyền phải có thể xóa từ theo phạm vi sở hữu/quyền truy cập.

#### FR-VOC-004 — Xem chi tiết từ

Hệ thống phải hiển thị thông tin chi tiết của từ.

#### FR-VOC-005 — Tra cứu từ

Người học phải có thể tìm/tra cứu các từ trong danh sách học tập.

**TBD:** Quy tắc tìm kiếm theo từ tiếng Anh, nghĩa, từ loại, chủ đề và mức độ tiến độ.

#### FR-VOC-006 — Quản trị nội dung dùng chung

Quản trị viên phải có thể quản lý các từ vựng dùng chung của hệ thống và xử lý dữ liệu không phù hợp hoặc sai.

---

### 3.4. Học từ mới

#### FR-LEARN-001 — Bắt đầu học từ mới

Người học có thể chọn một danh sách và bắt đầu chế độ học từ mới.

**Luồng chính:**
1. Người học chọn danh sách.
2. Chọn “Học từ mới”.
3. Hệ thống lấy các từ phù hợp trong danh sách.
4. Hệ thống hiển thị nội dung từ.
5. Người học xem và chuyển sang từ kế tiếp.

#### FR-LEARN-002 — Hiển thị thông tin từ khi học

Màn hình học phải có thể hiển thị:

- Từ tiếng Anh.
- Nghĩa tiếng Việt.
- Từ loại.
- Phiên âm.
- Câu ví dụ.
- Nút nghe phát âm.
- Thông tin bổ sung nếu có.

#### FR-LEARN-003 — Chuyển từ

Người học có thể chuyển sang từ tiếp theo trong phiên học.

**TBD:** Cách xác định thứ tự từ, có bỏ qua từ đã học hay không.

---

### 3.5. Ôn tập bằng lật thẻ

#### FR-REVIEW-FLASH-001 — Hiển thị mặt trước

Hệ thống hiển thị từ tiếng Anh ở mặt trước của thẻ.

#### FR-REVIEW-FLASH-002 — Lật thẻ

Người học chọn “Lật thẻ” để xem đáp án/nghĩa của từ.

#### FR-REVIEW-FLASH-003 — Đánh giá khả năng nhớ

Sau khi lật thẻ, người học có thể đánh giá:

- Nhớ.
- Không nhớ.
- Khó nhớ.

#### FR-REVIEW-FLASH-004 — Ghi nhận kết quả lật thẻ

Hệ thống phải ghi nhận đánh giá và sử dụng kết quả để cập nhật tiến độ và ưu tiên ôn tập.

---

### 3.6. Trắc nghiệm nghĩa của từ

#### FR-QUIZ-MCQ-001 — Tạo câu hỏi trắc nghiệm

Hệ thống phải đưa ra một từ tiếng Anh và nhiều phương án trả lời bằng tiếng Việt.

#### FR-QUIZ-MCQ-002 — Chỉ một đáp án đúng

Mỗi câu hỏi phải có đúng một đáp án đúng.

#### FR-QUIZ-MCQ-003 — Kiểm tra câu trả lời

Sau khi người học chọn đáp án, hệ thống phải:

1. Xác định đúng/sai.
2. Hiển thị đáp án đúng.
3. Ghi nhận kết quả.
4. Cập nhật tiến độ từ.

#### BR-QUIZ-001 — Chất lượng phương án

Các phương án sai phải hợp lý nhưng không được gây hiểu nhầm không cần thiết.

#### BR-QUIZ-002 — Phân bố đáp án đúng

Hệ thống nên tránh để đáp án đúng xuất hiện liên tục ở cùng một vị trí khi hệ thống có khả năng kiểm soát.

---

### 3.7. Việt → Anh

#### FR-QUIZ-V2E-001 — Hiển thị nghĩa tiếng Việt

Hệ thống phải hiển thị nghĩa tiếng Việt của từ mục tiêu và yêu cầu người học nhập từ tiếng Anh tương ứng.

#### FR-QUIZ-V2E-002 — Kiểm tra câu trả lời

Hệ thống phải kiểm tra câu trả lời và xác định đúng/sai.

**TBD:**

- Không phân biệt hoa/thường hay có.
- Xử lý khoảng trắng thừa.
- Chấp nhận biến thể từ/cách viết khác.
- Xử lý lỗi chính tả gần đúng.
- Từ đồng nghĩa có được chấp nhận hay không.

Các điểm trên phải được xác định trước khi phát triển chức năng chấm điểm chính thức.

---

### 3.8. Dịch câu Việt → Anh

#### FR-QUIZ-SENT-001 — Hiển thị câu hỏi

Hệ thống phải hiển thị một câu tiếng Việt gắn với từ vựng đang được ôn tập.

#### FR-QUIZ-SENT-002 — Nhập câu trả lời

Người học phải có thể nhập câu tiếng Anh tương ứng.

#### FR-QUIZ-SENT-003 — Hiển thị đáp án tham khảo

Sau khi trả lời, hệ thống phải cung cấp câu trả lời tham khảo.

#### FR-QUIZ-SENT-004 — Đánh giá câu trả lời

Trong phiên bản 1.0, hệ thống có thể đánh giá tập trung vào việc người dùng có sử dụng đúng từ mục tiêu hay không.

**TBD:** Cơ chế chấm điểm chi tiết và ngưỡng đúng/sai phải được xác nhận trước khi triển khai.

#### FR-QUIZ-SENT-005 — Ghi nhận kết quả

Kết quả phải được lưu vào tiến độ học của từ mục tiêu.

---

### 3.9. Luyện phát âm

#### FR-SPEECH-001 — Nghe phát âm

Người học phải có thể nghe âm thanh phát âm của từ.

#### FR-SPEECH-002 — Hiển thị phiên âm

Hệ thống phải hiển thị phiên âm để người học tham khảo.

#### FR-SPEECH-003 — Chuẩn phát âm

Hệ thống phải cung cấp tối thiểu một chuẩn phát âm tiếng Anh nhất quán trong phiên bản 1.0.

**TBD:** Chuẩn phát âm cụ thể và lựa chọn giọng cần được Product Owner xác nhận.

---

### 3.10. Phiên ôn tập

#### FR-SESSION-001 — Bắt đầu phiên ôn tập

Hệ thống phải cho phép người học bắt đầu một phiên ôn tập từ danh sách đã chọn.

#### FR-SESSION-002 — Xác định từ cần ôn

Khi bắt đầu phiên, hệ thống phải xác định tập từ phù hợp để ôn dựa trên trạng thái và dữ liệu tiến độ.

#### FR-SESSION-003 — Chọn dạng bài tập

Hệ thống phải hỗ trợ các dạng bài tập nằm trong phạm vi phiên bản 1.0.

#### FR-SESSION-004 — Ghi nhận từng câu

Mỗi câu hỏi trong phiên phải được ghi nhận kết quả riêng biệt.

#### FR-SESSION-005 — Hoàn thành phiên

Khi phiên kết thúc, hệ thống phải:

1. Tổng hợp kết quả.
2. Cập nhật tiến độ của các từ đã ôn.
3. Hiển thị kết quả cho người học.

#### FR-SESSION-006 — Ôn tập tổng hợp

Hệ thống có thể kết hợp:

- Lật thẻ.
- Trắc nghiệm nghĩa.
- Việt → Anh.
- Dịch câu Việt → Anh.
- Luyện phát âm.

Hệ thống nên ưu tiên các từ chưa nhớ tốt hoặc đến thời điểm cần ôn.

---

### 3.11. Theo dõi tiến độ học tập

#### FR-PROGRESS-001 — Ghi nhận kết quả

Hệ thống phải ghi nhận kết quả học và ôn tập của người dùng.

#### FR-PROGRESS-002 — Chỉ số học tập

Hệ thống phải có khả năng theo dõi các thông tin:

- Số từ đã học.
- Số từ đang học.
- Số từ đã ghi nhớ tốt.
- Số lần ôn tập.
- Số câu trả lời đúng.
- Số câu trả lời sai.
- Điểm hoặc tỷ lệ chính xác.
- Thời điểm ôn tập gần nhất.
- Thời điểm dự kiến cần ôn lại.

#### FR-PROGRESS-003 — Trạng thái từ

Một từ có thể ở một trong các trạng thái:

- **New** — Chưa học.
- **Learning** — Đang học.
- **Review** — Đang trong quá trình ôn tập.
- **Mastered** — Đã ghi nhớ tốt.

#### BR-PROGRESS-001 — Ưu tiên từ cần ôn

Hệ thống nên ưu tiên các từ:

- Trả lời sai nhiều lần.
- Được đánh giá “Khó nhớ”.
- Đã lâu chưa được ôn.
- Vừa học nhưng chưa đạt mức ghi nhớ mong muốn.

#### BR-PROGRESS-002 — Cập nhật sau kết quả

Kết quả một hoạt động học/ôn tập có thể làm thay đổi:

- Số lần ôn.
- Số lần đúng/sai.
- Điểm/tỷ lệ chính xác.
- Trạng thái ghi nhớ.
- Thời điểm ôn tập tiếp theo.

**TBD:** Thuật toán và ngưỡng chuyển trạng thái/đặt lịch ôn lại chưa được BRD quy định. Đây là một hạng mục cần Product Owner phê duyệt trước khi chốt acceptance test chi tiết.

---

### 3.12. Dashboard

#### FR-DASH-001 — Hiển thị tổng quan học tập

Sau khi đăng nhập, người học phải có thể xem Dashboard.

Dashboard nên hiển thị:

- Tổng số từ đã học.
- Số từ cần ôn hôm nay.
- Số từ đã ghi nhớ.
- Tiến độ theo từng danh sách/chủ đề.
- Điểm hoặc tỷ lệ chính xác gần đây.
- Số ngày duy trì việc học.
- Kết quả các phiên ôn gần nhất.

#### FR-DASH-002 — Cập nhật dữ liệu

Các số liệu Dashboard phải phản ánh dữ liệu học tập đã được hệ thống ghi nhận.

**TBD:** Định nghĩa chính xác “ngày duy trì việc học” và cách tính streak.

---

### 3.13. Quản trị người dùng

#### FR-ADMIN-USER-001 — Xem người dùng

Quản trị viên phải có thể xem danh sách người dùng.

#### FR-ADMIN-USER-002 — Quản lý người dùng

Quản trị viên phải có thể thực hiện các thao tác quản lý người dùng theo quyền được cấp.

**TBD:** Khóa/mở khóa, chỉnh sửa, xóa, tìm kiếm, lọc chưa được BRD mô tả chi tiết.

---

### 3.14. Quản trị nội dung dùng chung

#### FR-ADMIN-CONTENT-001 — Quản lý từ vựng dùng chung

Quản trị viên phải có thể tạo, xem, cập nhật và xử lý dữ liệu từ vựng dùng chung.

#### FR-ADMIN-CONTENT-002 — Quản lý chủ đề dùng chung

Quản trị viên phải có thể tạo, xem, cập nhật và xử lý chủ đề dùng chung.

#### FR-ADMIN-CONTENT-003 — Xử lý nội dung không phù hợp/sai

Quản trị viên phải có khả năng xử lý nội dung không phù hợp hoặc dữ liệu sai theo chính sách vận hành.

**TBD:** Quy trình và trạng thái xử lý nội dung chưa được BRD xác định.

---

## 4. QUY TẮC NGHIỆP VỤ

### BR-001 — Quyền truy cập dữ liệu

Người học chỉ được quản lý các danh sách/từ vựng thuộc phạm vi quyền của mình hoặc các nội dung dùng chung được hệ thống cho phép truy cập.

### BR-002 — Câu hỏi phải gắn với từ mục tiêu

Mỗi câu hỏi ôn tập phải liên quan đến từ vựng đang được kiểm tra.

### BR-003 — Một đáp án đúng cho trắc nghiệm

Mỗi câu hỏi trắc nghiệm nghĩa phải có đúng một đáp án đúng.

### BR-004 — Phương án sai phải hợp lý

Phương án sai phải đủ hợp lý để kiểm tra kiến thức nhưng không được gây hiểu nhầm không cần thiết.

### BR-005 — Ghi nhận kết quả

Sau mỗi hoạt động đánh giá, hệ thống phải ghi nhận kết quả để phục vụ theo dõi tiến độ.

### BR-006 — Cập nhật trạng thái từ

Kết quả học tập phải có khả năng ảnh hưởng đến trạng thái ghi nhớ của từ.

### BR-007 — Xác định từ cần ôn

Hệ thống phải sử dụng thông tin lịch sử học tập để xác định các từ nên được ưu tiên ôn tập.

### BR-008 — Cấu trúc phiên ôn tập

Mỗi phiên phải xác định tập từ, tạo câu hỏi tương ứng, ghi nhận từng kết quả và tổng hợp khi kết thúc.

### BR-009 — Phát âm

Mỗi từ có thông tin phát âm tương ứng để người học có thể nghe.

### BR-010 — Trạng thái từ

Hệ thống hỗ trợ các trạng thái nghiệp vụ New, Learning, Review và Mastered.

---

## 5. USE CASES

### UC-01 — Đăng ký tài khoản

**Actor chính:** Người học  
**Pre-condition:** Người dùng chưa có phiên đăng nhập.  
**Post-condition:** Tài khoản được tạo nếu thông tin hợp lệ.

**Main Flow:**
1. Người dùng chọn Đăng ký.
2. Hệ thống hiển thị form.
3. Người dùng nhập dữ liệu.
4. Hệ thống validate.
5. Hệ thống tạo tài khoản.
6. Hệ thống thông báo kết quả.

**Alternative/Exception:**
- Dữ liệu không hợp lệ.
- Tài khoản đã tồn tại.
- Hệ thống không thể hoàn tất thao tác.

### UC-02 — Học từ mới

**Actor chính:** Người học  
**Pre-condition:** Người dùng đã đăng nhập và có danh sách hợp lệ.  
**Post-condition:** Người học xem được nội dung từ trong phiên học.

**Main Flow:**
1. Chọn danh sách.
2. Chọn Học từ mới.
3. Hệ thống chọn/hiển thị từ.
4. Hiển thị thông tin từ.
5. Người học nghe phát âm nếu cần.
6. Chuyển sang từ kế tiếp.

### UC-03 — Ôn tập từ

**Actor chính:** Người học  
**Pre-condition:** Có ít nhất một từ phù hợp để ôn.  
**Post-condition:** Kết quả từng câu được ghi nhận và tiến độ được cập nhật.

**Main Flow:**
1. Chọn Ôn tập.
2. Hệ thống xác định từ cần ôn.
3. Người dùng chọn dạng bài.
4. Hệ thống hiển thị câu hỏi.
5. Người dùng trả lời/đánh giá.
6. Hệ thống chấm kết quả.
7. Hệ thống cập nhật tiến độ.
8. Hệ thống chuyển câu tiếp theo.
9. Kết thúc phiên và hiển thị tổng kết.

### UC-04 — Quản lý danh sách từ

**Actor chính:** Người học  
**Pre-condition:** Người dùng đã đăng nhập.

**Main Flow:**
1. Người dùng mở danh sách.
2. Tạo/đổi tên/xem/xóa danh sách.
3. Thêm hoặc xóa từ.
4. Hệ thống lưu thay đổi.

### UC-05 — Quản trị nội dung

**Actor chính:** Quản trị viên  
**Pre-condition:** Quản trị viên đã đăng nhập với quyền phù hợp.

**Main Flow:**
1. Mở khu vực quản trị.
2. Chọn người dùng hoặc nội dung.
3. Xem dữ liệu.
4. Thực hiện thao tác được phép.
5. Hệ thống validate và lưu thay đổi.

---

## 6. YÊU CẦU DỮ LIỆU

### 6.1. Thực thể mức nghiệp vụ

| Entity | Mô tả | Dữ liệu chính |
|---|---|---|
| User | Tài khoản người dùng | Định danh, thông tin đăng nhập, thông tin hồ sơ, vai trò, trạng thái |
| Vocabulary List | Danh sách từ của người học | Tên, người sở hữu, trạng thái |
| Topic | Chủ đề từ vựng | Tên, phạm vi dùng chung/cá nhân |
| Vocabulary | Từ vựng | Word, meaning, part of speech, examples, pronunciation, audio, metadata |
| Review Session | Phiên học/ôn | Người dùng, danh sách/tập từ, thời gian, trạng thái, kết quả tổng hợp |
| Review Attempt | Kết quả từng câu/hoạt động | Từ mục tiêu, loại bài, câu trả lời, đúng/sai, đánh giá, thời gian |
| Vocabulary Progress | Tiến độ của người dùng đối với từ | Trạng thái, số lần ôn, đúng/sai, score/accuracy, lần ôn gần nhất, lần ôn kế tiếp |

### 6.2. Quan hệ nghiệp vụ chính

- Một người học có thể có nhiều danh sách.
- Một danh sách có thể chứa nhiều từ vựng.
- Một từ vựng có thể xuất hiện trong nhiều danh sách nếu nghiệp vụ cho phép.
- Một người học có lịch sử tiến độ riêng đối với từng từ.
- Một phiên ôn tập có nhiều lần trả lời.
- Một lần trả lời thuộc về một từ mục tiêu.

**TBD:** Quan hệ chính thức giữa Topic, Vocabulary và List cần được chốt ở data model trước khi thiết kế database.

### 6.3. Dữ liệu lịch sử học tập

Hệ thống phải lưu đủ thông tin cần thiết để:

- Tính các chỉ số tiến độ.
- Hiển thị lịch sử gần đây.
- Xác định từ cần ôn.
- Cập nhật trạng thái ghi nhớ.
- Tổng hợp kết quả phiên học.

---

## 7. YÊU CẦU GIAO DIỆN VÀ TRẢI NGHIỆM

### NFR-UX-001 — Dễ sử dụng

Giao diện phải dễ hiểu đối với người mới.

### NFR-UX-002 — Ít bước để bắt đầu học

Người dùng đã đăng nhập phải có thể bắt đầu học/ôn với số thao tác tối thiểu hợp lý.

### NFR-UX-003 — Tập trung vào một nhiệm vụ

Mỗi màn hình học tập nên tập trung vào một nhiệm vụ chính.

### NFR-UX-004 — Phản hồi rõ ràng

Kết quả đúng/sai và đáp án đúng phải được hiển thị rõ ràng.

### NFR-UX-005 — Điều hướng bài tập

Người dùng phải dễ dàng chuyển sang từ/câu tiếp theo.

### NFR-UX-006 — Responsive

Website phải sử dụng thuận tiện trên máy tính và thiết bị di động.

### NFR-UX-007 — Không gây xao nhãng

Các thành phần không cần thiết không nên làm giảm sự tập trung khi học.

---

## 8. YÊU CẦU PHI CHỨC NĂNG

> BRD chủ yếu mô tả nghiệp vụ. Các chỉ số cụ thể dưới đây cần được xác nhận trong giai đoạn đặc tả kỹ thuật nếu dự án yêu cầu SLA/SLO chính thức.

### NFR-SEC-001 — Xác thực

Các chức năng yêu cầu tài khoản phải chỉ có thể truy cập sau khi người dùng được xác thực.

### NFR-SEC-002 — Phân quyền

Hệ thống phải phân biệt ít nhất quyền của Người học và Quản trị viên.

### NFR-SEC-003 — Bảo vệ dữ liệu người dùng

Dữ liệu cá nhân và lịch sử học tập phải được bảo vệ khỏi truy cập trái phép.

### NFR-SEC-004 — Bảo vệ dữ liệu đầu vào

Các dữ liệu nhập từ người dùng phải được kiểm tra trước khi xử lý/lưu trữ.

### NFR-PERF-001 — Phản hồi chức năng học tập

Các thao tác thông thường trong phiên học/ôn phải có thời gian phản hồi phù hợp để không làm gián đoạn quá trình học.

**Target:** TBD.

### NFR-PERF-002 — Đồng thời

Hệ thống phải hỗ trợ số lượng người dùng đồng thời theo quy mô kinh doanh được phê duyệt.

**Target:** TBD.

### NFR-AVAIL-001 — Sẵn sàng

Website phải có mức độ sẵn sàng phù hợp với nhu cầu sử dụng của sản phẩm.

**Target:** TBD.

### NFR-DATA-001 — Tính toàn vẹn

Kết quả học tập và tiến độ phải được lưu nhất quán, tránh mất hoặc ghi sai kết quả khi một hoạt động hoàn tất.

### NFR-COMP-001 — Tương thích trình duyệt

Website phải hoạt động trên các trình duyệt hiện đại được dự án hỗ trợ.

**Danh sách trình duyệt cụ thể:** TBD.

### NFR-RESP-001 — Responsive

Các màn hình chính phải hỗ trợ kích thước màn hình desktop và mobile web.

### NFR-ACCESS-001 — Khả năng sử dụng

Các thành phần tương tác và thông báo cần được thiết kế đủ rõ ràng để người dùng có thể hiểu trạng thái và hành động tiếp theo.

---

## 9. QUY TẮC VALIDATION VÀ ERROR HANDLING

### 9.1. Nguyên tắc chung

1. Không cho phép lưu dữ liệu không hợp lệ.
2. Thông báo lỗi phải chỉ ra vấn đề ở mức người dùng có thể hiểu.
3. Lỗi nghiệp vụ không được làm mất dữ liệu hợp lệ đã nhập.
4. Các thao tác cập nhật quan trọng phải trả về trạng thái thành công/thất bại rõ ràng.

### 9.2. Validation theo nhóm chức năng

| Nhóm | Validation tối thiểu |
|---|---|
| Tài khoản | Dữ liệu bắt buộc, định dạng email, chính sách mật khẩu |
| Danh sách | Tên danh sách hợp lệ |
| Từ vựng | Từ và các trường bắt buộc phải hợp lệ |
| Trắc nghiệm | Phải có đúng một đáp án đúng |
| Việt → Anh | So sánh câu trả lời với đáp án theo quy tắc chấm |
| Dịch câu | Kiểm tra sự tồn tại của từ mục tiêu và quy tắc đánh giá |
| Phiên ôn | Phiên phải có tập từ hợp lệ |

### 9.3. Trường hợp không có từ để ôn

Nếu hệ thống không xác định được từ nào cần ôn, hệ thống phải thông báo trạng thái phù hợp thay vì tạo phiên rỗng.

**Thông điệp cụ thể:** TBD.

### 9.4. Lỗi phát âm

Nếu không thể phát audio, hệ thống phải thông báo lỗi và không làm mất trạng thái học tập hiện tại.

---

## 10. PHÂN QUYỀN

| Chức năng | Người học | Admin |
|---|---:|---:|
| Đăng ký | ✓ | — |
| Đăng nhập | ✓ | ✓ |
| Quản lý hồ sơ | ✓ | Theo quyền quản trị |
| Tạo danh sách cá nhân | ✓ | — |
| Quản lý từ cá nhân | ✓ | — |
| Học/Ôn tập | ✓ | Không bắt buộc |
| Xem tiến độ cá nhân | ✓ | Theo nhu cầu vận hành |
| Quản lý người dùng | — | ✓ |
| Quản lý từ dùng chung | — | ✓ |
| Quản lý chủ đề dùng chung | — | ✓ |
| Xử lý dữ liệu sai/không phù hợp | — | ✓ |

**Lưu ý:** Chi tiết permission matrix ở cấp API/màn hình cần được chốt trong tài liệu thiết kế và security specification.

---

## 11. YÊU CẦU ĐỐI VỚI CÁC DẠNG BÀI TẬP

### 11.1. Flashcard

**Input:** Từ mục tiêu.  
**Output:** Từ → lật → nghĩa/đáp án → đánh giá nhớ.  
**Result:** Nhớ / Không nhớ / Khó nhớ.

### 11.2. Multiple Choice

**Input:** Từ mục tiêu + 4 lựa chọn hoặc số lựa chọn theo cấu hình.  
**Output:** Đúng/Sai + đáp án đúng.  
**Result:** Correct / Incorrect.

**TBD:** Số lượng phương án chính thức.

### 11.3. Vietnamese → English

**Input:** Nghĩa tiếng Việt.  
**Output:** Người dùng nhập từ tiếng Anh.  
**Result:** Correct / Incorrect.

### 11.4. Vietnamese Sentence → English

**Input:** Câu tiếng Việt.  
**Output:** Người dùng nhập câu tiếng Anh.  
**Result:** Đánh giá theo từ mục tiêu trong phiên bản 1.0; mức đánh giá chi tiết là TBD.

### 11.5. Pronunciation

**Input:** Từ tiếng Anh.  
**Output:** Audio + phiên âm.  
**Result:** Hệ thống ghi nhận việc luyện phát âm nếu cần cho thống kê; BRD chưa bắt buộc lưu một kết quả chấm điểm phát âm trong phiên bản 1.0.

---

## 12. QUY TẮC TIẾN ĐỘ VÀ ÔN TẬP

### 12.1. Trạng thái từ

| Trạng thái | Ý nghĩa nghiệp vụ |
|---|---|
| New | Người dùng chưa học từ |
| Learning | Người dùng đang học từ |
| Review | Người dùng đang ở giai đoạn ôn tập |
| Mastered | Người dùng đã ghi nhớ tốt |

### 12.2. Sự kiện làm thay đổi tiến độ

Các sự kiện có thể cập nhật tiến độ:

- Hoàn thành hoạt động flashcard và đánh giá.
- Trả lời trắc nghiệm.
- Trả lời Việt → Anh.
- Thực hiện bài dịch câu.
- Hoàn thành phiên ôn tập.

### 12.3. Xác định từ cần ôn

Hệ thống cần xét tối thiểu các tín hiệu nghiệp vụ được BRD nêu:

- Sai nhiều lần.
- Khó nhớ.
- Thời gian từ lần ôn gần nhất đã lâu.
- Vừa học và chưa đạt mức mong muốn.

### 12.4. Thuật toán Spaced Repetition

BRD định hướng phát triển **Spaced Repetition nâng cao** cho các phiên bản tương lai, vì vậy SRS phiên bản 1.0 không mặc định áp đặt một thuật toán cụ thể.

**TBD trước khi triển khai production:**

- Công thức điểm.
- Ngưỡng chuyển trạng thái.
- Công thức Next Review At.
- Mức độ ảnh hưởng của từng loại bài tập.
- Trọng số của “Remember / Don't remember / Hard”.

---

## 13. DASHBOARD VÀ BÁO CÁO

### 13.1. Dashboard người học

| Metric | Ý nghĩa |
|---|---|
| Total Learned | Tổng số từ đã học |
| Review Today | Số từ cần ôn hôm nay |
| Mastered | Số từ đã ghi nhớ tốt |
| Progress by List/Topic | Tiến độ theo danh sách/chủ đề |
| Recent Accuracy | Điểm/tỷ lệ chính xác gần đây |
| Learning Streak | Số ngày duy trì việc học |
| Recent Sessions | Các phiên ôn gần nhất |

### 13.2. Báo cáo phiên ôn tập

Sau khi kết thúc phiên, hệ thống nên hiển thị:

- Tổng số câu.
- Số câu đúng.
- Số câu sai.
- Tỷ lệ chính xác.
- Danh sách từ cần chú ý.
- Trạng thái/tiến độ được cập nhật.

**TBD:** Có hiển thị điểm tổng hợp hay không và công thức tính.

---

## 14. YÊU CẦU KIỂM THỬ VÀ NGHIỆM THU

### 14.1. Nguyên tắc

Mỗi yêu cầu chức năng Must phải có ít nhất một test case tương ứng.

### 14.2. Traceability cơ bản

| Requirement | Test focus |
|---|---|
| FR-AUTH-001 | Tạo tài khoản hợp lệ/không hợp lệ/trùng |
| FR-AUTH-002 | Đăng nhập đúng/sai/quyền |
| FR-LIST-001 | Tạo danh sách |
| FR-LIST-005 | Thêm từ vào danh sách |
| FR-VOC-002 | Chỉnh sửa từ |
| FR-LEARN-001 | Bắt đầu phiên học |
| FR-REVIEW-FLASH-003 | Đánh giá flashcard |
| FR-QUIZ-MCQ-003 | Chấm trắc nghiệm |
| FR-QUIZ-V2E-002 | Chấm Việt → Anh |
| FR-QUIZ-SENT-003 | Hiển thị đáp án tham khảo |
| FR-SPEECH-001 | Nghe phát âm |
| FR-SESSION-005 | Kết thúc phiên và tổng kết |
| FR-PROGRESS-002 | Cập nhật số liệu |
| FR-DASH-001 | Dashboard |
| FR-ADMIN-USER-002 | Quyền quản trị người dùng |

### 14.3. Tiêu chí nghiệm thu cấp sản phẩm

Sản phẩm phiên bản 1.0 được coi là đáp ứng BRD khi người dùng có thể:

1. Tạo hoặc chọn danh sách từ vựng.
2. Học các từ trong danh sách.
3. Ôn từ bằng nhiều hình thức.
4. Nghe phát âm của từ.
5. Nhận biết từ nhớ tốt và từ còn yếu thông qua tiến độ.
6. Xem tiến độ học tập.
7. Quay lại hệ thống và tiếp tục ôn các từ cần thiết.

---

## 15. YÊU CẦU CHƯA ĐỦ THÔNG TIN — OPEN ISSUES / TBD

Đây là các vấn đề cần BA/Product Owner/Khách hàng xác nhận trước khi đặc tả chi tiết và khóa scope kỹ thuật.

### Tài khoản

1. Trường dữ liệu đăng ký cụ thể.
2. Quy tắc mật khẩu.
3. Cơ chế xác minh tài khoản.
4. Cơ chế khôi phục mật khẩu.
5. Chính sách xóa tài khoản và dữ liệu liên quan.

### Danh sách và từ vựng

6. Một từ có thể thuộc nhiều danh sách hay không.
7. Một danh sách có thể chia theo topic thế nào.
8. Trường nào của Vocabulary là bắt buộc.
9. Cho phép trùng từ hay không.
10. Chính sách xóa từ: xóa bản ghi hay xóa liên kết.

### Chấm điểm

11. Quy tắc so sánh câu trả lời Việt → Anh.
12. Có bỏ qua hoa/thường không.
13. Có bỏ qua khoảng trắng thừa không.
14. Có chấp nhận biến thể/số nhiều/biến cách không.
15. Có chấp nhận đồng nghĩa không.
16. Cơ chế đánh giá câu dịch.

### Phát âm

17. Chuẩn giọng phát âm chính thức.
18. Có một hay nhiều giọng.
19. Cách lưu/cung cấp audio.

### Spaced Repetition và tiến độ

20. Công thức score/accuracy.
21. Điều kiện chuyển New → Learning.
22. Điều kiện chuyển Learning → Review.
23. Điều kiện chuyển Review → Mastered.
24. Công thức thời điểm ôn tiếp theo.
25. Quy tắc ưu tiên giữa các từ cùng mức độ.

### Dashboard

26. Công thức streak.
27. Khoảng thời gian của “Recent Accuracy”.
28. Định nghĩa chính xác “đã học”.
29. Cách tính “cần ôn hôm nay”.

### Quản trị

30. Danh sách thao tác Admin được phép.
31. Quy trình xử lý nội dung sai/không phù hợp.
32. Cơ chế audit hoạt động quản trị.

### Phi chức năng

33. Số người dùng đồng thời mục tiêu.
34. SLA/SLO availability.
35. Response time mục tiêu.
36. Browser/device support matrix.
37. Chính sách backup/recovery và retention dữ liệu.

---

## 16. RỦI RO VÀ PHỤ THUỘC NGHIỆP VỤ

### R-01 — Quy tắc chấm câu trả lời chưa đủ chi tiết

Việt → Anh và dịch câu có thể tạo nhiều câu trả lời hợp lệ. Nếu không chốt rubric trước, kết quả kiểm thử giữa BA, QA và khách hàng có thể khác nhau.

### R-02 — Thuật toán ôn tập chưa được định nghĩa

BRD mô tả mục tiêu ưu tiên từ yếu nhưng chưa đưa ra công thức chính thức. Việc này ảnh hưởng trực tiếp đến dữ liệu tiến độ và lịch ôn.

### R-03 — Mô hình dữ liệu danh sách/chủ đề chưa hoàn thiện

Chưa đủ thông tin để xác định chính xác quan hệ giữa Vocabulary, List và Topic.

### R-04 — Phát âm phụ thuộc nguồn audio

Chất lượng và tính sẵn sàng của audio phụ thuộc vào nguồn cung cấp phát âm.

### R-05 — Dashboard phụ thuộc dữ liệu lịch sử

Nếu lịch sử kết quả không được ghi nhận đầy đủ và nhất quán, các metric trên Dashboard sẽ không đáng tin cậy.

---

## 17. TRACABILITY BRD → SRS

| BRD | Nội dung | SRS chính |
|---|---|---|
| 2. Phạm vi sản phẩm | Scope | Section 2, Section 3 |
| 3. Vai trò | User/Admin | Section 2.2, Section 10 |
| 4.1 | Tài khoản | FR-AUTH-* |
| 4.2 | Danh sách/chủ đề | FR-LIST-* |
| 4.3 | Từ vựng | FR-VOC-* |
| 4.4 | Học từ mới | FR-LEARN-* |
| 4.5 | Flashcard | FR-REVIEW-FLASH-* |
| 4.6 | Trắc nghiệm | FR-QUIZ-MCQ-* |
| 4.7 | Việt → Anh | FR-QUIZ-V2E-* |
| 4.8 | Dịch câu | FR-QUIZ-SENT-* |
| 4.9 | Phát âm | FR-SPEECH-* |
| 4.10 | Ôn tập tổng hợp | FR-SESSION-* |
| 5 | Tiến độ | FR-PROGRESS-*, Section 12 |
| 6 | Luồng sử dụng | Section 5 |
| 7 | Dashboard | FR-DASH-*, Section 13 |
| 8 | Business Rules | Section 4 |
| 9 | UX | Section 7 |
| 10 | Success Criteria / Future | Section 14, Section 2.3 |

---

## 18. PHỤ LỤC — MA TRẬN CHỨC NĂNG PHIÊN BẢN 1.0

| Module | Requirement IDs | Priority |
|---|---|---|
| Authentication | FR-AUTH-001 → FR-AUTH-007 | Must |
| Vocabulary Lists | FR-LIST-001 → FR-LIST-007 | Must |
| Vocabulary | FR-VOC-001 → FR-VOC-006 | Must |
| Learning | FR-LEARN-001 → FR-LEARN-003 | Must |
| Flashcard | FR-REVIEW-FLASH-001 → FR-REVIEW-FLASH-004 | Must |
| Multiple Choice | FR-QUIZ-MCQ-001 → FR-QUIZ-MCQ-003 | Must |
| Vietnamese → English | FR-QUIZ-V2E-001 → FR-QUIZ-V2E-002 | Must |
| Sentence Translation | FR-QUIZ-SENT-001 → FR-QUIZ-SENT-005 | Must |
| Pronunciation | FR-SPEECH-001 → FR-SPEECH-003 | Must |
| Review Session | FR-SESSION-001 → FR-SESSION-006 | Must |
| Progress | FR-PROGRESS-001 → FR-PROGRESS-003 | Must |
| Dashboard | FR-DASH-001 → FR-DASH-002 | Must/Should |
| Admin User | FR-ADMIN-USER-001 → FR-ADMIN-USER-002 | Must |
| Admin Content | FR-ADMIN-CONTENT-001 → FR-ADMIN-CONTENT-003 | Must |

---

# KẾT LUẬN

SRS này chuyển các yêu cầu nghiệp vụ trong BRD thành baseline yêu cầu phần mềm cho phiên bản 1.0. Các yêu cầu chức năng đã được định danh bằng mã để đội phát triển và QA có thể truy vết từ nghiệp vụ đến thiết kế, implementation và test case.

Các điểm được đánh dấu **TBD** không phải là yêu cầu mới được tự ý áp đặt, mà là các thông tin BRD chưa quy định đủ để hệ thống có thể được đặc tả và kiểm thử một cách không mơ hồ. Những điểm này cần được chốt trong quá trình review SRS trước khi đóng yêu cầu.
