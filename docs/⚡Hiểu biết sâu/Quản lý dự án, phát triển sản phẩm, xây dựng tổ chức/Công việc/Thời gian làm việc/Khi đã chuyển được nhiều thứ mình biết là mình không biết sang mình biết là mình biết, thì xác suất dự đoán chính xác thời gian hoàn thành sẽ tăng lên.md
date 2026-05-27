---
share: true
created: 2026-04-16T11:21
updated: 2026-05-27T17:08
---
# Làm sao để biết rằng việc nghiên cứu không kéo dài mãi mãi?
Ban đầu ta có:
- $a_0$ điều mình không biết là mình không biết 
- $b_0$ điều mình biết là mình không biết 
- $c_0$ điều mình biết là mình biết

Sau một thời gian nghiên cứu, ta có:
- $a_1$ điều mình không biết là mình không biết 
- $b_1$ điều mình biết là mình không biết 
- $c_1$ điều mình biết là mình biết

Đặc điểm của việc nghiên cứu:
- Sẽ có những điều mình không biết là mình không biết và mình biết là mình không biết mới mà không đến từ những điều cũ
- Có thể cho là xác suất xổ ra những điều mình không biết là mình không biết là như nhau, hoặc thậm chí là giảm đi, nhưng chắc là không thể tăng lên
- Một số điều mình không biết là mình không biết sẽ được chuyển thành:
	- Điều mình biết là mình không biết. Tức là một lượng $b_1$ là đến từ $a_0$
	- Điều mình biết là mình biết. Tức là một lượng $c_1$ là đến từ $a_0$
- Một số điều mình biết là mình không biết sẽ được chuyển thành điều mình biết là mình biết. Tức là một lượng $c_1$ là đến từ $b_0$
- Những điều mình biết là mình biết thì vẫn sẽ là điều mình biết là mình biết
- Nghiên cứu sẽ kết thúc trong sự thỏa mãn nếu không còn điều gì mình biết là mình không biết. Tức là khi $b_1$ = 0
- Các đơn vị của sự hiểu biết là số tự nhiên

[![](https://mermaid.ink/img/pako:eNo9js1uhDAMhF8F-dJLQLBJ-Mm1fYYeqlwMmB8tJKtA1G4R715IaU_fjDW2Z4PGtgQK4jjWprGmG3ulTRQtaO70DPIwg_18x8nToqIOp4W0CfnfkDZHiuELu2mDJ7OTdWB0EVkTWF--vnxzERj0bmxBrc4Tg5ncjKeF7WygYR1oJg3qkC116KdVgzb7sfZA82Ht_LfprO8HUKElA_9ocaW3EXuH8__UkWnJvVpvVlBChBugNvgCdRNVkhayKGQmclEKXjJ4gso4T3JZ5WlecS4rXsidwXd4myZ5XpVHWGZFJksu9h83iWaW?type=png)](https://mermaid.live/edit#pako:eNo9js1uhDAMhF8F-dJLQLBJ-Mm1fYYeqlwMmB8tJKtA1G4R715IaU_fjDW2Z4PGtgQK4jjWprGmG3ulTRQtaO70DPIwg_18x8nToqIOp4W0CfnfkDZHiuELu2mDJ7OTdWB0EVkTWF--vnxzERj0bmxBrc4Tg5ncjKeF7WygYR1oJg3qkC116KdVgzb7sfZA82Ht_LfprO8HUKElA_9ocaW3EXuH8__UkWnJvVpvVlBChBugNvgCdRNVkhayKGQmclEKXjJ4gso4T3JZ5WlecS4rXsidwXd4myZ5XpVHWGZFJksu9h83iWaW)
Tức là: 
- $a_0 = a_{a_1} + a_{b_1} + a_{c_1}$
- $b_0 = b_{b_1} + b_{c_1}$
- $a_1 = a_{a_1} + x ≤ a_0$
- $b_1 = a_{b_1} + b_{b_1} + y$
- $c_1 = a_{c_1} + b_{c_1} + c_0 ≥ c_0$ 
- $a_0, b_0, c_0, a_1, b_1, c_1 \in\mathbb{N}$

Liệu rằng sau nhiều lần lặp thì $b_i$ sẽ tiến tới $0$?
$$
b_1 = a_{b_1} + b_{b_1} + y
$$
$$= (a_0 - a_{a_1} - a_{c_1}) + (b_0 - b_{c_1}) + y $$
$$= a_0 - a_{a_1} - (c_1 - b_{c_1}) + b_0 - b_{c_1} + y$$
$$= a_0 - a_{a_1} + b_0 - c_1 + y $$

Nếu $a_i$, $a_{a_i}$ và $y$ không đổi thì ta có $b_{i+1} = b_i - c_{i+1} + const$. Nếu $c_i$ luôn tăng thì chắc là $b_i$ sẽ tiến tới $0$.

Nguồn:: [Tự ngẫm nghĩ, trải nghiệm](../../../%CE%9E%20Ngu%E1%BB%93n/T%E1%BB%B1%20ng%E1%BA%ABm%20ngh%C4%A9,%20tr%E1%BA%A3i%20nghi%E1%BB%87m.md)
Khái niệm:: [Sự không biết](../../../%CE%9E%20Kh%C3%A1i%20ni%E1%BB%87m/S%E1%BB%B1%20kh%C3%B4ng%20bi%E1%BA%BFt.md), [Thời gian, lịch](../../../%CE%9E%20Kh%C3%A1i%20ni%E1%BB%87m/Th%E1%BB%9Di%20gian,%20l%E1%BB%8Bch.md), [Dự đoán](../../../%CE%9E%20Kh%C3%A1i%20ni%E1%BB%87m/D%E1%BB%B1%20%C4%91o%C3%A1n.md)
