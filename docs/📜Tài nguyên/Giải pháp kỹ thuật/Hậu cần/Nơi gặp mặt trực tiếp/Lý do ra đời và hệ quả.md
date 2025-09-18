---
share: true
created: 2025-05-06T12:52
description: Nó khác gì với những dự án tương tự khác? Nó chấp nhận những đánh đổi nào?
aliases:
  - Động lực
updated: 2025-09-18T19:43
---
# Lý do ra đời kho địa điểm để chọn nơi gặp mặt, và hệ quả của những lý do đó
[Kho địa điểm để chọn nơi gặp mặt](./index.md)
## Lý do ra đời
Trước đây đã có một số dự án tổng hợp địa điểm như Foody, Google Maps, D.Map, nhưng chúng đều không thoả mãn đồng thời cả 3 yêu cầu sau:
- Lấy người dùng làm trung tâm, chứ không phải xem họ như một loại tài nguyên
- Đáp ứng được các nhu cầu khác nhau một cách dễ dàng
- Người dùng có thể tự triển khai trên máy của họ với ít rào cản về kiến thức nhất

Tại sao lại có những yêu cầu này, và tại sao chương trình này chấp nhận đánh đổi những tiện lợi khác để đáp ứng các yêu cầu này?

### Lấy người dùng làm trung tâm, chứ không phải xem họ như một loại tài nguyên để trích xuất
Các SaaS tổng hợp địa điểm gặp mặt như Foody, do phải tính đến vấn đề tăng trưởng lợi nhuận, sẽ có xu hướng:
- Chèn quảng cáo, popup làm rối mắt
- Ưu tiên giới thiệu các cửa hàng trả tiền cho họ, chứ không giới thiệu thứ phù hợp nhất cho người dùng

Đây không phải là nơi để làm điều đó. Có người sẽ lập luận rằng việc kiếm tiền không xấu để ủng hộ cho hành vi này. Nhưng vẫn có những cách khác để kiếm tiền mà không phải làm những điều đó, như yêu cầu người dùng trả tiền để được sử dụng. (Nói cho chặt chẽ thì việc đó cũng không ngăn cản nhà phát hành cài cắm những kỹ thuật để thao túng, khai thác người dùng. Chỉ có những [phần mềm tự do và mã nguồn mở](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/T%E1%BB%B1%20tr%E1%BB%8B%20d%E1%BB%AF%20li%E1%BB%87u.%20M%C3%A3%20ngu%E1%BB%93n%20m%E1%BB%9F,%20ph%E1%BA%A7n%20m%E1%BB%81m%20t%E1%BB%B1%20do/Ph%E1%BA%A7n%20m%E1%BB%81m%20t%E1%BB%B1%20do%20v%C3%A0%20m%C3%A3%20ngu%E1%BB%93n%20m%E1%BB%9F/index.md) mới giải quyết triệt để vấn đề này.)

### Đáp ứng được các nhu cầu khác nhau một cách dễ dàng
Một người ở TPHCM sẽ có nhu cầu khác với một người ở Hà Nội: họ không quan tâm các địa điểm ở Hà Nội. Một người khuyết tật nhìn có nhu cầu khác với một người khuyết tật vận động: một người muốn đến nơi yên tĩnh, còn một người muốn đến nơi xe lăn đi lại dễ dàng được. Một người đi xe đạp có nhu cầu khác với một người đi xe buýt: người đi xe đạp muốn tìm quán gần nhà, còn người đi xe buýt muốn tìm quán gần các trạm xe.

Chưa kể, sự khác biệt đâu chỉ ở phía cầu, mà còn ở phía cung. Quán nước có những đặc điểm mà không gian làm việc chung, phòng họp riêng, địa điểm công cộng hay nhà riêng không có. Ngay cả trong quán nước cũng muôn hình vạn trạng: có quán cho dùng không gian miễn phí không cần gọi đồ uống, có quán thì cần gọi đồ uống. Có quán dùng ghế gây đau lưng, có quán dùng đèn gây đau mắt. Bất kể là tập trung vào đối tượng thụ hưởng nào thì những sự đa dạng này đã phải được tính đến.

Sẽ luôn luôn có những nhu cầu đặc biệt mà những người xây dựng nên nơi này cũng không tài nào đoán ra được. Sẽ có người hỏi rằng: tại sao không tập trung vào một nhu cầu và giải quyết nó cho thật tốt? Nhưng đó là nhu cầu nào? Chẳng lẽ lại là "nam dị tính hợp giới không khuyết tật trung niên trung lưu ở các quận nội thành TP.HCM cần tìm không gian thảo luận có máy chiếu và micro"? Còn nếu chỉ cần kiếm quán nước thôi thì cần gì tạo ra nơi này nữa, lên Google Maps luôn cho rồi. Động lực không phải là liệt kê tất cả các địa điểm đáp ứng một nhu cầu cụ thể, mà là không để việc thiếu thông tin xảy ra . Chứ 

Thực ra, việc đáp ứng thêm một nhu cầu nữa cũng đơn giản: chỉ cần thêm một *trường thông tin đầu vào* nữa thôi. Nên vấn đề không phải là lượng thông tin đầu vào, mà là cách ta phân loại chúng.

Trung tâm hoá dữ liệu. Nếu chỉ cho mình thôi thì đơn giản
Để giảm khả năng chết yểu
Tại sao lại cần điều này? Vì có như vậy nó mới tránh sự chết yểu

Google Sheet, Google Maps vì nó không nằm trong các

Không bỏ ai lại phía sau cũng có nghĩa là ai cũng biết được tới điều này. 

[Việc phân loại không quan trọng bằng việc chuẩn bị cho sự thay đổi cách phân loại](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Ngh%C4%A9%20v%E1%BB%81%20vi%E1%BB%87c%20ngh%C4%A9/B%E1%BA%A3n%20th%E1%BB%83%20lu%E1%BA%ADn/Ph%C3%A2n%20lo%E1%BA%A1i/Vi%E1%BB%87c%20ph%C3%A2n%20lo%E1%BA%A1i%20kh%C3%B4ng%20quan%20tr%E1%BB%8Dng%20b%E1%BA%B1ng%20vi%E1%BB%87c%20chu%E1%BA%A9n%20b%E1%BB%8B%20cho%20s%E1%BB%B1%20thay%20%C4%91%E1%BB%95i%20c%C3%A1ch%20ph%C3%A2n%20lo%E1%BA%A1i.md)

Đây
- Nhu cầu tùy biến cách phân loại, cấu trúc dữ liệu người dùng
- Nhu cầu về mở rộng chức năng


Thường gặp nhất là nhu cầu tùy biến cách phân loại, cấu trúc dữ liệu người dùng, và nhu cầu mở rộng chức năng.
### Tùy biến cách phân loại, cấu trúc dữ liệu người dùng

[Nhiệm vụ của kiến trúc sư không phải là liệt kê hết các tình huống sẽ xảy ra, mà là thiết kế để dù các tình huống không ngờ tới xảy ra thì vẫn hoạt động ổn định](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/K%E1%BB%B9%20thu%E1%BA%ADt%20ph%E1%BA%A7n%20m%E1%BB%81m/Ki%E1%BA%BFn%20tr%C3%BAc/Nhi%E1%BB%87m%20v%E1%BB%A5%20c%E1%BB%A7a%20ki%E1%BA%BFn%20tr%C3%BAc%20s%C6%B0%20kh%C3%B4ng%20ph%E1%BA%A3i%20l%C3%A0%20li%E1%BB%87t%20k%C3%AA%20h%E1%BA%BFt%20c%C3%A1c%20t%C3%ACnh%20hu%E1%BB%91ng%20s%E1%BA%BD%20x%E1%BA%A3y%20ra,%20m%C3%A0%20l%C3%A0%20thi%E1%BA%BFt%20k%E1%BA%BF%20%C4%91%E1%BB%83%20d%C3%B9%20c%C3%A1c%20t%C3%ACnh%20hu%E1%BB%91ng%20kh%C3%B4ng%20ng%E1%BB%9D%20t%E1%BB%9Bi%20x%E1%BA%A3y%20ra%20th%C3%AC%20v%E1%BA%ABn%20ho%E1%BA%A1t%20%C4%91%E1%BB%99ng%20%E1%BB%95n%20%C4%91%E1%BB%8Bnh.md). Một ngày nào đó các tỉnh thành được sắp xếp lại
Đòi hỏi chế độ dinh dưỡng đặc biệt mà những người xây dựng nên nơi này cũng không đoán ra được trước được

Không chỉ là nhu cầu về sự phân loại khác nhau, mà còn là sự trình bày khác nhau
Không phải là nơi gặp nói chuyện mà thư viện chẳng hạn

### Mở rộng chức năng. 

- Tự động cập nhật thông tin mới lên các nền tảng khác nhau
- Có thể truy vấn dữ liệu ở các nền tảng khác (VD: Discord) 
- Tự động tạo lịch Google Calendar

- [Tỉ lệ quay lại là thứ quan trọng nhất trong tăng trưởng](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Qu%E1%BA%A3n%20l%C3%BD%20d%E1%BB%B1%20%C3%A1n,%20ph%C3%A1t%20tri%E1%BB%83n%20s%E1%BA%A3n%20ph%E1%BA%A9m,%20x%C3%A2y%20d%E1%BB%B1ng%20t%E1%BB%95%20ch%E1%BB%A9c/Ph%C3%A1t%20tri%E1%BB%83n%20s%E1%BA%A3n%20ph%E1%BA%A9m/Ch%E1%BB%89%20s%E1%BB%91/T%C4%83ng%20tr%C6%B0%E1%BB%9Fng/T%E1%BB%89%20l%E1%BB%87%20quay%20l%E1%BA%A1i%20l%C3%A0%20th%E1%BB%A9%20quan%20tr%E1%BB%8Dng%20nh%E1%BA%A5t%20trong%20t%C4%83ng%20tr%C6%B0%E1%BB%9Fng.md)

### Người dùng có thể tự triển khai trên máy của họ với ít rào cản về kiến thức nhất
Trong kinh nghiệm của tôi, những dự án không vì lợi nhuận sau một thời gian đều lạc hậu do không có người quản lý kế thừa. Lý do là vì dữ liệu không được lưu trữ ở định dạng đơn giản, không dễ thao tác, khiến cho việc nhập liệu và chia sẻ dữ liệu trở nên khó khăn. 
giảm thiểu gánh nặng nhận thức trong việc nhập liệu và chia sẻ dữ liệu 

Đó là lý do các SaaS như Notion không phù hợp để làm nơi lưu trữ dữ liệu.
Ngay cả
Phải ở dạng dữ liệu đơn giản nhất 
sao chép dễ dàng, không khác gì sao chép tài liệu
dễ fork 

Ở ngay trong hệ thống dữ liệu
[Việc đổi mới sáng tạo bắt đầu bằng việc mỗi người có thể tự mình điều khiển được máy tính, chứ không phải có thêm một sản phẩm no code hay AI nữa](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/Vi%E1%BB%87c%20%C4%91%E1%BB%95i%20m%E1%BB%9Bi%20s%C3%A1ng%20t%E1%BA%A1o%20b%E1%BA%AFt%20%C4%91%E1%BA%A7u%20b%E1%BA%B1ng%20vi%E1%BB%87c%20m%E1%BB%97i%20ng%C6%B0%E1%BB%9Di%20c%C3%B3%20th%E1%BB%83%20t%E1%BB%B1%20m%C3%ACnh%20%C4%91i%E1%BB%81u%20khi%E1%BB%83n%20%C4%91%C6%B0%E1%BB%A3c%20m%C3%A1y%20t%C3%ADnh,%20ch%E1%BB%A9%20kh%C3%B4ng%20ph%E1%BA%A3i%20c%C3%B3%20th%C3%AAm%20m%E1%BB%99t%20s%E1%BA%A3n%20ph%E1%BA%A9m%20no%20code%20hay%20AI%20n%E1%BB%AFa.md)
[Những người tự thấy mình ngu công nghệ đơn giản là vì họ không được trao quyền tự trị dữ liệu](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/T%E1%BB%B1%20tr%E1%BB%8B%20d%E1%BB%AF%20li%E1%BB%87u.%20M%C3%A3%20ngu%E1%BB%93n%20m%E1%BB%9F,%20ph%E1%BA%A7n%20m%E1%BB%81m%20t%E1%BB%B1%20do/T%E1%BB%B1%20tr%E1%BB%8B%20d%E1%BB%AF%20li%E1%BB%87u/Nh%E1%BB%AFng%20ng%C6%B0%E1%BB%9Di%20t%E1%BB%B1%20th%E1%BA%A5y%20m%C3%ACnh%20ngu%20c%C3%B4ng%20ngh%E1%BB%87%20%C4%91%C6%A1n%20gi%E1%BA%A3n%20l%C3%A0%20v%C3%AC%20h%E1%BB%8D%20kh%C3%B4ng%20%C4%91%C6%B0%E1%BB%A3c%20trao%20quy%E1%BB%81n%20t%E1%BB%B1%20tr%E1%BB%8B%20d%E1%BB%AF%20li%E1%BB%87u.md)

Trung tâm hoá. Giảm gánh nặng cho người kế thừa

## Phân tích ca
Kho địa điểm này khác gì với những dự án tương tự khác?

### Bản đồ tiếp cận D.Map
[D.Map](https://dmap.drdvietnam.org/#/mapx) là một bản đồ hướng đến việc giúp người khuyết tật tìm kiếm các công trình công cộng tiếp cận. Dự án được USAID và UNDP Việt Nam tài trợ, và có sự tham gia của báo chí, tổ chức sự kiện ở nhiều tỉnh thành. Vào thời điểm ra mắt, nó có cả app cho Android và iOS, nhưng bây giờ đã bị gỡ xuống.

Kiến thức để tự vận hành một cơ sở dữ liệu thế này phức tạp hơn cho người không biết gì

![Pasted image 20250717114312.png](../../../../attachments/Pasted%20image%2020250717114312.png)
![Pasted image 20250717114251.png](../../../../attachments/Pasted%20image%2020250717114251.png)
Dường như dự án đã ngừng hoạt động. Trong [trang giới thiệu dự án](https://www.drdvietnam.org/vi/du-an/ban-do-tiep-can-dmap/gioi-thieu/), lần cuối cùng cập nhật là 2021. Các app Andoird và iOS cũng đã bị gỡ xuống. Chức năng đăng ký không hoạt động được.

## Hệ quả của các lý do trên
Giải pháp đáp ứng được tất cả các nhu cầu này là một [hệ thống tri thức cộng đồng](../../../Nhu%20c%E1%BA%A7u%20c%C3%B4ng%20ngh%E1%BB%87/H%E1%BB%87%20th%E1%BB%91ng%20th%C3%B4ng%20tin/X%C3%A2y%20d%E1%BB%B1ng%20h%E1%BB%87%20th%E1%BB%91ng%20tri%20th%E1%BB%A9c%20c%E1%BB%99ng%20%C4%91%E1%BB%93ng.md) dưới hình thức là một [tài liệu động](../../../Nhu%20c%E1%BA%A7u%20c%C3%B4ng%20ngh%E1%BB%87/Vi%E1%BA%BFt%20v%C3%A0%20qu%E1%BA%A3n%20l%C3%BD%20n%E1%BB%99i%20dung,%20ghi%20ch%C3%BA,%20t%C3%A0i%20li%E1%BB%87u/T%C3%A0i%20li%E1%BB%87u%20%C4%91%E1%BB%99ng.md) được lưu ở định dạng đơn giản nhất là văn bản thuần. 
[📐 Dự án](../../../../%F0%9F%93%90%20D%E1%BB%B1%20%C3%A1n/index.md)

Về mặt kỹ thuật, nó được viết bằng TypeScript với môi trường thực thi là Deno.

Nhược điểm 
Chuyển đổi sang Base có vẻ như là một xu hướng chung. 