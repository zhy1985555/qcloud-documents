## 简介

本文档提供获取对象访问 URL 的代码示例。

## 获取对象访问 URL

#### 功能说明

获取对象访问 URL用于匿名下载或分发。

#### 方法原型

```
get_object_url(Bucket, Key)
```

#### 请求示例

```python
# -*- coding=utf-8
from qcloud_cos import CosConfig
from qcloud_cos import CosS3Client
import sys
import logging
import requests

# 正常情况日志级别使用INFO，需要定位时可以修改为DEBUG，此时SDK会打印和服务端的通信信息
logging.basicConfig(level=logging.INFO, stream=sys.stdout)

# 1. 设置用户属性, 包括 secret_id, secret_key, region等。Appid 已在CosConfig中移除，请在参数 Bucket 中带上 Appid。Bucket 由 BucketName-Appid 组成
secret_id = 'SecretId'     # 替换为用户的 SecretId，请登录访问管理控制台进行查看和管理，https://console.cloud.tencent.com/cam/capi
secret_key = 'SecretKey'   # 替换为用户的 SecretKey，请登录访问管理控制台进行查看和管理，https://console.cloud.tencent.com/cam/capi
region = 'ap-beijing'      # 替换为用户的 region，已创建桶归属的region可以在控制台查看，https://console.cloud.tencent.com/cos5/bucket
                           # COS支持的所有region列表参见https://cloud.tencent.com/document/product/436/6224
token = None               # 如果使用永久密钥不需要填入token，如果使用临时密钥需要填入，临时密钥生成和使用指引参见https://cloud.tencent.com/document/product/436/14048
scheme = 'https'           # 指定使用 http/https 协议来访问 COS，默认为 https，可不填

config = CosConfig(Region=region, SecretId=secret_id, SecretKey=secret_key, Token=token, Scheme=scheme)
client = CosS3Client(config)

# 生成URL
url = client.get_object_url(
    Bucket='examplebucket-1250000000',
    Key='exampleobject'
)
print(url)

# 使用URL
response = requests.get(url)
print(response)
```

#### 参数说明

| 参数名称   | 参数描述   |类型 | 必填 | 
| -------------- | -------------- |---------- | ----------- |
 | Bucket  |存储桶名称，由 BucketName-APPID 构成 |  String |  是 | 
 | Key  | 对象键（Key）是对象在存储桶中的唯一标识。例如，在对象的访问域名 `examplebucket-1250000000.cos-internal.ap-guangzhou.tencentcos.cn/doc/pic.jpg` 中，对象键为 doc/pic.jpg | String | 是 | 

#### 返回结果说明

该方法返回值为对象访问的 URL。
