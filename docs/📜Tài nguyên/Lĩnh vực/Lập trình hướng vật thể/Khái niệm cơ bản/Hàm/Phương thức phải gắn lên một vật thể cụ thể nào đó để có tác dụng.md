---
share: true
created: 2023-06-09T11:16
updated: 2024-09-02T15:16
---
Hàm giúp ta làm một công việc nào đó. Công việc đó có thể liên quan tới một vật thể hoặc không. Còn phương thức chắc chắn phải làm những công việc liên quan tới một vật thể cụ thể. [Phương thức cho ta biết mình có thể làm gì với vật thể đó](./Ph%C6%B0%C6%A1ng%20th%E1%BB%A9c%20cho%20ta%20bi%E1%BA%BFt%20m%C3%ACnh%20c%C3%B3%20th%E1%BB%83%20l%C3%A0m%20g%C3%AC%20v%E1%BB%9Bi%20v%E1%BA%ADt%20th%E1%BB%83%20%C4%91%C3%B3.md). 

Ví dụ, bạn có một rổ trái cây:
![|300](https://upload.wikimedia.org/wikipedia/commons/thumb/b/b6/A_basket_of_fruits.jpg/600px-A_basket_of_fruits.jpg)

Bạn muốn cân khối lượng từng quả, nên bạn viết một **phương thức** `cân_nặng()` giúp bạn cân chúng:

```python
táo.cân_nặng()   # Kết quả: 30g
chuối.cân_nặng() # Kết quả: 40g
lê.cân_nặng()    # Kết quả: 50g
```

Bạn thấy, dù phương thức `cân_nặng()` không thay đổi, nhưng đối với mỗi một loại trái cây khác nhau sẽ cho một kết quả khác nhau. Phương thức này phải gắn lên một đối tượng cụ thể nào đó để có tác dụng. Bạn phải không thể cân không gì cả được. 

Trong khi đó, nếu bạn muốn biết ngày hôm nay là ngày gì, bạn chỉ cần dùng **hàm** `xem_ngày()`:

```python
xem_ngày() # Kết quả: "ngày 32 tháng 13 năm 12023" 
```

Bạn thấy là công việc `xem_ngày()` này không phụ thuộc vào vật thể nào. Dù bạn quyết định là sẽ ăn táo hay ăn lê thì kết quả cũng không thay đổi. Dù bạn không có vật thể nào bạn vẫn có thể xem ngày được. 

