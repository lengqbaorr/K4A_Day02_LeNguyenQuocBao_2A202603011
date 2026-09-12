# 02 - Group Problem Statement (Bản nộp nhóm)

> Làm chung một bản, mỗi thành viên sao chép vào kho lưu trữ cá nhân của mình.
> Đi theo các giai đoạn từ Phase 3 đến Phase 6 trong tài liệu 01-worksheet.md.
> Nhóm chỉ chọn candidate problem ở Phase 3, và chỉ hoàn thiện Problem Statement sau khi đã nghiên cứu, kiểm chứng và vẽ chi tiết workflow.

## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm (VD: facilitator, workflow, research, writer) |
|-----|-----------|-------------|---------------------------------------------------------------|
| 1   | Trần Nguyễn Tiến Đức | 2A202602871 | Primary Writer, Problem Structuring |
| 2   | Đinh Quang Lâm | 2A202602875 | Domain Expert (Computer Vision), Workflow Lead |
| 3   | Đào Quang Cảnh | 2A2O2602542 | Facilitator, Challenge & Operations |
| 4   | Hoàng Công Minh | 2A202602774 | Technical Architecture, Engineering Review |
| 5   | Lê Nguyễn Quốc Bảo | 2A202603011 | Process Analyst, Validation & Metrics |

**Candidate problem nhóm chọn (1 câu):**

Lọc các khung hình chứa tình huống biên (edge-cases) từ video camera giám sát dài để bổ sung vào tập dữ liệu huấn luyện mô hình thị giác máy tính.

---

## Phase 3 - Group Convergence: từ 15 candidates về 1

### 3.1. Trình bày top 3 mỗi người (mỗi candidate 1-2 phút)

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh của nhóm |
|---|---|---|---|---|---|
| 1 | Đào Quang Cảnh | Tối ưu lựa chọn điểm đón khách cho Robotaxi | Hành khách và đội vận hành robotaxi | Điểm đón theo bản đồ làm khách đi bộ xa và xe đỗ chờ lâu | Khó kiểm chứng thực tế tại Việt Nam vì chưa có hệ thống robotaxi thương mại. |
| 2 | Đào Quang Cảnh | Nhận diện và định vị Robotaxi tại điểm đón đông đúc | Hành khách tại sảnh đón đông đúc | Dò tìm biển số vật lý giữa nhiều xe dừng đỗ nối đuôi | Thiên về giải pháp phần cứng đèn LED hoặc nhận diện biển số, chưa cần AI phức tạp. |
| 3 | Đào Quang Cảnh | Tối ưu điểm trả khách tại các khu phức hợp lớn | Hành khách đến bệnh viện, trường học, khu đô thị | Thiếu dữ liệu đường nội khu nên xe thả khách ở mép đường ngoài cổng | Phụ thuộc dữ liệu bản đồ riêng của từng khu phức hợp, phạm vi giải pháp quá rộng. |
| 4 | Hoàng Công Minh | Debug lỗi TypeScript và NestJS | Backend và Full-stack Developer | Phân tích root cause từ error log và ngữ cảnh codebase | Khó đo lường mức độ cải thiện khách quan do độ phức tạp mỗi bug rất khác biệt. |
| 5 | Hoàng Công Minh | Hiểu codebase và repository mới khi nhận task | Developer chuyển sang repository chưa quen thuộc | Đọc nhiều tầng module để tìm đúng file cần sửa | Công cụ hỗ trợ code hiện có đã nhiều, khó xác lập metric độc lập trong lab. |
| 6 | Hoàng Công Minh | Bỏ sót edge cases khi thiết kế test cho REST API | Backend Developer | Nghĩ ra các trường hợp biên, dữ liệu không hợp lệ và phân quyền | Logic nghiệp vụ phụ thuộc chặt chẽ vào con người review, ranh giới AI khó kiểm soát. |
| 7 | Đinh Quang Lâm | Code bừa bãi trong Jupyter Notebook khó tái sử dụng | Kỹ sư ML thử nghiệm mô hình | Dọn dẹp biến toàn cục và tách code sang script modular | Có thể xử lý bằng quy ước kỷ luật lập trình và linter trước khi cần đến AI. |
| 8 | Đinh Quang Lâm | Lọc frame chứa edge-cases từ video camera giám sát dài | Kỹ sư Computer Vision và chuyên viên dữ liệu | Mất 2.5 giờ tua video tốc độ cao để tìm vài frame ca khó | Workflow tuyến tính rất rõ, tách bạch mạch lạc giữa Rule, Workflow AI và người duyệt. |
| 9 | Đinh Quang Lâm | Soạn slide và viết báo cáo tiến độ đồ án cho GVHD | Sinh viên nghiên cứu và kỹ sư R&D | Tổng hợp log thí nghiệm và viết diễn giải narrative báo cáo | Nỗi đau ngắn hạn theo đợt, template báo cáo chuẩn có thể giải quyết phần lớn. |
| 10 | Lê Nguyễn Quốc Bảo | Chỗ trống sau khi khách hủy lịch hẹn tại salon | Lễ tân và chủ salon làm đẹp | Tìm và liên hệ khách chờ phù hợp khi có người hủy lịch | Bài toán quy trình vận hành, giải pháp danh sách chờ bằng Rule đã đáp ứng tốt. |
| 11 | Lê Nguyễn Quốc Bảo | Nhân viên nhận sai phiên bản lịch làm việc theo ca | Quản lý và nhân viên ca kíp | Cập nhật lịch mới nhưng thiếu kênh công bố phiên bản chính thức | Nỗi đau giao tiếp nội bộ, dùng công cụ bảng tính hoặc form chuẩn là giải quyết được. |
| 12 | Lê Nguyễn Quốc Bảo | Bỏ sót lô hàng cận hạn cần ưu tiên xuất bán trước | Nhân viên kho và thu ngân bán lẻ | Dò hạn sử dụng từng lô trên kệ khi dữ liệu chưa có cấu trúc | Bài toán quản trị kho vật lý, sắp xếp theo quy tắc FIFO trước khi nghĩ đến AI. |
| 13 | Trần Nguyễn Tiến Đức | Vòng đời thuê trọ và bảo vệ tiền đặt cọc | Người trẻ thuê phòng trọ đô thị | Đọc hiểu hợp đồng in sẵn và thiếu biên bản ảnh hiện trạng | Dữ liệu cá nhân chưa đo, phụ thuộc nhiều vào thái độ hợp tác của chủ trọ. |
| 14 | Trần Nguyễn Tiến Đức | Phối hợp quản lý dùng thuốc cho người cao tuổi | Con cái có cha mẹ già mắc bệnh mạn tính | Đọc đơn thuốc viết tay và phân liều vào khay thuốc | Rủi ro sức khỏe rất cao, khó tiếp cận đơn thuốc thật và người già trong lab. |
| 15 | Trần Nguyễn Tiến Đức | Kiểm tra hồ sơ thủ tục dịch vụ công trước khi nộp | Công dân làm thủ tục hành chính trực tuyến | Hồ sơ bị trả lại do sai định dạng tệp hoặc mâu thuẫn thông tin | Tần suất cá nhân làm thủ tục thấp, rào cản bảo mật dữ liệu công dân cao. |

### 3.2. Gom trùng / cluster (gom 15 ý thành 4 cụm)

| Cluster | Candidates included | Pattern chung | Ghi chú |
|---|---|---|---|
| A | Đinh Quang Lâm #1, #2; Hoàng Công Minh #1, #2, #3 | Tối ưu hóa chu trình kỹ thuật phần mềm và phát triển mô hình AI | Đinh Quang Lâm #2 nổi bật nhờ dữ liệu đầu vào rõ ràng và bóc tách được Rule với AI. |
| B | Đào Quang Cảnh #1, #2, #3 | Vận hành phương tiện tự hành và tương tác đón trả khách đô thị | Khó tiếp cận phương tiện và dữ liệu đội xe thực tế trong phạm vi buổi lab. |
| C | Lê Nguyễn Quốc Bảo #1, #2, #3 | Chuẩn hóa quy trình vận hành dịch vụ salon, ca kíp và bán lẻ | Phần lớn giải quyết triệt để bằng Rule-based và form quy trình, chưa cần AI. |
| D | Trần Nguyễn Tiến Đức #1, #2, #3 | Bảo vệ quyền lợi dân sinh, sức khỏe gia đình và dịch vụ công | Bài toán nhân văn nhưng số liệu cá nhân đều chưa đo và vướng bảo mật dữ liệu. |

### 3.3. Shortlist (giữ 3 bài trả lời được 7 câu hỏi worksheet)

| Candidate | Vì sao vào shortlist (2-3 ý) | Rủi ro / điều chưa rõ |
|---|---|---|
| Đinh Quang Lâm Card #2: Lọc frame chứa edge-cases từ video camera | 1. Actor rất cụ thể là kỹ sư thị giác máy tính và chuyên viên xử lý dữ liệu.<br>2. Workflow 5 bước tuyến tính với điểm nghẽn 140 phút tua video được mô tả rõ.<br>3. Tách biệt được Rule lọc tĩnh với Workflow AI chấm độ khó và người kiểm duyệt. | 1. Các con số thời gian 180 phút và 25 phút mới là ước tính tự báo cáo của một thành viên.<br>2. Chưa có log benchmark chính thức trên video thực tế và chưa khảo sát người ngoài. |
| Đào Quang Cảnh Card #1: Tối ưu lựa chọn điểm đón khách Robotaxi | 1. Vấn đề đón khách đô thị có tác động kép đến trải nghiệm và hiệu suất đội xe.<br>2. Workflow 7 bước rõ ràng từ khi đặt xe đến khi xe lăn bánh.<br>3. Có các chỉ số vận hành hấp dẫn như thời gian chờ và cự ly đi bộ. | 1. Nhóm không có dữ liệu GPS, dữ liệu đội xe hay môi trường thử nghiệm robotaxi thật.<br>2. Ranh giới giữa Rule bản đồ và AI ranking dễ chồng chéo và khó chứng minh giá trị. |
| Trần Nguyễn Tiến Đức Card #1: Vòng đời thuê trọ và bảo vệ tiền cọc | 1. Đụng chạm trực tiếp đến rủi ro tài chính khoản tiền cọc của người trẻ đi làm.<br>2. Chu trình nhận phòng và lập biên bản đối soát hiện trạng có thể chuẩn hóa.<br>3. Khung pháp lý và quy định về giá điện, nhà ở đã có văn bản công bố rõ ràng. | 1. Toàn bộ số liệu về chi phí và tỷ lệ tranh chấp cá nhân trong bản draft đều ghi chưa đo.<br>2. Khó kiểm chứng xem chủ nhà trọ có chấp nhận biên bản số hóa hay không trong buổi lab. |

### 3.4. Score để đồng thuận (chấm 1-5, ép nói rõ vì sao cho 5 / cho 3)

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Đinh Quang Lâm Card #2 (Lọc frame edge-case video) | 5 | 5 | 3 | 4 | 4 | 5 | 5 | 31 |
| Đào Quang Cảnh Card #1 (Điểm đón Robotaxi) | 4 | 4 | 2 | 4 | 1 | 3 | 2 | 20 |
| Trần Nguyễn Tiến Đức Card #1 (Bảo vệ cọc thuê trọ) | 4 | 4 | 2 | 3 | 2 | 4 | 4 | 23 |

**Candidate nhóm chọn (1 bài duy nhất):**

```text
Lọc frame chứa edge-cases từ video camera giám sát dài để bổ sung vào tập dữ liệu huấn luyện mô hình thị giác máy tính (Đinh Quang Lâm - Card #2).
```

**Vì sao chọn (4-5 câu):**

```text
Nhóm chọn bài toán lọc frame edge-case vì đây là bài toán kỹ thuật có phạm vi khép kín và phân định trách nhiệm vô cùng rõ ràng giữa máy và người.
Thành viên trong nhóm có kinh nghiệm thực tế về thị giác máy tính nên hiểu sâu chu trình xử lý từ video thô đến tập dữ liệu huấn luyện.
Quy trình hiện tại có điểm nghẽn tập trung tại bước xem tua video thủ công kéo dài với tỷ lệ khung hình tĩnh vô ích rất cao.
Bài toán cho phép phân định ranh giới kỹ thuật mẫu mực khi kết hợp thuật toán lọc chuyển động cổ điển với mô hình AI chấm điểm bất định để tạo danh sách rút gọn.
Đặc biệt, vai trò của con người được giữ nguyên vẹn ở khâu phê duyệt cuối cùng, ngăn chặn triệt để nguy cơ dữ liệu rác tràn vào tập huấn luyện.
```

**Vì sao KHÔNG chọn các candidate còn lại (mỗi bài 2-3 câu):**

```text
Đối với bài toán điểm đón Robotaxi của Đào Quang Cảnh, nhóm không có quyền truy cập dữ liệu vận hành đội xe hay bản đồ giao thông nội bộ để kiểm chứng tính khả thi trong buổi lab.
Mô hình xe tự hành đòi hỏi hạ tầng dữ liệu chuyên biệt vượt quá khả năng thực nghiệm độc lập của nhóm học viên.
Đối với bài toán vòng đời thuê trọ của Trần Nguyễn Tiến Đức, toàn bộ chỉ số thời gian và tần suất tranh chấp cọc đều đang ở trạng thái chưa đo lường thực tế.
Hơn nữa, rào cản đàm phán hợp đồng phụ thuộc chủ yếu vào vị thế và thiện chí của chủ nhà trọ hơn là sự hỗ trợ từ một công cụ công nghệ.
Các bài toán về gỡ lỗi TypeScript, hiểu codebase hay đề xuất test case của Hoàng Công Minh tuy quen thuộc nhưng khó thiết lập thang đo khách quan và công cụ trên thị trường đã bão hòa.
```

**Disagreement (nếu có - ai lo gì, chốt ra sao):**

```text
Thành viên Đào Quang Cảnh và Trần Nguyễn Tiến Đức ban đầu muốn chọn bài toán có tác động xã hội rộng như điểm đón xe hoặc bảo vệ tiền cọc thuê trọ.
Tuy nhiên, sau khi phân tích điều kiện thực nghiệm trong 4 tiếng của buổi lab, nhóm nhận thấy cả hai bài toán này đều thiếu trầm trọng dữ liệu thực tế tại chỗ và không thể chạy thử nghiệm khép kín.
Thành viên Đinh Quang Lâm làm rõ rằng bài toán lọc video camera có thể kiểm chứng ngay cấu trúc pipeline và thuật toán trên máy trạm mà không cần phụ thuộc bên thứ ba.
Nhóm đã đồng thuận rằng tính chặt chẽ về mặt kỹ thuật, ranh giới AI rõ ràng và khả năng kiểm soát trong lab quan trọng hơn quy mô ý tưởng nhưng thiếu tính khả thi.
```

---

## Phase 4 - Quick Validation + Research

### 4.1. Quick validation (ít nhất 1 cách: interview 2-3 người hoặc survey 5-10 người)

| Nguồn | Số người / mẫu | Tín hiệu xác nhận (kèm quote nguyên văn) | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| Interview | 0 người (chưa thực hiện) | Chưa thực hiện phỏng vấn trực tiếp bên ngoài nhóm trong thời gian lab. | Chưa có dữ liệu phản bác độc lập từ chuyên gia bên ngoài. | Giữ nguyên phạm vi bài toán dựa trên trải nghiệm tự báo cáo và đánh dấu toàn bộ số đo là giả định cần kiểm chứng. |
| Survey / poll | 0 người (chưa thực hiện) | Chưa thực hiện khảo sát số đông trong thời gian lab. | Chưa có dữ liệu khảo sát. | Không tự ý đưa ra kết luận khảo sát khi chưa có dữ liệu thu thập thực tế. |
| Log / ticket / review (nếu có) | 1 kỹ sư (quan sát nội bộ) | Kỹ sư Đinh Quang Lâm tự ước tính mất 140 phút tua video tốc độ x4 đến x8 để nhặt vài frame ngược sáng hoặc che khuất từ 3-5 video dài 60 phút. | Đây hoàn toàn là số liệu tự báo cáo chủ quan, chưa có nhật ký ghi log tự động khách quan. | Giữ nhận định đây là điểm nghẽn giả định và quyết định đưa dự án về trạng thái Not Yet để đo lường thực nghiệm. |

**Insight sau validation (1-2 câu - pain thật nằm ở đâu):**

```text
Nhóm chưa thực hiện phỏng vấn hoặc khảo sát bên ngoài trong buổi lab, nên toàn bộ cơ sở hiện tại dựa trên số liệu tự báo cáo của một thành viên trong nhóm.
Điểm nghẽn thực sự được giả định nằm ở việc kỹ sư phải ngồi theo dõi thủ công hàng chục nghìn frame tĩnh vô ích bằng mắt thường để tìm một vài khoảnh khắc có góc quay và ánh sáng bất lợi.
```

Bằng chứng đính kèm (nếu có): Chưa thực hiện thu thập file minh chứng bên ngoài trong buổi lab; nhóm sử dụng trực tiếp bản mô tả tự báo cáo của thành viên Đinh Quang Lâm làm tài liệu cơ sở.

### 4.2. Research giải pháp đã có (ít nhất 2-3 tools/patterns + 1-2 link kiểm được)

| Nguồn / tool / case | Link | Họ giải quyết bước nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| OpenCV Background Subtraction (MOG2 / KNN) | https://docs.opencv.org/4.x/d1/dc5/tutorial_background_subtraction.html | Lọc bỏ các khung hình tĩnh không có chuyển động trong video giám sát. | Thuật toán Rule xử lý rất nhanh, không tốn tài nguyên GPU và loại bỏ hiệu quả khung hình bất động. | Không hiểu ngữ nghĩa hình ảnh, không phân biệt được chuyển động thông thường với tình huống biên phức tạp. | Bắt buộc dùng Rule OpenCV ở bước tiền xử lý để loại bỏ 70-80% khung hình tĩnh trước khi đưa vào mô hình AI. |
| Active Learning Pattern (Uncertainty Sampling) | https://en.wikipedia.org/wiki/Active_learning_(machine_learning) | Xếp hạng độ bất định (entropy và confidence score) để tìm mẫu dữ liệu khó cho mô hình. | Định vị chính xác các khung hình mà mô hình hiện tại kém tự tin nhất, tập trung sự chú ý của chuyên viên vào ca khó. | Có thể chọn nhầm các khung hình bị nhiễu cảm biến, nhòe mờ không thể gán nhãn thay vì ca khó có giá trị huấn luyện. | AI chỉ được đóng vai trò tạo danh sách rút gọn, bắt buộc chuyên viên phải duyệt từng ảnh trước khi đưa vào tập dữ liệu. |
| FiftyOne Dataset Curation (Voxel51) | https://voxel51.com/docs/fiftyone/ | Trực quan hóa, lọc và quản lý dữ liệu ảnh, video theo độ tự tin và embedding của mô hình. | Giao diện trực quan mạnh mẽ, hỗ trợ kỹ sư lọc nhanh các mẫu dữ liệu bất thường và tích hợp sâu với framework học sâu. | Đòi hỏi cài đặt hạ tầng quản lý dữ liệu hoàn chỉnh, quá nặng nề cho nhu cầu xử lý video ngoại tuyến đơn lẻ. | Giữ giải pháp ở mức một workflow script tinh gọn kết hợp lọc Rule với mô hình AI ngoại tuyến thay vì dựng hệ thống cồng kềnh. |

**Research takeaway (2-3 câu - nên build gì / không build gì):**

```text
Nhóm nhận thấy không nên cố gắng xây dựng một mô hình AI tự động xử lý toàn bộ quy trình vì thuật toán cổ điển OpenCV đã xử lý rất tốt việc lọc frame tĩnh.
Phương án tối ưu là một workflow phối hợp chặt chẽ: Rule xử lý bước lọc thô ban đầu, mô hình học sâu xếp hạng độ khó để tạo danh sách rút gọn, và kỹ sư là người kiểm duyệt quyết định cuối cùng.
Tuyệt đối không để AI tự động nạp ảnh vào tập dữ liệu mà không có sự kiểm tra của con người nhằm tránh rủi ro suy giảm chất lượng dữ liệu huấn luyện.
```

> Lưu ý: không dùng số liệu AI đưa nếu không verify được link chính thức.
> Ghi rõ các giả định chưa chắc chắn.

---

## Phase 5 - Workflow + Problem Statement

### 5.1. Current workflow bản nhóm

Dán workflow hoặc link file: Quy trình hiện tại dựa trên bản tự báo cáo của thành viên Đinh Quang Lâm.

```text
CURRENT STATE - 180 phút (ước tính tự báo cáo)

[1. Tải video camera dài về máy trạm: 10' - Kỹ sư CV]
       ↓
[2. Mở trình phát và tua video x4 đến x8: 140' - Kỹ sư CV]  <-- BOTTLENECK (Mỏi mắt, hơn 80% cảnh tĩnh vô ích)
       ↓
[3. Bấm dừng thủ công, chụp và cắt frame: 20' - Kỹ sư CV]
       ↓
[4. Đặt tên, phân loại thư mục ca khó: 10' - Kỹ sư CV]
       ↓
[5. Lưu ảnh vào kho lưu trữ tạm: --' - Kỹ sư CV]
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú (handoff? bottleneck?) |
|---|---|---|---|---|---|
| 1 | Kỹ sư CV | File video camera từ hệ thống giám sát (3-5 video, mỗi video 60 phút). | Video đã tải về lưu trữ cục bộ trên máy trạm. | 10 phút / Đợt lọc (1-2 lần/tuần) | Handoff từ hệ thống lưu trữ camera về máy tính cá nhân. |
| 2 | Kỹ sư CV | Video cục bộ trên máy trạm. | Phát hiện thời điểm xuất hiện tình huống biên. | 140 phút / Đợt lọc | Nút thắt lớn nhất; kỹ sư theo dõi liên tục ở tốc độ cao, rất dễ mỏi mắt và lướt qua khoảnh khắc 1-2 giây. |
| 3 | Kỹ sư CV | Video đang tạm dừng đúng khung hình cần lấy. | Các tệp ảnh khung hình thô đã chụp hoặc cắt. | 20 phút / Đợt lọc | Thao tác chụp màn hình hoặc cắt khung hình thủ công lặp đi lặp lại nhiều lần. |
| 4 | Kỹ sư CV | Các khung hình thô vừa cắt. | Ảnh đã được đổi tên và gom vào thư mục theo loại ca khó. | 10 phút / Đợt lọc | Phân loại dựa trên cảm quan cá nhân về góc tối, ngược sáng hoặc che khuất. |
| 5 | Kỹ sư CV | Ảnh đã phân loại. | Thư mục dữ liệu sẵn sàng cho khâu gán nhãn. | Chưa đo / Đợt lọc | Lưu trữ thủ công vào thư mục dự án trên máy trạm. |

**Bottleneck chính (2-3 câu):**

```text
Điểm nghẽn nghiêm trọng nhất nằm ở Bước 2 khi kỹ sư phải dành khoảng 140 phút để quan sát màn hình tua nhanh tốc độ cao.
Hơn 80% thời lượng video là khung cảnh tĩnh không có biến đổi ngữ cảnh, gây lãng phí lớn thời gian lao động chuyên môn.
Tình trạng mỏi mắt sau khoảng 30 phút theo dõi liên tục khiến con người rất dễ bỏ sót các khoảnh khắc biên diễn ra chớp nhoáng chỉ trong 1 đến 2 giây.
```

### 5.2. Future workflow bản nhóm

Phải nhìn ra 5 thứ: bước nào máy (Rule), bước nào AI, bước nào người, boundary ở đâu, fallback khi AI sai.

```text
FUTURE STATE - 25 phút (mục tiêu giả định)

[1. Script OpenCV Background Subtraction lọc frame tĩnh: 5' - Máy (Rule)]
       ↓
[2. Mô hình AI offline chấm điểm độ khó và bất định: 5' - Máy (AI Workflow)]
       ↓
[3. Hệ thống xuất shortlist top 50 frame có độ tự tin thấp nhất: 2' - Máy (Workflow)]
       ↓
[4. Kỹ sư CV rà soát và phê duyệt từng frame trong shortlist: 10' - Con người (HUMAN BOUNDARY)]
       ↓
[5. Script tự động xuất frame được duyệt vào dataset: 3' - Máy (Rule)]

Fallback: Nếu AI lọc sót tình huống biên quan trọng, kỹ sư hạ ngưỡng tin cậy để mở rộng danh sách rút gọn và kiểm tra ngẫu nhiên thêm một đoạn video 15 phút.
```

**Before/after impact:**

| Metric | Trước | Sau kỳ vọng | Cách đo |
|---|---:|---:|---|
| Tổng thời gian | 180 phút (ước tính tự báo cáo) | Dưới 25 phút (mục tiêu giả định) | Bấm giờ toàn bộ quá trình từ lúc bắt đầu chạy script đến khi hoàn tất lưu dataset. |
| Số bước | 5 bước | 5 bước | Đếm số bước thao tác trong toàn bộ chu trình xử lý dữ liệu. |
| Số bước thủ công | 4/5 bước thủ công hoàn toàn | 1/5 bước thủ công (chỉ ở khâu duyệt shortlist) | Đếm số bước cần sự tương tác trực tiếp của kỹ sư. |
| Bottleneck chính | Tua xem video thủ công (140 phút) | Kỹ sư rà soát shortlist 50 ảnh (10 phút) | Đo thời gian của bước chiếm tỷ trọng công sức lớn nhất. |
| Risk mới | Bỏ sót do mỏi mắt khi xem video dài | Bỏ sót do mô hình AI đặt ngưỡng sai | Đánh giá tỷ lệ ca khó thực tế bị mô hình loại bỏ trên một tập dữ liệu kiểm thử mẫu. |

### 5.3. Problem Statement v0 (mỗi field 2-3 câu)

| Field | Nội dung |
|---|---|
| **Actor** | Kỹ sư thị giác máy tính và chuyên viên dữ liệu chịu trách nhiệm xây dựng tập dữ liệu huấn luyện cho mô hình camera giám sát.<br>Họ là những người trực tiếp khai thác nguồn video thực tế để tìm kiếm các trường hợp bất thường nhằm cải thiện độ chính xác của mô hình. |
| **Workflow** | Kỹ sư tải các tệp video giám sát dài về máy trạm, mở phần mềm tua nhanh để quan sát bằng mắt thường.<br>Khi phát hiện tình huống khó, kỹ sư dừng video, chụp lại khung hình, phân loại sơ bộ và lưu trữ vào thư mục dữ liệu huấn luyện. |
| **Bottleneck** | Bước ngồi theo dõi video tua nhanh kéo dài tới 140 phút trong tổng số 180 phút của quy trình.<br>Hơn 80% thời lượng là cảnh tĩnh không có giá trị, khiến kỹ sư nhanh chóng mỏi mắt và bỏ sót các tình huống khó diễn ra ngắn ngủi. |
| **Impact** | Quy trình tiêu tốn từ 3 đến 6 giờ lao động chuyên môn mỗi tuần của kỹ sư cho tác vụ quan sát thụ động.<br>Việc bỏ sót các tình huống biên làm mô hình huấn luyện sau đó tiếp tục hoạt động kém tin cậy khi triển khai ngoài thực địa. |
| **Success Metric** | Rút ngắn tổng thời gian xử lý cho mỗi đợt lọc video từ 180 phút xuống dưới 25 phút dựa trên ước tính ban đầu.<br>Đảm bảo tỷ lệ giữ lại các khung hình có vật thể bị che khuất trên 50% hoặc biến đổi ánh sáng mạnh đạt yêu cầu kiểm tra của kỹ sư. |
| **Boundary** | Hệ thống chỉ tạo danh sách rút gọn các khung hình tiềm năng và tuyệt đối không tự ý chèn ảnh vào tập dữ liệu chính thức.<br>Giải pháp chạy hoàn toàn ở chế độ xử lý ngoại tuyến trên máy trạm nội bộ, không can thiệp vào luồng phát trực tiếp của camera. |

**Câu hỏi AI phản biện v0 (nếu có):**
- Field nào mơ hồ: Tiêu chí không bỏ sót ca khó trong Success Metric chưa có định lượng rõ ràng vì thiếu tập ground-truth đối chứng trên toàn bộ video dài.
  Các con số thời gian 180 phút và 25 phút hoàn toàn là ước tính chủ quan của một cá nhân và chưa được kiểm chứng độc lập.
- Tôi sửa gì: Nhóm gắn nhãn toàn bộ các chỉ số thời gian là ước tính tự báo cáo cần xác minh.
  Nhóm bổ sung yêu cầu xây dựng tập dữ liệu mẫu 60 phút có gán nhãn chuẩn để đo tỷ lệ bỏ sót một cách khách quan.

---

## Phase 6 - Rule / Workflow / Agent + Decision

### 6.0. Ma trận độ phù hợp (suy nghĩ nhanh, không thay quyết định cuối)

- Độ mơ hồ: [x] Thấp (có đúng/sai rõ) / [ ] Cao (nhiều cách trả lời vẫn OK) - Vì sao: Việc một khung hình có phải là cảnh tĩnh hay không được xác định rõ bằng biến thiên pixel, và tiêu chí khung hình bị che khuất hay ngược sáng là các đặc trưng hình học, quang học cụ thể của bài toán thị giác máy tính.
- Độ phức tạp: [x] Thấp (1-2 bước) / [ ] Cao (3+ bước/nguồn, phụ thuộc nhau) - Vì sao: Quy trình đi thẳng một đường ống tuần tự từ video thô qua lọc tĩnh, chạy suy luận chấm điểm bất định, đến xuất danh sách ảnh; không có nhiều nhánh rẽ phức tạp hay quyết định động.

**Bài toán nhóm nằm ở ô nào:**

```text
Độ mơ hồ thấp - Độ phức tạp thấp đến trung bình.
```

**Vì sao (2-3 câu):**

```text
Dữ liệu đầu vào và đầu ra của từng bước hoàn toàn xác định, không đòi hỏi sáng tạo ngôn ngữ hay suy luận đa bước phức tạp.
Thuật toán lọc chuyển động giải quyết dứt điểm phần lớn dữ liệu thừa, trong khi mô hình học sâu chỉ thực hiện một nhiệm vụ duy nhất là chấm điểm tin cậy.
Do đó, không có lý do kỹ thuật nào để sử dụng một kiến trúc Agent tự hành cho bài toán này.
```

### 6.1. So sánh Rule / Workflow / Agent (so trên cùng 1 bài)

| Mức | Phương án cho bài toán nhóm | Khi nào đủ | Rủi ro | Chọn? (Dùng cho bước nào?) |
|---|---|---|---|---|
| **Rule** | Dùng OpenCV Background Subtraction lọc bỏ các frame tĩnh không có chuyển động | Đủ nếu mục tiêu chỉ là loại bỏ thời gian chết của camera không có người qua lại. | Không phân biệt được chuyển động bình thường với tình huống biên khó như ngược sáng, che khuất. | Chọn một phần (Dùng riêng cho bước tiền xử lý lọc frame tĩnh). |
| **Workflow** | Pipeline kết hợp: Rule lọc tĩnh -> Mô hình AI offline chấm điểm bất định -> Xuất shortlist 50 frame -> Người CV duyệt | Đủ vì quy trình xử lý tuyến tính cố định, AI chỉ hỗ trợ bước xếp hạng ca khó và người kiểm soát hoàn toàn. | Mô hình AI có thể chấm điểm sai hoặc bỏ sót mẫu dị biệt nếu ngưỡng đặt không chuẩn xác. | Chọn toàn bộ giải pháp (Phù hợp nhất cho toàn bộ chu trình xử lý). |
| **Agent** | Agent tự động tải video, tự quyết định chiến lược lọc, tự gọi công cụ và tự nạp dữ liệu vào pipeline huấn luyện | Chỉ cần nếu hệ thống phải tự thích ứng động với nhiều loại camera và tự lên kế hoạch huấn luyện mô hình mới. | Chi phí tính toán cao, kiến trúc phức tạp không cần thiết, nguy cơ tự ý nạp dữ liệu rác gây hỏng mô hình. | Không chọn (Hoàn toàn không phù hợp với bài toán batch tuyến tính). |

**5 câu hỏi chốt (trả lời câu đầy đủ):**
1. Rule có giải được 70-80% case không?
Có, thuật toán Rule Background Subtraction của OpenCV có thể loại bỏ ngay 70 đến 80% các khung hình tĩnh hoàn toàn không có chuyển động.
2. Các bước có đi thẳng một đường không hay phải rẽ nhánh?
Toàn bộ quy trình đi thẳng theo một đường ống tuyến tính từ video thô qua lọc tĩnh, chấm điểm suy luận, đến xuất danh sách rút gọn mà không cần rẽ nhánh động.
3. Có thật sự cần Agent tự lập kế hoạch + gọi tool không?
Hoàn toàn không cần, vì thứ tự thực thi đã được cố định sẵn trong mã nguồn và không có quyết định nào cần Agent tự suy luận thời gian thực.
4. Nếu AI sai, ai phát hiện đầu tiên và sửa trong bao lâu?
Kỹ sư thị giác máy tính sẽ phát hiện ngay lập tức khi duyệt danh sách rút gọn 50 khung hình và chỉ mất vài giây để loại bỏ ảnh không đạt tiêu chuẩn.
5. Có hạ được từ Agent -> Workflow -> Rule không?
Có, kiến trúc đã được chủ động hạ từ Agent xuống cấp độ Workflow kết hợp Rule để tối ưu độ tin cậy và đơn giản hóa việc triển khai.

**Mức chọn:**

```text
Workflow kết hợp Rule (AI-assisted Linear Workflow with Human-in-the-Loop)
```

**Vì sao chọn (3-4 câu):**

```text
Nhóm chọn cấp độ Workflow vì cấu trúc xử lý của bài toán hoàn toàn mang tính tuyến tính và xác định từ đầu đến cuối.
Sự kết hợp giữa Rule để gạt bỏ khung hình tĩnh và AI để xếp hạng độ khó cho phép tận dụng tối đa thế mạnh của từng công cụ mà không phát sinh độ phức tạp dư thừa.
Mô hình AI chỉ đảm nhận một nhiệm vụ duy nhất là tạo danh sách rút gọn các khung hình tiềm năng, giúp giảm tải tối đa công sức quan sát cho con người.
Toàn bộ quyền kiểm soát dữ liệu huấn luyện được đặt trong tay kỹ sư thông qua bước phê duyệt bắt buộc, đảm bảo an toàn tuyệt đối cho mô hình sản phẩm.
```

**Vì sao không chọn mức đơn giản hơn (2-3 câu):**

```text
Nếu chỉ sử dụng giải pháp Rule thuần túy, hệ thống chỉ có thể nhận biết được chuyển động cơ học mà hoàn toàn bất lực trước các tình huống ngữ cảnh khó như bóng râm phức tạp, lóa sáng ban đêm hay vật thể bị che khuất một phần.
Điều này khiến kỹ sư vẫn phải tốn lượng lớn thời gian để quan sát hàng nghìn khung hình có chuyển động bình thường nhằm tìm kiếm các ca biên đặc thù.
Do đó, việc bổ sung thêm một bước suy luận AI để chấm điểm độ bất định là điều kiện bắt buộc để đạt được mục tiêu cắt giảm thời gian lọc dữ liệu.
```

### 6.2. Problem Statement v1 (v0 sửa chặt hơn + 3 field cuối)

| Field | Nội dung |
|---|---|
| **Actor** | Kỹ sư thị giác máy tính và chuyên viên dữ liệu chịu trách nhiệm tuyển chọn dữ liệu cho mô hình camera giám sát.<br>Họ am hiểu các tiêu chuẩn kỹ thuật của ảnh huấn luyện và là người trực tiếp chịu trách nhiệm về chất lượng đầu vào của tập dữ liệu. |
| **Workflow** | Nhận tệp video camera dài -> Chạy script OpenCV loại bỏ khung hình tĩnh -> Chạy mô hình học sâu chấm điểm độ bất định -> Xuất danh sách rút gọn top 50 khung hình nghi vấn -> Kỹ sư duyệt thủ công từng khung hình -> Lưu khung hình đạt chuẩn vào thư mục dữ liệu huấn luyện. |
| **Bottleneck** | Bước quan sát tua video thủ công kéo dài 140 phút trong tổng thời lượng 180 phút được tự báo cáo bởi kỹ sư.<br>Phần lớn thời gian bị lãng phí vào cảnh tĩnh vô ích và tình trạng mỏi mắt làm tăng nguy cơ bỏ sót các tình huống góc khuất hoặc ánh sáng biến đổi mạnh. |
| **Impact** | Tiêu tốn từ 3 đến 6 giờ mỗi tuần của nhân sự kỹ thuật cấp cao cho tác vụ tua video thụ động.<br>Tình trạng bỏ sót các ca biên khiến mô hình nhận diện thực tế liên tục lặp lại các lỗi nhận dạng sai trong môi trường vận hành thực tế. |
| **Success Metric** | Rút ngắn thời gian kỹ sư phải tương tác trực tiếp từ 180 phút xuống dưới 25 phút cho mỗi đợt lọc video theo mục tiêu giả định.<br>Giữ lại được ít nhất 90% các tình huống biên thực tế xuất hiện trong video được xác minh qua tập đối chứng mẫu. |
| **Boundary** (làm / không làm) | Làm việc lọc khung hình ngoại tuyến theo đợt trên tệp video có sẵn; làm việc chấm điểm bất định để sinh danh sách 50 khung hình nghi vấn; yêu cầu kỹ sư duyệt 100% trước khi lưu.<br>Không can thiệp vào luồng camera trực tiếp; không tự động đưa khung hình vào tập huấn luyện; không tự động sinh nhãn gán chi tiết. |
| **AI intervention point** (can thiệp sau bước nào, trước bước nào) | AI can thiệp ngay sau bước script Rule OpenCV loại bỏ các khung hình tĩnh, và hoàn tất nhiệm vụ trước khi kỹ sư mở danh sách rút gọn để phê duyệt. |
| **Mức chọn** (Rule / Workflow / Agent + 1 câu vì sao) | Workflow kết hợp Rule: Rule lọc thô chuyển động nhanh chóng, AI xếp hạng độ bất định để tạo shortlist, con người duyệt mọi khung hình. |
| **Rủi ro & người thật kiểm tra** (rủi ro lớn nhất + ai kiểm tra bằng cách nào) | Rủi ro lớn nhất là mô hình AI chấm điểm sai lệch dẫn đến việc loại bỏ các tình huống biên thực sự nguy hiểm khỏi danh sách rút gọn.<br>Người thật kiểm tra là kỹ sư thị giác máy tính, người sẽ trực tiếp duyệt qua từng khung hình trong danh sách 50 ảnh và định kỳ kiểm tra ngẫu nhiên các đoạn video bị loại bỏ để phát hiện tỷ lệ bỏ sót. |

### 6.3. Final decision

| Câu hỏi | Yes / Not Yet / No | Ghi chú (câu đầy đủ) |
|---|---|---|
| Actor + workflow rõ chưa? | Yes | Kỹ sư CV và 5 bước xử lý video rất rõ ràng, khép kín. |
| Baseline + metric đo được chưa? | Not Yet | Các con số 180 phút và 25 phút mới chỉ là ước tính tự báo cáo của thành viên Lâm, chưa có nhật ký đo lường thực nghiệm khách quan. |
| Data/input đủ dùng chưa? | Yes | Dữ liệu video camera giám sát thực tế có thể thu thập và chạy thử nghiệm ngoại tuyến nội bộ. |
| AI sai, hậu quả chấp nhận được không? | Yes | Con người trực tiếp duyệt toàn bộ danh sách rút gọn nên rủi ro dữ liệu sai tràn vào mô hình bị triệt tiêu hoàn toàn. |
| Có người review/owner không? | Yes | Kỹ sư thị giác máy tính là chủ sở hữu quy trình và chịu trách nhiệm phê duyệt từng khung hình. |
| Có cách non-AI đơn giản hơn không? | Not Yet | Giải pháp Rule OpenCV loại được cảnh tĩnh nhưng chưa đủ để nhận diện tình huống biên; cần thử nghiệm kết hợp để xác định rõ hiệu quả thực tế. |

**Decision:**

```text
Not Yet
```

**Lý do (3-4 câu dựa trên bằng chứng):**

```text
Quyết định của nhóm là Not Yet vì trong khuôn khổ 4 tiếng của buổi lab, nhóm hoàn toàn chưa thực hiện được các bước phỏng vấn độc lập hay khảo sát thực tế bên ngoài để kiểm chứng tính phổ quát của vấn đề.
Toàn bộ các thông số về thời gian xử lý 180 phút, tỷ lệ 80% khung hình tĩnh và mục tiêu rút ngắn xuống 25 phút hiện mới dừng lại ở mức ước tính tự báo cáo của cá nhân thành viên Đinh Quang Lâm.
Nhóm cần tiến hành một đợt đo lường baseline khách quan trên dữ liệu video thật và ghi nhận nhật ký thao tác chính xác trước khi cam kết nguồn lực phát triển giải pháp chính thức.
Việc giữ trạng thái Not Yet thể hiện tính trung thực khoa học, đúng nguyên tắc phát triển sản phẩm lấy bằng chứng làm trọng tâm thay vì vội vàng triển khai khi chưa xác thực giả thuyết.
```

**Nếu Go - pilot nhỏ nhất (data nào, chạy tay ra sao, đo 3 số nào):**

```text
Dữ liệu thử nghiệm: 01 tệp video camera giám sát dài đúng 60 phút có chứa các điều kiện ngược sáng và người đi vào vùng tối.
Chạy tay đối chứng: Kỹ sư CV ngồi xem tua và ghi chép nhật ký chính xác từng phút thao tác, lập danh sách các khung hình ca khó tìm được làm tập chuẩn đối chứng.
Đo lường 3 chỉ số chính: Tổng thời gian lọc thủ công thực tế tính bằng phút; tỷ lệ khung hình tĩnh thực tế được lọc bởi Rule OpenCV tính bằng phần trăm; tỷ lệ tình huống biên có trong ground truth lọt vào danh sách rút gọn của AI tính bằng phần trăm.
```

**Nếu Not Yet - cần validate gì trước:**

```text
Cần phỏng vấn đối soát với ít nhất 2 đến 3 kỹ sư Computer Vision hoặc chuyên viên xử lý dữ liệu ngoài nhóm để xác nhận xem họ có thực sự tốn nhiều thời gian cho việc tua video tìm ca khó hay không.
Cần thực hiện một phiên bấm giờ thực tế trên máy trạm khi lọc một video camera 60 phút để xác lập đường cơ sở thời gian khách quan thay cho số liệu ước tính tự báo cáo.
Cần kiểm tra xem các thuật toán lọc chuyển động có sẵn trong OpenCV có thể loại bỏ được bao nhiêu phần trăm dung lượng khung hình vô ích trên tập video camera thực tế của dự án.
```

**Nếu No-Go - làm gì thay AI:**

```text
Nếu kết quả thử nghiệm cho thấy việc lọc ca khó không thường xuyên diễn ra hoặc thuật toán Rule đã giải quyết được trên 80% nhu cầu, nhóm sẽ không sử dụng mô hình học sâu.
Thay vào đó, nhóm sẽ hoàn thiện một kịch bản dòng lệnh Python đơn giản sử dụng OpenCV Background Subtractor để tự động cắt bỏ mọi khung hình tĩnh, sau đó trích xuất các khung hình có biến thiên chuyển động mạnh để kỹ sư lướt nhanh bằng công cụ xem ảnh thông thường.
```

**Exit / rollback (khi nào dừng AI, quay về cách cũ):**

```text
Dừng sử dụng mô hình AI và quay lại quy trình lọc thủ công kết hợp Rule OpenCV nếu tỷ lệ bỏ sót tình huống biên thực tế của AI vượt quá ngưỡng 15% so với việc con người xem xét trực tiếp.
Dừng triển khai nếu thời gian kỹ sư phải thiết lập môi trường chạy mô hình và kiểm tra danh sách rút gọn vượt quá 60 phút cho mỗi video 60 phút, không đem lại hiệu quả tiết kiệm thời gian vượt trội so với quy trình cũ.
```

---

### Self-check nộp phần 02 (nhóm)
- [x] Có nhật ký hội tụ 15 -> 1 (cluster + shortlist + score)
- [x] Có validation trung thực (ghi nhận chưa thực hiện bên ngoài, dùng self-reported estimate) và research các công cụ kiểm chứng được
- [x] Có workflow trước/sau đủ thời gian, handoff, bottleneck, boundary, fallback
- [x] Có PS v0 -> v1, metric có trước/sau + cách đo, boundary có làm/không làm
- [x] Có so sánh Rule/Workflow/Agent + Decision Not Yet có lý do dựa trên bằng chứng
