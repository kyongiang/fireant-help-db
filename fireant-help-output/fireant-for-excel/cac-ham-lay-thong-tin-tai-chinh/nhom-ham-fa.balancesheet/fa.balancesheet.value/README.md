---
title: "FA.BalanceSheet.Value"
source: "https://help.fireant.vn/fireant-for-excel/cac-ham-lay-thong-tin-tai-chinh/nhom-ham-fa.balancesheet/fa.balancesheet.value"
---

# FA.BalanceSheet.Value

## Cú pháp

```
=FA.BalanceSheet.Value("Mã CK",Năm, Quý, [Chỉ tiêu bảng CĐKT]) 
```

**Trong đó:**

* **Mã CK**: là mã cổ phiếu niêm yết&#x20;
* **Năm:** là năm tương ứng với bảng CĐKT&#x20;
* **Quý:** là quý tương ứng với bảng CĐKT. Nếu Quý bằng 0 thì bảng CĐKT là bảng CĐKT năm&#x20;
* **Chỉ tiêu bảng CĐKT:** là một chỉ tiêu tương ứng trong bảng CĐKT.&#x20;

## Giá trị trả về

Giá trị một chỉ tiêu trong bảng cân đối kế toán

## Các chỉ tiêu bảng cân đối kế toán

### Các chỉ tiêu của bảng cân đối kế toán của các Doanh nghiệp thông thường:

* **TotalCurrentAssets**: Tổng tài sản ngắn hạn&#x20;
* **Cash:** Tiền mặt
* **CashEquivalents:** Tương đương tiền
* **ShortTermFinancialInvestment:** Các khoản đầu từ tài chính ngắn hạn
* **TotalShortTermReceivable:** Tổng các khoản phải thu ngắn hạn&#x20;
* **ShortTermAccountsReceivable:** Phải thu ngắn hạn của người mua&#x20;
* **TotalInventories:** Tổng hàng tồn kho
* **ShortTermPrepaidExpenses:** Chi phí trả trước ngắn hạn&#x20;
* **TotalNonCurrentAssets:** Tổng tài sản dài hạn&#x20;
* **TotalLongTermReceivable:** Tổng các khoản phải thu dài hạn
* **LongTermAccountsReceivable:** Phải thu dài hạn của người mua&#x20;
* **LongTermFinancialInvestment:** Các khoản đầu tư tài chính dài hạn&#x20;
* **FixedAssets:** &#x20;
* **TangibleAssets:**
* **IntangibleAssets:**&#x20;
* **RealEstateInvest:**&#x20;
* **InProgressLongTermAssets:**&#x20;
* **TotalOtherNonCurrentAssets:**
* **TotalShortTermLiabilities:**&#x20;
* **ShortTermInterestBearingLiabilities:**&#x20;
* **ShortTermAccountsPayable:**
* **TotalLongTermLiabilities:**&#x20;
* **LongTermInterestBearingLiabilities:**&#x20;
* **LongTermAccountsPayable:**
* **ConvertibleBonds:**&#x20;
* **StockHolderEquity:**&#x20;
* **AccumulatedDeficit:**&#x20;
* **TreasuryStock:**&#x20;
* **RetainedProfits:**
* **TotalCapital:**

### Các chỉ tiêu của bảng cân đối kế toán của các Ngân hàng:

* CustomersLoans, RiskProvisionsForCustomersLoans, CashGoldJewelry,DepositsAtStateBank, DepositsAtOtherCreditInstitutions, InvestmentSecurities, TotalInterestEarningAssets, DerivativeFinancialInstrumentsAndOtherFinancialAssets, TradingSecurities, LongTermInvestmentCapitalContribution, FixedAssets, InTangibleAssets, InvestmentRealEstate, OtherAssets, TotalNonInterestEarningAssets, TotalAssets, DepositOfCustomers, DebtToGovernmentAndStateBank, DepositsAndBorrowingsFromOtherCreditInstitutions, FinancingCapitalsInvestmentTrustRiskBearingLoans, IssuingValuablePapers, TotalInterestBearingLiabilities, DerivativeFinancialInstrumentsAndOtherFinancialLiabilities, OtherLiabilities, TotalNonInterestBearingLiabilities, TotalLiabilities, EquityAndFunds, EquityAttributableToNonControllingShareholders, TotalEquity, TotalLiabilitiesAndEquity
