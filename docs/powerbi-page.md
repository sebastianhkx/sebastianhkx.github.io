# Power BI

## Data Analysis Expressions (DAX)
```
CurrencyRates = 
DATATABLE(
    "Currency", STRING,
    "Exchange Rate", DOUBLE,
    {
        {"SGD", 1.00},
        {"USD", 1.35}
    }
)
```
Unit Price = 
VAR ExchangeRate = 1.35 -- Conversion rate from USD to SGD
VAR AdjustedCost = 
    SWITCH(
        TRUE(),
        SELECTEDVALUE('Raw Inv'[Currency]) = "USD", MAX('Raw Inv'[Cost Transacted Currency]) * ExchangeRate,
        MAX('Raw Inv'[Cost Transacted Currency]) -- No conversion for non-USD currencies
    )
RETURN
    DIVIDE(AdjustedCost, MAX('Raw Inv'[Quantity]), 0)



### functions 
### statements 