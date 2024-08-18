---
share: true
created: 2023-09-05T16:17
updated: 2024-07-21T00:29
---
# Lộ trình hướng dẫn cho chị Hoà (kế toán, dữ liệu) 
## Chương trình Beancount
Demo:
- Đầu vào: ["Managing Your Finances Using Python" - Brian Ryall - YouTube](https://www.youtube.com/watch?v=mFzctYkktXQ)
- Đầu ra: [Income Statement - Example Beancount file](https://fava.pythonanywhere.com/example-beancount-file/income_statement/)

| Đặc điểm                                   | Lợi ích                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| ------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Viết bằng Python                           | Cơ hội để thực hành Python                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| Là chương trình bút toán kép               | Ứng dụng được ngay vào công việc của chị                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| Dùng được trên CLI                         | <li>[Cơ hội làm quen với terminal](https://lậptrình.quảcầu.cc/✍️Lập%20trình/Hệ%20điều%20hành,%20path%20và%20terminal/Terminal,%20shell,%20console/Terminal%20là%20cái%20chương%20trình%20để%20làm%20việc%20với%20shell?utm_source=Vault+C+Obsidian%2C+quản+lý+dự+án+và+công+cụ+nghĩ+(Trang+chủ)&utm_medium=Vault&utm_campaign=C2&utm_content=&utm_term=), công cụ giúp chị bước vào cái lõi của hệ điều hành</li><li>Thấy được bản chất của việc đấu nối các phần mềm lại với nhau thế nào. Có thể minh hoạ việc này bằng việc kết hợp nó với Trấn Kỳ</li> |
| Dữ liệu chương trình lưu dưới dạng tập tin | Hiểu được giá trị của việc lưu dữ liệu tại máy người dùng. Hiểu được việc dùng [Git](https://lậptrình.quảcầu.cc/📊Tổ%20chức%20dữ%20liệu.%20Phân%20tích%20dữ%20liệu/Tổ%20chức%20dữ%20liệu/Git/Git%20giúp%20ta%20du%20hành%20thời%20gian?utm_source=Vault+C+Obsidian%2C+quản+lý+dự+án+và+công+cụ+nghĩ+(Trang+chủ)&utm_medium=Vault&utm_campaign=C2&utm_content=&utm_term=)                                                                                                                                                                                   |
| Tạo lệnh truy vấn phức tạp được            | Tương tự SQL nên cũng giúp làm quen với SQL được                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| Điều khiển hoàn toàn bằng bàn phím         | Giảm đau cổ tay do phải cầm chuột nhiều, nhưng sẽ phải chịu khó đọc hướng dẫn sử dụng                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| Là phần mềm tự do                          | Thấy được [các phần mềm mã nguồn đóng đã xiềng xích mình đến mức độ nào](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/Hi%E1%BB%83u%20bi%E1%BA%BFt%20li%C3%AAn%20ng%C3%A0nh%20trong%20CNTT/T%E1%BB%B1%20tr%E1%BB%8B%20d%E1%BB%AF%20li%E1%BB%87u.%20M%C3%A3%20ngu%E1%BB%93n%20m%E1%BB%9F,%20ph%E1%BA%A7n%20m%E1%BB%81m%20t%E1%BB%B1%20do/Ph%E1%BA%A7n%20m%E1%BB%81m%20t%E1%BB%B1%20do/Khi%20n%C3%B3i%20%C4%91%E1%BA%BFn%20m%C3%A3%20ngu%E1%BB%93n%20m%E1%BB%9F,%20%C4%91a%20s%E1%BB%91%20ch%E1%BB%89%20%C4%91%E1%BB%83%20%C3%BD%20t%E1%BB%9Bi%20vi%E1%BB%87c%20%C4%91%C6%B0%E1%BB%A3c%20%C4%91%E1%BB%8Dc%20m%C3%A3%20ngu%E1%BB%93n,%20ch%E1%BB%A9%20kh%C3%B4ng%20%C4%91%E1%BB%83%20%C3%BD%20%C4%91%E1%BA%BFn%20quy%E1%BB%81n%20%C4%91%C6%B0%E1%BB%A3c%20ch%E1%BB%89nh%20s%E1%BB%ADa%20v%C3%A0%20ph%C3%A2n%20ph%E1%BB%91i%20n%C3%B3.md)                                                                                                                                                                                                                                                                                                                                                    |
| Miễn phí                                   | Cắt giảm chi phí mua phần mềm                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Có sẵn trang báo cáo                       | Đỡ phải tạo trang báo cáo riêng                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |

Cân nhắc:
- Em chưa dùng nó bao giờ, thuật ngữ kế toán em cũng không rành
- Các giải pháp dữ liệu khác như PowerBI có thể cũng đáp ứng được các nhu cầu này. Nó sẽ tuỳ vào việc chị muốn một phần mềm chuyên môn hoá hay có khả năng linh hoạt

Xem thêm:: [So sách chức năng của Misa với Beancount](https://kiếmtiền.quảcầu.cc/Tài-nguyên-hỗ-trợ/Quang-cảnh-thị-trường/Chương-trình-quản-lý-tiền/4-Loại-chương-trình/Chương-trình-kế-toán?utm_source=Vault+C+Obsidian%2C+quản+lý+dự+án+và+công+cụ+nghĩ+(Dự+án)&utm_medium=Vault&utm_campaign=&utm_content=📐+Dự+án%2FCác+buổi+đáp+ứng+nhu+cầu+học+cách+sử+dụng+công+cụ+và+tư+duy+lập+trình+cho+nhu+cầu+công+việc%2F9+Blog%2FNgười+tham+gia%2FTrần+Thuý+Hoà.md&utm_term=) 
# Trấn Kỳ
[Làm sao để đưa VNPAY vào luồng hoạt động của cửa hàng?](https://slide.quảcầu.cc/Đáp%20ứng%20nhu%20cầu%20doanh%20nghiệp/VNPAY.html?utm_source=Vault+C+Obsidian%2C+quản+lý+dự+án+và+công+cụ+nghĩ+(Dự+án)&utm_medium=Vault&utm_campaign=&utm_content=📐+Dự+án%2FCác+buổi+đáp+ứng+nhu+cầu+học+cách+sử+dụng+công+cụ+và+tư+duy+lập+trình+cho+nhu+cầu+công+việc%2F9+Blog%2FNgười+tham+gia%2FTrần+Thuý+Hoà.md&utm_term=) 
# Các vấn đề về Excel 
- [Excel dịch chuyển một phần quyền lực của chuyên gia IT vào người sử dụng](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/H%E1%BB%87%20th%E1%BB%91ng%20th%C3%B4ng%20tin/No%20code,%20low%20code/Excel/Excel%20d%E1%BB%8Bch%20chuy%E1%BB%83n%20m%E1%BB%99t%20ph%E1%BA%A7n%20quy%E1%BB%81n%20l%E1%BB%B1c%20c%E1%BB%A7a%20chuy%C3%AAn%20gia%20IT%20v%C3%A0o%20ng%C6%B0%E1%BB%9Di%20s%E1%BB%AD%20d%E1%BB%A5ng.md)
- [Excel không cho ta quản lý phiên bản được](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/H%E1%BB%87%20th%E1%BB%91ng%20th%C3%B4ng%20tin/No%20code,%20low%20code/Excel/Excel%20kh%C3%B4ng%20cho%20ta%20qu%E1%BA%A3n%20l%C3%BD%20phi%C3%AAn%20b%E1%BA%A3n%20%C4%91%C6%B0%E1%BB%A3c.md)
- [Excel không cản ta làm điều mà ta sẽ hối tiếc](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/H%E1%BB%87%20th%E1%BB%91ng%20th%C3%B4ng%20tin/No%20code,%20low%20code/Excel/Excel%20kh%C3%B4ng%20c%E1%BA%A3n%20ta%20l%C3%A0m%20%C4%91i%E1%BB%81u%20m%C3%A0%20ta%20s%E1%BA%BD%20h%E1%BB%91i%20ti%E1%BA%BFc.md)
- [Excel không làm ta hiểu về lập trình một cách đúng đắn](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/H%E1%BB%87%20th%E1%BB%91ng%20th%C3%B4ng%20tin/No%20code,%20low%20code/Excel/Excel%20kh%C3%B4ng%20l%C3%A0m%20ta%20hi%E1%BB%83u%20v%E1%BB%81%20l%E1%BA%ADp%20tr%C3%ACnh%20m%E1%BB%99t%20c%C3%A1ch%20%C4%91%C3%BAng%20%C4%91%E1%BA%AFn.md)
- [Excel là loài gián trong ngành phần mềm](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/H%E1%BB%87%20th%E1%BB%91ng%20th%C3%B4ng%20tin/No%20code,%20low%20code/Excel/Excel%20l%C3%A0%20lo%C3%A0i%20gi%C3%A1n%20trong%20ng%C3%A0nh%20ph%E1%BA%A7n%20m%E1%BB%81m.md)
- [Excel là nguồn ý tưởng cũng như là kẻ thù lớn nhất của các SaaS](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/H%E1%BB%87%20th%E1%BB%91ng%20th%C3%B4ng%20tin/No%20code,%20low%20code/Excel/Excel%20l%C3%A0%20ngu%E1%BB%93n%20%C3%BD%20t%C6%B0%E1%BB%9Fng%20c%C5%A9ng%20nh%C6%B0%20l%C3%A0%20k%E1%BA%BB%20th%C3%B9%20l%E1%BB%9Bn%20nh%E1%BA%A5t%20c%E1%BB%A7a%20c%C3%A1c%20SaaS.md)
- [Excel là người bạn tuổi thơ tuyệt vời, nhưng là kẻ thù của tuổi dậy thì](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/H%E1%BB%87%20th%E1%BB%91ng%20th%C3%B4ng%20tin/No%20code,%20low%20code/Excel/Excel%20l%C3%A0%20ng%C6%B0%E1%BB%9Di%20b%E1%BA%A1n%20tu%E1%BB%95i%20th%C6%A1%20tuy%E1%BB%87t%20v%E1%BB%9Di,%20nh%C6%B0ng%20l%C3%A0%20k%E1%BA%BB%20th%C3%B9%20c%E1%BB%A7a%20tu%E1%BB%95i%20d%E1%BA%ADy%20th%C3%AC.md)
- [Excel là sản phẩm low code tồn tại lâu dài nhất](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/H%E1%BB%87%20th%E1%BB%91ng%20th%C3%B4ng%20tin/No%20code,%20low%20code/Excel/Excel%20l%C3%A0%20s%E1%BA%A3n%20ph%E1%BA%A9m%20low%20code%20t%E1%BB%93n%20t%E1%BA%A1i%20l%C3%A2u%20d%C3%A0i%20nh%E1%BA%A5t.md)
- [Excel đã làm một việc phi thường trong việc giáo dục hàng trăm triệu người về sức mạnh của phần mềm](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/H%E1%BB%87%20th%E1%BB%91ng%20th%C3%B4ng%20tin/No%20code,%20low%20code/Excel/Excel%20%C4%91%C3%A3%20l%C3%A0m%20m%E1%BB%99t%20vi%E1%BB%87c%20phi%20th%C6%B0%E1%BB%9Dng%20trong%20vi%E1%BB%87c%20gi%C3%A1o%20d%E1%BB%A5c%20h%C3%A0ng%20tr%C4%83m%20tri%E1%BB%87u%20ng%C6%B0%E1%BB%9Di%20v%E1%BB%81%20s%E1%BB%A9c%20m%E1%BA%A1nh%20c%E1%BB%A7a%20ph%E1%BA%A7n%20m%E1%BB%81m.md)
- [Excel không phù hợp cho việc lập cơ sở dữ liệu](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/H%E1%BB%87%20th%E1%BB%91ng%20th%C3%B4ng%20tin/No%20code,%20low%20code/Excel/Excel%20kh%C3%B4ng%20ph%C3%B9%20h%E1%BB%A3p%20cho%20vi%E1%BB%87c%20l%E1%BA%ADp%20c%C6%A1%20s%E1%BB%9F%20d%E1%BB%AF%20li%E1%BB%87u.md)
- [Excel là một ngôn ngữ lập trình mà không làm ta cảm giác là đang lập trình](../../../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/H%E1%BB%87%20th%E1%BB%91ng%20th%C3%B4ng%20tin/No%20code,%20low%20code/Excel/Excel%20l%C3%A0%20m%E1%BB%99t%20ng%C3%B4n%20ng%E1%BB%AF%20l%E1%BA%ADp%20tr%C3%ACnh%20m%C3%A0%20kh%C3%B4ng%20l%C3%A0m%20ta%20c%E1%BA%A3m%20gi%C3%A1c%20l%C3%A0%20%C4%91ang%20l%E1%BA%ADp%20tr%C3%ACnh.md)

# Giới thiệu chung
![Pasted image 20240221020431.png](../../../../attachments/Pasted%20image%2020240221020431.png)

E ơi như hôm trước trao đổi, chị gửi lại em 1 số nội dung liên quan đến data/lập trình chị muốn tìm hiểu và muốn nhờ em bố trí giúp chị 1 lộ trình Coach 1:1 để chị có thể tìm hiểu về lập trình/AI/data và các công cụ . Em xem và advise giúp chị 1 lộ trình nhé. 
Về thời điểm học, chị có thể start luôn tuần này vào buổi tối hoặc cuối tuần nhé. 
Về việc chi trả, chị cũng đọc và thấy em offer việc định giá "trả tùy tâm" nhưng chị cũng ko có nhiều insight lắm nên có thể em cho chị 1 range nào cụ thể để chị em mình trao đổi cho dễ e nhé.

---
## Tổng quan
Đầu tiên, em muốn giải thích một chút về ngành công nghệ thông tin. Ngành này chia ra 4 chuyên môn chính:
- **Khoa học máy tính:** hiểu biết chung về máy tính
- **Kỹ thuật phần mềm:** ứng dụng những hiểu biết về máy tính trong việc bảo nó làm điều mình cần nó làm (lập trình, tự động hoá, viết code) 
- **Hệ thống thông tin:** ứng dụng của việc viết code đó vào việc quản lý thông tin nội bộ. Các ERP, CRM là những ví dụ
- **Phân tích dữ liệu:** ứng dụng của việc viết code đó vào việc tạo báo cáo và thêm insight. Đây là cái chị cần

Bất cứ sản phẩm công nghệ nào cũng là tổ hợp của 4 cái này, đặc biệt là 2 cái đầu. Em có thể tự tin có thể giải đáp được mọi thắc mắc của chị về 2 cái đầu, cái thứ 3 cũng khá tự tin, nhưng cái cuối thì không tự tin bằng. 
## Phân tích dữ liệu
Một nghiệp vụ liên quan đến dữ liệu thường có 4 bước sau đây:
- Thu thập dữ liệu
- Lưu trữ dữ liệu
- Xử lý dữ liệu
- Báo cáo dữ liệu

Thì cũng tương tự như trên, em dự đoán mình có thể trả lời khoảng 70% những thắc mắc của chị liên quan tới 3 cái đầu, còn cái cuối thì không nhiều lắm. Mà có lẽ bước đó là cái chị quan tâm nhất.

Trong mục xử lý dữ liệu có một số chủ đề nữa:
- Xử lý ngôn ngữ tự nhiên
- Máy học và trí tuệ nhân tạo

Những cái này là cái mà em nghĩ chị nói tới khi nói "cập nhật xu thế công nghệ", vì khá nhiều xu thế công nghệ thực ra chỉ là 2 cái này. Em tự tin có thể nói về cái đầu và chắc đủ để nói về cái sau.
## Lộ trình
Em nghĩ trước mắt thì chị cứ hỏi em những gì chị muốn biết rồi mình trao đổi thêm. Câu hỏi nào em không biết thì em có thể cho chị một vài từ khoá, hoặc nếu chị cần tìm một người khác có chuyên môn hơn em về lĩnh vực này thì có thể giải thích thêm những thứ họ quảng cáo. Nếu có những cái em không mường tượng rõ lắm thì có lẽ em cần chị chia sẻ màn hình để thấy được thao tác của chị. 

Vì đây là để đáp ứng nhu cầu của chị nên khi nào chị muốn hỏi em và em rảnh thì mình sẽ gọi thôi. Chắc chỉ cần báo trước là được. Em cũng không muốn chị có cảm giác khó chịu khi mình còn nhiều câu hỏi mà phải nghỉ, nên mình cũng sẽ nói cho tới khi chị muốn nghỉ thì thôi.

## Chi phí
Nếu chị không muốn nhức đầu thì em có thể báo giá luôn cho chị. Nhưng nếu chị thấy việc tìm hiểu sâu hơn về nhau thú vị hơn thì mình có thể thảo luận thêm để mình có thể tạo ra được một cuộc trao đổi thoả mãn với cả hai bên.

## Các data coach khác
Do em không làm chuyên về dữ liệu, nên có thể có những coach khác giúp chị tốt hơn mảng này. Người này em thấy có vẻ tốt nhất:
![](https://i.imgur.com/JcGgmFq.png)
[Discord](https://discord.com/channels/1124195842820161637/1124195843323465802/1221398468560552066)

Ngoài ra các trung tâm khi đăng ký học cũng đều có coach. Em không biết mức độ phù hợp với chị thế nào:
- https://www.facebook.com/reel/268325176050954
- https://unigap.io/lien-he/
