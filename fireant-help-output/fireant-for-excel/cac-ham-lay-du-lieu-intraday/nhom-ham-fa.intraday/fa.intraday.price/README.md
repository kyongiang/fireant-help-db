---
title: "FA.Intraday.Price"
source: "https://help.fireant.vn/fireant-for-excel/cac-ham-lay-du-lieu-intraday/nhom-ham-fa.intraday/fa.intraday.price"
---

# FA.Intraday.Price

**Cú pháp:**

```
=FA.Intraday.Price("Mã CK hoặc Mã Index","Lần khớp")
```

Hàm FA.Intraday.Price có các tham số sau :

* **Mã chứng khoán:** Mã chứng khoán cần lấy thông tin hoặc index (VNINDEX, HNXINDEX, UPCOM, VN30, HNX30,...&#x20;
* **Lần khớp**: Thứ tự lần khớp (1, 2,... tương ứng với lần khớp gần nhất, gần nhì,...

**Trả về:**

Giá khớp lệnh trong ngày của 1 mã hoặc index

**Ví dụ:**

Để lấy giá khớp lệnh của mã FPT tương ứng với lần khớp thứ 10 tính từ lần khớp cuối, ta dùng công thức sau:

```
=FA.Intraday.Price("FPT",10)
```

**Kết quả:**

90700

Bạn cũng có thể ghi mã FPT ở một ô (cell), ví dụ A1, và dùng công thức sau:

```
=FA.Intraday.Price(A1,10)
```

Ưu điểm của phương pháp này là bạn có thể thay đổi mã chứng khoán mà không cần sửa công thức.

{% hint style="info" %}
**Lưu ý**: Nếu bạn truyền ô vào thay vì mã chứng khoán, thì ở ô đó cần chứa mã chứng khoán. Trong trường hợp này mã chứng khoán không cần nằm giữa 2 dấu nháy đôi.&#x20;
{% endhint %}

Tham số lần khớp cũng có thể sử dụng hàm lấy số dòng hoặc số cột để thay thế, trong trường hợp bạn muốn lấy thông tin của nhiều lần khớp. Bạn có thể dùng công thức sau, với giả sử ô A1 chứa mã, và bạn sử dụng công thức cho ô A2 trở đi:

```
=FA.Intraday.Price(A$1, ROW()-1)
```
