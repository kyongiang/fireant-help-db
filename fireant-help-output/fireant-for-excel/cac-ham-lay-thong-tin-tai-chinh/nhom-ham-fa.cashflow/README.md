---
title: "Lớp hàm FA.CashFlow"
source: "https://help.fireant.vn/fireant-for-excel/cac-ham-lay-thong-tin-tai-chinh/nhom-ham-fa.cashflow"
---

# Lớp hàm FA.CashFlow

**Mô tả:**

Các hàm thuộc nhóm này cho phép lấy 4 loại thông tin từ báo cáo LCTT:

* Thông tin về báo cáo LCTT mới nhất: Quý/Năm có báo cáo LCTT mới nhất (Year/Quarter), năm tài chính cuối có báo cáo LCTT năm (LFY)
* Một số hạng mục từ báo cáo LCTT quý cuối hoặc năm gần nhất
* Các hạng mục chính trong báo cáo LCTT của các năm hoặc quý đã nộp báo cáo&#x20;
* Toàn bộ báo cáo LCTT của các năm hoặc quý đã nộp báo cáo       &#x20;

Nhóm hàm lấy yhoong tin về báo cáo lưu chuyển tiền tệ mới nhất

**Cú pháp:**

Biểu thức lấy năm của báo cáo LCTT mới nhất của mã chứng khoán:

\=FA.CashFlow\.Year(""Mã CK"")

Mã CK: là mã cổ phiếu niêm yết"                                                                           &#x20;

Biểu thức lấy quý của báo cáo LCTT mới nhất của mã chứng khoán:&#x20;

\=FA.CashFlow\.Quarter(""Mã CK"")&#x20;

Mã CK: là mã cổ phiếu niêm yết"

Biểu thức lấy năm tài chính cuối có báo cáo LCTT của mã chứng khoán:&#x20;

\=FA.CashFlow\.LFY(""Mã CK"")&#x20;

Mã CK: là mã cổ phiếu niêm yết"

NHÓM HÀM LẤY CÁC CHỈ TIÊU TỔNG HỢP MỚI NHẤT TỪ BÁO CÁO LCTT

**Cú pháp:**

Biểu thức lấy một chỉ tiêu tổng hợp mới nhất từ báo cáo LCTT:&#x20;

\=FA.CashFlow.\[Chỉ tiêu báo cáo LCTT]\(""Mã CK"")&#x20;

**Trong đó:**

* Mã CK: là mã cổ phiếu niêm yết&#x20;
* Chỉ tiêu báo cáo LCTT: là một chỉ tiêu tương ứng trong báo cáo LCTT"

Ví dụ:

"Để lấy quý gần nhất có báo cáo LCTT của mã FPT ta dùng công thức:&#x20;

\=FA.CashFlow\.Quarter(""FPT"")"

## **Hàm lấy các chỉ tiêu chính từ báo cáo lưu chuyển tiền tệ của năm hoặc quý đã nộp báo cáo**

**Cú pháp:**

Biểu thức lấy một chỉ tiêu chính từ một báo cáo KQKD:&#x20;

\=FA.CashFlow\.Value(""Mã CK"",Năm, Quý, ""Chỉ tiêu báo cáo LCTT"")&#x20;

**Trong đó:**

* Mã CK: là mã cổ phiếu niêm yết&#x20;
* Năm: là năm tương ứng với báo cáo LCTT&#x20;
* Quý: là quý tương ứng với báo cáo LCTT. Nếu Quý bằng 0 thì báo cáo là báo cáo LCTT năm&#x20;
* Chỉ tiêu báo cáo LCTT: là một chỉ tiêu tương ứng trong báo cáo LCTT. Các chỉ tiêu chính được sử dụng để tính toán các chỉ số tài chính, các chỉ tiêu còn lại chỉ có ý nghĩa thuyết minh và không được sử dụng trong các tính toán.&#x20;

Ví dụ:

Để lấy Lưu chuyển tiền thuần từ hoạt động kinh doanh quý 3 năm 2016 của mã FPT ta dùng công thức:&#x20;

**=**&#x46;A.CashFlow\.Value(""FPT"", 2016, 3, ""CashflowFromOperatingActivities"")

## Hàm lấy toàn bộ báo cáo lưu chuyển tiền tệ

**Cú pháp:**

Biểu thức lấy toàn bộ một hay nhiều báo cáo LCTT:&#x20;

\=FA.IncomeStatement.Reports(""Mã CK"",Năm, Quý, \[Số lượng báo cáo LCTT], \[Đơn vị tiền])&#x20;

**Trong đó:**

* Mã CK: là mã cổ phiếu niêm yết&#x20;
* Năm: là năm tương ứng với báo cáo LCTT&#x20;
* Quý: là quý tương ứng với báo cáo LCTT. Nếu Quý bằng 0 thì báo cáo là báo cáo LCTT năm&#x20;
* Số lượng báo cáo LCTT: là số báo cáo LCTT muốn lấy ra tính từ báo cáo LCTT ứng với các tham số Năm và Quý.&#x20;
* Đơn vị tiền: là đơn vị tiền (tính bằng VNĐ) mà bạn muốn sử dụng cho kết quả. Mặc dù đơn vị tiền có thể là số bất kỳ, nhưng các số có ý nghĩa là 1, 1.000, 1.000.000, hoặc tỷ giá hối đoái của đồng ngoại tệ mà bạn muốn quy đổi."

Ví dụ:

Để lấy 4 báo cáo LCTT theo quý, tính từ quý 3/2016 trở về trước của mã FPT, với đơn vị tiền là triệu đồng, ta dùng công thức:&#x20;

\=FA.CashFlow\.Reports(""FPT"", 2016, 3, 4, 1000000)"
