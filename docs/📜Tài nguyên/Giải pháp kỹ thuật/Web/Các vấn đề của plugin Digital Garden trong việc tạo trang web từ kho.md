---
share: true
blog: done
created: 2024-08-17T11:00
updated: 2026-09-02T16:02
description: Plugin Digital Garden sử dụng 11ty làm chương trình tạo website, và Vercel làm dịch vụ hosting. Chúng có những nhược điểm gì?
---
Nếu bạn không muốn mua gói Publish nhưng vẫn muốn tạo một website từ kho của bạn thì bạn cần 3 thứ sau:
- Một plugin để đẩy ghi chú từ máy của bạn lên GitHub
- Một chương trình tạo website từ các ghi chú
- Một dịch vụ hosting để ai cũng có thể truy cập web của bạn

Qua buổi hướng dẫn tạo web từ kho đầu tiên thì mình thấy một điểm chung là dường như nhiều bạn bắt đầu hành trình của mình bằng plugin [Digital Garden](https://github.com/oleeskild/obsidian-digital-garden "oleeskild/obsidian-digital-garden"). Có thể là vì cái tên của nó khiến cho nó dễ được tìm đến nhất. 

Tuy nhiên, plugin này sử dụng **11ty** làm chương trình tạo website, và **Vercel** làm dịch vụ hosting. Mình thấy chúng có những bất cập sau:
- Digital Garden ít chức năng và ít cập nhật
- Dịch vụ hosting Vercel hoặc Netlify là những dao 
- Hướng dẫn sử dụng bỏ qua bước tạo website trên trên máy bạn

## Digital Garden ít chức năng và ít cập nhật
Vào thời điểm viết bài, hiện tại có tới [207 vấn đề được cộng đồng gửi đến](https://github.com/oleeskild/obsidian-digital-garden/issues "Issues · oleeskild/obsidian-digital-garden"). Gần như không có cái nào được tác giả phản hồi cả. Hồi mới tập tành làm web mình cũng bắt đầu với plugin này, nhưng không dùng được vì bị lỗi tiếng Việt. [Mình có gửi vấn đề lên](https://github.com/oleeskild/obsidian-digital-garden/issues/292 "Why are there so much 404 error? · Issue #292 · oleeskild/obsidian-digital-garden") nhưng cũng chịu số phận như rất nhiều vấn đề khác. 

Mình dùng plugin [Enveloppe](https://enveloppe.github.io/) để đưa ghi chú từ máy lên GitHub và chưa thấy có điểm gì để chê. Nó có nhiều tính năng để tuỳ chỉnh, và tác giả của nó rất nhiệt tình sửa lỗi và tương tác với người dùng. Mình cũng có đóng góp cho plugin này. 

## Dịch vụ hosting Vercel hoặc Netlify là những dao mổ trâu giết gà
Digital Garden mặc định là dùng Vercel vì bạn không tạo đồ thị bằng GitHub Page được. Nếu bạn không cần đồ thị cho web thì GitHub Page đơn giản hơn và phù hợp cho nhu cầu cơ bản của bạn. Tất nhiên, sau khi thành thạo rồi bạn sẽ thấy các dịch vụ này cho bạn nhiều tính năng hay ho hơn rất nhiều. Đến cả mình, sau khi dùng Netlify một thời gian, đủ để tạm hiểu nó và thấy GitHub Page ít chức năng thật, thì mình vẫn chuyển các trang web của mình từ Netlify về lại GitHub Page, vì mình vẫn thấy chưa thực sự cần phải đánh đổi sự phức tạp trong việc sử dụng để có được những tính năng này. Hồi mới lớ ngớ làm web mình dùng Netlify không cẩn thận nên bị nó mổ mất $7 vì build quá nhiều. Ở GitHub Page thì không lo chuyện đó.

## Hướng dẫn sử dụng bỏ qua bước tạo website trên trên máy bạn
Nếu mục đích là làm sao để tạo website cho nhanh để mà còn làm việc khác thì đúng là bạn sẽ không cần phải tạo web trên máy mình. Nhưng theo mình thì đây là bước giúp bạn vỡ ra được nhiều thứ về cách hoạt động của một trang web, vì nó sẽ đòi hỏi bạn cần dùng Git để quản lý phiên bản và terminal để ra lệnh cho các tất cả các chương trình liên quan. Khi bạn tuỳ chỉnh website, bạn sẽ phải thao tác trên tập tin cấu hình cũng như sắp xếp các thư mục cho các tập tin bổ trợ, và chắc chắn bạn sẽ phải xử lý nó trên máy của bạn trước. Kể cả khi bạn không cần làm việc đó thì nó cũng tiện lợi và an toàn hơn là đẩy trực tiếp lên hosting. 

## Có những chương trình tạo web mới khắc phục được những nhược điểm của 11ty
Để tạo ra website từ các tập tin markdown, bạn cần dùng một chương trình tạo website tĩnh (static site generator):
![Fetching Title#vu93](https://cdn-media-1.freecodecamp.org/images/0*CCMaHN9JpmvIFNdi)

11ty là chương trình tạo website tĩnh được tích hợp với Digital Garden. Nó dùng một môi trường thực thi tên là Node và nhập plugin bằng CommonJS. CommonJS thì lạc hậu, Node thì bất tiện với người dùng mới. Bài viết [Những chương trình tạo web từ kho tốt](./Nh%E1%BB%AFng%20ch%C6%B0%C6%A1ng%20tr%C3%ACnh%20t%E1%BA%A1o%20web%20t%E1%BB%AB%20kho%20t%E1%BB%91t.md) sẽ giới thiệu 3 chương trình tạo web tĩnh mà mình nghĩ là tốt hơn 11ty.