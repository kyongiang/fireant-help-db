---
title: "Advanced MACD"
source: "https://help.fireant.vn/fireant-for-web-1/cac-chi-so-ky-thuat/macd"
---

# Advanced MACD

<figure><img src="https://help.fireant.vn/files/cXQB56MOyM2CGx0t1yR0" alt=""><figcaption></figcaption></figure>

**MACD** là một trong những chỉ báo động lượng được phát triển bởi Gerald Appel, vào cuối những năm 70.

Các nhà phân tích kỹ thuật sử dụng **MACD** với hai mục đích chính: tìm ra phân kỳ/hội tụ hay động lượng của giá và xác định xu hướng.

**Phiên bản Advanced MACD của FireAnt** là một chỉ báo Hybrid được xây dựng trên nền tảng của chỉ báo MACD. Công cụ này kết hợp:

* Logic giao cắt MACD cổ điển&#x20;
* Năng Lượng Pha: Tính toán năng lượng sóng thực sự bằng cách sử dụng góc pha, tiết lộ sức mạnh đằng sau các chuyển động giá.
* Biến đổi Hilbert: Đo pha của một dạng sóng (chu kỳ giá) để phát hiện các điểm chuyển hướng.
* Mô hình Lượng tử: Xem giá như một hàm sóng, cung cấp cái nhìn dự đoán dựa trên động lực pha.

**Các Tính Năng Chính của Advanced MACD**&#x20;

* **Logic Năng Lượng Sóng**: Thay vì chỉ sử dụng giá và chênh lệch trung bình động, chỉ báo này tính toán động lượng được điều chỉnh pha, qua đó xác định năng lượng thực sự đằng sau các biến động giá.&#x20;
* **Phát Hiện Xu Hướng Dựa trên Pha**: Nó đọc các pha bằng logic tương tự Biến đổi Hilbert, cho phép bạn phát hiện động lượng trước khi nó hiển thị trên giá.&#x20;
* **Loại nhiễu**: Đường năng lượng (sử dụng thay cho đường MACD) và đường tin hiệu được loại bỏ phần lớn nhiễu có trong chỉ báo MACD truyền thống.&#x20;
* **Khuếch Đại Tín Hiệu qua Biểu đồ Năng Lượng**: Biểu đồ không chỉ hiển thị thay đổi động lượng — nó thể hiện cường độ của năng lượng sóng, giúp bạn xác nhận sức mạnh của xu hướng.&#x20;
* **Cấu trúc Dựa trên Vật lý**: Thuật toán bắt nguồn từ lý cơ chế sóng trong thế giới thực, mang lại lợi thế khoa học cho giao dịch — lý tưởng cho các nhà giao dịch tin vào các mô hình tự nhiên như dao động theo chu kỳ và cân bằng động.&#x20;
* **Xác Nhận Xu Hướng & Phát Hiện Đảo Chiều Sớm**: Nó có thể xác nhận các xu hướng mạnh và đồng thời nắm bắt các thay đổi tinh tế thường báo trước các đảo chiều lớn — mang lại cả độ tin cậy và khả năng dự đoán.&#x20;
* **Tương thích với nhiều thị trường**: Được thiết kế để hoạt động ttoost với các vùng thanh khoản, hành động giá, khối lệnh và giao dịch cấu trúc — phù hợp hoàn hảo với các hệ thống giao dịch hiện đại.

Các tham số mà chúng tôi sử dụng mặc định (người dùng có thể thay đổi):

* **Chu kỳ chậm**: Sử dụng đường EMA (đường trung bình mũ) với chu kỳ 26 nến
* **Chu kỳ nhanh**: Sử dụng đường EMA với chu kỳ 12 nến
* **Chu kỳ tín hiệu**: Sử dụng chu kỳ 9 nến
* **Nguồn**: Có thể chọn một trong các mức giá: mở cửa (o), đóng cửa (c), cao nhất (h), thấp nhất (l), trung bình cao nhất và thâp nhất (hl2), trung bình cao nhất thấp nhất và đóng cửa (hlc3) hoặc trung bình bốn mức giá (ohlc4). Mặc định là **giá đóng cửa.**
* **Tín hiệu sử dụng**: Có 2 lựa chọn là **Truyền thống** (chỉ số sẽ hoạt động như chỉ báo MACD truyền thống) và **Nâng cao**, chỉ số sẽ được tích hợp các cấu trúc mới được mô tả ở trên. Mặc định sẽ sử dụng tín hiệu **Nâng cao.**
* **Hệ số dịch pha**: Hệ số này được sử dụng để tính toán các thành phần pha, sử dụng trong biến đổi Hilbert. Mặc định là 14.
* **Hệ số làm mượt pha**: Hệ số này được sử dụng để làm mượt độ dịch pha và khuyếch đại sóng.

<figure><img src="https://help.fireant.vn/files/z22bnwhPBPdZBp1Zi6ch" alt=""><figcaption></figcaption></figure>

Bên cạnh các tham số, người dùng cũng có thể thay đổi màu sắc đường MACD, đường tính hiệu, màu tín hiệu gợi ý mua/bán, và các màu cho biểu đồ tần suất.

<figure><img src="https://help.fireant.vn/files/2mUe4VWeYdXMV2GkCgXe" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Gợi ý sử dụng:**&#x20;

**MACD** là một chỉ số có độ tin cậy cao, nhưng thường bị coi là tín hiệu chậm, do cách sử dụng truyền thống của MACD là mua khi MACD chuyển từ âm sang dương và bán khi MACD chuyển từ dương sang âm.&#x20;

Sử dụng đường tín hiệu và giao cắt giữa MACD với đường tín hiệu sẽ cho ra các tín hiệu gợi ý mua bán sớm hơn nhưng cũng có độ tin cậy thấp hơn do bị nhiễu.  Sử dụng tin hiệu nâng cao sẽ giúp cải thiện đáng kể độ tin cậy của tín hiệu.

Một cách sử dụng nữa là mua vào khi biểu đồ tần suất tạo đáy và bán ra khi biểu đồ tần suất tạo đỉnh.
{% endhint %}

Các ví dụ thực tế:

<figure><img src="https://help.fireant.vn/files/7DNCsnfOlJaHmSuDY3PI" alt=""><figcaption></figcaption></figure>

Biểu đồ trên so sánh giữa hai cách dùng tín hiệu MACD truyền thống và nâng cao cho mã VNINDEX. Tín hiệu nâng cao đã phát ra sớm 1 nến so với tín hiệu truyền thống và ở vị trí thuận lợi hơn cho vị thế mua.

<figure><img src="https://help.fireant.vn/files/6xkTHnKv8FTD8Pa8Dtbm" alt=""><figcaption></figcaption></figure>

Trong ví dụ tiếp theo, chúng ta so sánh hai cách dùng tín hiệu MACD truyền thống và nâng cao cho mã FPT. Lần này tín hiệu nâng cao đã phát ra muộn 3 nến so với tín hiệu truyền thống nhưng vẫn ở vị trí tốt  hơn cho vị thế mua, ngoài ra tín hiệu nâng cao cũng không xuất hiện ở sai vị trí như tín hiệu truyền thống trước đó
