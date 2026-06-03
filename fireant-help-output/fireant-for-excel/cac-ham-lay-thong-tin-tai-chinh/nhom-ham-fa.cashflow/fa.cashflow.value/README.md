---
title: "FA.CashFlow\.Value"
source: "https://help.fireant.vn/fireant-for-excel/cac-ham-lay-thong-tin-tai-chinh/nhom-ham-fa.cashflow/fa.cashflow.value"
---

# FA.CashFlow\.Value

## Cú pháp

```
=FA.CashFlow.Value("Mã CK", Năm, Quý, "Tên chỉ tiêu")
```

**Trong đó:**

* **Mã CK**: Mã chứng khoán của cổ phiếu cần lấy thông tin&#x20;
* **Năm**: Năm của báo cáo muốn lấy dữ liệu&#x20;
* **Quý**: Quý của báo cáo muốn lấy dữ liệu. Đặt bằng 0 nếu muốn lấy trong báo cáo năm&#x20;
* **Tên chỉ tiêu**: Tên của chỉ tiêu muốn lấy dữ liệu

## Giá trị trả về <a href="#gia-tri-tra-ve" id="gia-tri-tra-ve"></a>

Giá trị một chỉ tiêu trong báo cáo lưu chuyển tiền tệ

Tên chỉ tiêu:

* CashflowFromOperatingActivities: Lưu chuyển tiền từ HĐKD;
* CashflowFromInvestingActivities: Lưu chuyển tiền từ HĐĐT;
* CashflowFromFinancingActivities: Lưu chuyển tiền từ HĐTC;
* DepreciationAndAmortization: Khấu hao.
