---
title: "Lớp hàm FA.IncomeStatement"
source: "https://help.fireant.vn/fireant-for-excel/cac-ham-lay-thong-tin-tai-chinh/nhom-ham-fa.incomestatement"
---

# Lớp hàm FA.IncomeStatement

**Mô tả**\
Các hàm thuộc nhóm này cho phép lấy 4 loại thông tin từ báo cáo KQKD:

* Thông tin về báo cáo KQKD mới nhất: Quý/Năm có báo cáo KQKD mới nhất (Year/Quarter), năm tài chính cuối có báo cáo KQKD năm (LFY)
* Một số chỉ tiêu tổng hợp từ 4 quý cuối hoặc lấy từ báo cáo KQKD năm gần nhất
* Các chỉ tiêu chính trong báo cáo KQKD của các năm hoặc quý đã nộp báo cáo&#x20;
* Toàn bộ báo cáo KQKD của các năm hoặc quý đã nộp báo cáo "                                                                           &#x20;

## **Các hàm lấy thông tin về Báo cáo kết quả kinh doanh mới nhất**

**Cú pháp**

*=FA.IncomeStatement.\[Thông tin báo cáo KQKD]\(""Mã CK"")*

Trong đó:

* **Mã CK**: Là mã cổ phiếu niêm yết                                                                          &#x20;
* **Thông tin báo cáo KQKD:** Có 3 thông tin có thể lấy là Năm của báo cáo KQKD mới nhất [*FA.IncomeStatement.Year*](https://app.gitbook.com/@fireant/s/fireant-for-excel/~/drafts/-MfktyuhD7TbjhAP8ZZN/cac-ham-lay-thong-tin-tai-chinh/nhom-ham-fa.incomestatement/fa.incomestatement.year)*,* Quý của báo cáo KQKD mới nhất [*FA.IncomeStatement.Quarter*](https://app.gitbook.com/@fireant/s/fireant-for-excel/~/drafts/-MfktyuhD7TbjhAP8ZZN/cac-ham-lay-thong-tin-tai-chinh/nhom-ham-fa.incomestatement/fa.incomestatement.quarter)*,* và Năm tài chính cuối có báo cáo KQKD [*FA.IncomeStatement.LFY*](https://app.gitbook.com/@fireant/s/fireant-for-excel/~/drafts/-MfktyuhD7TbjhAP8ZZN/cac-ham-lay-thong-tin-tai-chinh/nhom-ham-fa.incomestatement/fa.incomestatement.lfy)

## **Các hàm lấy các chỉ tiêu tổng hợp mới nhất từ báo cáo KQKD**

**Cú pháp**

\=FA.IncomeStatement.\[Chỉ tiêu báo cáo KQKD]\(""Mã CK"")&#x20;

**Trong đó**

* **Mã CK**: Là mã cổ phiếu niêm yết
* **Chỉ tiêu báo cáo KQKD**: Là một chỉ tiêu tương ứng trong báo cáo KQKD. Các chỉ tiêu có thể là
  * [NetSales](https://app.gitbook.com/@fireant/s/fireant-for-excel/~/drafts/-MfktyuhD7TbjhAP8ZZN/cac-ham-lay-thong-tin-tai-chinh/nhom-ham-fa.incomestatement/fa.incomestatement.netsales)
  * [OtherProfit](https://app.gitbook.com/@fireant/s/fireant-for-excel/~/drafts/-MfktyuhD7TbjhAP8ZZN/cac-ham-lay-thong-tin-tai-chinh/nhom-ham-fa.incomestatement/fa.incomestatement.otherprofit)
  * [ProfitAfterIncomeTaxes](https://app.gitbook.com/@fireant/s/fireant-for-excel/~/drafts/-MfktyuhD7TbjhAP8ZZN/cac-ham-lay-thong-tin-tai-chinh/nhom-ham-fa.incomestatement/fa.incomestatement.profitafterincometaxes)
  * [ProfitBeforeIncomeTaxes](https://app.gitbook.com/@fireant/s/fireant-for-excel/~/drafts/-MfktyuhD7TbjhAP8ZZN/cac-ham-lay-thong-tin-tai-chinh/nhom-ham-fa.incomestatement/fa.incomestatement.profitbeforeincometaxes)
  * [ProfitFromFinancialActivities](https://app.gitbook.com/@fireant/s/fireant-for-excel/~/drafts/-MfktyuhD7TbjhAP8ZZN/cac-ham-lay-thong-tin-tai-chinh/nhom-ham-fa.incomestatement/fa.incomestatement.profitfromfinancialactivities)

## **Hàm lấy các chỉ tiêu chính từ báo cáo kết quả kinh doanh của năm hoặc quý đã nộp báo cáo**

**Cú pháp**

\=FA.IncomeStatement.Value(""Mã CK"",Năm, Quý, ""Chỉ tiêu báo cáo KQKD"")&#x20;

Trong đó

* **Mã CK**: Là mã cổ phiếu niêm yết
* **Năm**: Là năm tương ứng với báo cáo KQKD&#x20;
* **Quý**: Là quý tương ứng với báo cáo KQKD. Nếu Quý bằng 0 thì báo cáo là báo cáo KQKD năm&#x20;
* **Chỉ tiêu báo cáo KQKD**: Là một chỉ tiêu tương ứng trong báo cáo KQKD. Các chỉ tiêu chính được sử dụng để tính toán các chỉ số tài chính, trong khi đó các chỉ tiêu còn lại chỉ có ý nghĩa thuyết minh và không được sử dụng trong các tính toán. Bên cạnh các chỉ tiêu có sẵn trong báo cáo KQKD, chúng tôi cũng tổ hợp 1 số chỉ tiêu không có sẵn trong các báo cáo tài chính theo chuẩn VAS, nhưng có trong các báo cáo tài chính theo chuẩn IAS, như EBIT, EBITDA, Depreciation, Amortization, ...&#x20;

**Lưu ý**: do các loại hình doanh nghiệp khác nhau, nên có 1 số chỉ tiêu chỉ có ở loại hình doanh nghiệp này, mà không có ở các loại hình doanh nghiệp khác.

Các chỉ tiêu chính gồm có

* TotalRevenues: Tổng doanh thu
* NetSales: Doanh thu thuần
* CostOfGoodSold: Giá vốn hàng bán

**Ví dụ:**

Để lấy doanh thu thuần quý 3 năm 2016 của mã FPT ta dùng công thức:&#x20;

**=**&#x46;A.IncomeStatement.Value(""FPT"", 2016, 3, ""NetSales"")"

**Hàm lấy toàn bộ báo cáo kết quả kinh doanh**

**Cú pháp:**

Biểu thức lấy toàn bộ một hay nhiều báo cáo KQKD:&#x20;

\=FA.IncomeStatement.Reports(""Mã CK"",Năm, Quý, \[Số lượng báo cáo KQKD], \[Đơn vị tiền])&#x20;

**Trong đó:**

* **Mã CK**: là mã cổ phiếu niêm yết&#x20;
* **Năm:** là năm tương ứng với báo cáo KQKD.&#x20;
* **Quý:** là quý tương ứng với báo cáo KQKD. Nếu Quý bằng 0 thì báo cáo là báo cáo KQKD năm&#x20;
* **Số lượng báo cáo KQKD:** là số báo cáo KQKD muốn lấy ra tính từ báo cáo KQKD ứng với các tham số Năm và Quý.&#x20;
* **Đơn vị tiền**: là đơn vị tiền (tính bằng VNĐ) mà bạn muốn sử dụng cho kết quả. Mặc dù đơn vị tiền có thể là số bất kỳ, nhưng các số có ý nghĩa là 1, 1.000, 1.000.000, hoặc tỷ giá hối đoái của đồng ngoại tệ mà bạn muốn quy đổi.
