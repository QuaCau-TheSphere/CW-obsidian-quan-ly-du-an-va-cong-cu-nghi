---
share: true
created: 2023-06-03T11:28
updated: 2026-02-10T12:09
---
Khái niệm:: [Văn bản](../../../../../%CE%9E%20Kh%C3%A1i%20ni%E1%BB%87m/Nh%E1%BA%ADn%20th%E1%BB%A9c/V%C4%83n%20b%E1%BA%A3n.md)
Cho rất nhiều văn bản, mỗi văn bản chứa rất nhiều từ. Mục tiêu là tô màu các từ sao cho:
1. Mỗi văn bản càng chứa ít màu càng tốt
2. Mỗi từ phải dùng càng ít màu để tô càng tốt

Thuật toán Gibbs sẽ chạy như sau: Với mỗi từ chưa được tô màu sẽ thống kê các màu đã được tô trước, sau đó chọn màu cho từ đó theo xác suất. Như vậy màu nào thoả điều kiện thì sẽ có xác suất to hơn, nhưng vẫn không loại trừ những cái nhỏ hơn

![1](https://i.stack.imgur.com/BfTJjm.png)

Nguồn:: <iframe width="560" height="315" src="https://www.youtube.com/embed/watch?v=BaM1uiCpj_E&t=452s" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
