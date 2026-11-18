# BÀI THỰC HÀNH 3

## 1. PROMPT 

### C – Character
Bạn là Chuyên gia Phân tích Nghiệp vụ & Chăm sóc Khách hàng cấp cao tại một cửa hàng bán lẻ laptop, có kinh nghiệm xử lý khủng hoảng trải nghiệm khách hàng theo quy trình chuẩn và khách quan.

### R – Request 
Hãy phân tích và xử lý tình huống khiếu nại sau của khách hàng theo kỹ thuật **Chain-of-Thought**:
> *"Tôi mua laptop cách đây 10 ngày. Máy thường xuyên bị nóng, quạt kêu to và pin chỉ sử dụng được khoảng 2 tiếng. Tôi đã mang đến cửa hàng kiểm tra nhưng nhân viên chỉ vệ sinh máy và trả lại. Sau 2 ngày, tình trạng vẫn tiếp diễn. Tôi muốn đổi máy hoặc hoàn tiền."*

Thực hiện tuần tự 5 bước:
1. Xác định toàn bộ các vấn đề khách hàng gặp phải (tách biệt kỹ thuật và dịch vụ).
2. Đánh giá mức độ nghiêm trọng (Cao / Trung bình / Thấp) của từng vấn đề kèm căn cứ.
3. Liệt kê danh sách các thông tin còn thiếu cần xác minh lại với khách hàng, bộ phận kỹ thuật và chính sách nội bộ.
4. Đề xuất 2 phương án xử lý phù hợp kèm phân tích Ưu điểm và Hạn chế.
5. Soạn một email phản hồi chuyên nghiệp, thấu cảm gửi khách hàng.

### E – Examples (Ví dụ cách phân lọi dữ liệu)

- **[Dữ kiện]:** Khách mua máy cách đây 10 ngày, máy nóng và quạt kêu to.
- **[Giả thuyết]:** Có thể do lỗi keo tản nhiệt, lỗi pin hoặc phần mềm chạy ngầm chiếm CPU.
- **[Thông tin chưa xác định]:** Model máy là gì, thời lượng pin chuẩn của nhà sản xuất là bao nhiêu giờ.

### A – Adjustments (Điều chỉnh & Ràng buộc bắt buộc)
- **Tuyệt đối KHÔNG tự giả định chính sách** đổi trả/hoàn tiền của cửa hàng (không tự bịa quy định "1 đổi 1 trong 7 ngày" hay "hoàn tiền trong 30 ngày").
- Phân biệt rạch ròi 3 nhóm: `[Dữ kiện]`, `[Giả thuyết]`, và `[Thông tin chưa xác định]`.
- Không đưa ra kết luận kỹ thuật thiếu căn cứ và không hứa hẹn vượt thẩm quyền trong email gửi khách hàng.

### T – Type of output (Định dạng đầu ra)
Trình bày báo cáo rõ ràng theo 5 phần đánh số tương ứng với 5 bước; sử dụng **Bảng (Markdown Table)** cho Bước 2 (Đánh giá mức độ nghiêm trọng), danh sách gạch đầu dòng cho Bước 1, 3, 4 và định dạng **Email hoàn chỉnh** (có Tiêu đề, Lời chào, Nội dung, Ký tên) cho Bước 5.

### E – Extras (Thông tin bổ sung)
- Giọng điệu báo cáo phân tích: Khách quan, logic, chặt chẽ.
- Giọng điệu email gửi khách hàng: Chân thành, thấu cảm, cầu thị, chuyên nghiệp để xoa dịu bức xúc nhưng vẫn bảo vệ đúng quy trình nội bộ của cửa hàng.

---

## 2. KẾT QUẢ 

### Bước 1: Xác định các vấn đề của khách hàng
**A. Vấn đề về sản phẩm (Kỹ thuật):**
- **[Dữ kiện]:** Laptop mới mua 10 ngày gặp 3 hiện tượng: thường xuyên nóng, quạt kêu to, thời lượng pin chỉ đạt khoảng 2 tiếng. Tình trạng vẫn tiếp diễn sau 2 ngày kể từ lần kiểm tra đầu tiên.
- **[Giả thuyết]:** Có thể xuất phát từ lỗi phần cứng (hệ thống tản nhiệt, pin lỗi, keo tản nhiệt khô), xung đột phần mềm/driver chạy ngầm ngốn tài nguyên CPU, hoặc do khách hàng chạy các tác vụ nặng vượt mức thiết kế của dòng máy.

**B. Vấn đề về dịch vụ (Trải nghiệm khách hàng):**
- **[Dữ kiện]:** Khách đã mang máy đến cửa hàng kiểm tra nhưng nhân viên chỉ vệ sinh máy và trả lại; lỗi không được khắc phục dứt điểm sau 2 ngày. Hiện khách yêu cầu đổi máy hoặc hoàn tiền.
- **[Giả thuyết]:** Quy trình kiểm tra kỹ thuật lần 1 có thể chưa chuyên sâu (chưa test tải, chưa đo độ chai pin/kiểm tra phần mềm) hoặc nhân viên chưa giải thích rõ nguyên nhân cho khách hàng.

### Bước 2: Đánh giá mức độ nghiêm trọng của từng vấn đề

| Vấn đề | Mức độ nghiêm trọng | Căn cứ đánh giá |
| :--- | :---: | :--- |
| **Lỗi tái diễn sau khi đã mang đi kiểm tra** | **Cao** | Gây mất niềm tin trực tiếp vào chất lượng dịch vụ và đẩy cảm xúc khách hàng lên mức bức xúc, dẫn đến yêu cầu hoàn tiền/đổi máy. |
| **Máy thường xuyên nóng & quạt kêu to** | **Cao** | Tiềm ẩn nguy cơ hư hỏng linh kiện phần cứng (CPU/GPU) nếu là lỗi tản nhiệt thật sự; ảnh hưởng trực tiếp đến trải nghiệm cơ bản. |
| **Thời lượng pin chỉ khoảng 2 tiếng** | **Trung bình – Cao** | Nếu là máy văn phòng mới mua, 2 tiếng là bất thường; nhưng nếu là laptop gaming chạy tác vụ nặng thì có thể nằm trong ngưỡng bình thường (cần xác minh model máy). |
| **Yêu cầu đổi máy hoặc hoàn tiền** | **Cao (nghiệp vụ)** | Ảnh hưởng trực tiếp đến doanh thu và quy định nội bộ; nếu xử lý sai chính sách hoặc từ chối thiếu căn cứ dễ gây khủng hoảng truyền thông. |

### Bước 3: Danh sách thông tin cần xác minh (`[Thông tin chưa xác định]`)
1. **Thông tin sản phẩm & giao dịch:**
   - Mã đơn hàng / Số hóa đơn / Ngày mua chính xác.
   - Tên dòng máy (Model), cấu hình chi tiết (để đối chiếu thông số pin tiêu chuẩn của hãng).
2. **Thông tin kỹ thuật & bối cảnh sử dụng:**
   - Biên bản tiếp nhận và kết quả kiểm tra của nhân viên kỹ thuật lần 1 (lý do chỉ vệ sinh máy, đã đo nhiệt độ và độ chai pin chưa).
   - Thói quen sử dụng của khách khi gặp lỗi (phần mềm đang chạy, môi trường đặt máy, có vừa sạc vừa dùng không).
3. **Chính sách nội bộ của cửa hàng:**
   - Quy định chính thức hiện hành về điều kiện đổi trả/hoàn tiền tại thời điểm 10 ngày sau mua (yêu cầu xác nhận lỗi từ hãng hay từ cửa hàng, tình trạng vỏ hộp/phụ kiện).

### Bước 4: Đề xuất 2 phương án xử lý

**Phương án 1: Kiểm tra kỹ thuật chuyên sâu ưu tiên (Chưa quyết định đổi/trả ngay)**
- *Nội dung:* Mời khách mang máy đến (hoặc hỗ trợ nhận máy tận nơi) để kỹ thuật viên cấp cao kiểm tra toàn diện (test nhiệt độ, độ chai pin, phần mềm) và lập biên bản rõ ràng. Sau khi có kết luận kỹ thuật khách quan, đối chiếu với chính sách hiện hành của cửa hàng để quyết định đổi máy, hoàn tiền hoặc khắc phục triệt để.
- *Ưu điểm:* Đảm bảo đúng quy trình, có căn cứ kỹ thuật minh bạch, tránh rủi ro đổi trả sai chính sách nếu lỗi chỉ do phần mềm hoặc cách sử dụng.
- *Hạn chế:* Khách hàng phải chờ đợi thêm một lần nữa, dễ tăng bức xúc nếu thời gian kiểm tra kéo dài.

**Phương án 2: Kiểm tra nhanh kết hợp cung cấp máy dự phòng & đẩy nhanh xét duyệt đổi/trả**
- *Nội dung:* Xin lỗi về trải nghiệm lần kiểm tra trước, bố trí kỹ thuật viên trưởng tiếp nhận kiểm tra ngay trong ngày (2–4 giờ). Trong lúc chờ xác minh lỗi và đối chiếu chính sách đổi/hoàn tiền với quản lý, cung cấp máy dự phòng (nếu cửa hàng có sẵn) để không gián đoạn công việc của khách.
- *Ưu điểm:* Xoa dịu cảm xúc hiệu quả, thể hiện sự cầu thị và trách nhiệm cao sau thiếu sót ở lần kiểm tra đầu tiên, giữ vững uy tín thương hiệu.
- *Hạn chế:* Tốn thêm nguồn lực nhân sự ưu tiên và phụ thuộc vào việc cửa hàng có sẵn máy dự phòng hay không.

### Bước 5: Email phản hồi chuyên nghiệp gửi khách hàng

> **Tiêu đề:** Tiếp nhận khiếu nại và hỗ trợ kiểm tra ưu tiên cho laptop của Quý khách
>
> Chào Quý khách,
>
> Cửa hàng xin gửi lời xin lỗi chân thành vì những bất tiện mà Quý khách đang gặp phải với chiếc laptop mới mua, đặc biệt là việc tình trạng nóng máy, quạt kêu to và pin sụt nhanh vẫn chưa được khắc phục dứt điểm sau lần kiểm tra trước.
>
> Chúng tôi hoàn toàn thấu hiểu sự lo lắng cũng như mong muốn đổi máy hoặc hoàn tiền của Quý khách. Để đảm bảo quyền lợi tốt nhất cho Quý khách và có cơ sở xử lý chính xác theo đúng quy định của cửa hàng, chúng tôi xin phép được tiếp nhận lại trường hợp này theo **quy trình ưu tiên**:
>
> 1. Quý khách vui lòng cung cấp giúp chúng tôi **Mã đơn hàng / Số điện thoại mua hàng** và **tên dòng máy** để bộ phận CSKH tra cứu lại lịch sử kiểm tra lần trước.
> 2. Chúng tôi sẽ sắp xếp **Kỹ thuật viên trưởng** trực tiếp kiểm tra chuyên sâu toàn bộ phần cứng (tản nhiệt, pin) và phần mềm của máy trong thời gian sớm nhất, đồng thời lập biên bản xác nhận tình trạng cụ thể.
> 3. Ngay khi có kết quả kiểm tra chính thức, quản lý cửa hàng sẽ trực tiếp làm việc với Quý khách để đưa ra phương án giải quyết (đổi máy, hoàn tiền hoặc xử lý triệt để) phù hợp nhất theo chính sách hiện hành của cửa hàng.
>
> Quý khách có thể cho chúng tôi biết khung giờ thuận tiện để mang máy đến cửa hàng (hoặc để chúng tôi hỗ trợ tiếp nhận) không ạ?
>
> Một lần nữa, chúng tôi rất mong nhận được sự thông cảm của Quý khách và cam kết sẽ theo sát xử lý triệt để trường hợp này.
>
> Trân trọng,  
> **Bộ phận Chăm sóc Khách hàng**
