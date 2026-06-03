---
title: "FA.Historical.Basic"
source: "https://help.fireant.vn/fireant-for-excel/cac-ham-lay-du-lieu-giao-dich-qua-khu/nhom-ham-fa.historical/fa.historical.basic"
---

# FA.Historical.Basic

## Cú pháp

```
=FA.Historical.Basic("Mã CK", "Ngày bắt đầu", "Ngày kết thúc")
```

**Trong đó**:

* **Mã CK:** Mã chứng khoán cần lấy thông tin hoặc index (VNINDEX, HNXINDEX, UPINDEX, VN30, HNX30,...)&#x20;
* **Ngày bắt đầu**: Ngày bắt đầu lấy dữ liệu, định dạng "yyyy-MM-dd"
* **Ngày kết thúc:** Ngày kết thúc lấy dữ liệu, định dạng "yyyy-MM-dd"

## Giá trị trả về

Object Một chuỗi các giá trị trong đó mỗi phần tử là giá tham chiếu ứng với 1 ngày giao dịch trong khoảng thời gian
