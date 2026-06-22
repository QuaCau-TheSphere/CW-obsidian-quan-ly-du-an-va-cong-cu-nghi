---
share: true
created: 2023-10-27T18:59
updated: 2026-01-14T13:11
cssclasses:
  - wide-table
aliases:
  - heading
  - đặt tên
  - filename
  - title
description: Có nhiều vị trí tiêu đề với những chức năng khác nhau, và có nhiều cách khác nhau để thay đổi chúng. Nên dùng loại nào cho trường hợp nào?
---
Một tiêu đề có rất nhiều chức năng:
- Tạo kích thích cho người đọc, khiến họ thấy vì sao họ cần đọc bài đó, dù họ đang không tìm kiếm thông tin về nó
- Tóm tắt vấn đề
- Quản lý tập tin

Lý tưởng nhất thì chỉ cần dùng một thứ để đặt cho tất cả những cái này. Và đó là filename. Chính vì như vậy, nên filename nên là thứ mặc định. Nhưng có những lúc nó chứa ký tự đặc biệt hoặc đường dẫn quá dài thì Windows hoặc Git sẽ không chịu, nên ta nên có một trường khác có chức năng làm mặc định cho những thứ còn lại. Đó chính là `title` trong frontmatter hoặc `<h1>` trong body. 

Trên Obsidian có plugin [Front Matter Title](https://github.com/snezhig/obsidian-front-matter-title) giúp ta quản lý được những chuyện này.

## Khi nào dùng `title` trong frontmatter, còn khi nào dùng `<h1>` trong body? 
Khi bạn mở một ghi chú lên, bạn sẽ thấy ngay lập tức có một tiêu đề đập vào mắt bạn. Ví dụ, với ghi chú bạn đang đọc thì nó sẽ trông thế này: 
![](https://i.imgur.com/1HydSvK.png)

Khi sử dụng plugin Front Matter Title, ta có thể thiết lập sao cho `title` sẽ làm thay đổi tiêu đề trên cao này, còn `<h1>` thì không. Tuỳ thuộc vào câu chữ ta đang đinh ninh khi truy cập từ cây thư mục mà ta có những cách để thay đổi tiêu đề cho hiệu quả.

### Dùng `<h1>` khi tiêu đề đọc từ cây thư mục khác với tiêu đề nội dung về mặt ngữ nghĩa
Ví dụ, trong thư mục `📜Tài nguyên/Giải pháp kỹ thuật/Web` có [ghi chú này](../Web/WordPress%20gi%C3%BAp%20vi%E1%BB%87c%20t%E1%BA%A1o%20web%20d%E1%BB%85%20d%C3%A0ng%20nh%E1%BA%A5t,%20ch%E1%BB%A9%20kh%C3%B4ng%20ph%E1%BA%A3i%20l%C3%A0%20th%E1%BB%A9%20qu%E1%BA%A3n%20l%C3%BD%20web%20hi%E1%BB%87u%20qu%E1%BA%A3%20nh%E1%BA%A5t.md). Tên của nó trong cây thư mục là:
```
WordPress giúp việc tạo web dễ dàng nhất, chứ không phải là thứ tạo web hiệu quả nhất
```
Nhưng nếu bạn mở ra, thì bạn sẽ thấy nó là một bài viết dài. Nếu đọc bài đó thì sẽ thấy đặt tên nó thế này sẽ là hợp nhất.
```
Người dùng cá nhân hoặc dự án nhỏ có nên dùng WordPress hay không?
```
![](https://i.imgur.com/koC5yyi.png)

Giờ, nếu bạn không có tiêu đề thì đang đinh ninh tiêu đề phải giống, nếu khác thì sẽ bị khựng. Nhưng nếu để nguyên tiêu đề của cây thư mục thì sẽ bị lệch so với nội dung, nên cần phải có thể một tiêu đề khác để chuẩn bị cho mình rằng nội dung mới có tiêu đề khác với tiêu đề từ cây thư mục.

Các ghi chú tương tự: [📜Tài nguyên](../../index.md), [Nhu cầu công việc](../../Nhu%20c%E1%BA%A7u%20c%C3%B4ng%20vi%E1%BB%87c/index.md)

### Dùng `title` khi tiêu đề đọc từ cây thư mục giống với tiêu đề nội dung về mặt ngữ nghĩa
Ví dụ, trong thư mục `📜Tài nguyên/Giải pháp kỹ thuật/Hậu cần/Nơi gặp mặt trực tiếp/TP.HCM` có [ghi chú này](../H%E1%BA%ADu%20c%E1%BA%A7n/N%C6%A1i%20g%E1%BA%B7p%20m%E1%BA%B7t%20tr%E1%BB%B1c%20ti%E1%BA%BFp/TP.HCM/index.md). Bởi vì nó là ghi chú thư mục, nên nó cần có tên là:
```
TP.HCM
```
Nhưng lúc mở ra thì thấy hơi khó hiểu. Nếu tiêu đề trên cao là như này thì sẽ rõ nghĩa hơn:
```
Nơi gặp mặt trực tiếp tại TP.HCM
```

Ví dụ khác, [Kế hoạch (khái niệm)](../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/%CE%9E%20Kh%C3%A1i%20ni%E1%BB%87m/Ph%C3%A1t%20tri%E1%BB%83n%20s%E1%BA%A3n%20ph%E1%BA%A9m,%20l%C3%AAn%20k%E1%BA%BF%20ho%E1%BA%A1ch,%20c%C3%B4ng%20vi%E1%BB%87c/K%E1%BA%BF%20ho%E1%BA%A1ch%20(kh%C3%A1i%20ni%E1%BB%87m).md) phải mở ngoặc vì nếu không nó sẽ trùng tên với [Kế hoạch tổ chức các buổi đáp ứng nhu cầu học cách sử dụng công cụ và tư duy lập trình](../../../%F0%9F%93%90%20D%E1%BB%B1%20%C3%A1n/C%C3%A1c%20bu%E1%BB%95i%20hu%E1%BA%A5n%20luy%E1%BB%87n%20l%E1%BA%ADp%20tr%C3%ACnh/4%20Th%C3%A0nh%20ph%E1%BA%A9m/K%E1%BA%BF%20ho%E1%BA%A1ch/index.md). Dùng `title` để không phải thấy cái ngoặc.

Bổ sung những thông tin được hiểu ngầm trong lúc truy cập từ cây thư mục, nhưng không có khi liên kết từ nơi khác.

Nên trong trường hợp này là dùng `title` để thay đổi tiêu đề trên cao luôn.

| Vai trò                                                                                                            | Vị trí xuất hiện                                                    | Cách điều chỉnh | Nếu không điều chỉnh thì mặc định sẽ lấy giá trị từ | Sử dụng khi                                                                                                          |
| ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------- | --------------- | --------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| Quản lý tập tin từ hệ điều hành. Tạo slug                                                                          | filename: lúc xuất file, terminal, Windows Explorer, dữ liệu Dataview                | filename        | Luôn có                                             | Luôn sử dụng                                                                                                         |
| Cho phép filename không phải slugify quá nhiều ký tự đặc biệt                                                      | Enveloppe tạo git                                                   | `filename`      | filename                                            | Có thể dùng khi gặp tên dài, và thấy việc tránh alias dài quan trọng hơn việc URL trên web và trên vault giống nhau* |
| Nhận diện bài viết, tóm tắt nội dung, quản lý theo cấu trúc của tác giả hoặc người đang tìm kiếm theo một cấu trúc | Tiêu đề: trên cao, file explorer, breadcrumb, menu, navigation pane | `title`         | filename                                            | Tiêu đề chứa ký tự đặc biệt hoặc quá dài*. Tiêu đề đọc từ cây thư mục giống với tiêu đề nội dung về mặt ngữ nghĩa    |
| Tạo dự đoán cho người đọc về nội dung bên trong, làm cho họ thấy vì sao họ cần đọc bài đó, đáp ứng câu hỏi của họ  | Headline (`<title>`, `<h1>`)                                        | Markdown `#`    | `title`, filename                                   | Mental model của người đã hiểu nó rồi khác với mental model của người chưa hiểu nó                                   |
| Nối tiếp dòng suy nghĩ                                                                                             | Liên kết (`[[]]`, `<a>`)                                            | `alias`         | `title`, filename                                   |                                                                                                                      |
|                                                                                                                    | Search autocomplete, kết quả Google                                 | Không cần chỉnh | `alias`, `title`, filename                          |                                                                                                                      |
| Tiêu đề lúc chia sẻ trên Facebook                                                                                  | Tiêu đề trong Open Graph (`meta property="og:title"`)               | `ogTitle`       | `title`, filename                                   |                                                                                                                      |

Xem thêm:: [Các loại alias](./C%C3%A1c%20lo%E1%BA%A1i%20alias.md)

## \*Cách xử lý khi gặp tên dài và có ký tự đặc biệt
| Lựa chọn                                      | Ưu điểm                                                             | Nhược điểm                                                          |
| --------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| Không thay đổi tên, nhưng thay đổi `filename` |                                                                     | URL trên web và trên máy khác nhau. Không xử lý được ký tự đặc biệt |
| Thay đổi tên, và thay đổi `title`             | URL trên web và trên máy không khác nhau. Xử lý được ký tự đặc biệt |                                                                     |
| Không thay đổi tên và dùng `h1`               | URL trên web và trên máy không khác nhau. Xử lý được ký tự đặc biệt | Có 2 tiêu đề. Không tự động tạo alias cho tiêu đề thực sự           |

Điều đó khiến cho việc luôn dùng `title` luôn đảm bảo được các vấn đề kỹ thuật, và đỡ phải suy nghĩ phải lựa chọn cái nào.

`<h1>` dùng khi chắc chắn chỉ dùng tên thật chứ không dùng `<h1>` khi liên kết. VD: `Prudential` chứ không phải `Làm đại lý ảo Prudential`

---
- Có lúc chỉ muốn đặt tiêu đề là câu hỏi, dù có thể đặt theo chủ đề. VD: [Làm sao để tìm được thứ cần tìm khi không biết từ khoá chính xác của nó?](../H%E1%BB%8Dc%20t%E1%BA%ADp/L%C3%A0m%20sao%20%C4%91%E1%BB%83%20t%C3%ACm%20%C4%91%C6%B0%E1%BB%A3c%20th%E1%BB%A9%20c%E1%BA%A7n%20t%C3%ACm%20khi%20kh%C3%B4ng%20bi%E1%BA%BFt%20t%E1%BB%AB%20kh%C3%B3a%20ch%C3%ADnh%20x%C3%A1c%20c%E1%BB%A7a%20n%C3%B3.md)
- Có lúc thì chỉ muốn đặt theo chủ đề, dù có thể đặt theo câu hỏi. VD: [Các loại tiêu đề và cách dùng chúng](C%C3%A1c%20lo%E1%BA%A1i%20ti%C3%AAu%20%C4%91%E1%BB%81%20v%C3%A0%20c%C3%A1ch%20d%C3%B9ng%20ch%C3%BAng.md)

## Path
Giữ nguyên path?
Phản đối:
- Không đáng kể
- Người muốn tìm đến thì sẽ tìm được thôi. Search cũng không khó
