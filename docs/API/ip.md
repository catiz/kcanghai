# 获取IP地址

此接口可用来指定IP地址归属地

每个IP地址归属地缓存时间为24小时

## 接口地址

```
https://api.kseas.cn/public/ip
```

## 使用方法

请使用 GET/POST 方法访问

必选参数

| 参数 | 作用                   |
| ---- | ---------------------- |
| ip   | 需要获取归属地的IP地址 |

## 使用示例

GET请求

```
https://api.kseas.cn/public/ip?ip=36.134.76.72
```

请求结果

```json
{
  "status": "success",
  "message": null,
  "result": {
    "ip": "36.134.76.72",
    "location": {
      "lng": 112.55067,
      "lat": 37.87059
    },
    "ad_info": {
      "nation": "中国",
      "province": "山西省",
      "city": "太原市",
      "district": "",
      "adcode": 140100,
      "nation_code": 156
    }
  }
}
```
