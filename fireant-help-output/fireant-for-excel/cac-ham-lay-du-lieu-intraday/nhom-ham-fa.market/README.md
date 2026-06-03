---
title: "Lớp hàm FA.Market"
source: "https://help.fireant.vn/fireant-for-excel/cac-ham-lay-du-lieu-intraday/nhom-ham-fa.market"
---

# Lớp hàm FA.Market

## **Cú pháp**

```
=FA.Market.[Trường thông tin]("Mã Index hoặc Mã sàn")
```

**Trong đó:**

* Mã Index: là tên Index tương ứng, ví dụ: VNINDEX, HNXINDEX, UPINDEX, VN30, HNX30, …&#x20;
* Mã sàn: là tên sàn giao dịch chứng khoán nơi mã cổ phiếu được niêm yết. Mã sàn có thể nhận các giá trị sau: ""HSX"", ""HNX"", ""UPCOM""&#x20;
* Trường thông tin: là tên trường tương ứng với một thông tin nhất định về Index hoặc thị trường phiên hiện tại"

{% hint style="info" %}
**Lưu ý**: Giá trị giao dịch của nhà đầu tư nước ngoài trên sàn HSX được cập nhật trong phiên là giá trị ước tính.
{% endhint %}

## **Ví dụ**

Muốn xem giá trị hiện tại của VNINDEX ta dùng công thức:&#x20;

```
=FA.Market.IndexCurrent(""VNINDEX"") 
```

Muốn xem tổng giá trị giao dịch nước ngoài bán trên sàn HSX đến thời điểm hiện tại ta dùng công thức:&#x20;

```
=FA.Market.BuyForeignValue("HSX")
```
