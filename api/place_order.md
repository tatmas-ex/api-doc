
## 下单接口
POST
`
/api/v1/orders
`



```
  access_key: 从平台获取的access_key
  price: 价格
  volume: 数量
  market: 市场，例如: btceth
  side: "buy|sell"
  signature: 签名
  tonce: 时间戳，精确到秒
```

返回示例

```
{
    "head": {
        "code": "1000",
        "msg": "Success."
    },
    "body": {
                "id": 375404588,
                "created_at": 1565580288,
                "updated_at": 1565580288,
                "ask": 70,
                "bid": 30,
                "price": "100",
                "volume": "17.43",
                "origin_volume": "17.43",
                "type": "OrderAsk",
                "member_id": 17605,
                "sn": "",
                "source": "APIv4",
                "ord_type": "limit",
                "locked": "17.43",
                "origin_locked": "17.43",
                "funds_received": "0",
                "trades_count": 0,
                "new_client_order_id": "",
                "market": "btcusdt",
                "state": "wait",
                "base_unit": "btc",
                "quote_unit": "usdt",
                "avg_price": "0",
                "total_ask_fee": "0",
                "total_bid_fee": "0"
            }
}
```
