---
title: "FA.Intraday.Side"
source: "https://help.fireant.vn/fireant-for-excel/cac-ham-lay-du-lieu-intraday/nhom-ham-fa.intraday/untitled"
---

# FA.Intraday.Side

Nếu phía chủ động là bên mua hàm này sẽ trả về B, ngược lại nếu phía chủ động là bên bán, hàm sẽ trả về S, nếu cả bên đồng thời đưa lệnh vào khớp và không thể phân biệt thứ tự trước sau, hàm sẽ trả về null. khối lượng mua bán chủ động sẽ được chia đều cho 2 phía

**Cú pháp:**

```
=FA.Intraday.Side("Mã CK hoặc Mã Index","Lần khớp")
```

Hàm FA.Intraday.Side có các tham số sau :

* **Mã chứng khoán:** Mã chứng khoán của cổ phiếu cần lấy thông tin&#x20;
* **Lần khớp**: Thứ tự lần khớp (1, 2,... tương ứng với lần khớp gần nhất, gần nhì,...

Trả về

Phía quyết định khớp lệnh trong ngày (B nếu lệnh do bên mua chủ động, S nếu lệnh do bên bán chủ động) của 1 mã chứng khoán

**Ví dụ:**

Để biết phía nào chủ động khớp lệnh mã FPT tương ứng với lần khớp thứ 10 tính từ lần khớp cuối, ta dùng công thức sau:

```
=FA.Intraday.Side("FPT",10)
```

**Kết quả:**

S

Bạn cũng có thể ghi mã FPT ở một ô (cell), ví dụ A1, và dùng công thức sau:

```
=FA.Intraday.Side(A1,10)
```

Ưu điểm của phương pháp này là bạn có thể thay đổi mã chứng khoán mà không cần sửa công thức.

{% hint style="info" %}
**Lưu ý**: Nếu bạn truyền ô vào thay vì mã chứng khoán, thì ở ô đó cần chứa mã chứng khoán. Trong trường hợp này mã chứng khoán không cần nằm giữa 2 dấu nháy đôi.&#x20;
{% endhint %}

Tham số lần khớp cũng có thể sử dụng hàm lấy số dòng hoặc số cột để thay thế, trong trường hợp bạn muốn lấy thông tin của nhiều lần khớp. Bạn có thể dùng công thức sau, với giả sử ô A1 chứa mã, và bạn sử dụng công thức cho ô A2 trở đi:

```
=FA.Intraday.Side(A$1, ROW()-1)
```
