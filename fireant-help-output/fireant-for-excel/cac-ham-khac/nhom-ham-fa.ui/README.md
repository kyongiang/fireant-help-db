---
title: "Lớp hàm FA.UI"
source: "https://help.fireant.vn/fireant-for-excel/cac-ham-khac/nhom-ham-fa.ui"
---

# Lớp hàm FA.UI

## **Mô tả**

Tập hợp các hàm lấy về đường dẫn tới các giao diện đồ họa dựng sẵn tương ứng với một mã cổ phiếu. Có cả thảy 4 giao diện:

* Giao diện đồ thị Intraday: cho phép xem đồ thị diễn biến giá trong phiên
* Giao diện phân tích kỹ thuật: cho phép xem đồ thị phân tích kỹ thuật
* Giao diện thống kê giao dịch: cho phép xem các thống kê giao dịch thời gian thực
* Giao diện thông tin doanh nghiệp: cho phép xem trực quan các thông tin hồ sơ doanh nghiệp"                                           &#x20;

## **Cú pháp**

Để lấy đường dẫn tới một giao diện đồ họa dựng sẵn tương ứng với một mã cổ phiếu, nhập công thức theo dạng sau vào một ô mà bạn dự định hiện thị kết quả:&#x20;

```
=FA.UI.[Trường thông tin]("Mã CK", [Tiêu đề])
```

**Trong đó**:

* Mã CK: là mã của chứng khoán niêm yết
* Trường thông tin: là tên trường tương ứng với một loại giao diện đồ họa.
* Tiêu đề: tiêu đề cho đường dẫn đến giao diện đồ họa. Trường này có thể bỏ trống, khi đó tiêu đề mặc định sẽ được sử dụng.

## **Ví dụ**

Nếu muốn lấy đường dẫn đến giao diện đồ thị Intraday của mã AAA, ta sử dụng công thức:&#x20;

```
=FA.UI.IntradayChart("AAA","Đồ thị Intraday mã AAA")
```
