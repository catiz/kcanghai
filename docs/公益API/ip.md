# 获取IP地址

可用来获取本机IP地址以及归属地，或获取指定IP地址归属地

## 接口地址

```
https://api.kseas.cn/ip.php
```

## 使用方法

请使用GET方法访问

必选参数

| 参数 | 作用                   |
| ---- | ---------------------- |
| ip   | 需要获取归属地的IP地址 |

## 使用示例

GET请求

```
https://api.kseas.cn/ip.php?ip=8.8.8.8
```

请求结果

```json
{
  "status": 0,
  "message": "Success",
  "request_id": "f1ecb98c822f474a885fe78ee0789ebe",
  "result": {
    "ip": "8.8.8.8",
    "location": {
      "lat": 38.8833,
      "lng": -77
    },
    "ad_info": {
      "nation": "美国",
      "province": "",
      "city": "",
      "district": "",
      "adcode": -1,
      "nation_code": 840
    }
  }
}
```
