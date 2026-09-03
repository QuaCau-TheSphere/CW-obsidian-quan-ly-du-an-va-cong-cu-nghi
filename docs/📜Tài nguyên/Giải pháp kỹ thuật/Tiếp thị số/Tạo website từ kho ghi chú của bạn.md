---
share: true
created: 2026-09-02T15:57
updated: 2026-09-03T13:29
aliases:
  - mkdocs, lume, quartz
---
Nếu bạn muốn tạo một website từ kho ghi chú của bạn mà không muốn bỏ tiền mua gói Publish, bạn cần dùng một chương trình tạo website tĩnh (static site generator).  Dưới đây là 3 chương trình tạo web tĩnh mình nghĩ là tốt.

> [!Attention] Ý đồ trình bày 
> Với mỗi một chương trình sẽ có một phần giới thiệu chung, và phần nói về ưu điểm và nhược điểm. Phần ưu điểm và nhược điểm **chỉ liên quan đến nhu cầu tạo web cá nhân từ kho**. Những ưu điểm và nhược điểm đối với các nhu cầu khác sẽ được để vào phần giới thiệu.

### Mkdocs
Mkdocs được viết bằng Python, một ngôn ngữ đề cao việc dễ đọc, dễ viết, và được dùng nhiều cho những bạn làm về dữ liệu. Đặc biệt, theme Material của nó dùng thiết kế Material của Google, là một kiểu thiết kế phẳng theo nhiều lớp để tạo độ sâu. Theme này phù hợp khi bạn cần một trang web có một thanh điều hướng với nhiều nút, đủ đơn giản để không làm rối, nhưng lại không quá đơn giản để tạo ra được một giao diện ấn tượng với người dùng. 

Ưu điểm:
- Tập tin cấu hình `mkdocs.yml` là một tập tin YAML quen thuộc, không phải code gì cả
- Số lượng tính năng phong phú, đặc biệt là có nhiều kiểu markdown cho các nhu cầu đặc thù

Nhược điểm:
- Cài Python trên Windows có thể gặp trục trặc về đường dẫn. Cái này thì có người bị có người không. Nếu bị thì thêm `py -m` trước mọi dòng lệnh. Ví dụ `mkdocs serve` → `py -m mkdocs serve`

### Lume
Lume viết bằng JavaScript, Obsidian cũng viết bằng JavaScript, nên với Lume bạn chỉ cần học một ngôn ngữ để là đã có thể thao tác với Obsidian tốt hơn, ví dụ như viết DataviewJS, TemplaterJS. Nó phù hợp cho các trang blog hoặc wiki đơn giản.

Ưu điểm:
- Với mỗi thư mục bạn có thể đặt một tập tin cấu hình `_data.yaml` để cấu hình cho toàn bộ thư mục. Nếu bạn muốn một thư mục con có cấu hình khác thì chỉ cần tạo một tập tin `_data.yaml` khác vào trong thư mục con đó
- Trong trường hợp bạn phải chỉnh code, thì Lume dùng Deno, một môi trường thực thi tích hợp sẵn những tiến bộ mới nhất của JavaScript, tiện lợi hơn Node nhiều

Nhược điểm:
- Số theme còn ít
- Không có đồ thị liên kết các nút cho người dùng

### Quartz
Đây là một chương trình tạo web tĩnh được viết đặc biệt dành cho người dùng Obsidian. Tác giả của nó muốn thúc đẩy *sự giải trung tâm hoá ở web*, hay còn gọi là *dweb* hoặc *web 3.0*. Mình đoán là cái gọi là khu vườn số cũng nằm trong dòng chảy này. Bạn có thể xem video phỏng vấn tác giả ở [đây](https://www.youtube.com/watch?v=YCvV7Izqggc). Quartz phù hợp cho người cần có đồ thị mạng lưới mối quan hệ giữa các ghi chú trên web.

Ưu điểm:
- Có sẵn đồ thị và backlink

Nhược điểm: 
- Tập tin cấu hình là `quartz.config.ts` hoặc `quartz.layout.ts`, nghĩa là để cấu hình là bạn phải dùng TypeScript để chỉnh
- Dùng Node

Nếu bạn muốn tìm hiểu thêm về môi trường thực thi Node và Deno thì có thể đọc bài này: [Code giống như các nốt nhạc, engine giống như nhạc công, còn runtime giống như nhạc cụ](https://doi-thoai.deno.dev/We.48.1)

## Xem thêm
- [Người dùng cá nhân hoặc dự án nhỏ có nên dùng WordPress hay không?](./WordPress%20gi%C3%BAp%20vi%E1%BB%87c%20t%E1%BA%A1o%20web%20d%E1%BB%85%20d%C3%A0ng%20nh%E1%BA%A5t,%20ch%E1%BB%A9%20kh%C3%B4ng%20ph%E1%BA%A3i%20l%C3%A0%20th%E1%BB%A9%20qu%E1%BA%A3n%20l%C3%BD%20web%20hi%E1%BB%87u%20qu%E1%BA%A3%20nh%E1%BA%A5t.md)
- [Các buổi đáp ứng nhu cầu học cách sử dụng công cụ và tư duy lập trình cho nhu cầu công việc](../../../%F0%9F%93%90%20D%E1%BB%B1%20%C3%A1n/C%C3%A1c%20bu%E1%BB%95i%20hu%E1%BA%A5n%20luy%E1%BB%87n%20l%E1%BA%ADp%20tr%C3%ACnh/9%20Blog/C%C3%A1c%20bu%E1%BB%95i%20%C4%91%C3%A1p%20%E1%BB%A9ng%20nhu%20c%E1%BA%A7u%20h%E1%BB%8Dc%20c%C3%A1ch%20s%E1%BB%AD%20d%E1%BB%A5ng%20c%C3%B4ng%20c%E1%BB%A5%20v%C3%A0%20t%C6%B0%20duy%20l%E1%BA%ADp%20tr%C3%ACnh%20cho%20nhu%20c%E1%BA%A7u%20c%C3%B4ng%20vi%E1%BB%87c.md)

## Nơi thảo luận
![](https://i.imgur.com/4fq665i.png)
