<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [bitburner](./bitburner.md) &gt; [TIX](./bitburner.tix.md) &gt; [sell](./bitburner.tix.sell.md)

## TIX.sell() method

Attempts to sell shares of a stock using a Market Order.

If the specified number of shares in the function exceeds the amount that the player actually owns, then this function will sell all owned shares. Remember that every transaction on the stock exchange costs a certain commission fee.

The net profit made from selling stocks with this function is reflected in the script’s statistics. This net profit is calculated as:

shares \* (sell\_price - average\_price\_of\_purchased\_shares)

If the sale is successful, this function will return the stock price at which each share was sold. Otherwise, it will return 0.

<b>Signature:</b>

```typescript
sell(sym: StockSymbol, shares: number): number;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  sym | [StockSymbol](./bitburner.stocksymbol.md) | Stock symbol. |
|  shares | number | Number of shares to sell. Must be positive. Will be rounded to nearest integer. |

<b>Returns:</b>

number

The stock price at which each share was sold, otherwise 0 if the shares weren't sold.

## Remarks

2.5 GB
