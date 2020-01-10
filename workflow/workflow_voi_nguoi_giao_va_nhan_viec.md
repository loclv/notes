# How to view this document

read `../how_to_read_sequence_diagram.md`

---

# workflow

read `./workflow_voi_nguoi_giao_va_nhan_viec_common.md`

## nhận yêu cầu từ khách hàng

```sequence
participant K
participant Mình
participant Team
K->Mình: nói việc muốn làm
Note over Mình: nếu dự án có spec rõ \n ràng từ ban đầu Mình \n check xem việc này \n có trong trách \n nhiệm của mình \n không?

Mình-->K: xác nhận lại điều \n đang nghĩ nếu cần
K-->Mình: 2 bên đều OK

Note over Mình: có làm được \n không?

Mình-->Team: nếu cần thì hỏi team xem có làm được không

Note right of Team: check xem có \n làm được hay không
Team-->Mình: nếu không làm được thì phải có lý do cụ thể \n Với quy tắc là không có việc gì không làm được \n chỉ có việc khó, phạm vi ảnh hưởng lớn nên \n tốn time
Note over Mình: tự mình suy nghĩ \n xem lý do có \n hợp lý không? \n vì trước khi giao \n cho mình, K đã phải \n suy nghĩ rồi
Mình-->K: xác nhận lại điều \n đang nghĩ
K-->Mình: 2 bên đều OK

Note over Mình: nếu K đồng ý \n không làm nữa thì \n dừng ở đây

Note over Mình: tạo task cho K

Note over Mình: chọn người phụ \n trách task là Mình

Mình->Team: truyền đạt cho team \n (tạo task bên team)

Note over Mình: chuyển trạng thái \n task từ `open` \n sang `progress`

Team->Mình: Q&A, báo xong và đã test trên môi trường stg

Note over Mình: update nội dung task \n ví dụ các bước để \n K xác nhận task đã \n hoàn thành

Note over Mình: chuyển trạng thái \n task từ `progress` \n sang `resolved`

Mình->K: gửi yêu cầu xác \n nhận task đã xong \n trên chat-tool

K-->Mình: đưa feedback và lặp \n lại những bước trên \n nếu cần

Note over K: test trên stg

Note over K: check task OK
Note over K: chuyển trạng thái \n task từ `resolved` \n sang `close`
```
