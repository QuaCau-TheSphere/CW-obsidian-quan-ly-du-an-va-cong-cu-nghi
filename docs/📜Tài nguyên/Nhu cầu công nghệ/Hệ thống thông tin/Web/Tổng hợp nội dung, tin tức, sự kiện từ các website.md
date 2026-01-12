---
share: true
created: 2024-11-29T12:19
updated: 2026-01-10T12:14
---
Đáp ứng cho nhu cầu công việc: [Cập nhật thông tin bên ngoài, tổng hợp sự kiện sẽ diễn ra](../../../Nhu%20c%E1%BA%A7u%20c%C3%B4ng%20vi%E1%BB%87c/V%E1%BA%ADn%20h%C3%A0nh/C%E1%BA%ADp%20nh%E1%BA%ADt%20th%C3%B4ng%20tin%20b%C3%AAn%20ngo%C3%A0i,%20t%E1%BB%95ng%20h%E1%BB%A3p%20s%E1%BB%B1%20ki%E1%BB%87n%20s%E1%BA%BD%20di%E1%BB%85n%20ra.md),[Nắm bắt xu hướng mạng](../../../Nhu%20c%E1%BA%A7u%20c%C3%B4ng%20vi%E1%BB%87c/Nghi%C3%AAn%20c%E1%BB%A9u/Thu%20th%E1%BA%ADp%20d%E1%BB%AF%20li%E1%BB%87u/N%E1%BA%AFm%20b%E1%BA%AFt%20xu%20h%C6%B0%E1%BB%9Bng%20m%E1%BA%A1ng.md)

Lĩnh vực:: 
Giải pháp kỹ thuật:: 
Nhu cầu công nghệ:: [Cào web](./C%C3%A0o%20web.md)

## Tin tức
**news aggregator**, also termed a **feed aggregator**, **content aggregator**, **feed reader**, **news reader**, or simply an **aggregator**
[News aggregator - Wikipedia](https://en.wikipedia.org/wiki/News_aggregator)
Những cái này đọc qua RSS

Nếu không dùng RSS thì phải [Cào web](./C%C3%A0o%20web.md)

[Internet Aggregator: Khám phá công cụ tổng hợp thông tin trực tuyến hiệu quả](https://rdsic.edu.vn/blog/blog-4/internet-aggregator-vi-cb.html)
Tổng hợp các thông tin mà các báo đăng mỗi ngày: [Trung tâm báo chí Thành phố Hồ Chí Minh](https://ttbc-hcm.gov.vn/)

Hot trend trên reddit, Facebook
[News Minimalist — All news ranked by significance](https://www.newsminimalist.com/?sort=significance)

## Sự kiện
- Sự kiện doanh nghiệp: [VietBest® Khám phá Sự kiện - Hội chợ Triển lãm - Ở đâu Khuyến mãi giá tốt gần nhất !](https://vietbest.vn/kham-pha)

## Nội dung
![](https://nodetics.com/feedbro/shots/integrations.png)
### Nhập toàn bộ danh sách theo dõi từ Facebook
![Nhập toàn bộ danh sách theo dõi từ Facebook.png](../../../../attachments/Nh%E1%BA%ADp%20to%C3%A0n%20b%E1%BB%99%20danh%20s%C3%A1ch%20theo%20d%C3%B5i%20t%E1%BB%AB%20Facebook.png)

1. Vào profile của mình, mở followings, cuộn xuống cho đến khi FB load hết, rồi mở Firefox Dev Console, copy inner HTML chứa toàn bộ thẻ div của cái danh sách theo dõi ấy.
  (Với Firefox, cần vào `about:config`, set `devtools.markup.beautifyOnCopy` true trước, để giữ format/indent khi copy)

2. Dán vào sublime, rồi xài chức năng find and replace with regex để format lại.
  Đầu tiên dùng chức năng find → find all trước, để lọc ra thẻ liên quan.
   ```html
   <a class="" href="(https://www.facebook.com/[^"]+)"[^>]*> (https://www%5C.facebook%5C.com/%5B%5E%22%5D+)%22%5B%5E%3E%5D*%3E)<span class="" dir="auto">([^<]+)</span>
   ```
  Rồi ấn Ctrl+C để copy toàn bộ cái được lọc ra, paste lại nó lên sublime.
Sau đó nhấn Ctrl + H, và sử dụng pattern  `<outline text="$2" title="$2" type="rss" \n xmlUrl="$1" htmlUrl="$1"/>` để convert sang định đạng OPML dùng cho FeedBro.

3. Mở FeedBro, chọn Setting, chọn xuất ra OPML file.
  Mở cái file đó ra, tạo thêm thư mục mới với thẻ outline, và copy toàn bộ bên kia sang và lưu lại.
  Rồi nhập ngược lại vào FeedBro là xong

Ngoại trừ một số tài khoản để trang cá nhân "chỉ bạn bè" thì đành chịu, chưa có cách. 
Cái này có vấn đề với bài đăng được chia sẻ từ bên thứ ba, video hoặc reel. Nhưng text thì có vẻ hoạt động.

Xem theo dòng thời gian, lọc bởi từ khóa, hay xem song song nhiều tab cùng lúc (như TweetDesk) khá tiện
