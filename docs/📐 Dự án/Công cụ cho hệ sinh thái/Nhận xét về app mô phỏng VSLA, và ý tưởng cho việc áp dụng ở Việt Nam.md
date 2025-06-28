---
share: true
created: 2025-05-26T19:55
updated: 2025-06-28T15:35
---
## Nhận xét về app mô phỏng VSLA
(Nhận xét có được sau khi chơi được một nửa [app mô phỏng VSLA](https://fabo.org/dca/VSLA_training), đọc hết [tài liệu cho người điều phối](https://fabo.org/pluginfile.php/180950/mod_resource/content/2/VSLA_SimulationGameApp_guideline.pdf) và xem hết [webminar](https://careorg.zoom.us/rec/play/HKnQzNXB9gbPYCjljaGvVTB-RtIpYbMGVAco53mwInmEvCaKhyoIo4GxsRdEXxs3h4-p3bPTbQHkeTZj.YxB6EWTGgLRqcS8M?continueMode=true&_x_zm_rtaid=z95Dco_2QRa5GnzWSjahbA.1642670731961.030913f153adafd79a992fa11e7eda2e&_x_zm_rhtaid=917). Webminar phát âm khó nghe nên cũng lõm bõm)


| Đặc điểm người dùng                                | Hệ quả                                                             |
| -------------------------------------------------- | ------------------------------------------------------------------ |
| Không biết chữ                                     | Cần dùng âm thanh                                                  |
| Trình độ tin học thấp                              | Phải có nhiều affordance: dễ bấm, sinh động                        |
| Không có internet                                  | Phải là chương trình trên máy tính chứ không chạy trên server được |
| Nguồn điện không ổn định, app nặng có lúc bị crash | Cần có bản giấy phòng hờ                                           |
| Không có thiết bị riêng                            | Xem chi tiết ở dưới                                                |

Việc thành viên nhóm không có thiết bị riêng đem lại những hệ quả gì?
- Điểm mạnh:
	- Tăng thêm hứng thú khi được thấy đồ công nghệ
	- Thấy mình đẳng cấp hơn
- Điểm yếu:
	- Do thiết bị được giao cho người điều phối cầm nên họ cần phải cẩn thận để tránh bị trộm cướp
	- Trình diễn cho nhóm đông người xem nên phải là màn hình lớn như tablet hoặc laptop, không thể là điện thoại
		- Người dùng không cá nhân hoá theo số tiền của mình được

Về mặt thiết kế thì cái này không nên gọi là game, vì game là phải cho người dùng được thử nghiệm, khám phá. App này thì cũng gọi là có tương tác, nhưng người dùng chỉ có một lựa chọn để bấm chứ không có tương tác và lựa chọn hành động theo ý của mình được. Nó chỉ dùng để học luật mà thôi.

Về mặt kỹ thuật thì app này dùng Adobe Air, và chạy ActionScript. Adobe Air là một môi trường runtime, còn ActionScript là một ngôn ngữ dựa trên JavaScript. Cơ bản không khác gì Electron với TypeScript ngày nay. Cả Adobe Air và Electron đều không chạy trên trình duyệt được mà phải xuất thành tệp chương trình. Nhưng viết bằng TypeScript thì có thể chuyển đổi sang JavaScript để chạy trên web dễ dàng, còn ActionScript thì không chắc. 

Do chỉ là bấm chuột nên app này làm trên PowerPoint cũng được.

Câu hỏi khác:
- App chỉ có tiếng Anh, trong khi bản giấy thì lại được dịch ra nhiều ngôn ngữ. Bên DanChurchAid đã nguồn lực để làm app và làm nghiên cứu cho 3 quốc gia thì sao lại không dịch được app?
- Vào trang của [VSLA](https://www.vsla.net/) thì không thấy giới thiệu gì về app? 
- Có vẻ như các chương trình VSLA này ở các nước đều đến từ các NGO nước ngoài? Khi nào thì nó phá hoại, khi nào không? 
- CARE có hoạt động ở VN. Nó có thử nghiệm mô hình này ở VN ko?

## Ý tưởng cho việc áp dụng ở Việt Nam
Nếu người ở các cộng đồng làng xã cũng không có thiết bị riêng, mù chữ và khó tiếp cận internet, thì việc dịch app thì đúng là tiết kiệm thời gian hơn. Nếu mà dịch thì chắc dịch thêm cả tiếng bản địa luôn?

Với các quỹ cộng đồng mà thành phần tham dự chủ yếu là người ở đô thị, thì có thể có những điều kiện và nhu cầu khác, như:
- Biết tiếng Anh, 
- Có internet
- Có điện thoại và laptop riêng
- Được tiếp xúc với game lâu rồi
- Không phải ngồi chung với nhau mỗi tuần
- Dễ tiếp cận hệ thống tín dụng hơn

Việc dùng app dịch có lẽ cũng đủ để hướng dẫn họ, chưa phát huy được hết tiềm năng đang có? Ví dụ:
- Thay vì dùng app chỉ phù hợp cho màn hình lớn thì tạo giao diện phù hợp cho điện thoại (mobile-first) và sử dụng được ngay trên web luôn, không cần phải tải về?
- Thay vì chỉ là một app dùng cho việc đào tạo, dùng xong rồi bỏ thì sao không tích hợp với các chương trình khác, như chương trình kết nối AMAP, chương trình tính lãi suất, chương trình quản lý tiền? Hoặc thậm chí là biến nó thành một môi trường giải thích khám phá được ([explorable explanations](https://explorabl.es/))?
  <iframe title="vimeo-player" src="https://player.vimeo.com/video/67076984?h=f57f26cc02" width="640" height="360" frameborder="0"    allowfullscreen></iframe>

Mấy cái đồng coin hay có mấy cái game dùng để làm quen với nó, chắc cũng áp dụng ý tưởng tương tự.

Đọc thêm: 
- [Môi trường nghĩ là nơi ta có thể có những loại suy nghĩ mới, những suy nghĩ mà trước đây ta không thể hình thành](../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Ngh%C4%A9%20v%E1%BB%81%20vi%E1%BB%87c%20ngh%C4%A9/M%C3%B4i%20tr%C6%B0%E1%BB%9Dng%20ngh%C4%A9,%20nh%E1%BA%ADn%20th%E1%BB%A9c%20t%C4%83ng%20c%C6%B0%E1%BB%9Dng/M%C3%B4i%20tr%C6%B0%E1%BB%9Dng%20ngh%C4%A9%20l%C3%A0%20n%C6%A1i%20ta%20c%C3%B3%20th%E1%BB%83%20c%C3%B3%20nh%E1%BB%AFng%20lo%E1%BA%A1i%20suy%20ngh%C4%A9%20m%E1%BB%9Bi,%20nh%E1%BB%AFng%20suy%20ngh%C4%A9%20m%C3%A0%20tr%C6%B0%E1%BB%9Bc%20%C4%91%C3%A2y%20ta%20kh%C3%B4ng%20th%E1%BB%83%20h%C3%ACnh%20th%C3%A0nh.md)
- [Cần nghĩ về công việc như là một cách để kiểm định giả thiết, chứ không phải chỉ để hoàn thành](../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Qu%E1%BA%A3n%20l%C3%BD%20d%E1%BB%B1%20%C3%A1n,%20ph%C3%A1t%20tri%E1%BB%83n%20s%E1%BA%A3n%20ph%E1%BA%A9m,%20x%C3%A2y%20d%E1%BB%B1ng%20t%E1%BB%95%20ch%E1%BB%A9c/C%C3%B4ng%20vi%E1%BB%87c/C%E1%BA%A7n%20ngh%C4%A9%20v%E1%BB%81%20c%C3%B4ng%20vi%E1%BB%87c%20nh%C6%B0%20l%C3%A0%20m%E1%BB%99t%20c%C3%A1ch%20%C4%91%E1%BB%83%20ki%E1%BB%83m%20%C4%91%E1%BB%8Bnh%20gi%E1%BA%A3%20thi%E1%BA%BFt,%20ch%E1%BB%A9%20kh%C3%B4ng%20ph%E1%BA%A3i%20ch%E1%BB%89%20%C4%91%E1%BB%83%20ho%C3%A0n%20th%C3%A0nh.md)


## Về Quỹ Đồng Hành của Kulavietnam
Theo [Hướng dẫn về Quỹ Đồng Hành](https://docs.google.com/document/u/0/d/1A5eW3CkKm55YSxaODh50mr_DDLG0ssM9DTOt3emef5I/mobilebasic "https://docs.google.com/document/u/0/d/1A5eW3CkKm55YSxaODh50mr_DDLG0ssM9DTOt3emef5I/mobilebasic"), các thông tin sẽ được công khai trong hệ thống online, ví dụ như mỗi lần mua cổ phần.

Liên kết:
- https://studio--quy-cong-dong.us-central1.hosted.app/
- https://studio.firebase.google.com/studio-5700039935
- https://www.perplexity.ai/search/toi-co-the-tao-trang-web-voi-1-2IwHvf2TTf.npkyrgZTCzg#5

Câu hỏi:
- Tại sao chỉ cho nhu cầu học tập hoặc kinh doanh? Tại sao không cho vay tiêu dùng, sinh hoạt? Hình như trong mô hình VSLA thì việc vay cho tiêu dùng vẫn cho phép? Nếu mua xe tải để chở hàng thì đó là vật dụng sinh hoạt hay là để kinh doanh?
- Tại sao kinh doanh lại được mà đầu tư thì không? Mua hàng áp mã giảm giá trên Shopee xong bán lại cho shop ngoài là kinh doanh hay đầu tư?
- Có phải mô hình này chỉ là tài chính vi mô, không phải là VSLA vì nó không phải họp mặt mỗi tuần và không cần tới 3 người giữ khoá?
- Có lẽ câu trả lời cho những câu hỏi trên nên được ghi vào trong bài hướng dẫn?