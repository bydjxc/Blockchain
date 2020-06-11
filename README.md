# Blockchain
# 1.区块链入门

## 1.1.区块链前世今生

密码朋克(Cypherpunk)：

​		密码朋克（cypherpunk），1993年在Eric Hughes’的《A Cypherpunk’s Manifesto》中出现的一个术语，它结合了电脑朋克的思想，使用强加密（密文）保护个人隐私。

​		20世纪80年代末开始，一股“密码朋克”的潮流悄然兴起。其参与者是一批神秘的“极客天才”，他们提倡大规模使用**强加密算法**来保护自身基本自由免受攻击，同时**反对任何政府规则**的密码系统。该联盟没有正式的领导阶层，一般情况下通过加密邮件列表进行联系。

​		1992年，英特尔的高级科学家Tim May最先发起这一加密邮件列表组织。而“密码朋克”这一术语的首次出现，则是在1993年埃里克·休斯出版书《密码朋克宣言》上。

​		该邮件列表内上千名用户，主要讨论包括数学、加密技术、计算机技术、政治、哲学等方面的内容。其早期成员有不少IT精英，

比如：

“维基解密”创始人Julian Assange、朱利安·阿桑奇

BT下载支付Bram Cohen、布拉姆·科恩

万维网发明者Tim Berners-Lee、蒂姆·伯纳斯·李

智能合约概念提出者Nick Szabo、尼克·萨博

Facebook创始人之一Sean Parker、肖恩·帕克

中本聪等。

​		《比特币白皮书：一种点对点的电子现金系统》最早就是在“密码朋克”邮件列表上发布的。此外据不完全统计，在比特币出现之前，密码朋克内成员至少讨论及发表过十种以上类似的数字货币及支付系统，比如E-cash、B-money，不过这些货币大都以失败告终。

- Adam Back发明 Hashcash,使用了POW

- Haber/ Stornetta提出时间戳方法保证数字文件安全的协议
- 戴伟发明了B- money,强调点对点交易和不可更改记录
- 哈尔-芬尼推出了“加密现金
- 2008年中本聪《比特币:ー个点对点的电子现金系统》
- 比特币
- 区块链

## 1.2.区块链前景

应用场景：

- 资产:数字资产发行、支付(跨境支付)、交易、结算
- 记账:股权交易、供应链金融、商业积分
- 不可算改:溯源、众筹、医疗证明、存在性证明
- 点对点:共享经济、物联网
- 隐私:匿名交易

人才缺口巨大：

## 1.3.比特币是什么

- 比特币是数字货币

- 什么是货币
  凯恩斯《货币论》货币是可以承载价值的一般等价物

- 货币历史

  ​	铜币、金银

  ​	银票

  ​	法币

- 数字货币

  ​	一串数字

- 信任从何而来

  ​	财产只受自己控制

  ​	无通胀

  ​	没有假钞

  ​	流通性好

- 去中心化记账系统

  ​	数据以节点方式保存

  ​	每一个用户都存有所有用户的数据

## 1.4.比特币原理

- 账本如何验证

  ​	![1564732337135](C:\Users\kevin\AppData\Roaming\Typora\typora-user-images\1564732337135.png)

  张三修改金额30 为300

  ![1564732367324](C:\Users\kevin\AppData\Roaming\Typora\typora-user-images\1564732367324.png)

  - 方案1
    			一一核对账本记录
    			少数服从多数
    			No!!!

  -  Hash
             哈希函数:Hash(原始信息)=摘要信息

    ​	特点：

    ​			同样的原始信息用同一个哈希函数总能得到相同的摘要信息
    ​			原始信息任何微小的变化都会哈希出面目全非的摘要信息
    ​			从摘要信息无法逆向推算出原始信息

    ![1564732820376](C:\Users\kevin\AppData\Roaming\Typora\typora-user-images\1564732820376.png)

  - 区块

    ​		![1564732863992](C:\Users\kevin\AppData\Roaming\Typora\typora-user-images\1564732863992.png)

    ![1564732954900](C:\Users\kevin\AppData\Roaming\Typora\typora-user-images\1564732954900.png)

    ![1564732972857](C:\Users\kevin\AppData\Roaming\Typora\typora-user-images\1564732972857.png)

    

- 所有权问题

  - 银行系统

  - 银行开户

  - 银行记账

  - 比特币系统

    ​	点对点交易

    ​	没有第三方

  - 账户->地址

    {

    "付款地址”:"2A39CBa2390FDe
    "收款地址":"AAC9CBa239aFcc
    金额":"0.2btc"

    }

  - 密码->私钥

    ​	地址:2A39CBa239FDe
    ​	私钥: sdghsdninihdsgakihkgnakgaihnkhiskdgal
    ​	Hash( Hash(fun(sdghsdninihdsgakihkgnakgaihnkhiskdgal)))-> 2A39CBA2390FDE

  - 非对称加密技术（交易签名）

    ​		交易进行hash得到摘要
    ​		用私钥对摘要进行签名

  - 签名过程

    ​	hash

    ![1564733811048](C:\Users\kevin\AppData\Roaming\Typora\typora-user-images\1564733811048.png)

    签名

    ![1564733834355](C:\Users\kevin\AppData\Roaming\Typora\typora-user-images\1564733834355.png)

  - 广播交易

    ​	![1564733906475](C:\Users\kevin\AppData\Roaming\Typora\typora-user-images\1564733906475.png)

  - 验证

    ​	![1564733936176](C:\Users\kevin\AppData\Roaming\Typora\typora-user-images\1564733936176.png)

  - 签名及验证

    ​	![1564734025170](C:\Users\kevin\AppData\Roaming\Typora\typora-user-images\1564734025170.png)

    

- 为什么记账（挖坑）

  ​	记账：Hash打包

  ​	消耗资源

  ​	奖励

  ​	规则

  ​		一段时间内只有一人可以记账成功
  ​		通过解决密码学难题(即工作量证明)竟争获得唯一记账权

  ​		其他节点复制记账结果

  工作量证明

  ​		Hash(上ー个Hash值,交易记录集)=456635BCD
  ​		Hash(上ー个Hash值,交易记录集,随机数)=0000aFD635BCD

  交易的记录集

  ​		收集广播中还没有被记录账本的交易
  ​		交易的有效性验证

  ​		添加一笔给自己转账的交易(挖矿奖励)

  工作量分析

  ​		![1564734587634](C:\Users\kevin\AppData\Roaming\Typora\typora-user-images\1564734587634.png)

  

- 以谁的账本为准

  两个节点同时完成工作量证明,使用谁的区块?

  **共识机制**

  - 为什么要遵守协议?

    ​	节点工作量只有在其他的节点认同其是有效的

  - 累计工作量最大的区块链

    ​	独立

    ​	延长最长链

  - 分叉

    ​	

拓展：

比特币P2P网络
区块结构 Merkle树
比特币UTXO及交易脚本
比特币白皮书