## 全部市场接口
GET
`
/api/v1/markets
`

返回示例
```
head: {
  code: "1000",
  msg: "success"
}
body: {
  [
    {
      id: "btcusdt",  // 交易对的标示
      name: "BTC/USDT",
      logo: "xxxx/icons/btc.png",
      coinmarketcap_url: "",
      code: 82,
      base_unit: "btc",
      quote_unit: "usdt",
      price_group_fixed: "8",
      sort_order: 1,
      bid: {
        fee: "0.001",
        currency: "usdt",
        fixed: 8  // 价格小数位精度
      },
      ask: {
        fee: "0.001",
        currency: "btc",
        fixed: 8  // 数量小数位精度
      },
      visible: true, // 是否为开放使用的交易对
      tradable: true,
      scalp_market: true,
      watt_market: false,
      rise_limit: "0",
      decline_limit: "0"
    },
    {
      id: "ethusdt",
      name: "ETH/USDT",
      logo: "xxx/icons/eth.png",
      coinmarketcap_url: "",
      code: 47,
      base_unit: "eth",
      quote_unit: "usdt",
      price_group_fixed: "8",
      sort_order: 2,
      bid: {
        fee: "0.001",
        currency: "usdt",
        fixed: 6
      },
      ask: {
        fee: "0.001",
        currency: "eth",
        fixed: 8
      },
      visible: true,
      tradable: true,
      scalp_market: true,
      watt_market: false,
      rise_limit: "0",
      decline_limit: "0"
    },
    {
      id: "ethusdt",
      name: "ETH/USDT",
      logo: "xxx/icons/eth.png",
      coinmarketcap_url: "",
      code: 99,
      base_unit: "eth",
      quote_unit: "usdt",
      price_group_fixed: "8",
      sort_order: 3,
      bid: {
        fee: "0.001",
        currency: "usdt",
        fixed: 6
      },
      ask: {
        fee: "0.001",
        currency: "eth",
        fixed: 2
      },
      visible: true,
      tradable: true,
      scalp_market: false,
      watt_market: false,
      rise_limit: "0.1",
      decline_limit: "0"
    },
    // 以下省略....
  ]
}
```
