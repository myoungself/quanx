# 参考来源
墨鱼：https://github.com/ddgksf2013

【版权归墨鱼所有，修改只供个人使用】


# 修改地方

1. [policy] 增加一个 crypto 的策略。

> static=Crypto, 香港节点, 台湾节点, 日本节点, 狮城节点, 美国节点, proxy, img-url=https://raw.githubusercontent.com/myoungself/quanx/dev/icon/crypto.png


2. [filter_remote] 修改两个地方：

- 修改全球加速的规则链接，去掉原先链接的里 crypto 的部分
> https://raw.githubusercontent.com/myoungself/quanx/dev/rules/Proxy.list, tag=全球加速, force-policy=全球加速, update-interval=172800, opt-parser=true, enabled=true

- 增加一个crypto的规则
> https://raw.githubusercontent.com/myoungself/quanx/dev/rules/CryptoHK.list, tag=Crypto, force-policy=Crypto, update-interval=172800, opt-parser=true, enabled=true
