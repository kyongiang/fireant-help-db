---
title: "Accumulative Swing Index"
source: "https://help.fireant.vn/thu-vien-chi-bao/accumulative-swing-index"
---

# Accumulative Swing Index

**Chỉ số dao động tích lũy** (Accumulative Swing Index, viết tắt là ASI) là một [chỉ báo kỹ thuật](https://help.fireant.vn/thuat-ngu-chung-khoan/) trong [phân tích kỹ thuật](https://help.fireant.vn/thuat-ngu-chung-khoan/), được sử dụng để xác định xu hướng giá của một tài sản tài chính. Nó được phát triển bởi J. Welles Wilder và được giới thiệu trong cuốn sách của ông "New Concepts in Technical Trading Systems".

<figure><img src="https://help.fireant.vn/files/m8E5Nqgoo2RXjQhRQAmi" alt=""><figcaption><p>Chỉ số dao động tích lũy (ASI)</p></figcaption></figure>

ASI tính toán dựa trên giá mở cửa, giá đóng cửa, cao nhất và thấp nhất của mỗi ngày giao dịch. Nó sử dụng các thông tin này để tạo ra một chỉ báo với giá trị tích lũy, giúp đánh giá xu hướng và mức độ tăng trưởng của tài sản tài chính.

Để tính toán ASI, đầu tiên phải tính toán một giá trị **Swing Index** (**SI**) dựa trên giá mở cửa, giá đóng cửa, giá cao nhất và giá thấp nhất của mỗi ngày. Sau đó, giá trị SI được tích lũy để tạo ra giá trị ASI tích lũy.

Công thức tính Accumulative Swing Index (ASI) như sau:

Tính giá trị của Swing Index (SI) cho ngày giao dịch hiện tại:

$$
SI=50\times \left( \frac{Cy-C+\frac{1}{2} (Cy-Oy)+\frac{1}{4} (C-O)}{R} \right) \times\frac{K}{T}
$$

Trong đó:

* SI: Giá trị Swing index&#x20;
* C: Giá đóng cửa&#x20;
* Cy: Gíá đóng cửa phiên trước
* H: Giá cao nhất
* Hy: Giá cao nhất phiên trước
* K: max(Hy​ − C, Ly ​ − C)&#x20;
* L: Giá thấp nhất&#x20;
* L&#x79;*:* Giá thấp nhất phiên trước&#x20;
* O: Giá mở cửa
* O&#x79;*:* Giá mở cửa phiên trước
* R: Được tính dựa trên tương quan giữa C, Hy ​và Ly ​ (xem cách tính phía dưới)&#x20;
* T: Thay đổi giá tối đa trong ngày​, tính bằng H-L

Để tính R, chúng ta tính các chênh lệch giá sau:

$$
\begin{align\*}
\text{(1)} \quad & H - C\_y \\
\text{(2)} \quad & L - C\_y \\
\text{(3)} \quad & H - L \\
\end{align\*}
$$

Nếu (1) lớn nhất, ta có:

$$
R = (H - C\_y) - \frac{1}{2} (L - C\_y) + \frac{1}{4} (C\_y - O\_y)
$$

Nếu (2) lớn nhất, ta có:

$$
R = (L - C\_y) - \frac{1}{2} (H - C\_y) + \frac{1}{4} (C\_y - O\_y)
$$

Nếu (3) lớn nhất, ta có:

$$
R = (H - L) + \frac{1}{4} (C\_y - O\_y)
$$

Khi đã tính được giá trị SI cho phiên hiện tại, nó sẽ được cộng vào ASI của kỳ trước để tính ASI phiên hiện tại:

ASI = ASI trước + SI

$$
ASI = ASI\_y +SI
$$

### So sánh ASI với SI

Sự khác biệt giữa ASI và SI chủ yếu nằm ở phạm vi thời gian và ứng dụng của chúng. SI là một chỉ số đơn kỳ tập trung vào biến động giá từ một phiên giao dịch sang phiên giao dịch tiếp theo. Nó chỉ bao hàm động thái giá ngắn hạn, và có thể quan trọng với những nhà giao dịch trong ngày hoặc những người đang tìm kiếm nhanh thông tin mã chứng khoán hoặc index.

Ngược lại, ASI là tổng lũy kế của các giá trị SI này. Bằng cách liên tục cộng dồn các giá trị SI, ASI cung cấp một cái nhìn dài hạn, theo dõi đà và hướng của giá qua các giai đoạn kéo dài. Đây giống như việc so sánh một bức ảnh (SI) với một bộ phim (ASI). SI chụp lại một khoảnh khắc trong khi ASI kể toàn bộ câu chuyện.

Đối với các nhà giao dịch, sự phân biệt này rất quan trọng. SI cung cấp thông tin nhanh chóng cho các quyết định ngắn hạn, trong khi ASI cung cấp cái nhìn tổng quan, giúp nhà đầu tư nắm được xu hướng giá.

### Sử dụng ASI trong giao dịch

Sử dụng ASI trong một chiến lược giao dịch có thể giúp cải thiện quá trình ra quyết định của bạn. Dưới đây là cách các nhà giao dịch sử dụng ASI.

#### Nhận diện xu hướng&#x20;

Để xác định xu hướng hãy bắt đầu bằng cách quan sát đường ASI. ASI tăng xác nhận một xu hướng tăng, và chỉ ra các cơ hội mua tiềm năng. Ngược lại, ASI giảm cho phép nhận diện một xu hướng giảm, cơ hội tiềm năng để bán. Quy tắc cần nhớ là bạn cần xác nhận xu hướng với các chu kỳ khác nhau để đảm bảo có được sự đồng thuận.

<figure><img src="https://help.fireant.vn/files/UFKHxFRdkzcxvAya3Lsy" alt=""><figcaption><p>Nhận diện xu hướng với ASI</p></figcaption></figure>

#### Phân tích sự phân kỳ với giá

Phân kỳ xảy ra khi biểu đồ giá và biểu đồ ASI di chuyển theo các hướng ngược nhau. Trong xu hướng tăng nếu giá cổ phiếu đang tạo ra các đỉnh giá cao dần, nhưng ASI không tạo ra các đỉnh cao dần, điều này chỉ ra xu hướng tăng nhiều khả năng là yếu đi, và đó là dấu hiệu đảo chiều giảm giá tiềm năng. Ngược lại, nếu giá đang trong xu hướng giảm và liên tục tảo đáy giá thấp dần, nhưng ASI lại không tạo ra các đáy  thấp dần, thì đây cũng là dắu hiệu nhận biết sắp có đảo chiều tăng giá.

<figure><img src="https://help.fireant.vn/files/N9UTmad3RauCBk1ODJom" alt=""><figcaption><p>Phân kỳ giữa ASI và giá báo hiệu sắp có đảo chiều xu hướng</p></figcaption></figure>

#### Xác nhận đột phá&#x20;

ASI có thể xác nhận các tình huống đột phá. Ví dụ, nếu giá đột phá qua một mức kháng cự dài hạn và ASI đồng thời đạt mức cao mới, điều này củng cố tính hợp lệ của sự đột phá. Các di chuyển đồng bộ như vậy có thể tăng sự tự tin của nhà đầu tư khi mở vị thế mua.

### Hạn chế của chỉ số ASI

Mặc dù chỉ số ASI rất hữu ích trong phân tích kỹ thuật, nhưng nó vẫn có những hạn chế nhất định. Giống như nhiều chỉ báo khác, nó có thể tạo ra các tín hiệu giả, đặc biệt là trong các thị trường biến động mạnh.

Ngoài ra, nếu chỉ dựa vào ASI mà không đối chiếu với các chỉ báo khác có thể dẫn đến nhận thức không đầy đủ về diễn biến giá. Kết hợp ASI với một vài chỉ báo đo lường các khía cạnh khác của diễn biến giá, như RSI hoặc MACD, có thể cung cấp các tín hiệu giao dịch có độ tin cậy cao hơn và giảm thiểu các tín hiệu giả.

### Kết Luận&#x20;

Tóm lại, ASI là một công cụ mạnh mẽ, giúp nhà đầu tư thay vì phải theo dõi các biến động giá phức tạp thì chỉ cần theo dõi những thông tin dễ hiểu từ chỉ báo. Với khả năng cung cấp một cái nhìn nhanh và tổng thể cũng như dài hạn về xu hướng giá, nó là bổ sung hữu ích cho các chỉ báo khác và có vị trí quan trọng trong một chiến lược giao dịch toàn diện.

{% hint style="info" %}
**Thuật ngữ liên quan**

* [Chỉ báo Vortex](https://help.fireant.vn/thu-vien-chi-bao/)
* [Gann HiLo Activator](https://help.fireant.vn/thu-vien-chi-bao/)
* [RSI](https://help.fireant.vn/thu-vien-chi-bao/)
  {% endhint %}
