---
title: "Lớp hàm FA.Historical"
source: "https://help.fireant.vn/fireant-for-excel/cac-ham-lay-du-lieu-giao-dich-qua-khu/nhom-ham-fa.historical"
---

# Lớp hàm FA.Historical

## **Cú pháp**

Biểu thức lấy thông tin giao dịch cổ phiếu quá khứ có dạng như sau:&#x20;

```
=FA.Historical.[Trường thông tin]("Mã CK", "Ngày đầu tiên", "Ngày cuối cùng")
```

**Trong đó:**

* **Mã CK**: Là mã cổ phiếu niêm yết hoặc Index(VNINDEX, HNXINDEX,UPINDEX, VN30, HNX30,…)
* **Trường thông tin:** là tên trường tương ứng với một thông tin nhất định về giao dịch cổ phiếu trong quá khứ
* **Ngày đầu tiên, Ngày cuối cùng**: là khoảng thời gian bạn muốn xem thông tin. Hai ngày này không nhất thiết phải là ngày có giao dịch. Định dạng như sau: "YYYY-MM-DD"

**Ví dụ:**

Nếu muốn lấy giá đóng cửa các phiên giao dịch từ ngày 15-06-2016 đến ngày 22-06-2016 của mã ACB, ta dùng công thức:&#x20;

```
=FA.Historical.Close("ACB","2016-06-15","2016-06-22") 
```

Và để biết các ngày đó là ngày nào, ta dùng công thức:&#x20;

```
=FA.Historical.Date("ACB","2016-06-15","2016-06-22") 
```

Khoảng thời gian trong hai công thức phải giống nhau, và công thức cần nhập vào 2 ô thuộc 2 cột khác nhau nhưng cùng trên 1 dòng.

{% hint style="info" %}
**Lưu ý:** Bạn có thể lưu các tham số vào các ô rồi truyền vào các công thức. Trong trường hợp này bạn cần bảo đảm tham số **Ngày đầu tiên** và **Ngày cuối cùng** là Text và có định dạng YYYY-MM-DD. Bạn có thể dùng hàm Text của Excel để chuyển dữ liệu thời gian thành Text với định dạng mong muốn.
{% endhint %}
