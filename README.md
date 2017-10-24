## 通讯方式: http(s)+json api

**json数据通过body传输**

### 1. 新订单(青云推给门丁)

```json
{
  "orderNo": "qingyun-5888888",//订单号
  "roomNum": "509",//房间号
  "totalPrice": "12.35",//订单总价格
  "createTime": "2015-13-32 10:00:00",//创建时间
  "payTime": "2017-13-31 10:00:00",//支付时间
  "payType": "WECHAT",//付款方式
  "itemList": [
        {
            "productCode": "qingyun-0215457878",//商品编码
            "price": "12.23",//价格
            "productName": "方便面",//商品名称
            "amount": 10 //购买数量
        }
   ]
}
```



### 2. 订单状态变化(门丁推给青云)

```json
{
  "orderNo": "xxdfdfdfd",
  "status": 0// 0 已确认
}
```
