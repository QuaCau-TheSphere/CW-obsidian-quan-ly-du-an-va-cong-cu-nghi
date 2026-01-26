---
share: true
created: 2025-05-06T12:52
updated: 2026-01-Mo'T'16:32
description: Nó khác gì với những dự án tương tự khác? Nó chấp nhận những đánh đổi nào?
aliases:
  - Động lực
---
# Lý do ra đời kho địa điểm để chọn nơi gặp mặt, và hệ quả của những lý do đó
## Lý do ra đời
[Kho địa điểm để chọn nơi gặp mặt](./index.md) đến từ mong muốn kết nối người cần tìm địa điểm với người có địa điểm. Dự án mong muốn một điều *duy nhất*: **Làm cho người cần tìm địa điểm gặp mặt có thể tìm được địa điểm phù hợp với nhu cầu riêng biệt của mình một cách nhanh nhất**.

Để làm được điều đó thì nó cần đáp ứng được các yêu cầu sau:
- Lấy người dùng làm trung tâm, chứ không phải xem họ như một loại tài nguyên để khai thác
- Giảm gánh nặng nhận thức trong việc cung cấp, quản lý, sử dụng và chia sẻ dữ liệu theo những nhu cầu đặc thù của họ. Điều này bao gồm:
	- Người dùng có thể tạo dữ liệu mới bằng ít lần bấm nhất có thể
	- Hệ thống phân loại địa điểm phải có khả năng chuẩn bị cho sự thay đổi cách phân loại một cách dễ dàng
	- Dữ liệu có sẵn trong kho thông tin của người dùng có thể được tải lên kho chung một cách thụ động và hàng loạt 
	- Người dùng có thể tự triển khai hệ thống của riêng họ cho nhóm người dùng của riêng họ
	- Chức năng mới có thể bổ sung dễ dàng 

Do không tìm được chương trình nào thỏa mãn được những điều đó nên tôi bắt tay vào làm. Đây là một phần của dự án [Phá vỡ silo thông tin, nắm bắt nhu cầu các bên và sử dụng các nguồn tài nguyên cộng đồng hiệu quả](../../../../%F0%9F%93%90%20D%E1%BB%B1%20%C3%A1n/M%C3%B4%20t%E1%BA%A3%20d%E1%BB%B1%20%C3%A1n.md)

## Phân tích ca
Để hiểu được vì sao cần những lý do này, có thể xem qua những dự án tương tự trước đây. Trước đây đã có một số dự án tổng hợp địa điểm như Foody, Google Maps, D.Map, nhưng chúng đều không thoả mãn đồng thời các yêu cầu trên. Tại sao lại có những yêu cầu này, và tại sao chương trình này chấp nhận đánh đổi những tiện lợi khác để đáp ứng các yêu cầu này?
Kho địa điểm này khác gì với những dự án tương tự khác?

### Foody
Chỉ tập trung vào ăn uống

### Google Maps
### Notion
[Google Sheet hoặc Notion không phù hợp khi dữ liệu trở nên phức tạp](../../T%E1%BB%95%20ch%E1%BB%A9c,%20s%E1%BA%AFp%20x%E1%BA%BFp%20d%E1%BB%AF%20li%E1%BB%87u/Ch%C6%B0%C6%A1ng%20tr%C3%ACnh/Google%20Sheet%20ho%E1%BA%B7c%20Notion%20kh%C3%B4ng%20ph%C3%B9%20h%E1%BB%A3p%20khi%20d%E1%BB%AF%20li%E1%BB%87u%20tr%E1%BB%9F%20n%C3%AAn%20ph%E1%BB%A9c%20t%E1%BA%A1p.md)
### Bản đồ tiếp cận D.Map
[D.Map](https://dmap.drdvietnam.org/#/mapx) là một bản đồ hướng đến việc giúp người khuyết tật tìm kiếm các công trình công cộng tiếp cận. Dự án được USAID và UNDP Việt Nam tài trợ, và có sự tham gia của báo chí, tổ chức sự kiện ở nhiều tỉnh thành. Vào thời điểm ra mắt, nó có cả app cho Android và iOS.

Kiến thức để tự vận hành một cơ sở dữ liệu thế này phức tạp hơn cho người không biết gì

![Pasted image 20250717114312.png](../../../../attachments/Pasted%20image%2020250717114312.png)
![Pasted image 20250717114251.png](../../../../attachments/Pasted%20image%2020250717114251.png)
Dường như dự án đã ngừng hoạt động. Trong [trang giới thiệu dự án](https://www.drdvietnam.org/vi/du-an/ban-do-tiep-can-dmap/gioi-thieu/), lần cuối cùng cập nhật là 2021. Các app Andoird và iOS cũng đã bị gỡ xuống. Chức năng đăng ký không hoạt động được.

## Yêu cầu
### Lấy người dùng làm trung tâm, chứ không phải xem họ như một loại tài nguyên để trích xuất
Các SaaS tổng hợp địa điểm gặp mặt như Foody, do phải tính đến vấn đề lợi nhuận, sẽ có xu hướng:
- Chèn quảng cáo, popup làm rối mắt
- Ưu tiên giới thiệu các cửa hàng trả tiền cho họ, chứ không giới thiệu thứ phù hợp nhất cho người dùng

Đây không phải là nơi để làm điều đó. Có người sẽ lập luận rằng việc kiếm tiền không xấu. Nhưng vẫn có những cách khác để kiếm tiền mà không phải làm những điều đó, như yêu cầu người dùng trả tiền để được sử dụng. (Nói cho chặt chẽ thì việc đó cũng không ngăn cản nhà phát hành cài cắm những kỹ thuật để khai thác người dùng. Chỉ có những [phần mềm tự do và mã nguồn mở](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/T%E1%BB%B1%20tr%E1%BB%8B%20d%E1%BB%AF%20li%E1%BB%87u.%20M%C3%A3%20ngu%E1%BB%93n%20m%E1%BB%9F,%20ph%E1%BA%A7n%20m%E1%BB%81m%20t%E1%BB%B1%20do/Ph%E1%BA%A7n%20m%E1%BB%81m%20t%E1%BB%B1%20do%20v%C3%A0%20m%C3%A3%20ngu%E1%BB%93n%20m%E1%BB%9F/index.md) mới giải quyết triệt để vấn đề này.) Việc yêu cầu người dùng trả tiền không đi ngược lại yêu cầu này.

### Giảm gánh nặng nhận thức trong việc cung cấp, quản lý, sử dụng và chia sẻ dữ liệu theo những nhu cầu đặc thù của họ
Trong quan sát của tôi, những dự án không vì lợi nhuận sau một thời gian đều lạc hậu do không có người quản lý kế thừa. Lý do là vì dữ liệu không được lưu trữ ở định dạng đơn giản, không dễ thao tác, khiến cho việc nhập liệu và chia sẻ dữ liệu trở nên khó khăn. 
giảm thiểu gánh nặng nhận thức trong việc nhập liệu và chia sẻ dữ liệu 

Để tránh điều này, hệ thống cần phải:
- Người dùng có thể tạo dữ liệu mới bằng ít lần bấm nhất có thể
- Hệ thống phân loại địa điểm phải có khả năng chuẩn bị cho sự thay đổi cách phân loại một cách dễ dàng
- Dữ liệu có sẵn trong kho thông tin của người dùng có thể được tải lên kho chung một cách thụ động và hàng loạt 
- Người dùng có thể tự triển khai hệ thống của riêng họ cho nhóm người dùng của riêng họ
- Chức năng mới có thể bổ sung dễ dàng 

#### Hệ thống phân loại địa điểm phải có khả năng chuẩn bị cho sự thay đổi cách phân loại một cách dễ dàng
Một người ở TPHCM sẽ có nhu cầu khác với một người ở Hà Nội: họ không quan tâm các địa điểm ở Hà Nội. Một người khuyết tật nhìn có nhu cầu khác với một người khuyết tật vận động: một người muốn đến nơi yên tĩnh, còn một người muốn đến nơi xe lăn đi lại dễ dàng được. Một người đi xe đạp có nhu cầu khác với một người đi xe buýt: người đi xe đạp muốn tìm quán gần nhà, còn người đi xe buýt muốn tìm quán gần các trạm xe.

Chưa kể, sự khác biệt đâu chỉ ở phía cầu, mà còn ở phía cung. Quán nước có những đặc điểm mà không gian làm việc chung, phòng họp riêng, địa điểm công cộng hay nhà riêng không có. Ngay cả trong quán nước cũng muôn hình vạn trạng: có quán cho dùng không gian miễn phí không cần gọi đồ uống, có quán thì cần gọi đồ uống. Có quán dùng ghế gây đau lưng, có quán dùng đèn gây đau mắt. Bất kể là tập trung vào đối tượng thụ hưởng nào thì những sự đa dạng này đã phải được tính đến.

Sẽ luôn luôn có những nhu cầu đặc biệt mà những người xây dựng nên hệ thống này cũng không tài nào đoán ra được. Sẽ có người hỏi rằng: tại sao không tập trung vào một nhu cầu cụ thể nào đó và giải quyết nó cho thật tốt? Nhưng nhu cầu cụ thể đó là nhu cầu nào? Chẳng lẽ lại là "nhu cầu tìm không gian thảo luận ở các quận nội thành TP.HCM cho 30 người có máy chiếu và micro, với người tham gia là nam dị tính hợp giới trung niên trung lưu không khuyết tật không quan tâm đến rác thải nhựa đi xe máy"? Nếu thế thì cứ kiếm những bài tổng hợp địa điểm là được rồi. Xác suất cao là dù tiêu đề bài chỉ chung chung là tổng hợp các nơi gặp mặt, thì cũng chỉ phục vụ nhu cầu của nhóm người cụ thể đó. Nếu vẫn muốn giải quyết nhu cầu "tìm nơi gặp mặt trực tiếp", thì cần đáp ứng được bất kì tổ hợp đặc điểm nào. 

Ngoài ra, việc đáp ứng thêm một nhu cầu nữa cũng đơn giản: chỉ cần thêm một *trường thông tin đầu vào* nữa thôi. 
Đòi hỏi chế độ dinh dưỡng đặc biệt mà những người xây dựng nên nơi này cũng không đoán ra được trước được
Không phải là nơi gặp nói chuyện mà thư viện chẳng hạn
Các bộ chỉ số như esg, sử dụng mã nguồn mở 

tất cả các bài tổng hợp địa điểm trên mạng đều loanh quanh một vài tổ hợp như vậy, dù chỉ mang tiêu đề chung chung. Còn nếu nhu cầu chỉ là kiếm quán nước thôi thì lên Google Maps luôn cho rồi, cần gì tạo thêm nữa. Một nơi đáng bỏ công sức để làm phải vừa chung chung như kiếm nơi gặp mặt, nhưng cũng phải 

Một ngày nào đó các tỉnh thành được sắp xếp lại. [Nhiệm vụ của kiến trúc sư không phải là liệt kê hết các tình huống sẽ xảy ra, mà là thiết kế để dù các tình huống không ngờ tới xảy ra thì vẫn hoạt động ổn định](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/K%E1%BB%B9%20thu%E1%BA%ADt%20ph%E1%BA%A7n%20m%E1%BB%81m/Ki%E1%BA%BFn%20tr%C3%BAc/Nhi%E1%BB%87m%20v%E1%BB%A5%20c%E1%BB%A7a%20ki%E1%BA%BFn%20tr%C3%BAc%20s%C6%B0%20kh%C3%B4ng%20ph%E1%BA%A3i%20l%C3%A0%20li%E1%BB%87t%20k%C3%AA%20h%E1%BA%BFt%20c%C3%A1c%20t%C3%ACnh%20hu%E1%BB%91ng%20s%E1%BA%BD%20x%E1%BA%A3y%20ra,%20m%C3%A0%20l%C3%A0%20thi%E1%BA%BFt%20k%E1%BA%BF%20%C4%91%E1%BB%83%20d%C3%B9%20c%C3%A1c%20t%C3%ACnh%20hu%E1%BB%91ng%20kh%C3%B4ng%20ng%E1%BB%9D%20t%E1%BB%9Bi%20x%E1%BA%A3y%20ra%20th%C3%AC%20v%E1%BA%ABn%20ho%E1%BA%A1t%20%C4%91%E1%BB%99ng%20%E1%BB%95n%20%C4%91%E1%BB%8Bnh.md). [Việc phân loại không quan trọng bằng việc chuẩn bị cho sự thay đổi cách phân loại](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Ngh%C4%A9%20v%E1%BB%81%20vi%E1%BB%87c%20ngh%C4%A9/B%E1%BA%A3n%20th%E1%BB%83%20lu%E1%BA%ADn/Ph%C3%A2n%20lo%E1%BA%A1i/Vi%E1%BB%87c%20ph%C3%A2n%20lo%E1%BA%A1i%20kh%C3%B4ng%20quan%20tr%E1%BB%8Dng%20b%E1%BA%B1ng%20vi%E1%BB%87c%20chu%E1%BA%A9n%20b%E1%BB%8B%20cho%20s%E1%BB%B1%20thay%20%C4%91%E1%BB%95i%20c%C3%A1ch%20ph%C3%A2n%20lo%E1%BA%A1i.md)

#### Người dùng có thể tạo dữ liệu mới bằng ít lần bấm nhất có thể
[Để một hệ sinh thái hoạt động thực sự hiệu quả thì lượng năng lượng dành ra để nắm bắt tín hiệu của môi trường phải giảm tới mức gần như bằng 0](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%E1%BB%99ng%20%C4%91%E1%BB%93ng,%20h%E1%BB%87%20sinh%20th%C3%A1i,%20h%E1%BB%87%20ph%E1%BB%A9c%20h%E1%BB%A3p/H%E1%BB%87%20sinh%20th%C3%A1i/%C4%90%E1%BB%83%20m%E1%BB%99t%20h%E1%BB%87%20sinh%20th%C3%A1i%20ho%E1%BA%A1t%20%C4%91%E1%BB%99ng%20th%E1%BB%B1c%20s%E1%BB%B1%20hi%E1%BB%87u%20qu%E1%BA%A3%20th%C3%AC%20l%C6%B0%E1%BB%A3ng%20n%C4%83ng%20l%C6%B0%E1%BB%A3ng%20d%C3%A0nh%20ra%20%C4%91%E1%BB%83%20n%E1%BA%AFm%20b%E1%BA%AFt%20t%C3%ADn%20hi%E1%BB%87u%20c%E1%BB%A7a%20m%C3%B4i%20tr%C6%B0%E1%BB%9Dng%20ph%E1%BA%A3i%20gi%E1%BA%A3m%20t%E1%BB%9Bi%20m%E1%BB%A9c%20g%E1%BA%A7n%20nh%C6%B0%20b%E1%BA%B1ng%200.md)

[Việc giúp đỡ người đã giúp mình không đủ khẩn cấp hoặc nhiều cảm hứng bằng việc giải quyết vấn đề tiếp theo, hoặc đủ cảm hứng bằng việc cải tiến giải pháp hiện có](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Kinh%20t%E1%BA%BF.%20T%C3%A2m%20l%C3%BD%20h%E1%BB%8Dc%20qu%E1%BA%A3n%20l%C3%BD%20v%C3%A0%20lao%20%C4%91%E1%BB%99ng/T%C3%A2m%20l%C3%BD%20h%E1%BB%8Dc%20qu%E1%BA%A3n%20l%C3%BD%20v%C3%A0%20lao%20%C4%91%E1%BB%99ng/Gi%C3%BAp%20%C4%91%E1%BB%A1%20nhau/Vi%E1%BB%87c%20gi%C3%BAp%20%C4%91%E1%BB%A1%20ng%C6%B0%E1%BB%9Di%20%C4%91%C3%A3%20gi%C3%BAp%20m%C3%ACnh%20kh%C3%B4ng%20%C4%91%E1%BB%A7%20kh%E1%BA%A9n%20c%E1%BA%A5p%20ho%E1%BA%B7c%20nhi%E1%BB%81u%20c%E1%BA%A3m%20h%E1%BB%A9ng%20b%E1%BA%B1ng%20vi%E1%BB%87c%20gi%E1%BA%A3i%20quy%E1%BA%BFt%20v%E1%BA%A5n%20%C4%91%E1%BB%81%20ti%E1%BA%BFp%20theo,%20ho%E1%BA%B7c%20%C4%91%E1%BB%A7%20c%E1%BA%A3m%20h%E1%BB%A9ng%20b%E1%BA%B1ng%20vi%E1%BB%87c%20c%E1%BA%A3i%20ti%E1%BA%BFn%20gi%E1%BA%A3i%20ph%C3%A1p%20hi%E1%BB%87n%20c%C3%B3.md)
Không chỉ là biết những đồ vậtowr trong đó, mà còn là môi trường và các thiết chế xung quanh

Động lực không phải là liệt kê tất cả các địa điểm đáp ứng một nhu cầu cụ thể, mà là không để việc thiếu thông tin xảy ra . Chứ 
Để giảm khả năng chết yểu
Tại sao lại cần điều này? Vì có như vậy nó mới tránh sự chết yểu. Kinh tế quy mô 
Không bỏ ai lại phía sau cũng có nghĩa là ai cũng biết được tới điều này. 
[Tỉ lệ quay lại là thứ quan trọng nhất trong tăng trưởng](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Qu%E1%BA%A3n%20l%C3%BD%20d%E1%BB%B1%20%C3%A1n,%20ph%C3%A1t%20tri%E1%BB%83n%20s%E1%BA%A3n%20ph%E1%BA%A9m,%20x%C3%A2y%20d%E1%BB%B1ng%20t%E1%BB%95%20ch%E1%BB%A9c/Ph%C3%A1t%20tri%E1%BB%83n%20s%E1%BA%A3n%20ph%E1%BA%A9m/Ch%E1%BB%89%20s%E1%BB%91/T%C4%83ng%20tr%C6%B0%E1%BB%9Fng/T%E1%BB%89%20l%E1%BB%87%20quay%20l%E1%BA%A1i%20l%C3%A0%20th%E1%BB%A9%20quan%20tr%E1%BB%8Dng%20nh%E1%BA%A5t%20trong%20t%C4%83ng%20tr%C6%B0%E1%BB%9Fng.md)


Nếu dữ liệu đã có sẵn trong kho thông tin của người dùng có thể được tải lên kho chung một cách thụ động và hàng loạt.

ở ngay trong hệ thống ghi chép
Tự động hoá việc đẩy dữ liệu. Phải tính đến việc họ không có đầu óc để làm điều đó
Nhu cầu của người có địa điểm:
- Nếu là kinh doanh hoặc muốn hỗ trợ cộng đồng thì có động lực đóng góp
- Nếu là nhà riêng thì chỉ muốn cho người quen xài

Người làm dự án

Người cần tìm địa điểm
[❓Liệu quy luật 90-9-1 vẫn còn đúng cho nhóm nòng cốt](%E2%9D%93Li%E1%BB%87u%20quy%20lu%E1%BA%ADt%2090-9-1%20v%E1%BA%ABn%20c%C3%B2n%20%C4%91%C3%BAng%20cho%20nh%C3%B3m%20n%C3%B2ng%20c%E1%BB%91t.md)

#### Người dùng có thể tự triển khai hệ thống của riêng họ cho nhóm người dùng của riêng họ
Nó phải scale về mặt ý tưởng, nhưng phải phân tán về mặt dữ liệu
Đó là lý do các SaaS như Notion không phù hợp để làm nơi lưu trữ dữ liệu.
Ngay cả
Phải ở dạng dữ liệu đơn giản nhất 
sao chép dễ dàng, không khác gì sao chép tài liệu
Quay về với thứ luôn sẵn có, ai cũng biết xài
dễ fork 
Ở ngay trong kho dữ liệu của họ
Khi cần trung tâm hóa thì mới 

Ở ngay trong hệ thống dữ liệu
[Việc đổi mới sáng tạo bắt đầu bằng việc mỗi người có thể tự mình điều khiển được máy tính, chứ không phải có thêm một sản phẩm no code hay AI nữa](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/Vi%E1%BB%87c%20%C4%91%E1%BB%95i%20m%E1%BB%9Bi%20s%C3%A1ng%20t%E1%BA%A1o%20b%E1%BA%AFt%20%C4%91%E1%BA%A7u%20b%E1%BA%B1ng%20vi%E1%BB%87c%20m%E1%BB%97i%20ng%C6%B0%E1%BB%9Di%20c%C3%B3%20th%E1%BB%83%20t%E1%BB%B1%20m%C3%ACnh%20%C4%91i%E1%BB%81u%20khi%E1%BB%83n%20%C4%91%C6%B0%E1%BB%A3c%20m%C3%A1y%20t%C3%ADnh,%20ch%E1%BB%A9%20kh%C3%B4ng%20ph%E1%BA%A3i%20c%C3%B3%20th%C3%AAm%20m%E1%BB%99t%20s%E1%BA%A3n%20ph%E1%BA%A9m%20no%20code%20hay%20AI%20n%E1%BB%AFa.md)
[Những người tự thấy mình ngu công nghệ đơn giản là vì họ không được trao quyền tự trị dữ liệu](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/T%E1%BB%B1%20tr%E1%BB%8B%20d%E1%BB%AF%20li%E1%BB%87u.%20M%C3%A3%20ngu%E1%BB%93n%20m%E1%BB%9F,%20ph%E1%BA%A7n%20m%E1%BB%81m%20t%E1%BB%B1%20do/T%E1%BB%B1%20tr%E1%BB%8B%20d%E1%BB%AF%20li%E1%BB%87u/Nh%E1%BB%AFng%20ng%C6%B0%E1%BB%9Di%20t%E1%BB%B1%20th%E1%BA%A5y%20m%C3%ACnh%20ngu%20c%C3%B4ng%20ngh%E1%BB%87%20%C4%91%C6%A1n%20gi%E1%BA%A3n%20l%C3%A0%20v%C3%AC%20h%E1%BB%8D%20kh%C3%B4ng%20%C4%91%C6%B0%E1%BB%A3c%20trao%20quy%E1%BB%81n%20t%E1%BB%B1%20tr%E1%BB%8B%20d%E1%BB%AF%20li%E1%BB%87u.md)

Trung tâm hoá. Giảm gánh nặng cho người kế thừa
Trung tâm hoá dữ liệu. Nếu chỉ cho mình thôi thì đơn giản
Google Sheet, Google Maps vì nó không nằm trong các

#### Chức năng mới có thể bổ sung dễ dàng 
- Tự động cập nhật thông tin mới lên các nền tảng khác nhau
- Có thể truy vấn dữ liệu ở các nền tảng khác (VD: Discord) 
- Tự động tạo lịch Google Calendar
- Có cách trình bày khác

[Đừng chạy theo tính năng, mà hãy xác định vấn đề cần ưu tiên giải quyết và nhanh chóng kiểm tra các giả thuyết](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Qu%E1%BA%A3n%20l%C3%BD%20d%E1%BB%B1%20%C3%A1n,%20ph%C3%A1t%20tri%E1%BB%83n%20s%E1%BA%A3n%20ph%E1%BA%A9m,%20x%C3%A2y%20d%E1%BB%B1ng%20t%E1%BB%95%20ch%E1%BB%A9c/Ph%C3%A1t%20tri%E1%BB%83n%20s%E1%BA%A3n%20ph%E1%BA%A9m/Ki%E1%BB%83m%20%C4%91%E1%BB%8Bnh%20gi%E1%BA%A3%20thuy%E1%BA%BFt/%C4%90%E1%BB%ABng%20ch%E1%BA%A1y%20theo%20t%C3%ADnh%20n%C4%83ng,%20m%C3%A0%20h%C3%A3y%20x%C3%A1c%20%C4%91%E1%BB%8Bnh%20v%E1%BA%A5n%20%C4%91%E1%BB%81%20c%E1%BA%A7n%20%C6%B0u%20ti%C3%AAn%20gi%E1%BA%A3i%20quy%E1%BA%BFt%20v%C3%A0%20nhanh%20ch%C3%B3ng%20ki%E1%BB%83m%20tra%20c%C3%A1c%20gi%E1%BA%A3%20thuy%E1%BA%BFt.md)
Phải đợi đến khi nhiều người chia sẻ thì mới bắt tay vào làm

## Hệ quả của các yêu cầu trên
Giải pháp đáp ứng được tất cả các nhu cầu này là một [hệ thống tri thức cộng đồng](../../../Nhu%20c%E1%BA%A7u%20c%C3%B4ng%20vi%E1%BB%87c/Vi%E1%BA%BFt%20v%C3%A0%20chia%20s%E1%BA%BB%20tri%20th%E1%BB%A9c/Chia%20s%E1%BA%BB%20kho%20tri%20th%E1%BB%A9c%20c%E1%BB%A7a%20m%C3%ACnh%20cho%20m%E1%BB%8Di%20ng%C6%B0%E1%BB%9Di.md) dưới hình thức là một [Tài liệu động](../../../Nhu%20c%E1%BA%A7u%20c%C3%B4ng%20ngh%E1%BB%87/Vi%E1%BA%BFt%20v%C3%A0%20qu%E1%BA%A3n%20l%C3%BD%20n%E1%BB%99i%20dung,%20ghi%20ch%C3%BA,%20t%C3%A0i%20li%E1%BB%87u/T%C3%A0i%20li%E1%BB%87u%20%C4%91%E1%BB%99ng.md) được lưu ở định dạng đơn giản nhất là văn bản thuần. 

| Yêu cầu                                                                                                        | Hệ quả                         |
| -------------------------------------------------------------------------------------------------------------- | ------------------------------ |
| Người dùng có thể tạo dữ liệu mới bằng ít lần bấm nhất có thể                                                  | Có bản web                     |
| Hệ thống phân loại địa điểm phải có khả năng chuẩn bị cho sự thay đổi cách phân loại một cách dễ dàng          | Dùng tệp trơn                  |
| Dữ liệu có sẵn trong kho thông tin của người dùng có thể được tải lên kho chung một cách thụ động và hàng loạt | Cung cấp API                   |
| Người dùng có thể tự triển khai hệ thống của riêng họ cho nhóm người dùng của riêng họ                         | Local first, Deno, Murmuration |
| Chức năng mới có thể bổ sung dễ dàng                                                                           | Cung cấp API, Deno             |

Về mặt kỹ thuật, nó được viết bằng TypeScript với môi trường thực thi là Deno.

- Đa số mọi người sẽ dùng Base? 
Gold view nâng cao là cần thiết không? Và nếu để vô thì ntn?
