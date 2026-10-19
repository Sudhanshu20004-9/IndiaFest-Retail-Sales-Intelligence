# IndiaFest-Retail-Sales-Intelligence
Power BI analytics project exploring Indian retail sales, customer behavior, product performance, RFM segmentation, and festive-season trends.


IndiaFest Power BI Dataset
IMPORTANT: This is a synthetic/simulated dataset created for learning and portfolio demonstration. It is not actual sales data from a real Indian retailer.
Tables:
- FactSales: one row per order line; contains sales, cost, freight and profit.
- DimCustomer: customer attributes and Indian cities/states.
- DimProduct: product categories, brands and prices.
- DimDate: daily calendar, year/month fields and illustrative sale/festival periods.
- DimPayment: payment method lookup.
Relationship keys:
FactSales[ProductID] -> DimProduct[ProductID]
FactSales[OrderID] -> Orders table? Order-level attributes are embedded in FactSales in this starter pack only in a separate Orders file not included.
- FactOrders: one row per order; customer, date, payment, status, festival period and review score.
Relationships: FactOrders[OrderID] -> FactSales[OrderID] (1:*); FactOrders[CustomerID] -> DimCustomer[CustomerID]; FactOrders[PaymentKey] -> DimPayment[PaymentKey]; FactOrders[OrderDate] -> DimDate[Date]; FactSales[ProductID] -> DimProduct[ProductID].
