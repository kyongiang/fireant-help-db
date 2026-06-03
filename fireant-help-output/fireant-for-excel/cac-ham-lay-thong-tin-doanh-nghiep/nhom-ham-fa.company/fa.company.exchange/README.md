---
title: "FA.Company.Exchange"
source: "https://help.fireant.vn/fireant-for-excel/cac-ham-lay-thong-tin-doanh-nghiep/nhom-ham-fa.company/fa.company.exchange"
---

# FA.Company.Exchange

## **Cú pháp**

```
=FA.Company.Exchange("Mã CK")
```

**Trong đó**:

* **Mã CK**: Mã chứng khoán của cổ phiếu cần lấy thông tin. Tham số **Mã CK** nếu đưa trực tiếp vào hàm phải nằm giữa hai dấu nháy đôi. Hoặc bạn có thể ghi mã chứng khoán ở 1 ô rồi truyền ô đó vào thành tham số.

## Giá trị trả về

Sàn niêm yết cổ phiếu

## **Ví dụ**

```
=FA.Company.Exchange("FPT")
```

Sẽ trả về HSX

Bạn cũng có thể ghi mã FPT vào ô A1 và gọi công thức như sau:

```
=FA.Company.Exchange(A1)
```

Cách truyền tham số giá tiếp cho phép bạn thay đổi mã chứng khoán mà không cần sửa ở công thức. Ví dụ bạn thay SHB vào ô A1, khi đó hàm trên sẽ trả về HNX
