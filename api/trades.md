
## 成交查询接口
GET
`
/api/v1/trades/my
`

参数在query部分传递

```
  access_key: 从平台获取的access_key
  signature: 签名
  tonce: 时间戳，精确到秒
  
  market 市场，
  page 当前页，默认1
  limit 每页多少条记录，默认30
  order 排序方式，asc/desc二选一, 默认不传为 desc
  min_id 指定查询ID大于此值的记录，默认不使用
```

返回示例

```
{
    "head": {
        "code": "1000",
        "msg": "Success."
    },
    "body": [
            {
                "id": 25285189,
                "created_at": 1563148340,
                "updated_at": 1563148340,
                "price": "7.02",
                "volume": "71.5548725",
                "trend": 1,
                "funds": "502.31520495",
                "side": "sell",
                "market": "usdtbtc",
                "ask_member_id": 17605,
                "bid_member_id": 211961,
                "ask_fee": {
                    "currency_id": 23,
                    "currency_code": "usdt",
                    "amount": "0.0715548725"
                },
                "bid_fee": {
                    "currency_id": 30,
                    "currency_code": "btc",
                    "amount": "0.50231520495"
                }
            },
            {
                "id": 25284189,
                "created_at": 1563146890,
                "updated_at": 1563146890,
                "price": "7.02",
                "volume": "1.03212069",
                "trend": 1,
                "funds": "7.2454872438",
                "side": "sell",
                "market": "usdtbtc",
                "ask_member_id": 17605,
                "bid_member_id": 92987,
                "ask_fee": {
                    "currency_id": 23,
                    "currency_code": "usdt",
                    "amount": "0.00103212069"
                },
                "bid_fee": {
                    "currency_id": 30,
                    "currency_code": "btc",
                    "amount": "0.0072454872438"
                }
            },
           ..... // 省略更多
]
}
```
