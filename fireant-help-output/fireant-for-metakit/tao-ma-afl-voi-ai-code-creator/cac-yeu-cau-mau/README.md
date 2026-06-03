---
title: "Các yêu cầu mẫu"
source: "https://help.fireant.vn/fireant-for-metakit/tao-ma-afl-voi-ai-code-creator/cac-yeu-cau-mau"
---

# Các yêu cầu mẫu

## Tạo code mức độ cơ bản

### Prompt tạo code bộ lọc

1. Viết code AFL lọc ra các mã có khối lượng giao dịch hôm nay lớn hơn 1 triệu cổ phiếu và giá đóng cửa cao hơn giá mở cửa.
2. Tạo AFL filter chọn những cổ phiếu tăng liên tiếp ít nhất 3 phiên và RSI(14) dưới 70.
3. Lọc các mã có giá vượt MA20 với khối lượng gấp 1.5 lần trung bình 20 phiên gần nhất.
4. Viết AFL lọc cổ phiếu có giá nằm trong vùng 52-week high và MACD cắt lên đường signal.
5. Code AFL để chọn ra cổ phiếu có thanh khoản trung bình 10 phiên lớn hơn 20 tỷ và P/E < 15 (sử dụng dữ liệu fundamental nếu có).

### Prompt tạo code backtest

1. Viết code AFL backtest chiến lược mua khi giá đóng cửa vượt MA50 và bán khi giá đóng cửa cắt xuống MA20.
2. Tạo AFL backtest với điều kiện: mua khi MACD cắt lên signal, bán khi RSI(14) > 70.
3. Code AFL để backtest chiến lược breakout: mua khi giá vượt đỉnh 20 ngày, bán khi giá thủng đáy 10 ngày.
4. Backtest chiến lược mua khi Bollinger Band width thu hẹp và giá breakout khỏi band trên, bán khi giá chạm band dưới.
5. Tạo AFL backtest với tỷ lệ phân bổ vốn 20% cho mỗi lệnh, stop loss 7% và take profit 15%.&#x20;

### Prompt tạo code chỉ báo kỹ thuật

1. Viết code AFL tạo indicator hiển thị đường EMA 20, EMA 50 và EMA 200 trên chart.
2. Tạo chỉ báo AFL custom RSI với thông số 10 phiên, thêm vẽ đường cảnh báo khi RSI vượt 80 hoặc dưới 20.
3. Code AFL vẽ chỉ báo kết hợp MACD histogram với volume trung bình 20 phiên.
4. Viết AFL indicator hiển thị đường VWAP kèm theo highlight các nến có giá đóng cửa cao hơn VWAP.
5. Tạo chỉ báo AFL hiển thị vùng hỗ trợ/kháng cự bằng cách vẽ đường nối các đáy/đỉnh gần nhất.&#x20;

### Prompt tạo code hỗn hợp&#x20;

Dùng cho code có nhiều mục đích: vừa hiển thị, vừa lọc, vừa backtest.

1. Viết AFL vừa hiển thị MA20 và MA50 trên chart, vừa lọc ra các mã có MA20 cắt lên MA50, đồng thời chạy backtest với quy tắc mua/bán đó.
2. Tạo AFL vừa vẽ RSI(14), vừa lọc cổ phiếu có RSI dưới 30, đồng thời backtest mua khi RSI < 30 và bán khi RSI > 70.
3. Code AFL kết hợp Bollinger Bands: hiển thị trên chart, lọc cổ phiếu breakout band trên, và backtest chiến lược breakout.
4. Viết AFL hiển thị MACD và signal, lọc ra các mã MACD cắt lên signal trong 3 phiên gần nhất, đồng thời backtest với stop loss 5%.
5. Tạo AFL vừa vẽ đường trendline tự động, vừa lọc cổ phiếu phá vỡ trendline, và backtest với quy tắc buy breakout - sell breakdown.

## Tạo code nâng cao

### &#xD;Prompt tạo code bộ lọc

1. Viết code AFL lọc cổ phiếu có: giá đóng cửa > MA50 và MA200, khối lượng phiên hiện tại cao hơn 200% khối lượng trung bình 20 phiên, đồng thời RSI(14) nằm trong vùng 40–60 (tích lũy). Thêm cột xuất ra % thay đổi giá so với 52-week low và 52-week high.
2. Tạo AFL filter để tìm các cổ phiếu vừa tạo gap up > 3% so với phiên trước, nhưng giá đóng cửa vẫn nằm dưới MA100. Kết hợp thêm điều kiện P/B < 2 (nếu có dữ liệu cơ bản).
3. Viết code AFL lọc cổ phiếu có mô hình nến engulfing tăng ở cuối xu hướng giảm, khối lượng xác nhận lớn hơn 1.5 lần trung bình 10 phiên, và MACD histogram dương.
4. Code AFL lọc ra cổ phiếu có beta > 1.2 so với VN-Index, biến động trong 30 ngày qua lớn hơn 15%, và khối lượng trung bình > 500k cổ phiếu/phiên.
5. Tạo AFL filter để chọn cổ phiếu đang ở xu hướng tăng (ADX > 25, +DI > –DI), nhưng hiện tại đang điều chỉnh về vùng MA20 ± 2%, kèm theo điều kiện RSI(14) > 45.

### Prompt tạo code backtest

1. Viết AFL backtest chiến lược mua khi giá vượt đỉnh 55 ngày (Donchian channel breakout), bán khi giá thủng đáy 20 ngày, có stop loss 7% và trailing stop 10%. Vốn khởi điểm 1 tỷ, phân bổ 25% cho mỗi lệnh, không mua trùng mã.
2. Tạo AFL backtest chiến lược mean-reversion: mua khi RSI(2) < 10, bán khi RSI(2) > 70 hoặc sau 5 phiên nắm giữ, dùng vốn cố định 100 triệu/lệnh, phí giao dịch 0.15%.
3. Code AFL backtest hệ thống giao dịch Bollinger Bands với entry khi giá đóng cửa vượt band trên và exit khi giá đóng cửa chạm MA20, thêm stop loss 5%, take profit 12%, và chỉ mở tối đa 3 lệnh cùng lúc.
4. Backtest chiến lược kết hợp: mua khi MA20 cắt lên MA50, xác nhận bằng MACD histogram dương, bán khi MA20 cắt xuống MA50 hoặc khi giá giảm 10% từ đỉnh gần nhất. Tính thêm Sharpe ratio và Max Drawdown.
5. Tạo AFL backtest giao dịch theo trend: chỉ vào lệnh mua nếu VN-Index cũng đang trên MA200, mỗi lệnh mua tối đa 10% vốn, giữ lệnh tối đa 60 ngày, và thoát khi RSI(14) > 80.&#x20;

### Prompt tạo code chỉ báo kỹ thuật

1. Viết AFL indicator vẽ hệ thống Ichimoku đầy đủ (Tenkan, Kijun, Senkou, Chikou), đồng thời highlight các điểm giao cắt Tenkan-Kijun bằng mũi tên, và tô màu vùng Kumo khác nhau khi dày/ mỏng.
2. Tạo AFL indicator vẽ 3 timeframe EMA (20 trên daily, 50 trên weekly, 200 trên monthly) chồng lên chart daily, có chú thích màu rõ ràng.
3. Code AFL chỉ báo Price Action Zones: tự động vẽ vùng hỗ trợ/kháng cự mạnh bằng cách phát hiện các cụm nến đảo chiều trong 50 phiên gần nhất.
4. Viết AFL indicator custom RSI với chu kỳ động: khi thị trường sideway (ADX < 20) thì dùng RSI(7), khi thị trường có trend (ADX > 25) thì dùng RSI(14). Vẽ cả hai trên chart.
5. Tạo AFL indicator hiển thị Volume Profile (phân phối khối lượng theo mức giá) trong 100 phiên gần nhất, kèm theo highlight vùng giá có volume lớn nhất (POC).&#x20;

### Prompt tạo code hỗn hợp

1. Viết AFL vừa hiển thị Bollinger Bands, vừa lọc cổ phiếu có giá đóng cửa breakout band trên kèm khối lượng > 2 lần trung bình 20 phiên, đồng thời backtest chiến lược mua breakout band trên – bán khi giá thủng MA20, với stop loss 8%.
2. Tạo AFL vừa vẽ EMA 20/50/200, vừa lọc cổ phiếu có Golden Cross (EMA20 cắt lên EMA50 và cả hai nằm trên EMA200), đồng thời backtest chiến lược mua Golden Cross – bán khi EMA20 cắt xuống EMA50.
3. Code AFL hiển thị RSI(14), highlight vùng quá bán, lọc cổ phiếu có RSI < 30 và giá đang chạm hỗ trợ mạnh, đồng thời backtest chiến lược mua khi RSI < 30 và bán khi RSI > 70, với trailing stop 10%.
4. Viết AFL hiển thị chỉ báo MACD, đồng thời lọc cổ phiếu có MACD cắt lên signal trong 5 phiên gần nhất, và chạy backtest chiến lược mua khi MACD cắt lên signal, bán khi cắt xuống signal, vốn cố định 100 triệu/lệnh.
5. Tạo AFL vừa vẽ Ichimoku Cloud, vừa lọc cổ phiếu breakout khỏi Kumo, đồng thời backtest chiến lược buy breakout khỏi mây – sell khi giá quay lại vào mây, stop loss 5%.&#x20;

## Tao code có độ khó cao&#x20;

### Prompt tạo code bộ lọc

1. Viết code AFL lọc cổ phiếu có giá đóng cửa hôm nay nằm trên MA50 và MA200 ở khung daily, đồng thời trên khung weekly cũng phải nằm trên MA50. RSI(14) daily trong vùng 40–60 (sideway tích lũy), ADX(14) > 25 ở weekly (thị trường có trend). Khối lượng phiên hiện tại phải lớn hơn 3 lần khối lượng trung bình 20 phiên, và P/E < 15. Xuất ra bảng gồm: mã, % thay đổi 1 tháng, % thay đổi 3 tháng, khối lượng trung bình 20 phiên.
2. Tạo AFL filter chọn cổ phiếu có mô hình tam giác (giá dao động với biên độ co hẹp dần trong 30 phiên gần nhất), kèm điều kiện giá > MA200, Volume giảm dần trong giai đoạn co hẹp, nhưng phiên hôm nay breakout khỏi trendline tam giác với khối lượng > 250% trung bình 20 phiên.
3. Viết AFL lọc các mã có beta > 1.2 so với VN-Index, giá biến động 30 ngày qua > 15%, đồng thời phải tạo đáy cao hơn đáy trước (higher low). Ngoài ra, ROC(20) > 0 và MACD histogram chuyển từ âm sang dương.
4. Code AFL lọc cổ phiếu có dòng tiền lớn: CMF(20) > 0.15, khối lượng hôm nay cao nhất trong 50 phiên, đồng thời đường OBV tạo đỉnh mới cao hơn đỉnh trước. Chỉ chọn cổ phiếu có vốn hóa > 5,000 tỷ (nếu dữ liệu cơ bản có).
5. Tạo AFL filter tìm cổ phiếu chuẩn bị bứt phá: giá tích lũy trong biên độ < 8% suốt 20 phiên gần nhất, Volume giảm liên tục, RSI(14) trong vùng 45–55, nhưng khối lượng hôm nay tăng gấp đôi và giá đóng cửa phá vỡ biên trên của range.&#x20;

### Prompt tạo code Backtest

1. Viết AFL backtest chiến lược trend-following đa khung thời gian: chỉ mua nếu MA50 daily > MA200 daily và MA20 weekly > MA50 weekly. Entry khi giá đóng cửa vượt đỉnh 20 ngày với Volume > 2 lần trung bình. Exit khi giá thủng MA20 daily hoặc sau 60 phiên. Thêm stop loss 7%, trailing stop 10%, phí giao dịch 0.15%, vốn khởi điểm 2 tỷ, phân bổ tối đa 20% vốn mỗi lệnh, không mua trùng mã. Tính kết quả: CAGR, Sharpe Ratio, Max Drawdown.
2. Tạo AFL backtest hệ thống breakout Volatility Squeeze: phát hiện khi Bollinger Band width thấp hơn 10% giá trị trung bình 200 ngày, entry khi giá breakout band trên kèm ADX > 25. Exit khi giá thủng band giữa hoặc RSI > 80. Áp dụng trailing stop ATR(14)\*2, tối đa 5 lệnh mở, vốn 500 triệu/lệnh, không mua trong 5 ngày trước T+3 ngày lễ.
3. Code AFL backtest hệ thống rotation sector: mỗi cuối tuần chọn 3 cổ phiếu có sức mạnh tương đối cao nhất (ROC 20 ngày so với VN-Index), lọc thêm điều kiện > MA100. Mua phân bổ đều vốn, giữ trong 20 ngày, bán khi cổ phiếu rớt khỏi top 3 hoặc giá thủng MA50.
4. Backtest chiến lược kết hợp Price Action + Indicator: entry khi xuất hiện mô hình nến Morning Star sau một nhịp giảm, xác nhận bằng RSI(14) < 40 chuyển hướng tăng, MACD histogram từ âm sang dương. Exit khi xuất hiện nến Shooting Star kèm RSI > 70 hoặc giá thủng EMA20. Stop loss 6% từ entry.
5. Tạo AFL backtest hệ thống theo xu hướng dài hạn: chỉ vào lệnh khi VN-Index > MA200. Entry khi giá cổ phiếu vượt đỉnh 100 ngày, exit khi giá thủng đáy 50 ngày hoặc khi lợi nhuận đạt 25%. Quản trị rủi ro: vốn 1 tỷ, chỉ đầu tư 10% vốn mỗi lệnh, tối đa 5 lệnh mở, stop loss 8%, trailing stop 12%.&#x20;

### Prompt tạo code chỉ báo kỹ thuật

1. Viết AFL indicator hiển thị hệ thống Ichimoku Cloud đầy đủ, thêm highlight tín hiệu 'Kumo breakout' và gắn mũi tên khi Chikou Span cắt lên giá. Đồng thời overlay thêm EMA200 và tô nền chart xanh khi giá nằm trên mây + EMA200.
2. Tạo AFL indicator vẽ Volume Profile cho 100 phiên gần nhất, highlight vùng POC (Point of Control), Value Area High/Low, và đánh dấu breakout khi giá vượt Value Area High với Volume đột biến.
3. Code AFL indicator kết hợp: hiển thị RSI(14) kèm 2 mức động (RSI overbought = 60 khi thị trường giảm, = 80 khi thị trường tăng), thêm histogram MACD dưới cùng chart, highlight tín hiệu đồng pha (MACD dương và RSI trên 50).
4. Viết AFL indicator vẽ Fibonacci Retracement tự động cho swing high – swing low gần nhất trong 50 phiên, highlight vùng 0.618 và 0.382, thêm cảnh báo khi giá bật lại tại các mức này.
5. Tạo AFL indicator đa timeframe: trên chart daily hiển thị MA20/50/200, RSI(14) của khung weekly trong subwindow, MACD của khung monthly ở subwindow khác. Thêm màu nền thể hiện trạng thái trend: xanh (bull), đỏ (bear), vàng (sideway).&#x20;

### Prompt tạo code hỗn hợp

1. Viết AFL vừa vẽ Bollinger Bands, vừa lọc cổ phiếu có Bollinger squeeze (band width thấp nhất 100 phiên), đồng thời backtest chiến lược breakout band trên với stop loss ATR(14)\*2, trailing stop 10%, vốn 200 triệu/lệnh. Xuất ra bảng filter hiển thị: mã, % thay đổi 1 tuần, % thay đổi 1 tháng.
2. Tạo AFL vừa vẽ Ichimoku Cloud trên chart, vừa lọc cổ phiếu breakout khỏi Kumo với Volume > 2 lần trung bình, đồng thời backtest chiến lược buy breakout – sell khi giá quay vào Kumo, với stop loss 7% và vốn khởi điểm 1 tỷ.
3. Code AFL kết hợp: hiển thị EMA20/50/200 + MACD dưới chart, lọc cổ phiếu có Golden Cross (EMA20 cắt lên EMA50 trên EMA200) kèm MACD dương, đồng thời backtest hệ thống Golden Cross này với trailing stop 12%, tối đa 3 lệnh mở.
4. Viết AFL vừa hiển thị RSI(14) và highlight vùng quá bán, vừa lọc cổ phiếu có RSI < 30 + khối lượng tăng đột biến, đồng thời backtest chiến lược mua tại RSI < 30, bán khi RSI > 70 hoặc sau 15 phiên, vốn 100 triệu/lệnh.
5. Tạo AFL hệ thống đa năng: hiển thị đường trendline tự động, lọc cổ phiếu phá vỡ trendline giảm, đồng thời backtest chiến lược buy breakout trendline – sell khi giá phá vỡ trendline tăng. Quản trị vốn: 5% risk per trade, tính Kelly ratio để điều chỉnh size lệnh.
