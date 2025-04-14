---
share: true
created: 2023-05-26T14:51
cssClass: wide-table
updated: 2025-03-28T01:38
---
Khái niệm:: [Công việc](../../../%CE%9E%20Kh%C3%A1i%20ni%E1%BB%87m/Ph%C3%A1t%20tri%E1%BB%83n%20s%E1%BA%A3n%20ph%E1%BA%A9m,%20l%C3%AAn%20k%E1%BA%BF%20ho%E1%BA%A1ch,%20c%C3%B4ng%20vi%E1%BB%87c/C%C3%B4ng%20vi%E1%BB%87c.md)

| Khía cạnh                                                           | Công việc khai phá (exploration)                                                                                                                                          | Công việc khai thác (exploitation)                                                                                                                                                                                                     |
| ------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tên gọi khác                                                        | Công việc khám phá                                                                                                                                                        | Công việc quy trình                                                                                                                                                                                                                    |
| Dạng bài toán                                                       | Không dễ để mô tả nó một cách rõ ràng. Thường là một công việc vẫn còn đang làm lần đầu và chưa hoàn thành. Sự thay đổi phương pháp trong quá trình làm gần như chắc chắn | Chỉ cần nói một lần là ai cũng hiểu. Là một danh sách/quy trình các tác vụ cụ thể (task), bước thực hiện (step) hoặc đơn vị công việc (unit) đã được khám phá đầy đủ và chỉ cần thực hiện. Ít xảy ra việc thay đổi trong quá trình làm |
| Kết quả đầu ra                                                      | Chưa làm xong thì cũng không chắc lắm kết quả trông như thế nào                                                                                                           | Chưa làm cũng biết chính xác kết quả trông như thế nào                                                                                                                                                                                 |
| Thường có trong giai đoạn                                           | Lên chiến lược                                                                                                                                                            | Thực thi chiến lược                                                                                                                                                                                                                    |
| Sự chiếm dụng tâm trí                                               | Chỉ cần bị phân tâm một tí là mất mạch suy nghĩ ngay. Phải dồn toàn lực để làm. Thiên về hệ thống 2 (tư duy chậm)                                                         | Bị phân tâm một tí cũng không sao. Làm lai rai không phải là vấn đề. Thiên về hệ thống 1 (tư duy nhanh)                                                                                                                                |
| Mối quan hệ tới các thực thể khác*                                  | Kết nối trực tiếp tới một hoặc nhiều mục tiêu, và cũng có thể là một thành phần của một hoặc nhiều công việc khai phá khác                                                | Thường là một thành phần của một công việc khai phá nào đó, hiếm khi là thành phần của nhiều công việc khác hoặc kết nối trực tiếp tới mục tiêu                                                                                        |
| Có phải là câu trả lời cho câu hỏi "Giờ bạn đang cần làm gì" không? | Có                                                                                                                                                                        | Không                                                                                                                                                                                                                                  |
| Sử dụng loại tư duy                                                 | Rhizome/phi tuyến tính                                                                                                                                                    | Rễ cọc/tuyến tính                                                                                                                                                                                                                      |
| Kiểu dữ liệu                                                        | Phi cấu trúc                                                                                                                                                              | Cấu trúc                                                                                                                                                                                                                               |
| Ví dụ                                                               | Xây dựng nhóm                                                                                                                                                             | Thêm chức năng của vault, thiết kế, dịch                                                                                                                                                                                               |

Trước đây có chia ra công việc cấp ban, công việc cấp tiểu ban, công việc cấp cá nhân, và  công việc thành phần, nhưng giờ bỏ.

## \*Ví dụ về mối quan hệ với các thực thể (entity) khác
Ở bảng trên, phần *Mối quan hệ tói các thực thể khác* của công việc khai phá được ghi là:
> Kết nối trực tiếp tới một hoặc nhiều mục tiêu, và cũng có thể là một thành phần của một hoặc nhiều công việc khai phá khác

Điều này có nghĩa là gì?

Ví dụ ta có mục tiêu *Các thành viên hiểu đúng tổ chức muốn đi đến đâu*. Gọi M là mục tiêu này:
```mermaid
flowchart TB
M{{"M: Các thành viên hiểu đúng tổ chức muốn đi đến đâu"}}
style M stroke-width:4px
```
Để đạt được M, ta cần làm công việc khai phá A:
```mermaid
flowchart TB
M{{"M: Các thành viên hiểu đúng tổ chức muốn đi đến đâu"}}
A["A: Đánh giá mức độ hiểu biết của thành viên với tổ chức"]
M-->A
style M stroke-width:4px
```
Tức là A đang đính trực tiếp vào M. 

Khi suy nghĩ cách để làm A ta thấy rằng cần phải chia A thành 2 công việc nhỏ hơn, A1 và A2: 
```mermaid
flowchart TB
A["A: Đánh giá mức độ hiểu biết của thành viên với tổ chức"]
A1["A1: Lập bảng khảo sát TNV định kỳ"]
A2["A2: Đánh giá sự hiệu quả của kế hoạch hành động"]
A-->A1
A-->A2
```
Giờ, ta có thể đính A1 và A2 gián tiếp vào M:
```mermaid
flowchart TB
M{{"M: Các thành viên hiểu đúng tổ chức muốn đi đến đâu"}}
A["A: Đánh giá mức độ hiểu biết của thành viên với tổ chức"]
A1["A1: Lập bảng khảo sát TNV định kỳ"]
A2["A2: Đánh giá sự hiệu quả của kế hoạch hành động"]
M-->A-->A1
A-->A2
style M stroke-width:4px
```
Hoặc trực tiếp vào M đều được:
```mermaid
flowchart TB
M{{"M: Các thành viên hiểu đúng tổ chức muốn đi đến đâu"}}
A1["A1: Lập bảng khảo sát TNV định kỳ"]
A2["A2: Đánh giá sự hiệu quả của kế hoạch hành động"]
M-->A1
M-->A2
style M stroke-width:4px
```
Tuy việc này sẽ làm cây mục tiêu đồ sộ hơn so với chỉ đính A vào M, nhưng nó cũng minh hoạ cho việc sau khi nhìn thấy được các công việc khai phá thành phần của một công việc khai phá, thì ta cũng có thể đính trực tiếp nó vào mục tiêu như thể ta không cần phải nghĩ gì đến công việc khai phá ban đầu. Trong khi với công việc khai thác thì ta không làm được vậy. 

%%Dù sao thì nó cũng không có cảm giác đồ sộ bằng việc (khúc này quên ý)%%
Xem thêm:: 
- [Áp lực giết chết sự sáng tạo](../%C3%81p%20l%E1%BB%B1c%20gi%E1%BA%BFt%20ch%E1%BA%BFt%20s%E1%BB%B1%20s%C3%A1ng%20t%E1%BA%A1o.md)
- [Học là quá trình cấu trúc hoá những thứ phi cấu trúc](../../../Ngh%C4%A9%20v%E1%BB%81%20vi%E1%BB%87c%20ngh%C4%A9/H%E1%BB%8Dc%20t%E1%BA%ADp,%20hi%E1%BB%83u%20bi%E1%BA%BFt/H%E1%BB%8Dc%20l%C3%A0%20qu%C3%A1%20tr%C3%ACnh%20c%E1%BA%A5u%20tr%C3%BAc%20ho%C3%A1%20nh%E1%BB%AFng%20th%E1%BB%A9%20phi%20c%E1%BA%A5u%20tr%C3%BAc.md)
- [Hệ thống 1 dựa vào trí nhớ dài hạn. Hệ thống 2 dựa vào trí nhớ ngắn hạn](../../../Ngh%C4%A9%20v%E1%BB%81%20vi%E1%BB%87c%20ngh%C4%A9/Khoa%20h%E1%BB%8Dc%20nh%E1%BA%ADn%20th%E1%BB%A9c/H%E1%BB%87%20th%E1%BB%91ng%201%20d%E1%BB%B1a%20v%C3%A0o%20tr%C3%AD%20nh%E1%BB%9B%20d%C3%A0i%20h%E1%BA%A1n.%20H%E1%BB%87%20th%E1%BB%91ng%202%20d%E1%BB%B1a%20v%C3%A0o%20tr%C3%AD%20nh%E1%BB%9B%20ng%E1%BA%AFn%20h%E1%BA%A1n.md) 
- [Người người vạch chiến lược hay nhiều khi được giao triển khai luôn, hoặc người làm chuyên môn tốt nhiều khi được đề bạt lên làm quản lý, lãnh đạo](../../X%C3%A2y%20d%E1%BB%B1ng%20nh%C3%B3m,%20qu%E1%BA%A3n%20l%C3%BD%20nh%C3%A2n%20s%E1%BB%B1/Ph%C3%A2n%20c%E1%BA%A5p,%20qu%E1%BA%A3n%20l%C3%BD/Ng%C6%B0%E1%BB%9Di%20ng%C6%B0%E1%BB%9Di%20v%E1%BA%A1ch%20chi%E1%BA%BFn%20l%C6%B0%E1%BB%A3c%20hay%20nhi%E1%BB%81u%20khi%20%C4%91%C6%B0%E1%BB%A3c%20giao%20tri%E1%BB%83n%20khai%20lu%C3%B4n,%20ho%E1%BA%B7c%20ng%C6%B0%E1%BB%9Di%20l%C3%A0m%20chuy%C3%AAn%20m%C3%B4n%20t%E1%BB%91t%20nhi%E1%BB%81u%20khi%20%C4%91%C6%B0%E1%BB%A3c%20%C4%91%E1%BB%81%20b%E1%BA%A1t%20l%C3%AAn%20l%C3%A0m%20qu%E1%BA%A3n%20l%C3%BD,%20l%C3%A3nh%20%C4%91%E1%BA%A1o.md)
