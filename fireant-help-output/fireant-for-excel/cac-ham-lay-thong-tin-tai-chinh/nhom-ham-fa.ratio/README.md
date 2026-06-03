---
title: "Lớp hàm FA.Ratio"
source: "https://help.fireant.vn/fireant-for-excel/cac-ham-lay-thong-tin-tai-chinh/nhom-ham-fa.ratio"
---

# Lớp hàm FA.Ratio

**Mô tả:**

Các hàm lấy chỉ số tài chính trả về giá trị mới nhất (MRQ hoặc TTM tùy vào tính chất chỉ số) của các chỉ số tài chính ứng với mỗi mã chứng khoán, trong đó các chỉ số tài chính được tính dựa trên các báo cáo tài chính và các thông tin doanh nghiệp mới nhất.

**Cú pháp:**

Để lấy giá trị một chỉ số tài chính doanh nghiệp ta dùng công thức sau:&#x20;

**=FA.Ratio**.\[Chỉ số]\("Mã CK")

**Trong đó**:

* Mã CK: là mã của chứng khoán niêm yết
* Chỉ số: là tên tương ứng với một chỉ số tài chính doanh nghiệp.

**Ví dụ:**

"Để lấy biên lợi nhuận gộp mới nhất (TTM) của FPT ta dùng công thức:&#x20;

\=FA.Ratio.GrossMargin("FPT")
