---
title: "Lớp hàm FA.Quote"
source: "https://help.fireant.vn/fireant-for-excel/cac-ham-lay-du-lieu-intraday/nhom-ham-fa.quote"
---

# Lớp hàm FA.Quote

## **Cú pháp**

Để lấy thông tin giao dịch của mã cổ phiếu ở thời điểm hiện tại, nhập công thức theo dạng sau vào một ô mà bạn dự định hiện thị kết quả:&#x20;

```
=FA.Quote.[Trường thông tin]("Mã CK")
```

**Trong đó:**

* **Mã CK**: là mã của chứng khoán niêm yết
* **Trường thông tin**: là tên trường tương ứng với một thông tin nhất định về giao dịch cổ phiếu hiện tại

## **Ví dụ**

Nếu muốn lấy giá hiện tại của mã AAA, nhập biểu thức:&#x20;

```
=FA.Quote.PriceLast("AAA")
```

Bạn cũng có thể ghi mã chứng khoán ở một ô (cell), ví dụ A1, và dùng công thức sau:

```
=FA.Intraday.PriceLast(A1)
```

Ưu điểm của phương pháp này là bạn có thể thay đổi mã chứng khoán mà không cần sửa công thức.

{% hint style="info" %}
**Lưu ý**: Nếu bạn truyền ô vào thay vì mã chứng khoán, thì ở ô đó cần chứa mã chứng khoán. Trong trường hợp này mã chứng khoán không cần nằm giữa 2 dấu nháy đôi.&#x20;
{% endhint %}
