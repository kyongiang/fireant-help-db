---
title: "Volume Profile Visible Range"
source: "https://help.fireant.vn/thu-vien-chi-bao/volume-profile-visible-range"
---

# Volume Profile Visible Range

**Định nghĩa**

Volume Profile Visible Range (VPVR) là một chỉ báo nâng cao cho phép thống kê khối lượng giao dịch trong một khoảng thời gian xác định ở các mức giá khác nhau. Khoảng thời gian được xác định là từ nến giá đầu đến nến giá cuối trong phạm vi hiển thị (nghĩa là các nến giá mà bạn nhìn thấy được trên biểu đồ). Chỉ báo (tùy vào các tham số mà người dùng thiết lập như số mức giá) sẽ sử dụng một biểu đồ tần suất (được đặt ở lề trái hoặc lề phải của biểu đồ giá) để thống kê tổng khối lượng ở các mức giá có khối lượng giao dịch lớn nhất (số mức giá tối đa tùy thuộc vào thiết lập của người dùng). Tổng khối lượng giao dịch ở các mức giá có thể thiết lập để chia thành tổng khối lượng ứng với giá tăng và tổng khối lượng ứng với giá giảm (tăng và giảm so với phiên liên trước phiên có giá ở mức giá tương ứng).

![](https://help.fireant.vn/files/VPZdueoHYmZZK84xji4T)

**Các thông số quan trọng**

·         ***Point of Control (POC)***: Mức giá trong khoảng thời gian có khối lượng giao dịch cao nhất, còn gọi là điểm kiểm soát

·         ***Profile High***: Mức giá cao nhất trong trong số các mức giá được thống kê.

·         ***Profile Low***: Mức giá thấp nhất trong trong số các mức giá được thống kê.

·         ***Value Area (VA)***: Vùng giá mà tổng khối lượng giao dịch của chúng chiếm số phần trăm tổng khối lượng giao dịch được thống kê. Tỷ lệ phầ trăm được thiết lập bởi tham số **Value Area Volume (Khối lượng vùng giá trị)** có giá trị mặc định 70%

**Mức hỗ trợ và kháng cự**

VPVR trước hết được sử dụng để xác định các mức hỗ trợ và kháng cự cơ bản. Nếu như các phương pháp xác định ngưỡng hỗ trơ/kháng cự như sử dụng đường xu hướng hay các đường trung bình động dựa trên hành động và phân tích giá hiện tại để dự đoán biến động giá trong tương lai, thì VPVR lại dựa vào biến động giá và khối lượng trong quá khứ. Các mức giá ở phía trên của biểu đồ VPVR với khối lượng bán áp đảo thường là các ngưỡng kháng cự mạnh. Ngược lại các mức giá ở phía dưới biểu đồ VPVR với khối lượng mua áp đảo sẽ thường là các ngưỡng hỗ trợ mạnh.

![](https://help.fireant.vn/files/rNtGnpQC0QiAZ5pELHUM)

**Đỉnh và đáy khối lượng**

*Các **đỉnh khối lượng** (High Volume Nodes – HVN) thường tương ứng với các vùng tích lũy, giá lập nền tại đây, nên khả năng giá có thể đột phá qua vùng này một cách nhanh chóng là thấp. Vùng giá ở quanh mức đỉnh khối lượng còn được gọi là vùng giá hợp lý (fair value area).*

![](https://help.fireant.vn/files/1AqLBQ5p44JTTOofDlen)

&#x20;*Với các **Đáy khối lượng (**&#x4C;ow Volume Nodes - LVN)* thì ngược lại, giá ở quanh mức này thể hiện vùng giá yếu (unfair value area), và thường là kết quả của các lần đột phá giá. Khi giá tiến đến vùng giá yếu, thì khả năng là nó sẽ đi qua vùng giá này một cách nhanh chóng.

![](https://help.fireant.vn/files/Vwf7hspPizKtSlsstdZP)

**Ví dụ về cách sử dụng VPVR**

Cũng giống như các công cụ hoặc chỉ báo khác, VPVR có một số cách sử dụng khác nhau. Dưới đây là ví dụ cách sử dụng VPVR dựa trên việc so sánh giá mở cửa của phiên hiện tại với VPVR của phiên hôm trước.

* Nếu phiên hiện tại mở cửa cao hơn **điểm kiểm soát** của phiên hôm trước, nhưng vẫn ở dưới mức **profile high**, hãy chờ cho giá giảm về điểm kiểm soát và mua vào.
* Nếu phiên hiện tại mở cửa thấp hơn **điểm kiểm soát** của phiên hôm trước, nhưng vẫn ở trên mức **profile low**, hãy chờ khi giá tăng trở lại **điểm kiểm soát** và bán ra.
* Nếu giá mở cửa của phiên hiện tại cao hơn **profile high**, hoặc thấp hơn **profile low** phiên hôm trước, xu hướng thường sẽ tiếp diễn.

**Kết luận**

VPVR là một chỉ báo phân tích kỹ thuật cực kỳ giá trị được sử dụng phổ biến bởi các nhà giao dịch trên toàn thế giới. Mặc dù có nhiều cách sử dụng khác nhau, VPVR được công nhận một cách rộng rãi trong cộng đồng về tính hữu dụng của nó..
