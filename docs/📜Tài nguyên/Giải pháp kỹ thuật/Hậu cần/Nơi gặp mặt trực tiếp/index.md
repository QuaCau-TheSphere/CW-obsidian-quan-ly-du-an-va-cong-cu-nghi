---
share: true
created: 2024-08-23T15:06
updated: 2025-05-06T12:55
alias:
  - Kho địa điểm để chọn nơi gặp mặt
  - Hướng dẫn sử dụng kho địa điểm để chọn nơi gặp mặt
description: Làm sao để tìm được nơi phù hợp để gặp mặt trực tiếp?
title: Nơi gặp mặt trực tiếp
---
![](https://i.imgur.com/CXHXI7y.png)
# Kho địa điểm để chọn nơi gặp mặt 
Đây là một danh sách tổng hợp các địa điểm gặp mặt trực tiếp, bao gồm:
- Địa điểm công cộng
- Không gian làm việc chung
- Phòng họp riêng
- Quán có phòng riêng
- Quán không có phòng riêng
- Nhà riêng

Chọn [TP.HCM](./TP.HCM/index.md) hoặc [Hà Nội](./H%C3%A0%20N%E1%BB%99i/index.md) để bắt đầu. 

## Tiêu chí thêm địa điểm
- Có chính sách hỗ trợ các dự án phi lợi nhuận, hoặc có lợi ích cho người làm phi lợi nhuận hoặc đối tượng hưởng lợi của họ (VD: gần nhà nhau, có người quen, tiếp cận được cho người khuyết tật, v.v.)
- Được đề xuất trong nơi thảo luận, hoặc được yêu cầu kéo dữ liệu mới (pull request) trên GitHub
- Có điểm cộng khác lạ

Bạn có thể fork repo này để làm bộ tài nguyên cho riêng bạn.

## Ý đồ thiết kế
### Định nghĩa điểm cộng, điểm trừ
- Những thuộc tính được xem là **điểm cộng** khi ta không mặc định là nó luôn có ở đó. Có thì tốt, không có thì thường là không sao. Nên với những thuộc tính này, nếu địa điểm đó có thì sẽ liệt kê ra, còn nếu không thì sẽ không nói gì
- Những thuộc tính được xem là **điểm trừ** khi ta mặc định là nó luôn có ở đó. Nếu không có thì thường là có sao. Nên với những thuộc tính này, nếu địa điểm đó không có thì sẽ có cảnh báo, còn nếu có thì sẽ không nói gì

#### Những thuộc tính là điểm trừ cho mọi loại địa điểm
Đây là những thuộc tính mặc định là luôn có cho mọi loại địa điểm:
- [x] Nhà vệ sinh
- [x] Xe lăn tiếp cận được
- [x] Không có loa làm ồn
- [x] Không cần đặt chỗ trước
- [x] Không có đèn nhấp nháy hoặc quảng cáo động
- [x] Giá đã bao gồm thuế

#### Những thuộc tính là điểm cộng cho mọi loại địa điểm
Đây là những thuộc tính mặc định là luôn không có cho mọi loại địa điểm:
- [x] Nằm la liệt được
- [x] Không gian ngoài trời
- [x] Có đàn hoặc sân khấu nhỏ
- [x] Nuôi chó mèo
- [x] Webcam

#### Những thuộc tính mà việc là điểm cộng hoặc điểm trừ tuỳ vào loại địa điểm
Với **không gian ngoài trời** thì những thuộc tính này mặc định là không có, nếu có thì là điểm cộng. Với các loại hình khác thì mặc định là luôn có, nếu không có thì là điểm trừ:
- [x] Wifi 
- [x] Ổ điện
- [x] Bàn đúng kích thước làm việc
- [x] Không có khói thuốc lá

Với **phòng họp riêng** hoặc **quán có phòng riêng** thì những thuộc tính này mặc định là luôn có, nếu không có thì là điểm trừ. Với những loại hình khác thì mặc định là không có, nếu có thì là điểm cộng:
- [x] Nói to được
- [x] Vận động cơ thể được
- [x] Máy chiếu
- [x] Loa 
- [x] Mic (không phải là điểm trừ với phòng 20 người trở xuống)
- [x] Bảng và bút lông
- [x] Không bị ồn từ bên ngoài

### Cách thông tin được ghi chú
Với các **quán nước**, giá nước sẽ là giá món đắt nhất trong 3 món rẻ nhất. Lý do là vì một người muốn tiết kiệm vẫn có thể sẵn sàng mua một thứ đắt hơn thứ rẻ nhất một chút. Trong các bảng so sánh thì giá sẽ bằng tổng của giá nước và giá giữ xe.

Các **quán có phòng riêng**  thu tiền bằng việc bán nước cho khách, nên cơ bản là họ cũng không có giá phòng, mà chỉ có giá nước. Điều này khiến cho quán ràng buộc số lượng người đi tối thiểu để được mượn phòng. Cộng với việc người tổ chức quan tâm xem có phòng nào đủ cho sự kiện hay không, trường `Số lượng` sẽ được ghi dưới dạng sau:
```
Số lượng:: sốLượngTốiThiểuCủaPhòngNhỏNhất - sốLượngTốiĐaCủaPhòngLớnNhất
```

- Ví dụ, một quán có 3 phòng riêng. Để được thuê phòng nhỏ nhất thì cần tối thiểu 5 người đi (đi ít hơn nhưng mua 5 ly thì cũng thuê được). Phòng lớn nhất chỉ chứa được tối đa 30 người. Vậy trường này sẽ ghi là `Số lượng:: 5 - 30`
- Nếu chỉ có một số (VD: `Số lượng:: 30`) thì mặc định sẽ là số lượng tối đa của phòng lớn nhất. Thường đó là trường hợp bao nguyên quán, nên không cần ghi số lượng nhỏ nhất

Các **dịch vụ cho thuê phòng họp**, khác với các quán nước, thu tiền từ người tổ chức. Bạn thuê phòng lớn nhất nhưng chỉ đến một người họ cũng không quan tâm. Nên chỉ cần tạo một bảng giá theo số lượng tối đa của phòng là đủ.

Khi một địa điểm có điểm cộng thì ghi đơn giản là *Điểm cộng*, nhưng khi nó có điểm trừ thì lại không ghi là *Điểm trừ*, mà ghi là *Lưu ý*. Bởi vì từ "điểm trừ" tạo cảm giác không thay đổi được, chắc chắn sẽ tạo ra vấn đề, còn từ "lưu ý" thì tạo cảm giác tuỳ nhu cầu của mỗi người, có người quan tâm nhiều có người quan tâm ít. Nó cũng tạo cảm giác có thể có cách xử lý (dù tất nhiên không phải xử lý gì thì cũng vui hơn).

## Xem thêm
- [Lý do ra đời kho địa điểm để chọn nơi gặp mặt](./L%C3%BD%20do%20ra%20%C4%91%E1%BB%9Di.md)   
- [Hướng dẫn đóng góp kho địa điểm để chọn nơi gặp mặt](./H%C6%B0%E1%BB%9Bng%20d%E1%BA%ABn%20%C4%91%C3%B3ng%20g%C3%B3p.md)

## Nơi thảo luận
<button onclick="location.href='https://doi-thoai.deno.dev/Discord.4s.1'" type="button">Mở Discord</button>
[![](https://i.imgur.com/ds6m65A.png)](https://doi-thoai.deno.dev/Discord.4s.1)