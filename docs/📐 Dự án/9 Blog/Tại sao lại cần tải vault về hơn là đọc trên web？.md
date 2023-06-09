---
share: True
---
Trong ngành khoa học máy tính, [[../../⚡Hiểu biết sâu/Khoa học máy tính/Hợp tác làm việc/Việc hợp tác làm việc thời gian thực với dữ liệu được lưu ở local là một bài toán khó|Việc hợp tác làm việc thời gian thực với dữ liệu được lưu ở local là một bài toán khó]]. Điều đó khiến cho [[../../⚡Hiểu biết sâu/Khoa học máy tính/Hợp tác làm việc/Có sự đánh đổi giữa sự tự do sử dụng dữ liệu và sự tiện lợi trong việc hợp tác|chúng ta phải đánh đổi giữa sự tự do sử dụng dữ liệu và sự tiện lợi trong việc hợp tác]]. Hay nói cách khác, [[../../⚡Hiểu biết sâu/Khoa học máy tính/Hợp tác làm việc/Việc trung tâm hoá việc lưu trữ dữ liệu trên máy chủ sẽ lấy đi autonomy và agency của người dùng cuối|Việc trung tâm hoá việc lưu trữ dữ liệu trên máy chủ sẽ lấy đi autonomy và agency của người dùng cuối]]. Xu thế hiện nay là [[../../⚡Hiểu biết sâu/Khoa học máy tính/Hợp tác làm việc/Các nhóm làm việc qua mạng ngày càng nhiều|Các nhóm làm việc qua mạng ngày càng nhiều]], đến nỗi khi được hỏi về app đa số mọi người sẽ chỉ nhắc đến những cloud app như Google Drive hay Notion. Nghĩa là chúng ta đã hy sinh quá nhiều sự tự chủ dữ liệu cho sự tiện lợi đến nỗi chúng ta không còn biết gì về một loạt các phần mềm khác mạnh mẽ hơn. Việc đánh mất sự tự chủ đó là lý do khiến cho chúng ta luôn cảm thấy mình mù công nghệ, và chấp nhận rằng mình sẽ chẳng hiểu gì về công nghệ cả. Đây chính là một sự bất lực học được. [[../../⚡Hiểu biết sâu/Khoa học máy tính/Người không học về lập trình thấy việc lập trình như làm phép thuật|Người không học về lập trình thấy việc lập trình như làm phép thuật]], trong khi [[../../⚡Hiểu biết sâu/Khoa học máy tính/Lập trình viên biết lập trình chủ yếu là nhờ biết google|Lập trình viên biết lập trình chủ yếu là nhờ biết google]]. Bạn cũng biết google vậy, vậy tại sao vẫn thấy nó giống như làm phép thuật? Chúng tôi nghĩ một phần lớn là vì đã từ lâu bạn không còn cảm giác mình có sự tự chủ với dữ liệu của mình rồi. Khi bạn đã có lại được cảm giác đó, bạn sẽ thấy mình tự tin hơn về công nghệ.

Bạn có thể bắt đầu có lại cảm giác đó bằng cách tải dữ liệu của web này về.

[[../3 Thành phẩm/Phần mềm/Bộ cài/Hướng dẫn tải vault|Hướng dẫn tải vault]]{ .md-button .md-button--primary }

# Những thứ mà chỉ phiên bản trên Obsidian mới có mà bản web không có
Về cơ bản, những thứ này có được là do [[../../📜 Tài nguyên/💎 Giới thiệu về Obsidian/Mô tả về Obsidian/Obsidian lưu dữ liệu nằm trên máy của người dùng|Obsidian lưu dữ liệu nằm trên máy của người dùng]]. Đây là một số hệ quả của việc đó:

## Tất cả các phím tắt, chức năng và plugin của Obsidian, bao gồm cả những thứ bạn thiết lập riêng cho mình
Ví dụ, ở trên Obsidian, bạn có thể xem được đồ thị mối liên hệ giữa các ghi chú trong phần [[../../⚡Hiểu biết sâu/⚡Hiểu biết sâu|⚡Hiểu biết sâu]]:
![](https://i.imgur.com/gwdeLlL.png)

Đồ thị này cho thấy được có những ghi chú nào nổi trội trong đây, cũng như mức độ liên kết của chúng. Bạn có thể thấy chúng rời rạc khá nhiều.

Hoặc nếu đọc trên web bạn sẽ không có phần biết xem có những ghi chú nào liên kết tới trang bạn đang đọc như thế này:
![](https://i.imgur.com/UbXZspz.png)

Xem thêm:: [[../../📜 Tài nguyên/💎 Giới thiệu về Obsidian/Theo tính năng của plugin/Theo tính năng của plugin|Obsidian có những tính năng nào hay?]]

## Thời gian chuyển trang gần như là tức thời
Điều này giúp bạn nhanh chóng kiểm tra giả thiết các câu hỏi của bạn.

## Các file không thể hoặc không cần phải để lên web
Ví dụ:
- Các file PDF hoặc thu âm do không phải là định dạng markdown nên sẽ không có YAML. Mà plugin tạo web, [Mkdocs Publisher](https://obsidian-publisher.netlify.app/github%20publisher/commands/#upload "Commands - Obsidian Mkdocs Publisher") đòi hỏi phải có từ khoá `share` trong YAML thì mới đăng lên web
- Các file trong thư mục `Thiết lập` dù ở dạng markdown nhưng việc để lên web cũng không cần thiết
- Các file có dung lượng lớn hơn 100 MB thì GitHub không chịu nhận

# Vậy bản web được sinh ra để làm gì?
- Dễ giới thiệu cho người mới, 
- Dễ quảng bá dự án,
- ~~Tăng SEO~~  Thêm nguồn tài nguyên chất lượng cho các máy tìm kiếm như Google, Bing
- Thêm nguồn ngữ liệu chất lượng để huấn luyện cho máy

## Những lỗi trên bản web 
- Search 
- Nếu có h1 ngay đầu ghi chú thì tiêu đề sẽ là cái h1 đó
- Không tự chuyển trang nên hay gặp 404
- Cache 🤡

Ví dụ, những trang có dataview sẽ không chắc được cập nhật, do plugin tạo web không thấy trang đó có sự thay đổi gì.

Về cơ bản, **những lỗi này không được ưu tiên sửa**. Do nhiệm vụ của nó là để dễ giới thiệu cho người mới, nên khi nó đã làm xong nhiệm vụ của mình thì có lẽ nên tập trung sức lực cho những thứ khác. Để biết những thứ cần được ưu tiên hơn, bạn có thể đọc trong [[../📐 Dự án|📐 Dự án]].

[[../3 Thành phẩm/Phần mềm/Bộ cài/Hướng dẫn tải vault|Hướng dẫn tải vault]]{ .md-button .md-button--primary }
