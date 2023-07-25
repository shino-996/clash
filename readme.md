Clash Pro 配置文件

- 使用 [subconverter][subconverter] 生成
  [subconverter][subconverter] 功能太花花了，看完觉得都用不上，最后只用来解析机场的代理，没有使用其他功能，也只留了二进制和、一个配置文件（pref.yml)、和一个模板(clash.yaml)。
- 规则参考 [clash-rules][clash-rules] 项目，添加了几条公司内网等自用规则，并且配置了 DNS。

# 使用方式

- 在 pref.yml 中填上自己机场的订阅链接

```
  default_url:
  # 替换成机场的订阅链接
  - https://sub.91unicorn.club/api/v1/client/subscribe?token=token
```

- 使用 [subconverter][subconverter] 生成配置文件
  比如在 shell 直接执行:

```
./subconverter
```

更多用法参考 [subconverter][subconverter] 的官方文档。

- Clash Pro 中的托管配置链接这么填

```
http://127.0.0.1:25500/clashr
```

[subconverter]:https://github.com/tindy2013/subconverter
[clash-rules]:https://github.com/Loyalsoldier/clash-rules
