# workflow khi làm BrSE

## Mở đầu

Về đặc thù của vị trí `BrSE` bạn có thể `google` để biết thêm. Trong các bài viết đó thì bài viết [này](https://itviec.com/blog/ky-su-cau-noi-la-gi/) giới thiệu mình thấy khá là dễ hiểu.

Với kinh nghiệm làm `BrSE` dự án đầu tiên ăn hành tỏi thì bài viết chỉ mang tính tự thuật và mang cho người ngoài ngành cái nhìn rõ hơn 1 chút về nghề này.

Còn đối với các bạn mới làm `BrSE` thì theo mình nghĩ các bạn nên tự mình trải nghiệm.

Bài viết đưa ra `workflow` của cá nhân mình, có thể chưa phù hợp, chưa đúng thì mong các bạn comment để mình học hỏi thêm.

## workflow là gì

Dịch sang tiếng Việt thì là `luồng công việc` hoặc `quy trình`.

Các ví dụ về `luồng công việc` như:
- các bước để tán gái
- các bước để hút thuốc lào đúng cách
- các bộ phận logic trong 1 cái máy
- các quy trình khi sử dụng git với team
- ...

workflow cũng có tính tương đối đúng sai và khi sử dụng không nên quá cứng nhắc.


## workflow để làm gì

- tránh gây ra những thiệt hại không đáng có khi làm việc
- giúp quá trình diễn ra dễ tự động hoá
- điều tra sai sót 1 cách dễ dàng (dễ quy trách nhiệm :D)
- công việc nhanh và hiệu quả, dễ quản lý

tuy nhiên:
- workflow nhiều khi quá cứng nhắc, ví dụ như vụ xả nước lũ ở đập thuỷ điện Bản Vẽ là `đúng quy trình`.
  - nguyên nhân: workflow khó lường hết các case, đặc biệt là các case ngoại lệ
- với các dự án không phù hợp mà cố áp dụng thì thành ra mất rất nhiều thời gian
  - nguyên nhân: nhiều bước thừa


## Nội dung chính - workflow khi làm BrSE

### các thông tin chung - thuật ngữ
workflow khi trao đổi với *Khách hàng/PM* - ký hiệu là `K`

có thể áp dụng cho *BrSE, technical leader, team leader* - ký hiệu là `Mình`

phần mềm quản lý task thông thường như:
- backlog
- jira
- trello
- ...

`stg` là môi trường staging (cho bạn nào chưa biết thì có thể đọc ở [đây](https://toidicodedao.com/2019/07/02/environment-trong-lap-trinh/))

`open` là trạng thái task mới được khởi tạo - đang trong quá trình trao đổi QA, phân chia công việc hoặc tạm dừng

`progress` là trạng thái task đang làm

`resolved` là trạng thái task đã giải quyết được rồi - đã coding xong, tự mình test thử ok, tự mình cho là hợp lý, tuy nhiên chưa được người khác kiểm trứng, đánh giá

`close` là trạng thái task không còn được quan tâm nữa - có thể đã xong hẳn (test, release ở stg xong), có thể là không làm nữa

ngoài ra trạng thái task còn có thể có thể được custom và có `workflow` khác

### workflow nhận yêu cầu từ khách hàng

![](./output/workflow_voi_nguoi_giao_va_nhan_viec.svg)

### workflow đưa ra ý tưởng

![](./output/workflow_voi_nguoi_giao_va_nhan_viec_dua_ra_y_tuong.svg)

# tham khảo

- tham khảo 1 số từ workflow của DienDD(https://kipalog.com/users/DangDien/mypage)
- biểu đồ sequence diagram (https://bramp.github.io/js-sequence-diagrams/)
