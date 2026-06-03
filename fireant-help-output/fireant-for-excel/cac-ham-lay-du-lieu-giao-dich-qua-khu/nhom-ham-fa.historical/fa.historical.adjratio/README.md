---
title: "FA.Historical.AdjRatio"
source: "https://help.fireant.vn/fireant-for-excel/cac-ham-lay-du-lieu-giao-dich-qua-khu/nhom-ham-fa.historical/fa.historical.adjratio"
---

# FA.Historical.AdjRatio

## Cú pháp

```
=FA.Historical.AdjRatio("Mã CK", "Ngày bắt đầu", "Ngày kết thúc")
```

**Trong đó**:

* **Mã CK:** Mã chứng khoán cần lấy thông tin hoặc index (VNINDEX, HNXINDEX, UPINDEX, VN30, HNX30,...)&#x20;
* **Ngày bắt đầu**: Ngày bắt đầu lấy dữ liệu, định dạng "yyyy-MM-dd"
* **Ngày kết thúc:** Ngày kết thúc lấy dữ liệu, định dạng "yyyy-MM-dd"

## Giá trị trả về

Một cột các giá trị trong đó mỗi ô là hệ số điều chỉnh giá ứng với 1 ngày giao dịch trong khoảng thời gian từ **Ngày bắt đầu** đến **Ngày kết thúc**

{% hint style="info" %}
**Lưu ý:** Hệ số điều chỉnh của các index luôn có giá trị là 1
{% endhint %}
