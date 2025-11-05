---
share: true
created: 2023-07-13T19:21
updated: 2025-11-05T19:59
---
Bạn không muốn lệ thuộc.

Bạn muốn biết lập trình chứ không phải là không, nhưng:
- Còn nhiều nhu cầu khác bạn phải xử lý, nên dù bạn cứ suy nghĩ rằng một ngày nào đó mình phải dành thời gian cho nó, nhưng mãi mà bạn vẫn không thể biến nó trở thành ưu tiên cao nhất
- Tài liệu hướng dẫn mang danh là dành cho người mới, nhưng nó vẫn quá nhiều thứ với bạn

Vàààààààà đến một ngày bạn có một bài toán thực sự cần phải code, và AI không thể giúp bạn được, và bạn không thể nhờ ai khác code cho được. Thực sự là bạn phải xắn tay vào làm rồi.

Nhưng thực sự là bạn không thể thong thả để làm được. Bạn biết là việc học thì sẽ mất thời gian, và nếu nó cần phải mất nhiều thời gian thì bạn cũng phải chịu thôi nhưng bạn vẫn cảm thấy mình cần phải . Cái trạng thái đó không phải là cái trạng thái phù hợp cho việc học, nhưng the brain is funny.

Việc nhảy ngang như vậy làm cho không một tài liệu hướng dẫn nào theo kịp bạn. Vì muốn hướng dẫn bạn thì phải áng chừng được trình độ bạn đang ở đâu. Và một code product thì người ta không kỳ vọng rằng phải giải thích tất cả những thứ căn bản
[Mỗi một thắc mắc đều làm tăng thêm khối lượng nhận thức mà chúng ta có trong tâm trí, qua đó làm phân tán sự tập trung của ta khỏi thứ mà ta định làm](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Ngh%C4%A9%20v%E1%BB%81%20vi%E1%BB%87c%20ngh%C4%A9/G%C3%A1nh%20n%E1%BA%B7ng%20nh%E1%BA%ADn%20th%E1%BB%A9c.%20Thi%E1%BA%BFt%20k%E1%BA%BF/M%E1%BB%97i%20m%E1%BB%99t%20th%E1%BA%AFc%20m%E1%BA%AFc%20%C4%91%E1%BB%81u%20l%C3%A0m%20t%C4%83ng%20th%C3%AAm%20kh%E1%BB%91i%20l%C6%B0%E1%BB%A3ng%20nh%E1%BA%ADn%20th%E1%BB%A9c%20m%C3%A0%20ch%C3%BAng%20ta%20c%C3%B3%20trong%20t%C3%A2m%20tr%C3%AD,%20qua%20%C4%91%C3%B3%20l%C3%A0m%20ph%C3%A2n%20t%C3%A1n%20s%E1%BB%B1%20t%E1%BA%ADp%20trung%20c%E1%BB%A7a%20ta%20kh%E1%BB%8Fi%20th%E1%BB%A9%20m%C3%A0%20ta%20%C4%91%E1%BB%8Bnh%20l%C3%A0m.md)

Lao ngay vào code trong product thì hổng kiến thức do nhiều chỗ viết tắt cho dễ đọc, dễ quản lý. Học từ từ thì thấy lãng phí thời gian.
Để đọc được tới dòng này là cả một sự nỗ lực ở lại của bạn. Dù bạn có từng đọc bao nhiêu trang khác rồi thì 
Chỉ ghi lại những thứ mất nhiều thời gian để nhận ra. Cái nào dễ thấy thì ko ghi 
- muốn nhưng google được là có thì không ghi. Khi nào bị bug rồi mới phát hiện ra một cái gì đó mà không thấy ai nói gì thì mới ghi
- Nếu cản trở sự đọc hiểu mà phải google thì cũng ghi ra 



[❓ Học code bằng việc debug product code sẽ nhanh hơn](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/K%E1%BB%B9%20thu%E1%BA%ADt%20ph%E1%BA%A7n%20m%E1%BB%81m/%E2%9D%93%20H%E1%BB%8Dc%20code%20b%E1%BA%B1ng%20vi%E1%BB%87c%20debug%20product%20code%20s%E1%BA%BD%20nhanh%20h%C6%A1n.md)
Nó là cách học qua bắt chước
Git blame
Hướng dẫn đọc hiểu code cho người rất lờ mờ về code
Biết được cách debug là sẽ dần dần biết cách bắt chước
Làm trên code sản phẩm là sát sườn nhất
cố gắng tái tạo lại ý đồ của người viết lúc tạo ra đoạn code đó
nói gì, bạn muốn biết phải bắt đầu google từ đâu, nhưng 

Một số thứ sẽ giúp bạn hiểu code nói gì:
- Biết thao tác với IDE,
- Hiểu được một số khái niệm và từ khoá cơ bản: object, method, array, for, if, import, function, type
- Hiểu một số quy ước viết code
- Hiểu được IDE đang cố gắng nói cho mình cái gì
- Biết một số kỹ thuật debug: console.log, debugger, unit test
## Thao tác với IDE
[Phím tắt cho VS Code](Ph%C3%ADm%20t%E1%BA%AFt%20cho%20VS%20Code.md)

## Hiểu quy tắc viết tài liệu
```js
/**
 * Tên hàm
 * @constructor
 * @param {string} title - The title of the book.
 * @param {string} author - The author of the book.
 */
function hàm(biến1, biến2) {
}
```

[Các buổi đáp ứng nhu cầu học cách sử dụng công cụ và tư duy lập trình cho nhu cầu công việc](../C%C3%A1c%20bu%E1%BB%95i%20%C4%91%C3%A1p%20%E1%BB%A9ng%20nhu%20c%E1%BA%A7u%20h%E1%BB%8Dc%20c%C3%A1ch%20s%E1%BB%AD%20d%E1%BB%A5ng%20c%C3%B4ng%20c%E1%BB%A5%20v%C3%A0%20t%C6%B0%20duy%20l%E1%BA%ADp%20tr%C3%ACnh%20cho%20nhu%20c%E1%BA%A7u%20c%C3%B4ng%20vi%E1%BB%87c.md)


