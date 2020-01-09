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
Note right of Mình: nếu dự án có spec rõ\nràng từ ban đầu Mình\ncheck xem việc này\ncó trong trách\nnhiệm của mình\nkhông? có làm được\nkhông?

Mình-->Team: nếu cần thì hỏi team xem có làm được không
Note right of Team: check xem có\nlàm được hay không
Team-->Mình: nếu không làm được thì phải có lý do cụ thể\nVới quy tắc là không có việc gì không làm được\nchỉ có việc khó, phạm vi ảnh hưởng lớn nên\ntốn time
Note right of Mình: tự mình suy nghĩ xem\ncó hợp lý không
Mình-->K: xác nhận lại điều\nđang nghĩ nếu cần
K-->Mình: 2 bên đều OK
Note right of Mình: tạo task cho K

Note right of Mình: chọn người phụ\ntrách task là Mình

Mình->Team: truyền đạt cho team\n(tạo task bên team)

Note right of Mình: chuyển trạng thái\ntask từ `open`\nsang `progress` nếu\nđã truyền đạt với\nteam

Note left of K: K test trên stg
```

## đưa ra ý tưởng

```sequence
Mình->K: Says Hello
Note right of K: K thinks\nabout it
K->Mình: How are you?
Mình->K: I am good thanks!
```

# How to view this document

## preview

https://medium.com/technical-writing-is-easy/diagrams-in-documentation-markdown-guide-4e78419e8d2f

https://shd101wyy.github.io/markdown-preview-enhanced/#/

## from this resource to svg
https://bramp.github.io/js-sequence-diagrams/

click into `Download as SVG` button
