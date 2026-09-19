# IPLC 流量计费：双向流量怎么算、超量会怎样，MKCloud 各线路套餐价格与选购清单

买 IPLC 专线 VPS 的人，十个里有八个会卡在同一个问题上：页面上写的"1TB 流量/月"，到底是怎么个用法？上传算不算？下载算不算？用超了是扣钱还是直接停机？这篇文章把 MKCloud 官网目前在售的 IPLC 流量计费套餐逐一拉出来，讲清计费规则、各档价格和适用场景，最后帮你算一笔账：到底该买哪一档。

## 先把规则说清楚：IPLC 流量计费到底怎么算

MKCloud 官方知识库对计费方式的描述很明确，几个关键点直接决定你的使用体验：

**流量按双向统计。** 上行加下行的总量都计入套餐额度。这一点和部分只计算出站的海外 VPS 商家不同。标 1TB 就是上行+下行合计 1TB，跑直播推流或大文件传输时要把消耗算双倍。

**超量后暂停，不是按量扣费。** 套餐流量用完后机器会停机，不会产生账单外的流量费。后续有两个补救办法：自助购买流量重置，或者提交工单补差价升级到更高档位。

**共享带宽只承诺峰值。** 流量计费套餐对应的带宽（比如 200M、300M）都是共享带宽的峰值上限，不保证任何时刻都能跑满。这和独享带宽产品是两种计费资源，后面会专门对比。

**流量是月度额度。** 按自然计费周期统计，月付套餐每月重置。

这些规则看起来限制不少，但换个角度想：超量停机意味着成本完全可预期，不存在"月底收到一张天价流量账单"的惊喜。对预算敏感的跨境业务来说，这反而好规划。

## MKCloud 在售的 IPLC 流量计费套餐全表

下面三张表的数据全部来自 MKCloud 官方商店页当前展示的套餐，均为月付价格，单位人民币。

**沪日 IPLC（上海-日本，端内延迟 25~28ms，上海电信入口，日本 BGP 出口）**

| 套餐 | CPU/内存 | 硬盘 | 带宽峰值 | 月流量 | 价格 | 购买 |
| --- | --- | --- | --- | --- | --- | --- |
| 1TB 流量 | 1核2GB | 20GB | 200M | 1TB | ¥358/月 | [ 查看沪日 1TB 套餐](https://www.mkcloud.net/aff.php?aff=390&url=https%3A%2F%2Fwww.mkcloud.net%2Findex.php%2Fstore%2Fsh-jp-sh) |
| 2TB 流量 | 2核4GB | 40GB | 300M | 2TB | ¥568/月 | [ 查看沪日 2TB 套餐](https://www.mkcloud.net/aff.php?aff=390&url=https%3A%2F%2Fwww.mkcloud.net%2Findex.php%2Fstore%2Fsh-jp-sh) |
| 4TB 流量 | 2核4GB | 40GB | 300M | 4TB | ¥998/月 | [ 查看沪日 4TB 套餐](https://www.mkcloud.net/aff.php?aff=390&url=https%3A%2F%2Fwww.mkcloud.net%2Findex.php%2Fstore%2Fsh-jp-sh) |
| 6TB 流量 | 4核8GB | 60GB | 500M | 6TB | ¥1388/月 | [ 查看沪日 6TB 套餐](https://www.mkcloud.net/aff.php?aff=390&url=https%3A%2F%2Fwww.mkcloud.net%2Findex.php%2Fstore%2Fsh-jp-sh) |
| 10TB 流量 | 4核8GB | 60GB | 500M | 10TB | ¥2288/月 | [ 查看沪日 10TB 套餐](https://www.mkcloud.net/aff.php?aff=390&url=https%3A%2F%2Fwww.mkcloud.net%2Findex.php%2Fstore%2Fsh-jp-sh) |
| 20TB 流量 | 4核8GB | 60GB | 1G | 20TB | ¥4500/月 | [ 查看沪日 20TB 套餐](https://www.mkcloud.net/aff.php?aff=390&url=https%3A%2F%2Fwww.mkcloud.net%2Findex.php%2Fstore%2Fsh-jp-sh) |

**沪港 IPLC（上海-香港，端内延迟 21ms，上海电信入口，香港 BGP 出口）**

| 套餐 | CPU/内存 | 硬盘 | 带宽峰值 | 月流量 | 价格 | 购买 |
| --- | --- | --- | --- | --- | --- | --- |
| 1TB 流量 | 1核2GB | 20GB | 200M | 1TB | ¥288/月 | [ 查看沪港 1TB 套餐](https://www.mkcloud.net/aff.php?aff=390&url=https%3A%2F%2Fwww.mkcloud.net%2Findex.php%2Fstore%2Fsh-hk-sh) |
| 2TB 流量 | 2核4GB | 40GB | 300M | 2TB | ¥428/月 | [ 查看沪港 2TB 套餐](https://www.mkcloud.net/aff.php?aff=390&url=https%3A%2F%2Fwww.mkcloud.net%2Findex.php%2Fstore%2Fsh-hk-sh) |
| 4TB 流量 | 2核4GB | 40GB | 300M | 4TB | ¥696/月 | [ 查看沪港 4TB 套餐](https://www.mkcloud.net/aff.php?aff=390&url=https%3A%2F%2Fwww.mkcloud.net%2Findex.php%2Fstore%2Fsh-hk-sh) |
| 6TB 流量 | 4核8GB | 60GB | 500M | 6TB | ¥988/月 | [ 查看沪港 6TB 套餐](https://www.mkcloud.net/aff.php?aff=390&url=https%3A%2F%2Fwww.mkcloud.net%2Findex.php%2Fstore%2Fsh-hk-sh) |
| 10TB 流量 | 4核8GB | 60GB | 500M | 10TB | ¥1536/月 | [ 查看沪港 10TB 套餐](https://www.mkcloud.net/aff.php?aff=390&url=https%3A%2F%2Fwww.mkcloud.net%2Findex.php%2Fstore%2Fsh-hk-sh) |
| 20TB 流量 | 4核8GB | 60GB | 1G | 20TB | ¥3072/月 | [ 查看沪港 20TB 套餐](https://www.mkcloud.net/aff.php?aff=390&url=https%3A%2F%2Fwww.mkcloud.net%2Findex.php%2Fstore%2Fsh-hk-sh) |

**沪美 IPLC（上海-美国，端内延迟 124~134ms，上海电信入口，美国 BGP 出口）**

| 套餐 | CPU/内存 | 硬盘 | 带宽峰值 | 月流量 | 价格 | 购买 |
| --- | --- | --- | --- | --- | --- | --- |
| 1TB 流量 | 1核2GB | 20GB | 200M | 1TB | ¥428/月 | [ 查看沪美 1TB 套餐](https://www.mkcloud.net/aff.php?aff=390&url=https%3A%2F%2Fwww.mkcloud.net%2Findex.php%2Fstore%2Fsh-us-sh) |
| 2TB 流量 | 2核4GB | 40GB | 300M | 2TB | ¥698/月 | [ 查看沪美 2TB 套餐](https://www.mkcloud.net/aff.php?aff=390&url=https%3A%2F%2Fwww.mkcloud.net%2Findex.php%2Fstore%2Fsh-us-sh) |
| 4TB 流量 | 2核4GB | 40GB | 300M | 4TB | ¥1258/月 | [ 查看沪美 4TB 套餐](https://www.mkcloud.net/aff.php?aff=390&url=https%3A%2F%2Fwww.mkcloud.net%2Findex.php%2Fstore%2Fsh-us-sh) |
| 6TB 流量 | 4核8GB | 60GB | 500M | 6TB | ¥1758/月 | [ 查看沪美 6TB 套餐](https://www.mkcloud.net/aff.php?aff=390&url=https%3A%2F%2Fwww.mkcloud.net%2Findex.php%2Fstore%2Fsh-us-sh) |
| 10TB 流量 | 4核8GB | 60GB | 500M | 10TB | ¥2888/月 | [ 查看沪美 10TB 套餐](https://www.mkcloud.net/aff.php?aff=390&url=https%3A%2F%2Fwww.mkcloud.net%2Findex.php%2Fstore%2Fsh-us-sh) |
| 20TB 流量 | 4核8GB | 60GB | 1G | 20TB | ¥5666/月 | [ 查看沪美 20TB 套餐](https://www.mkcloud.net/aff.php?aff=390&url=https%3A%2F%2Fwww.mkcloud.net%2Findex.php%2Fstore%2Fsh-us-sh) |

所有套餐都附带一对独立 IPv4（入口+出口各一个），系统可选 Ubuntu、Debian、CentOS、AlmaLinux 等主流发行版，下单后自动开通。顺带提一句，第三方测评站 VPS.Dance 早前测过沪美线的 100GB 小档（¥198/月），但那个档位在当前官方商店页已经不再展示，实际以商店实时标价为准。

## 和独享带宽计费差在哪：一笔账算明白

MKCloud 每条 IPLC 线路都同时提供"流量计费（共享带宽）"和"带宽计费（独享带宽）"两种类型。沪美线的独享档目前官方商店标价如下：

| 套餐 | CPU/内存 | 独享带宽 | 月流量 | 价格 |
| --- | --- | --- | --- | --- |
| 5M 独享 | 2核4GB | 5Mbps | 不限 | ¥800/月 |
| 10M 独享 | 2核4GB | 10Mbps | 不限 | ¥1100/月 |
| 20M 独享 | 2核4GB | 20Mbps | 不限 | ¥2100/月 |
| 50M 独享 | 4核8GB | 50Mbps | 不限 | ¥5000/月 |
| 100M 独享 | 4核8GB | 100Mbps | 不限 | ¥9000/月 |

（更高还有 200M、300M 档，月付分别到 ¥18000 和 ¥27000，属于明确的企业级预算了。）

[👉 对比沪美独享带宽套餐](https://www.mkcloud.net/aff.php?aff=390&url=https%3A%2F%2Fwww.mkcloud.net%2Findex.php%2Fstore%2Fsh-us-ex)

关键问题是：同样花几百块，选哪种？官方知识库给过一个沪港线的对照，思路可以直接搬过来用。独享 5M 带宽如果持续跑满一个月，理论传输量约 1.5TB，折算下来每 GB 成本比流量计费更便宜；但前提是你真的能让带宽长时间保持满载。

所以判断标准很直接：

- **流量小、突发型**（收单、后台管理、低频采集）：流量计费划算。比如沪美 1TB 档 ¥428/月，就算全部用完，折合约 ¥0.42/GB，用不完更省。
- **流量大且持续**（直播推流、持续同步、数据回传）：独享带宽更划算，而且速率稳定，不受共享高峰影响。
- **介于两者之间**：先按双向口径估一个月的真实流量，再回头对比表格。官方知识库也建议记录一个有代表性的业务周期再下单。

一条线路上还有个容易被忽略的价差：沪日和沪港方向比沪美便宜，沪港 1TB 只要 ¥288，比沪美同流量便宜 140 元。业务对节点位置没硬性要求的话，选近的线路就是纯省钱。

## 对照项：上云互联（IXP）流量计费，更便宜但有前置条件

MKCloud 还有一条产品线经常和 IPLC 放在一起比：上云互联优化专线（IXP）。以沪港 IXP 为例，流量计费档位如下：

| 套餐 | CPU/内存 | 带宽峰值 | 月流量 | 价格 |
| --- | --- | --- | --- | --- |
| 2TB | 2核4GB | 500M | 2TB | ¥198/月 |
| 3TB | 2核4GB | 500M | 3TB | ¥288/月 |
| 6TB | 4核8GB | 1G | 6TB | ¥398/月 |
| 10TB | 4核8GB | 1G | 10TB | ¥666/月 |
| 20TB | 4核8GB | 1G | 20TB | ¥1290/月 |
| 30TB | 4核8GB | 2G | 30TB | ¥1900/月 |
| 50TB | 8核8GB | 2G | 50TB | ¥3120/月 |

[👉 查看沪港 IXP 流量计费套餐](https://www.mkcloud.net/aff.php?aff=390&url=https%3A%2F%2Fwww.mkcloud.net%2Findex.php%2Fstore%2Fcloud-sh-hk-sh)

2TB 只要 ¥198，单价不到沪港 IPLC 同流量的一半。便宜的原因是接入方式不同：IXP 产品**只允许云厂商 BGP 网络连入**（阿里云国内全网、腾讯云国内全网、百度云国内全网、火山云华东、华为云华东、UCloud 华东等），你需要自己有一台国内云服务器做前置，前置机器的费用要另外算。而 IPLC 产品用上海电信入口，直接拨号或普通网络就能连。

另外官网还有广港 IEPL 线（广州八线 BGP 入口，端内延迟 1~2ms，1TB 档 ¥358/月起），[👉 查看广港 IEPL 套餐](https://www.mkcloud.net/aff.php?aff=390&url=https%3A%2F%2Fwww.mkcloud.net%2Findex.php%2Fstore%2Fsh-hk-gd)。IEPL 和 IPLC 的计费结构一致，区别在底层线路形态，这里不展开。

简单说：已有国内云服务器、出口方向是港/日/美的，IXP 的流量计费档是全站性价比最高的一档；需要电信直连入口或者没有云前置的，走 IPLC。

## 下单前必须知道的几条限制

这些条款直接影响购买决策，全部来自官网下单页和知识库的明确说明：

- **实名认证**：产品需遵守中国法律，需要中国身份信息实名。
- **省级白名单**：IPLC 产品仅允许一个省份的 IP 连入，下单时选择省份，开通后可以修改。想防同行蹭网的，这个机制反而是加分项。
- **退款政策**：仅支持质量问题退款，而且需要提交具体、可验证的问题证明（准确的延迟数据、速度数据）。开通后不支持更换到其他地域。
- **用途限制**：禁止机场、回国等违法违规用途，违者清退不退款。
- **付款方式**：目前仅支持支付宝。
- **升降级**：需要提交工单处理，降级到更低价格套餐时差价不退。

买之前把这些过一遍，能省掉后面九成的扯皮。

## 优惠码怎么用

MKCloud 是 WHMCS 商店体系，优惠券在下单页的"优惠劵码"一栏填，登录后系统会显示你能用的券。官方知识库的活动回顾里出现过这些码：流量计费产品全场循环折扣码 **MK-8.8**、独享带宽产品首月折扣码 **MK-7.8**、IPLC 线路九折码 **MK-IPLC-WELCOME**、沪美/沪日 IXP 的 **US-6.9** / **JP-7.7** 等。

不过要注意，官方对已结束活动的标注很清楚：优惠码仅活动期内有效，历史折后价不能用来计算新订单。所以正确姿势是：先选好套餐，下单时登录账号查看优惠码栏实际可用的券，能叠加就填，不能就按原价对比其他家。[👉 进入商店查看当前价格](https://bit.ly/MKCLoud)

## 怎么估算自己该买哪一档

给你一个可以照抄的流程：

1. **按双向口径估流量**。把业务的上行流量和下行流量都列出来，相加后乘以 1.2 左右的冗余系数。比如每天推流 20GB，一个月就是 600GB，按双向和冗余算，实际要按 1.2TB 找档位。
2. **对照方向选线路**。日本方向看沪日表，美国方向看沪美表，香港方向先对比沪港 IPLC 和沪港 IXP 两张表，确认自己有没有云前置条件。
3. **检查档位边界**。用满一档的总成本 = 月租 + 可能的流量重置费；升到下一档的总成本 = 下一档月租。如果业务流量经常贴着档位上限跑，直接买大一级的档通常更省心。
4. **持续满载的场景切独享**。月流量估算超过 1.5TB 且几乎全天有传输的，独享带宽的每 GB 成本会反超流量计费，而且速率有保障。

最后补一句选购之外的实话：IPLC 流量计费这种模式，本质上是用"流量上限"换"价格下限"。它能便宜，是因为你替服务商承担了用量预测的责任——估得准，就是全站最划算的方案；估不准，超量停机比多花几十块难受得多。花一个晚上记录真实用量，比事后升级省的钱多得多。
