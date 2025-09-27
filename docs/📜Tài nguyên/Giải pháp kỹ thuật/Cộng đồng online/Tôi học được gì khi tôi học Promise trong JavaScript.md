---
share: true
created: 2024-11-24T21:23
updated: 2025-06-25T12:19
---
Tôi đang trong cơn muốn tìm hiểu về đường cú pháp, và tôi google [`syntactic sugar`](https://www.google.com/search?client=firefox-b-d&q=syntactic+sugar). Tôi bấm các liên kết tôi thấy hấp dẫn, và trong đó có bài [On syntactic sugar](https://evertpot.com/syntactic-sugar/). Dường như trong những kết quả được lên trang nhất Google, thì tôi thấy muốn đọc các blog cá nhân hơn, vì cảm giác mình sẽ dễ thu lượm được những thứ mà những nền tảng blog khác như dev.to, freeCodeCamp, Quora, v.v. ít khi cung cấp. Tôi nghĩ nhiều bài trên đó cũng đáng xem, nhưng để biết được những thứ thực sự rất rốt ráo thì . Bài viết dẫn tới hai bài này:
- [Why Async/Await Is More Than Just Syntactic Sugar](https://www.zhenghao.io/posts/await-vs-promise)
- [JS classes are not “just syntactic sugar”](https://webreflection.medium.com/js-classes-are-not-just-syntactic-sugar-28690fedf078)

Tôi thấy hứng thú đọc cả hai. Bài đầu tiên đọc cũng không thấy hiểu lắm, nhưng cũng không khó hiểu khi nó có nói là nó giả định người đọc đã có kiến thức nền tảng về `Promise`. Tác giả bảo rằng anh không có ý định cạnh tranh với các bài hướng dẫn trên [MDN](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous) và [javascript.info](https://javascript.info/promise-basics).

Tôi đã biết về hàm bất đồng bộ. Tôi đã thành thạo việc sử dụng await. Tôi đã hiểu về callback, và đã hiểu await là cách để sử dụng hàm bất đồng bộ với tư duy khi viết hàm đồng bộ. Dù chưa hiểu về promise hay callback hell thì tôi cũng đã hiểu là promise giúp giải quyết callback hell. Tôi biết rằng nếu gặp phải hàm bất đồng bộ thì cứ thêm await phía trước là nó chạy được. 

Nên là dù tôi cũng muốn hiểu thêm về `Promise`, tôi chưa thấy mình cần phải hiểu nó ngay bây giờ lắm. Tôi còn nhiều bài khác cần đọc, còn nhiều việc khác phải làm, và nhiều người khác đang rất cần những sản phẩm tôi tạo ra. 

Nhưng sự tò mò của tôi đã chiến thắng. Cũng đâu phải Dù sao cái `promise` này cứ thỉnh thoảng lại gặp phải. Biết một lần cho xong, những lần sau sẽ nhanh chóng lĩnh hội hơn. 
[Hiểu biết sâu làm ta thấy khoái cảm](../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Ngh%C4%A9%20v%E1%BB%81%20vi%E1%BB%87c%20ngh%C4%A9/Khoa%20h%E1%BB%8Dc%20nh%E1%BA%ADn%20th%E1%BB%A9c/Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u%20l%C3%A0m%20ta%20th%E1%BA%A5y%20kho%C3%A1i%20c%E1%BA%A3m.md), [Hiểu biết không chỉ để mình làm một cái gì đó, mà còn để mình không làm một cái gì đó](../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Ngh%C4%A9%20v%E1%BB%81%20vi%E1%BB%87c%20ngh%C4%A9/H%E1%BB%8Dc%20t%E1%BA%ADp,%20hi%E1%BB%83u%20bi%E1%BA%BFt/Hi%E1%BB%83u%20bi%E1%BA%BFt%20kh%C3%B4ng%20ch%E1%BB%89%20%C4%91%E1%BB%83%20m%C3%ACnh%20l%C3%A0m%20m%E1%BB%99t%20c%C3%A1i%20g%C3%AC%20%C4%91%C3%B3,%20m%C3%A0%20c%C3%B2n%20%C4%91%E1%BB%83%20m%C3%ACnh%20kh%C3%B4ng%20l%C3%A0m%20m%E1%BB%99t%20c%C3%A1i%20g%C3%AC%20%C4%91%C3%B3.md).Việc được tiếp cận tới những nguồn mới, mà xem lướt qua có vẻ có tiềm năng, đã dẫn đến kết cục là tôi là mở chục tab trên trình duyệt cùng lúc. 
[Con người chuyển từ kỹ năng này sang kỹ năng khác ngay cả khi họ chỉ có một khái niệm mơ hồ về đích đến cuối cùng](../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Kinh%20t%E1%BA%BF.%20T%C3%A2m%20l%C3%BD%20h%E1%BB%8Dc%20qu%E1%BA%A3n%20l%C3%BD%20v%C3%A0%20lao%20%C4%91%E1%BB%99ng/T%C3%A2m%20l%C3%BD%20h%E1%BB%8Dc%20qu%E1%BA%A3n%20l%C3%BD%20v%C3%A0%20lao%20%C4%91%E1%BB%99ng/K%E1%BB%B9%20n%C4%83ng,%20%C4%91%E1%BB%99ng%20l%E1%BB%B1c/Con%20ng%C6%B0%E1%BB%9Di%20chuy%E1%BB%83n%20t%E1%BB%AB%20k%E1%BB%B9%20n%C4%83ng%20n%C3%A0y%20sang%20k%E1%BB%B9%20n%C4%83ng%20kh%C3%A1c%20ngay%20c%E1%BA%A3%20khi%20h%E1%BB%8D%20ch%E1%BB%89%20c%C3%B3%20m%E1%BB%99t%20kh%C3%A1i%20ni%E1%BB%87m%20m%C6%A1%20h%E1%BB%93%20v%E1%BB%81%20%C4%91%C3%ADch%20%C4%91%E1%BA%BFn%20cu%E1%BB%91i%20c%C3%B9ng.md)

[Trải nghiệm truy cập web giống như trải nghiệm được dịch chuyển tức thời đến một nơi xa lạ](../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Ngh%C4%A9%20v%E1%BB%81%20vi%E1%BB%87c%20ngh%C4%A9/G%C3%A1nh%20n%E1%BA%B7ng%20nh%E1%BA%ADn%20th%E1%BB%A9c,%20thi%E1%BA%BFt%20k%E1%BA%BF/Thi%E1%BA%BFt%20k%E1%BA%BF/Tr%E1%BA%A3i%20nghi%E1%BB%87m%20truy%20c%E1%BA%ADp%20web%20gi%E1%BB%91ng%20nh%C6%B0%20tr%E1%BA%A3i%20nghi%E1%BB%87m%20%C4%91%C6%B0%E1%BB%A3c%20d%E1%BB%8Bch%20chuy%E1%BB%83n%20t%E1%BB%A9c%20th%E1%BB%9Di%20%C4%91%E1%BA%BFn%20m%E1%BB%99t%20n%C6%A1i%20xa%20l%E1%BA%A1.md). Việc đầu tiên bạn làm là định thần mình đang ở đâu. Nhưng khác với việc đến những vùng đất mới, bạn có thể dùng cả có thể để định hướng, thì ở trên web, bạn chỉ có thể định hướng bằng mắt 

Việc phải đọc code mẫu cần ít phải hiểu các hàm khác càng nhiều càng tốt.
Không đủ kiên nhẫn để đọc từ đầu
Khi đã thấy đủ để xong việc rồi thì không đủ kiên nhẫn để đọc tiếp
[Việc mò mẫm vui, đỡ phải nghĩ và thường là hiệu quả hơn là đọc hướng dẫn cẩn thận](../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Ngh%C4%A9%20v%E1%BB%81%20vi%E1%BB%87c%20ngh%C4%A9/G%C3%A1nh%20n%E1%BA%B7ng%20nh%E1%BA%ADn%20th%E1%BB%A9c,%20thi%E1%BA%BFt%20k%E1%BA%BF/Vi%E1%BB%87c%20m%C3%B2%20m%E1%BA%ABm%20vui,%20%C4%91%E1%BB%A1%20ph%E1%BA%A3i%20ngh%C4%A9%20v%C3%A0%20th%C6%B0%E1%BB%9Dng%20l%C3%A0%20hi%E1%BB%87u%20qu%E1%BA%A3%20h%C6%A1n%20l%C3%A0%20%C4%91%E1%BB%8Dc%20h%C6%B0%E1%BB%9Bng%20d%E1%BA%ABn%20c%E1%BA%A9n%20th%E1%BA%ADn.md). Nhưng vì việc [Đọc lướt không giúp ta tiếp thu được gì cả](../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Ngh%C4%A9%20v%E1%BB%81%20vi%E1%BB%87c%20ngh%C4%A9/M%C3%B4i%20tr%C6%B0%E1%BB%9Dng%20ngh%C4%A9,%20nh%E1%BA%ADn%20th%E1%BB%A9c%20t%C4%83ng%20c%C6%B0%E1%BB%9Dng/%C4%90%E1%BB%8Dc%20v%C3%A0%20vi%E1%BA%BFt/Ghi%20ch%C3%BA%20th%C3%B4ng%20tin/%C4%90%E1%BB%8Dc%20l%C6%B0%E1%BB%9Bt%20kh%C3%B4ng%20gi%C3%BAp%20ta%20ti%E1%BA%BFp%20thu%20%C4%91%C6%B0%E1%BB%A3c%20g%C3%AC%20c%E1%BA%A3.md), nên ta sẽ thấy nhức đầu khi bật trang mới dù ta không cảm thấy áp lực gì cả. Dễ thấy nhất khi cần ngồi nghiên cứu và ta bật rất nhiều tab. [Vấn đề của việc đọc lướt không phải vì nó có khả năng thành công cao, mà là vì khi mình đã kết luận là khả năng thành công không cao rồi, thì sự chuyển trạng thái sang thực sự đọc cẩn thận không suôn sẻ và tự nhiên](../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Ngh%C4%A9%20v%E1%BB%81%20vi%E1%BB%87c%20ngh%C4%A9/G%C3%A1nh%20n%E1%BA%B7ng%20nh%E1%BA%ADn%20th%E1%BB%A9c,%20thi%E1%BA%BFt%20k%E1%BA%BF/Ta%20d%C6%B0%E1%BB%9Dng%20nh%C6%B0%20kh%C3%B3%20c%C3%B3%20th%E1%BB%83%20chuy%E1%BB%83n%20tr%E1%BA%A1ng%20th%C3%A1i%20t%E1%BB%AB%20vi%E1%BB%87c%20%C4%91%E1%BB%8Dc%20l%C6%B0%E1%BB%9Bt%20sang%20vi%E1%BB%87c%20%C4%91%E1%BB%8Dc%20c%E1%BA%A9n%20th%E1%BA%ADn%20m%E1%BB%99t%20c%C3%A1ch%20su%C3%B4n%20s%E1%BA%BB%20v%C3%A0%20t%E1%BB%B1%20nhi%C3%AAn.md)  

[Dùng thuật ngữ chính xác hơn dùng từ bình dân, nhưng ngay cả chuyên gia cũng không phàn nàn về việc dùng từ bình dân, miễn là việc đó không tạo ra sự mơ hồ](../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Ngh%C4%A9%20v%E1%BB%81%20vi%E1%BB%87c%20ngh%C4%A9/M%C3%B4i%20tr%C6%B0%E1%BB%9Dng%20ngh%C4%A9,%20nh%E1%BA%ADn%20th%E1%BB%A9c%20t%C4%83ng%20c%C6%B0%E1%BB%9Dng/%C4%90%E1%BB%8Dc%20v%C3%A0%20vi%E1%BA%BFt/D%C3%B9ng%20thu%E1%BA%ADt%20ng%E1%BB%AF%20ch%C3%ADnh%20x%C3%A1c%20h%C6%A1n%20d%C3%B9ng%20t%E1%BB%AB%20b%C3%ACnh%20d%C3%A2n,%20nh%C6%B0ng%20ngay%20c%E1%BA%A3%20chuy%C3%AAn%20gia%20c%C5%A9ng%20kh%C3%B4ng%20ph%C3%A0n%20n%C3%A0n%20v%E1%BB%81%20vi%E1%BB%87c%20d%C3%B9ng%20t%E1%BB%AB%20b%C3%ACnh%20d%C3%A2n,%20mi%E1%BB%85n%20l%C3%A0%20vi%E1%BB%87c%20%C4%91%C3%B3%20kh%C3%B4ng%20t%E1%BA%A1o%20ra%20s%E1%BB%B1%20m%C6%A1%20h%E1%BB%93.md)
[Sự dễ hiểu làm tăng sự đáng tin, dù có thể nó không hợp lý](../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Ngh%C4%A9%20v%E1%BB%81%20vi%E1%BB%87c%20ngh%C4%A9/Khoa%20h%E1%BB%8Dc%20nh%E1%BA%ADn%20th%E1%BB%A9c/Suy%20lu%E1%BA%ADn/S%E1%BB%B1%20d%E1%BB%85%20hi%E1%BB%83u%20l%C3%A0m%20t%C4%83ng%20s%E1%BB%B1%20%C4%91%C3%A1ng%20tin,%20d%C3%B9%20c%C3%B3%20th%E1%BB%83%20n%C3%B3%20kh%C3%B4ng%20h%E1%BB%A3p%20l%C3%BD.md)

[Ta hiểu một đoạn 100 chữ nếu có không quá 3 từ không biết](../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Ngh%C4%A9%20v%E1%BB%81%20vi%E1%BB%87c%20ngh%C4%A9/M%C3%B4i%20tr%C6%B0%E1%BB%9Dng%20ngh%C4%A9,%20nh%E1%BA%ADn%20th%E1%BB%A9c%20t%C4%83ng%20c%C6%B0%E1%BB%9Dng/%C4%90%E1%BB%8Dc%20v%C3%A0%20vi%E1%BA%BFt/Ta%20hi%E1%BB%83u%20m%E1%BB%99t%20%C4%91o%E1%BA%A1n%20100%20ch%E1%BB%AF%20n%E1%BA%BFu%20c%C3%B3%20kh%C3%B4ng%20qu%C3%A1%203%20t%E1%BB%AB%20kh%C3%B4ng%20bi%E1%BA%BFt.md)
Ban đầu, bài viết này được đặt tiêu đề "Chuyện tôi tự học Promise trong JavaScript". Nhưng việc miêu tả hành trình tự học giữa các tab này tôi thấy vụn vặt quá. Tôi không thấy việc đọc chúng sẽ cho bạn thứ gì hữu ích. Nó sẽ có hữu ích với người làm nghiên cứu về trải nghiệm người dùng chẳng hạn. Theo trình tự thời gian khó mà tạo ra những tình tiết hấp dẫn.
Nó không nói được gì về những gì tôi đã biết trước đó hoặc sau đó 

### [Promise](https://javascript.info/promise-basics)
bắt đầu bằng hình ảnh những người hâm mộ đón chờ một bài hát, nhưng ca sĩ thì mệt mỏi bởi những mong đợi này.

### [Asynchronous Programming :: Eloquent JavaScript](https://eloquentjavascript.net/11_async.html)
Mở đầu bằng việc trích 2 câu của Lão Tử ở chương 15:
> Ai có thể đợi trong im lặng để chờ bùn lắng?
> Ai có thể giữ tĩnh cho đến lúc hành động

Đoạn tiếp theo cũng chỉ nói lại về callback, promise. Tôi đọc thì thấy cũng không quá dễ hiểu cho người mới. không nghĩ nó dễ hiểu 
Một câu chuyện về một con quạ tên là Carla. 
### [Introducing asynchronous JavaScript - Learn web development | MDN](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous/Introducing)
Ví dụ chỉ đơn giản là một đoạn code chạy lâu, nhưng làm bạn hiểu thêm được về những vấn đề kỹ thuật khác. Ngay sau khi bước qua đoạn đó là ví dụ ngay đến event handler
Kết nối ngay tới những khái niệm quan trọng khác đã được nói trước đó
Không có nhiều tình tiết
Các khái niệm tự nó đã tạo ra tình tiết rồi


Cuối cùng, tôi chọn quay về lại trang javascript.info. Tôi thấy họ đã làm được điều đó tốt nhất. 
Viết được xong cho bài "Đối số của Promise là một hàm. Nó được gọi là hàm thực thi (executor)" thì tôi nghĩ đã đủ rồi, không cần hiểu thêm nữa. Khi nào cần dùng tới then chain thì lại quay lại đọc tiếp
### MDN Learn
[JavaScript — Dynamic client-side scripting - Learn web development | MDN](https://developer.mozilla.org/en-US/docs/Learn/JavaScript "JavaScript — Dynamic client-side scripting - Learn web development | MDN")
Tập trung vào việc làm web, nên những bài đầu tiên là html, css. JS được dùng cũng chỉ tập trung vào xử lý. Những nguồn khác tập trung vào việc xem JS là một ngôn ngữ hơn
Yêu cầu phải có khái niệm về HTML và CSS rồi
### [Khan Academy](https://www.khanacademy.org/computing/computer-programming)
có interactive editor như kiểu của Bret Victor

[Foundations of asynchronous programming in JavaScript](https://exploringjs.com/js/book/ch_async-js.html#ch_async-js)
[CodeAnalogies Blog – Visual explanations of HTML, CSS and JavaScript concepts](https://blog.codeanalogies.com/)
## Bình luận
Tất nhiên là khi đọc cái này rồi đọc cái kia thì mình cũng đã tiếp thu được phần nào rồi. Không có cái đầu trống trơn không biết gì. Nhưng nó cũng không quá đầy, vì đọc gần nhau, nên tận dụng việc chưa kịp thấm bài 1 để đánh giá sự dễ hiểu của bài 2
[Việc mò mẫm vui, đỡ phải nghĩ và thường là hiệu quả hơn là đọc hướng dẫn cẩn thận](../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Ngh%C4%A9%20v%E1%BB%81%20vi%E1%BB%87c%20ngh%C4%A9/G%C3%A1nh%20n%E1%BA%B7ng%20nh%E1%BA%ADn%20th%E1%BB%A9c,%20thi%E1%BA%BFt%20k%E1%BA%BF/Vi%E1%BB%87c%20m%C3%B2%20m%E1%BA%ABm%20vui,%20%C4%91%E1%BB%A1%20ph%E1%BA%A3i%20ngh%C4%A9%20v%C3%A0%20th%C6%B0%E1%BB%9Dng%20l%C3%A0%20hi%E1%BB%87u%20qu%E1%BA%A3%20h%C6%A1n%20l%C3%A0%20%C4%91%E1%BB%8Dc%20h%C6%B0%E1%BB%9Bng%20d%E1%BA%ABn%20c%E1%BA%A9n%20th%E1%BA%ADn.md)
Một cái tiêu đề phải khiến ta tự thấy mình phải đọc kỹ nó
Dùng ManicTime để dò lại lịch sử
[Tình tiết là các sự kiện cá nhân](../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Nh%C3%A2n%20h%E1%BB%8Dc/Di%E1%BB%85n%20gi%E1%BA%A3i%20v%C3%A0%20m%C3%B4%20t%E1%BA%A3/%C3%9D%20ngh%C4%A9a%20v%C3%A0%20bi%E1%BB%83u%20t%C6%B0%E1%BB%A3ng/T%C3%ACnh%20ti%E1%BA%BFt%20l%C3%A0%20c%C3%A1c%20s%E1%BB%B1%20ki%E1%BB%87n%20c%C3%A1%20nh%C3%A2n.md)
[Trí nhớ tình tiết và thủ tục thường để não nhớ. Trí nhớ ngữ nghĩa và tương lai thường để cho não ngoài](../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Ngh%C4%A9%20v%E1%BB%81%20vi%E1%BB%87c%20ngh%C4%A9/Khoa%20h%E1%BB%8Dc%20nh%E1%BA%ADn%20th%E1%BB%A9c/Tr%C3%AD%20nh%E1%BB%9B/Tr%C3%AD%20nh%E1%BB%9B%20t%C3%ACnh%20ti%E1%BA%BFt%20v%C3%A0%20th%E1%BB%A7%20t%E1%BB%A5c%20th%C6%B0%E1%BB%9Dng%20%C4%91%E1%BB%83%20n%C3%A3o%20nh%E1%BB%9B.%20Tr%C3%AD%20nh%E1%BB%9B%20ng%E1%BB%AF%20ngh%C4%A9a%20v%C3%A0%20t%C6%B0%C6%A1ng%20lai%20th%C6%B0%E1%BB%9Dng%20%C4%91%E1%BB%83%20cho%20n%C3%A3o%20ngo%C3%A0i.md)

Xanadu
Việc chỉ biết về `await` khiến mình chỉ biết sử dụng hàm bất đồng bộ do người khác viết sẵn, chứ không tự mình tạo ra một hàm bất đồng bộ được.
[Diátaxis](https://diataxis.fr/)

Việc tự học làm nhức đầu. Các buổi chia sẻ kx năng
Liệu đọc bài của tôi có dễ hiểu cho bạn không? Tôi... không biết
[Thông diễn học bắt nguồn từ việc chú giải kinh thánh](../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Nh%C3%A2n%20h%E1%BB%8Dc/Di%E1%BB%85n%20gi%E1%BA%A3i%20v%C3%A0%20m%C3%B4%20t%E1%BA%A3/Di%E1%BB%85n%20gi%E1%BA%A3i/Th%C3%B4ng%20di%E1%BB%85n%20h%E1%BB%8Dc%20b%E1%BA%AFt%20ngu%E1%BB%93n%20t%E1%BB%AB%20vi%E1%BB%87c%20ch%C3%BA%20gi%E1%BA%A3i%20kinh%20th%C3%A1nh.md)

[Một văn bản không nên chỉ là thứ để truyền đạt thông tin hay hiểu biết một chiều và thụ động, mà còn nên trở thành một sân chơi cho người đọc khám phá](../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Ngh%C4%A9%20v%E1%BB%81%20vi%E1%BB%87c%20ngh%C4%A9/M%C3%B4i%20tr%C6%B0%E1%BB%9Dng%20ngh%C4%A9,%20nh%E1%BA%ADn%20th%E1%BB%A9c%20t%C4%83ng%20c%C6%B0%E1%BB%9Dng/%C4%90%E1%BB%8Dc%20v%C3%A0%20vi%E1%BA%BFt/M%E1%BB%99t%20v%C4%83n%20b%E1%BA%A3n%20kh%C3%B4ng%20n%C3%AAn%20ch%E1%BB%89%20l%C3%A0%20th%E1%BB%A9%20%C4%91%E1%BB%83%20truy%E1%BB%81n%20%C4%91%E1%BA%A1t%20th%C3%B4ng%20tin%20hay%20hi%E1%BB%83u%20bi%E1%BA%BFt%20m%E1%BB%99t%20chi%E1%BB%81u%20v%C3%A0%20th%E1%BB%A5%20%C4%91%E1%BB%99ng,%20m%C3%A0%20c%C3%B2n%20n%C3%AAn%20tr%E1%BB%9F%20th%C3%A0nh%20m%E1%BB%99t%20s%C3%A2n%20ch%C6%A1i%20cho%20ng%C6%B0%E1%BB%9Di%20%C4%91%E1%BB%8Dc%20kh%C3%A1m%20ph%C3%A1.md)