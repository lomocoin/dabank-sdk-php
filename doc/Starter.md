# 开始使用

## 注册bigbang账号

注册bigbang账号(注册方式待补充). 并上传你的RSA公钥, 妥善保管你的RSA私钥和bigbang分配给你的App id及bigbang的公钥.

## Prerequisite

- PHP 5.4+

- curl

- openssl

## 安装

待补充.

## 如何使用Api


首先创建`Bigbang\Client`.

```php
$client = new Client(
    $gateway,
    '1',
    $appId,
    $appPrivKey,
    $bigbangPubKey
);
```

随后, 可以通过`$client->api($apiName)`获得你想使用的Api的包装对象, 然后根据业务需要调用该对象的对应方法. 

目前可用的`$apiName`:

- transfer

  交易相关

- address

  币种地址相关
  
- app
  
  应用的账户信息等
  
- debug
  
  用于调试
  
- utils

  辅助工具
  
  