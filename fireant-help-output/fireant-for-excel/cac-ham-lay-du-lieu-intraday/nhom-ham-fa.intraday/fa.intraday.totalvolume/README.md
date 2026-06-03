---
title: "FA.Intraday.TotalVolume"
source: "https://help.fireant.vn/fireant-for-excel/cac-ham-lay-du-lieu-intraday/nhom-ham-fa.intraday/fa.intraday.totalvolume"
---

# FA.Intraday.TotalVolume

**Cú pháp**

```
=FA.Intraday.TotalVolume(Mã chứng khoán, Lần khớp)
```

Hàm FA.Intraday.TotalVolume có các tham số sau :

* **Mã chứng khoán:** Mã chứng khoán của cổ phiếu cần lấy thông tin&#x20;
* **Lần khớp**: Thứ tự lần khớp (1, 2,... tương ứng với lần khớp gần nhất, gần nhì,...

**Trả về**

Tổng khối lượng khớp lệnh tích lũy trong ngày của 1 mã hoặc index

**Ví dụ:**

Để biết tổng khối lượng khớp lệnh của mã FPT tính đến lần khớp thứ 10 tính từ lần khớp cuối, ta dùng công thức sau:

```
=FA.Intraday.TotalVolume("FPT",10)
```

**Kết quả:**

753700

Bạn cũng có thể ghi mã FPT ở một ô (cell), ví dụ A1, và dùng công thức sau:

```
=FA.Intraday.TotalVolume(A1,10)
```

Ưu điểm của phương pháp này là bạn có thể thay đổi mã chứng khoán mà không cần sửa công thức.

{% hint style="info" %}
**Lưu ý**: Nếu bạn truyền ô vào thay vì mã chứng khoán, thì ở ô đó cần chứa mã chứng khoán. Trong trường hợp này mã chứng khoán không cần nằm giữa 2 dấu nháy đôi.&#x20;
{% endhint %}

Tham số lần khớp cũng có thể sử dụng hàm lấy số dòng hoặc số cột để thay thế, trong trường hợp bạn muốn lấy thông tin của nhiều lần khớp. Bạn có thể dùng công thức sau, với giả sử ô A1 chứa mã, và bạn sử dụng công thức cho ô A2 trở đi:

```
=FA.Intraday.TotalVolume(A$1, ROW()-1)
```
