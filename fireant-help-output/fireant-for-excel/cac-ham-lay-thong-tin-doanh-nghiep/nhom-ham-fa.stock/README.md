---
title: "Lớp hàm FA.Stock"
source: "https://help.fireant.vn/fireant-for-excel/cac-ham-lay-thong-tin-doanh-nghiep/nhom-ham-fa.stock"
---

# Lớp hàm FA.Stock

Các hàm thuộc lớp này chia làm hai loại, nhóm hàm lấy giá trị đơn, và nhóm hàm lấy giá trị dạng bảng.

Các hàm thống kê giao dịch, và các hàm lấy thông tin mã chứng khoán (trừ thông tin cổ tức), trả về giá trị đơn.&#x20;

Các hàm lấy toàn bộ danh sách mã chứng khoán, lấy danh sách mã chứng khoán theo sàn hoặc theo ngành, cũng như thông tin cổ tức trả về giá trị dạng bảng.

## Nhóm hàm trả về giá trị đơn

**Mô tả:**

Tập hợp các hàm thống kê giao dịch của mã cổ phiếu trong quá khứ tính đến phiên đã kết thúc giao dịch cuối cùng, và các hàm lấy thông tin mã chứng khoán (số CP tự do, số CP lưu hành, tên doanh nghiệp, …)

**Cú pháp**:&#x20;

Biểu thức lấy dữ liệu đơn có dạng:&#x20;

```
=FA.Stock.[Trường thông tin](""Mã CK"")"
```

**Trong đó:**

* **Mã CK:** là mã chứng khoán niêm yết&#x20;
* **Trường thông tin**: là tên trường tương ứng với một thống kê giao dịch của cổ phiếu hoặc thông tin nhất định về cổ phiếu

**Ví dụ:**

Nếu muốn lấy KLGD trung bình 20 ngày gần nhất (từ 8h sáng ngày hôm sau sẽ bao gồm phiên hiện tại) của mã ACB, ta dùng công thức:&#x20;

```
=FA.Stock.AvgVolume20d("ACB")
```

## **Nhóm hàm trả về giá trị dạng bảng**

**Mô tả:**

Bao gồm các hàm lấy danh sách toàn bộ cổ phiếu, danh sách cổ phiếu của một sàn, danh sách cổ phiếu của một ngành và hàm lấy thông tin cổ tức và các chỉ số cổ tức qua các năm

**Cú pháp:**&#x20;

Biểu thức lấy danh sách toàn bộ các mã cổ phiếu:&#x20;

```
=FA.Stock.AllStockSymbols()
```

Biểu thức lấy danh sách các mã cổ phiếu của 1 sàn:&#x20;

```
=FA.Stock.StockSymbolsByExchange("Mã sàn")
```

Trong đó:&#x20;

* **Mã sàn**: là tên sàn giao dịch chứng khoán nơi mã cổ phiếu được niêm yết. Mã sàn có thể nhận các giá trị sau: "HSX", "HNX", "UPCOM"

Biểu thức lấy danh sách các mã cổ phiếu của một ngành:&#x20;

```
=FA.Stock.StockSymbolsByIndustry("Mã ngành ICB")
```

**Trong đó:**&#x20;

* **Mã ngành ICB:** là mã của ngành tương ứng theo chuẩn ICB (chi tiết xem ở mục mô tả lớp hàm cho thông tin ngành - FA.Industry)

Biểu thức lấy thông tin cổ tức và các chỉ số về cổ tức qua các năm:&#x20;

```
=FA.Stock.DividendHistory("Mã CK")
```

**Trong đó:**&#x20;

* **Mã CK**: là mã chứng khoán niêm yết
