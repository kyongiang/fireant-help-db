---
title: "Lớp hàm FA.Company"
source: "https://help.fireant.vn/fireant-for-excel/cac-ham-lay-thong-tin-doanh-nghiep/nhom-ham-fa.company"
---

# Lớp hàm FA.Company

## **Mô tả**

Các hàm thuộc nhóm này cho phép lấy 3 loại thông tin về sơ doanh nghiệp

* **Thông tin định dạng doanh nghiệp**: tên, địa chỉ, email, năm thành lập, số nhân viên, số chi nhánh, loại hình DN, ...
* **Thông tin mô tả doanh nghiệp**: mô tả tổng quan, lịch sử phát triển, ngành nghề kinh doanh, tỷ lệ sở hữu các nhóm chính
* **Thông tin hồ sơ doanh nghiệp**: danh sách ban lãnh đạo, danh sách cổ đông chính, danh sách các giao dịch của cổ đông nội bộ"                                                                           &#x20;

## Nhóm hàm lấy thông tin định dạng doanh nghiệp

### **Cú pháp**&#x20;

```
=FA.Company.[Trường thông tin]("Mã CK")
```

**Trong đó**:&#x20;

* **Mã CK:** là mã cổ phiếu niêm yết&#x20;
* **Trường thông tin:** tên tương ứng với một thông tin định dạng nhất định của mã chứng khoán"

**Ví dụ:**

Để lấy ngày niêm yết của mã FPT ta dùng công thức:&#x20;

```
=FA.Company.DateOfIssue("FPT")
```

## Nhóm hàm lấy thông tin mô tả doanh nghiệp

**Cú pháp:**

Biểu thức lấy thông tin mô tả doanh nghiệp có cấu trúc giống biểu thức lấy thông tin định dạng doanh nghiệp, tuy nhiên dữ liệu trả về phức tạp hơn và cần biến đổi định dạng trước khi có thể hiển thị.

* **Hàm lấy thông tin mô tả tổng quan**, **thông tin lịch sử phát triển và thông tin ngành nghề kinh doanh** trả về mô tả bằng tiếng việt viết liền, không phân đoạn
* **Các hàm lấy thông tin tỷ lệ sở hữu các nhóm** (nhà nước, nước ngoài, sở hữu khác) trả về giá trị số thay vì phần trăm.

## Nhóm hàm lấy thông tin hồ sơ doanh nghiệp

**Cú pháp:**

Biểu thức lấy danh sách ban lãnh đạo như sau:&#x20;

```
=FA.Company.Officers("Mã CK") 
```

Biểu thức lấy danh sách cổ đông chính như sau:

```
=FA.Company.MajorHolders("Mã CK") 
```

Biểu thức lấy danh sách giao dịch nội bộ:&#x20;

```
=FA.Company.InsiderTransactions("Mã CK", "Ngày bắt đầu", "Ngày kết thúc") 
```

**Trong đó:**

* **Mã CK**: Là mã cổ phiếu niêm yết
* **Trường thông tin:** là tên trường tương ứng với một thông tin nhất định về giao dịch cổ phiếu trong quá khứ
* **Ngày đầu tiên, Ngày cuối cùng**: là khoảng thời gian bạn muốn xem thông tin. Hai ngày này không nhất thiết phải là ngày có giao dịch. Định dạng như sau: "YYYY-MM-DD"

**Ví dụ:**

Để lấy danh sách các giao dịch nội bộ của FPT trong khoảng thời gian từ 1/6/2016 đến 30/9/2016 ta sử dụng công thức:&#x20;

```
=FA.Company.InsiderTransactions("FPT", "2016-06-01", "2016-09-30")
```
