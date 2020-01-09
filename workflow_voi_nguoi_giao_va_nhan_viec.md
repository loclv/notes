# How to view this document

## preview

https://medium.com/technical-writing-is-easy/diagrams-in-documentation-markdown-guide-4e78419e8d2f

https://shd101wyy.github.io/markdown-preview-enhanced/#/

## from this resource to svg
https://bramp.github.io/js-sequence-diagrams/

click into `Download as SVG` button

---

# workflow

workflow khi trao đổi với *Khách hàng/PM* - ký hiệu là `K`

có thể áp dụng cho *BrSE, technical leader, team leader* - ký hiệu là `Mình`

phần mềm quản lý task thông thường như:
- backlog
- jira
- trello
- ...

## nhận yêu cầu từ khách hàng

```sequence
K->Mình: nói việc muốn làm
Note right of Mình: nếu dự án có spec rõ \n ràng từ ban đầu Mình \n check xem việc này \n có trong trách \n nhiệm của mình \n không?

Mình-->K: xác nhận lại điều \n đang nghĩ nếu cần
K-->Mình: 2 bên đều OK

Note right of Mình: có làm được \n không?

Mình-->Team: nếu cần thì hỏi team xem có làm được không

Note right of Team: check xem có \n làm được hay không
Team-->Mình: nếu không làm được thì phải có lý do cụ thể \n Với quy tắc là không có việc gì không làm được \n chỉ có việc khó, phạm vi ảnh hưởng lớn nên \n tốn time
Note right of Mình: tự mình suy nghĩ \n xem lý do có \n hợp lý không? \n vì trước khi giao \n cho mình, K đã phải \n suy nghĩ rồi
Mình-->K: xác nhận lại điều \n đang nghĩ nếu cần
K-->Mình: 2 bên đều OK

Note right of Mình: nếu K đồng ý \n không làm nữa thì \n dừng ở đây

Note right of Mình: tạo task cho K

Note right of Mình: chọn người phụ \n trách task là Mình

Mình->Team: truyền đạt cho team \n (tạo task bên team)

Note right of Mình: chuyển trạng thái \n task từ `open` \n sang `progress`

Note left of K: K test trên stg
```

## đưa ra ý tưởng

```sequence
Mình->K: Says Hello
Note right of K: K thinks \n about it
K->Mình: How are you?
Mình->K: I am good thanks!
```
