---
title: "Lớp hàm FA.BalanceSheet"
source: "https://help.fireant.vn/fireant-for-excel/cac-ham-lay-thong-tin-tai-chinh/nhom-ham-fa.balancesheet"
---

# Lớp hàm FA.BalanceSheet

## **Mô tả**

Các hàm thuộc nhóm này cho phép lấy 4 loại thông tin từ bảng CĐKT:

* **Thông tin về bảng CĐKT mới nhất:** Quý/Năm có bảng CĐKT mới nhất (Year/Quarter), năm tài chính cuối có bảng CĐKT năm (LFY)
* **Chỉ tiêu tổng hợp mới nhất**: Một số hạng mục từ bảng CĐKT quý cuối  hoặc năm gần nhất
* **Các chỉ tiêu chính**: Các hạng mục chính trong bảng CĐKT của các năm hoặc quý đã nộp báo cáo&#x20;
* **Toàn bộ Bảng CĐKT**: Bảng CĐKT của các năm hoặc quý đã nộp báo cáo                                                                         &#x20;

## Nhóm hàm lấy thông tin về bảng cân đối kế toán mới nhất&#x20;

### **Cú pháp**                                                                           &#x20;

Biểu thức lấy năm của bảng CĐKT mới nhất của mã chứng khoán:

```
=FA.BalanceSheet.Year("Mã CK")
```

Biểu thức lấy quý của bảng CĐKT mới nhất của mã chứng khoán:&#x20;

```
=FA.BalanceSheet.Quarter("Mã CK")
```

Biểu thức lấy năm tài chính cuối có bảng CĐKT của mã chứng khoán:&#x20;

```
=FA.BalanceSheet.LFY("Mã CK")
```

**Trong đó:**

* **Mã CK:** là mã cổ phiếu niêm yết"                                                                           &#x20;

## Nhóm hàm lấy các chỉ tiêu tổng hợp mới nhất từ bảng cân đối kế toán

### **Cú pháp**

Biểu thức lấy một chỉ tiêu tổng hợp mới nhất từ bảng CĐK&#x54;**:**&#x20;

```
=FA.BalanceSheet.[Chỉ tiêu bảng CĐKT]("Mã CK") 
```

**Trong đó:**

* **Mã CK:** là mã cổ phiếu niêm yết&#x20;
* **Chỉ tiêu bảng CĐKT:** là một chỉ tiêu tương ứng trong bảng CĐKT

### **Ví dụ**

Để lấy tổng tài sản ngắn hạn quý gần nhất (hoặc năm gần nhất, tùy vào việc báo cáo quý cuối và báo cáo năm cuối báo cáo nào mới hơn) của mã FPT ta dùng công thức:&#x20;

```
=FA.BalanceSheet.CurrentAssets("FPT")
```

## Hàm lấy chỉ tiêu từ bảng **CĐKT** của năm hoặc quý đã nộp báo cáo

### **Cú pháp**

Biểu thức lấy một chỉ tiêu chính từ một bảng CĐKT:&#x20;

```
=FA.BalanceSheet.Value("Mã CK",Năm, Quý, "Chỉ tiêu bảng CĐKT") 
```

**Trong đó:**

* **Mã CK**: là mã cổ phiếu niêm yết&#x20;
* **Năm:** là năm tương ứng với bảng CĐKT&#x20;
* **Quý:** là quý tương ứng với bảng CĐKT. Nếu Quý bằng 0 thì bảng CĐKT là bảng CĐKT năm&#x20;
* **Chỉ tiêu bảng CĐKT:** là một chỉ tiêu tương ứng trong bảng CĐKT.&#x20;

Các chỉ tiêu chính được sử dụng để tính toán các chỉ số tài chính, các chỉ tiêu còn lại chỉ có ý nghĩa thuyết minh và không được sử dụng trong các tính toán. Bên cạnh các chỉ tiêu có sẵn trong bảng CĐKT, chúng tôi cũng tổ hợp 1 số chỉ tiêu không có sẵn trong các báo cáo tài chính theo chuẩn VAS, nhưng có trong các báo cáo tài chính theo chuẩn IAS, như nợ phải trả lãi, tài sản sinh lãi, ...&#x20;

{% hint style="info" %}
**Lưu ý**: do các loại hình doanh nghiệp khác nhau, nên có 1 số chỉ tiêu chỉ có ở loại hình doanh nghiệp này, mà không có ở các loại hình doanh nghiệp khác.
{% endhint %}

### **Ví dụ**

Để lấy tiền mặt quý 3 năm 2016 của mã FPT ta dùng công thức:&#x20;

```
=FA.BalanceSheet.Value("FPT", 2016, 3, "Cash")
```

## Hàm lấy toàn bộ bảng cân đối kế toán

### **Cú pháp**

Biểu thức lấy toàn bộ một hay nhiều bảng CĐKT:&#x20;

```
=FA.IncomeStatement.Reports("Mã CK", Năm, Quý, [Số lượng bảng CĐKT], [Đơn vị tiền]) 
```

**Trong đó:**

* **Mã CK:** là mã cổ phiếu niêm yết&#x20;
* **Năm:** là năm tương ứng với bảng CĐKT Quý: là quý tương ứng với báo cáo. Nếu Quý bằng 0 thì bảng CĐKT là bảng CĐKT năm&#x20;
* **Số lượng bảng CĐKT:** là số bảng CĐKT muốn lấy ra tính từ bảng CĐKT ứng với các tham số Năm và Quý.&#x20;
* **Đơn vị tiền:** là đơn vị tiền (tính bằng VNĐ) mà bạn muốn sử dụng cho kết quả. Mặc dù đơn vị tiền có thể là số bất kỳ, nhưng các số có ý nghĩa là 1, 1.000, 1.000.000, hoặc tỷ giá hối đoái của đồng ngoại tệ mà bạn muốn quy đổi.

### **Ví dụ**

Để lấy 4 bảng CĐKT theo quý, tính từ quý 2/2021 trở về trước của mã FPT, với đơn vị tiền là triệu đồng, ta dùng công thức:&#x20;

```
=FA.BalanceSheet.Reports("FPT", 2021, 2, 4, 1000000)
```
