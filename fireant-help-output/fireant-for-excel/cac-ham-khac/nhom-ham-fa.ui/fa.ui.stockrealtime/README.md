---
title: "FA.UI.StockRealtime"
source: "https://help.fireant.vn/fireant-for-excel/cac-ham-khac/nhom-ham-fa.ui/fa.ui.stockrealtime"
---

# FA.UI.StockRealtime

## **Cú pháp**

```
FA.UI.StockRealtime("Mã CK", ["Tiêu đề"])
```

**Trong đó:**

* **Mã CK**: Mã chứng khoán của cổ phiếu cần xem thông tin
* **Tiêu đề:** Tiêu đề của liên kết dùng để mở biểu đồ. Nếu không truyền tham số này thì hàm sẽ dùng giá trị mặc định là "**Realtime**"

Các tham số không nhất thiết phải nhập trực tiếp, bạn có thể tham chiếu đến các ô chứa thông tin tương ứng.

## Giá trị trả về

Giá trị trả về là một liên kết. Khi bấm vào liên kết này, Các thống kê thời gian thực về giao dịch (tổng quan giao dịch, thống kê khớp lệnh, giao dịch của nhà đầu tư nước ngoài) của mã chứng khoán tương ứng sẽ được nạp vào một cửa sổ mới.
