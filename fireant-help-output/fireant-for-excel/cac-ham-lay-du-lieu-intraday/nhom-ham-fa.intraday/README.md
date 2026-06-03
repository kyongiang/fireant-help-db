---
title: "Lớp hàm FA.Intraday"
source: "https://help.fireant.vn/fireant-for-excel/cac-ham-lay-du-lieu-intraday/nhom-ham-fa.intraday"
---

# Lớp hàm FA.Intraday

## **Cú pháp**

```
=FA.Intraday.[Trường thông tin]("Mã CK hoặc Mã Index","Lần khớp") 
```

**Trong đó:**

* **Mã CK**: là mã của những chứng khoán niêm yết
* **Mã Index**: là tên Index tương ứng, ví dụ: VNINDEX, HNXINDEX, UPINDEX, VN30, HNX30, …&#x20;
* **Trường thông tin**: tên trường tương ứng với một thông tin nhất định của mã chứng khoán hoặc Index
* **Lần khớp**: là số thứ tự của lần khớp. Số thứ tự được tính từ 1, tương ứng với lần khớp gần nhất của mã hoặc lần tổng hợp gần nhất của Index

**Ví dụ**\
Giả sử từ đầu ngày đến giờ, Mã FPT đã có tất cả 10 lần khớp lệnh. Nếu muốn xem giá của lần khớp thứ 8 ta dùng công thức:&#x20;
------------------------------------------------------------------------------------------------------------------------------

```
=FA.Intraday.Price("FPT",8)
```

Bạn cũng có thể ghi mã chứng khoán ở một ô (cell), ví dụ A1, và dùng công thức sau:

```
=FA.Intraday.Price(A1,10)
```

Ưu điểm của phương pháp này là bạn có thể thay đổi mã chứng khoán mà không cần sửa công thức.

{% hint style="info" %}
**Lưu ý**: Nếu bạn truyền ô vào thay vì mã chứng khoán, thì ở ô đó cần chứa mã chứng khoán. Trong trường hợp này mã chứng khoán không cần nằm giữa 2 dấu nháy đôi.&#x20;
{% endhint %}

Trong trường hợp muốn hiển thị bảng intraday (hiển thị tất cả các kết quả khớp lệnh), có thể lợi dụng hàm ROW() hoặc COLUMN() làm giá trị cho tham số **Lần khớp.** Bạn có thể dùng công thức sau, với giả sử ô A1 chứa mã, và bạn sử dụng công thức cho ô A2 trở đi:

```
=FA.Intraday.Price(A$1, ROW()-1)
```

{% hint style="info" %}
**Lưu ý:** Dấu chấm phẩy hoặc dấu phẩy được sử dụng làm dấu ngăn cách giữa các tham số trong công thức tùy theo hệ thống bạn đang sử dụn&#x67;**.**
{% endhint %}
