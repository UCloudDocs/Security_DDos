{{indexmenu_n>5}}

# UCloud黑洞策略

## 什么是黑洞？

黑洞是指当外网IP的入向流量速率超过其所在数据中心的限定阈值时，该IP会触发流量封堵机制，即对该IP的访问流量会被丢弃。

## 黑洞策略的必要性

为什么会有黑洞策略？为什么不能直接帮用户免费抗攻击？

1.  发生大流量攻击时，除了被攻击者，整个云网络都会受到影响，为了避免影响范围扩大，所以需要有黑洞策略。
2.  DDoS防御需要两方面的成本：1）带宽成本，2）清洗成本。最大的成本就是带宽费用，而收取带宽费用的联通、电信、移动等运营商不会区分是正常流量还是攻击流量。UCloud会尽力为客户提供基础的攻击防御，但是当攻击超过限定的阈值就需要采取黑洞策略封堵IP。

## 黑洞时长多久？

对于被封堵的IP，一般会在24小时后进行解封。

<wrap em>注意：

针对最近一周内触发封堵机制超过3次的用户，UCloud保留延长封堵时间、限制购买外网IP及解绑并冻结外网IP等措施的权利。</wrap>

## 被黑洞了怎么办？

如果不希望被黑洞，希望避免DDoS攻击影响业务应该怎么办？

**如果是境内的机房：**

受到攻击后，为了避免IP再被攻击而影响业务，建议更换源站IP并接入
[高防](https://www.ucloud.cn/site/product/uads.html) 进行防护。

**如果是境外的机房：**

受到攻击后，无需更换源站IP，采用境外防护服务，保证业务的正常进行。

## 附：各数据中心的防护阈值

### 境内机房

| 地域名称 | 下属可用区    | 防护阈值  |
| ---- | -------- | ----- |
| 北京一  | 可用区A     | 3Gbps |
| 北京二  | 可用区B/C/D | 3Gbps |
| 上海一  | 上海可用区A   | 2Gbps |
| 上海二  | 上海可用区A/B | 2Gbps |
| 广东   | 广东可用区B   | 2Gbps |

### 境外机房

<table>
<thead>
<tr class="header">
<th>地域名称</th>
<th>下属可用区</th>
<th>防护阈值</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>香港</td>
<td>香港可用区A/B</td>
<td>1Gbps<br />
回大陆线路500Mbps</td>
</tr>
<tr class="even">
<td>洛杉矶</td>
<td>洛杉矶可用区A</td>
<td>1Gbps</td>
</tr>
<tr class="odd">
<td>华盛顿</td>
<td>华盛顿可用区A</td>
<td>1Gbps</td>
</tr>
<tr class="even">
<td>法兰克福</td>
<td>法兰克福可用区A</td>
<td>1Gbps</td>
</tr>
<tr class="odd">
<td>曼谷</td>
<td>曼谷可用区A</td>
<td>1Gbps</td>
</tr>
<tr class="even">
<td>首尔</td>
<td>首尔可用区A</td>
<td>700Mbps</td>
</tr>
<tr class="odd">
<td>新加坡</td>
<td>新加坡可用区A</td>
<td>1Gbps</td>
</tr>
<tr class="even">
<td>高雄</td>
<td>高雄可用区A</td>
<td>1Gbps</td>
</tr>
<tr class="odd">
<td>莫斯科</td>
<td>莫斯科可用区A</td>
<td>1Gbps</td>
</tr>
<tr class="even">
<td>东京</td>
<td>东京可用区A</td>
<td>1Gbps</td>
</tr>
<tr class="odd">
<td>台北</td>
<td>台北可用区A</td>
<td>1Gbps</td>
</tr>
<tr class="even">
<td>迪拜</td>
<td>迪拜可用区A</td>
<td>1Gbps</td>
</tr>
<tr class="odd">
<td>雅加达</td>
<td>雅加达可用区A</td>
<td>1Gbps</td>
</tr>
<tr class="even">
<td>孟买</td>
<td>孟买可用区A</td>
<td>1Gbps</td>
</tr>
<tr class="odd">
<td>圣保罗</td>
<td>圣保罗可用区A</td>
<td>1Gbps</td>
</tr>
<tr class="even">
<td>伦敦</td>
<td>伦敦可用区A</td>
<td>1Gbps</td>
</tr>
<tr class="odd">
<td>拉各斯</td>
<td>尼日利亚可用区A</td>
<td>900Mbps</td>
</tr>
<tr class="even">
<td>胡志明市</td>
<td>胡志明市可用区A</td>
<td>1Gbps</td>
</tr>
</tbody>
</table>

<wrap em>注意：香港机房如果回大陆线路超过了500M则会封堵。</wrap>
