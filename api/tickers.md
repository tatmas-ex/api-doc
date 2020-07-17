
## 单个行情接口
GET
`
/api/v1/tickers/ethusdt
`

```
{
    "head": {
        "code": "1000",
        "msg": "Success."
    },
    "body": {
		at: 1563260065,
		name: "ethusdt",
		price_group_fixed: "8",
		ticker: {
			buy: "1600",
			sell: "1615",
			low: "1565",
			high: "1811.161898",
			last: "1608.579917",
			vol: "15213.6128",
			open: "1569.590102"
		},
		base_unit: "eth",
		quote_unit: "usdt",
	}
}
```


## 全部行情接口
GET
`
/api/v1/tickers
`

```
{
    "head": {
        "code": "1000",
        "msg": "Success."
    },
    "body": [
		{
			at: 1563260065,
			name: "ethusdt",
			price_group_fixed: "8",
			ticker: {
				buy: "1600",
				sell: "1615",
				low: "1565",
				high: "1811.161898",
				last: "1608.579917",
				vol: "15213.6128",
				open: "1569.590102"
			},
			base_unit: "eth",
			quote_unit: "usdt",
		},
		// 以下省略....
	]
}
```
