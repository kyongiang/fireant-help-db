---
title: "Relative Rotation Graph (RRG)"
source: "https://help.fireant.vn/fireant-for-web-1/cac-chi-so-ky-thuat/relative-rotation-graph-rrg"
---

# Relative Rotation Graph (RRG)

![](https://help.fireant.vn/files/BbFxNEQUio5YVjyuPGU9)

Relative Rotation Graphs (Đồ thị chuyển vị tương đối) là một công cụ trực quan hóa để phân tích Sức mạnh tương đối (Relative Strength - RS). Nhà đầu tư có thể sử dụng RRG để phân tích xu hướng sức mạnh tương đối của một tài sản so với một tài sản tham chiếu nào đó.

Điểm mạnh của công cụ này là khả năng biểu diễn hiệu suất tương đối của các tài sản trên 1 biểu đồ. RRG sử dụng bốn góc phần tư để xác định vị thế của tài sản theo dõi so với tài sản tham chiếu. Sư chvị được hình thành RRG di chuyển từ góc phần tư này sang góc phần tư khác.

RRG được phát triển trong khoảng thời gian từ năm 2004-2005 bởi Julius de Kempenaer, người sau đó trở thành Giám đốc Nghiên cứu về RRG. Trong suốt thời gian làm việc với tư cách là Nhà phân tích bên bán cho một ngân hàng đầu tư ở Amsterdam, ông đã phải đối mặt với hai vấn đề khi nghiên cứu phân tích kỹ thuật và định lượng. Thứ nhất, các khách hàng tổ chức quan tâm nhiều đến hiệu suất tương đối hơn là các dự báo mang tính định hướng; họ muốn biết nơi nào "thừa" và nơi nào "thiếu" trong danh mục đầu tư của họ. Thứ hai, các nhà đầu tư tổ chức này phải đối mặt với tình trạng quá tải do lượng thông tin khổng lồ; họ cần một công cụ có thể tách biệt rõ ràng những "kẻ dẫn đầu" và những "kẻ tụt hậu" trong danh mục đầu tư.

Đồ thị chuyển vị tương đối giúp giải quyết những vấn đề này bằng các góc phần tư được mã hóa bằng các màu sắc khác nhau, giúp các nhà đầu tư dễ dàng hơn trong việc theo dõi một cá tổng thể.

## **Cấu trúc RRG**

![](https://help.fireant.vn/files/J4BZi2qpsGo0dF0c46qk)

Cấu trúc đồ thị RRG gồm 4 góc phần tư xung quanh gốc tọa độ RS=100, RM=100. Trong đó

Chỉ số RS (Julius de Kempenaer Relative Strength Ratio) là một chỉ báo được thiết kế để xác định xu hướng dựa trên hiệu suất tương đối của một tài sản (so với một tài sản khác được chọn làm tham chiếu) và để đo lường sức mạnh của xu hướng đó.  RS trong biểu đồ RRG đóng vai trò trục hoành.

Chỉ số RM (Julius de Kempenaer Relative Strength Momentum Ratio) là một chỉ số đo lường động lượng (tỷ lệ thay đổi) của RS. Cũng giống như các chỉ báo động lượng khác, RM sẽ đi trước RS và có thể sử dụng để dự đoán sự đảo chiều của RS. RM trong biểu đồ RRG đóng vai trò trục tung.

Mỗi điểm trên biểu đồ RRG sẽ tương ứng với 1 giá trị RS và RM. Bốn góc phần tư được hiểu như sau:

* **Góc phần tư thứ nhất được gọi là vùng dẫn dắt (màu xanh lá cây)**: sức mạnh tương đối của tài sản so sánh so với tài sản tham chiếu là mạnh và động lượng của nó cũng mạnh.
* **Góc phần tư thứ hai được gọi là vùng suy yếu** **(màu vàng):** sức mạnh tương đối của tài sản so sánh so với tài sản tham chiếu là mạnh nhưng động lượng của nó đã bị suy yếu.&#x20;
* **Góc phần tư thứ ba được gọi là vùng tụt hậu (màu đỏ):** sức mạnh tương đối của tài sản so sánh so với tài sản tham chiếu là yếu và động lượng của nó cũng yếu.&#x20;
* **Góc phần tư thứ tư được gọi là vùng cải thiện (màu xanh dương):** sức mạnh tương đối của tài sản so sánh so với tài sản tham chiếu vẫn yếu nhưng động lượng của nó đang mạnh lên.&#x20;

Có thể thấy là nếu một tài sản đang ở vùng dẫn dắt hoặc cải thiện, thì nó đang có xu hướng mạnh lên so với tài sản tham chiếu, và tất nhiên, nếu chúng ta muốn mua, hãy chọn những tài sản này. Ngược lại, nếu một tài sản đang ở vùng màu vàng hoặc đỏ, thì tài sản đó đang hoặc sẽ yếu hơn so với tài sản tham chiếu, trong trường hợp này chúng ta sẽ chọn không mua hoặc bán ra.

**Chỉ báo FireAnt RRG**&#x20;

FireAnt tích hợp chỉ báo RRG lên biểu đồ bằng cách chiếu đồ thị RRG từ không gian hai chiều xuống không gian một chiều. Chỉ báo RRG sử dụng 2 đường RS (màu đỏ) và RM (xanh) và các phân vùng có màu sac tương ứng với các góc phần tư được mô tả ở trên. VNINDEX được sử dụng làm tham chiếu cho các mã cổ phiếu.&#x20;

Tùy theo giá trị của RS và RM ta có 4 phân vùng:

* **Xanh lá**: vùng dẫn dắt có RS>=100 và RM>=100.
* **Vàng**: vùng suy yếu có RS>100 và RM<100
* **Đỏ**: vùng tụt hậu có RS<100 và RM <100
* **Xanh dương:** vùng cải thiện có RS<100 và RM>100
