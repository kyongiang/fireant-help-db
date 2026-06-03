---
title: "FA.BalanceSheet.Cash"
source: "https://help.fireant.vn/fireant-for-excel/cac-ham-lay-thong-tin-tai-chinh/nhom-ham-fa.balancesheet/fa.balancesheet.cash"
---

# FA.BalanceSheet.Cash

## **Cú pháp**

```
=FA.BalanceSheet.Cash("Mã chứng khoán")
```

**Trong đó:**

* **Mã chứng khoán:** Mã chứng khoán của cổ phiếu cần lấy thông tin

## Giá trị trả về

Tiền mặt (quý gần nhất) của công ty tương ứng với mã chứng khoán

## **Ví dụ**

Bạn muốn biết công ty FPT có bao nhiều tiền mặt ở thời điểm cuối quý cuối cùng có bảng cân đối kế toán, bạn dùng công thức

```
=FA.BalanceSheet.Cash("FPT")
```

Hoặc gõ FPT ở một ô, chẳng hạn A1, và dùng công thức

```
=FA.BalanceSheet.Cash(A1)
```

Với cách thứ 2, bạn sẽ dễ dàng thay đổi mã chứng khoán mã không cần gõ lại công thức

**Kết quả**

2.671.613.358.430
