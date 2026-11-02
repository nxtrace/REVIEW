---
layout: default
title: "不换路由只提优先级？北京电信国际访问加速服务（163Plus）晚高峰双线对照实测"
seo_keywords: "北京电信, 163Plus, 国际加速, C–I, 晚高峰, MTR, iperf3"
---

# 不换路由只提优先级？北京电信国际访问加速服务（163Plus）晚高峰双线对照实测

<style>
.telecom163-table {
  max-width: 100%;
  overflow-x: auto;
  margin: 1rem 0 1.25rem;
  border: 1px solid var(--separator, #dde4ea);
  border-radius: 14px;
}
.telecom163-table table {
  display: table;
  width: 100%;
  min-width: 34rem;
  max-width: none;
  margin: 0;
  border-radius: 0;
}
.main-content:has(.telecom163-tariff) :is(h2, h3) {
  scroll-margin-top: 5rem;
}
img.telecom163-tariff {
  display: block;
  width: auto;
  max-width: min(100%, 440px);
  max-height: 65vh;
  height: auto;
  margin: 1rem auto;
}
</style>

晚高峰访问海外节点，开通北京电信“家庭宽带国际加速服务”（俗称 163Plus）能带来多大改善？本次实测在北京时间 21–23 点对比两条配置相同的家宽，涵盖六组空载 MTR 路由追踪与四组采用 BBR 的单连接 iperf3 反向下载测试。**163Plus 在四条测试路径上的单连接平均下载速率均显著提升，六组 MTR 末跳丢包率均降至 0%–0.6%。各路径的表现仍有差异：末跳 RTT 波动增大，部分节点出现吞吐骤降或密集重传。**

## 一、业务内容与开通后的变化

- **资费**：30 元/月，首月按天折算，限 200M 及以上 FTTH 家庭宽带办理。
- **办理与退订**：可通过 10000 号或线下渠道办理，订购后立即生效；可通过营业厅或 10000 号退订，次月生效。
- **有效期**：24 个月。到期前 30 日双方均未提出异议，每次自动续展 24 个月；无在网要求，无违约责任。

<img class="telecom163-tariff" src="/assets/images/beijing-telecom-163plus/official-service.jpg" alt="家庭宽带国际加速服务官方资费介绍">

*图 1：北京电信“家庭宽带国际加速服务”官方资费说明（方案编号：25BJ100098）*

除资费单列出的条款外，实测开通该业务后还有三项直接影响使用方式的变更（已向电信官方确认）：**IPv4 变为 CGNAT 内网地址、IPv6 被收回，且该业务与公网 IP 包互斥。** 下文分别用“普通家宽”和“163Plus 家宽”指代两条测试线路。

## 二、业务原理：同路由体系下的 C–I 段保障

此业务开通后仍走普通 163（AS4134）路由体系，核心变化在于 **C–I 段的转发保障**。C 是国内核心层，I 是国际出口层。海外服务器向北京家宽发送数据时，流量沿 I → C 方向通过这一段。

![C–I 段在下载方向上的逻辑位置](/assets/images/beijing-telecom-163plus/00-ci-principle.png)

*图 2：海外下载方向上的 C–I 段*

C–I 段（国内核心层至国际出口层）拥塞是普通 163 家宽晚高峰访问海外的主要瓶颈之一。163Plus 的核心机制是在不改变原有 AS4134 骨干路由的前提下，通过 QoS 提高用户流量在 C–I 段拥塞时的转发优先级与队列待遇。不过，按照 Luminous 的分层体系，海外流量进入国内前还需经过国际接入层（F）与国际交换层（X/S）。如果瓶颈出在海外上游互联端口（Peering/Transit）或海外 PoP 接入段（X–F），仅靠提升国内 C–I 段的转发优先级并不能拓宽海外侧的可用带宽，也不能改变跨境绕行路径。

## 三、测试方法与路径

两条宽带在**北京时间 21–23 点晚高峰**同时对比，有线设备和客户端配置相同。MTR 在空载时单独运行，保留逐跳记录并汇总末跳统计；ICMP 响应丢包率不等于 TCP 转发丢包率。iperf3 采用 BBR，单 TCP 流反向下载 15 秒，速率和 Retr 均取服务端 sender 日志。

```sh
iperf3 -t 15 -R -c <测试服务器>
```

<div class="telecom163-table" markdown="1">

| 本文标签 | 实际测试起点与路径 | iperf3 |
|---|---|---|
| FRA 163 · AWS FRA | AWS FRA → FRA 接入 163 | 有 |
| FRA TATA | FRA 节点 → TATA → 163 | 有 |
| LAX 163 · AWS PDX | AWS PDX → LAX 接入 163 | 有 |
| FRA Cogent · AWS SIN | AWS SIN → Cogent（经 FRA）→ 163 | 未测 |
| FRA 163 · AWS LHR | AWS LHR → FRA 接入 163 | 未测 |
| LAX Arelion | LAX 节点 → Arelion → 163 | 有 |

</div>

表中按**流量进入 163 骨干网前的接入点与上游运营商**命名标签，例如 AWS 新加坡样本经 Cogent 绕行法兰克福接入 163，故标记为 `FRA Cogent · AWS SIN`。

## 四、MTR：六组回程路由与逐跳表现

### FRA 163 · AWS FRA

[![FRA 163 · AWS FRA MTR 逐跳对照](/assets/images/beijing-telecom-163plus/mtr-fra-aws.png)](/assets/images/beijing-telecom-163plus/mtr-fra-aws.png)

*图 3：FRA 163 · AWS FRA 回程 MTR，左侧为 163Plus 家宽，右侧为普通家宽。*

两侧第 3 跳同为 AS4134 的 `81.173.22.57`。第 4 跳开始分开，163Plus 经 `202.97.83.161`，普通家宽经 `202.97.58.53`。两侧第 7 跳均进入 AS4847。163Plus 侧的 `219.141.152.62` 显示 99.8% 响应丢包，第 8 跳未响应，第 9 跳目标却是 0.0%。普通家宽侧第 8、9 跳仍有北京网内节点响应，第 10 跳未响应，第 11 跳到达目标，末跳丢包率为 9.9%。

### FRA TATA

[![FRA TATA MTR 逐跳对照](/assets/images/beijing-telecom-163plus/mtr-fra-tata.png)](/assets/images/beijing-telecom-163plus/mtr-fra-tata.png)

*图 4：FRA TATA 回程 MTR，左侧为 163Plus 家宽，右侧为普通家宽。*

xTom 第 2 跳分别为 `a1.cr01.fra01.xtom.de` 和 `a1.cr02.fra01.xtom.de`。两侧随后经过相同的 TATA（AS6453）ecore2、qcore2 节点，第 5 跳均由 `81.173.21.33` 响应。第 6 跳再次分开，分别为 `110.94.123.2` 和 `110.94.123.98`。进入北京 AS4847 后，163Plus 经 `106.37.255.118`、`36.112.226.157`，第 12 跳到达目标；普通家宽经 `106.37.254.102`、`1.203.89.153` 和 `36.112.226.174`，第 14 跳到达目标。

### LAX 163 · AWS PDX

[![LAX 163 · AWS PDX MTR 逐跳对照](/assets/images/beijing-telecom-163plus/mtr-lax-pdx.png)](/assets/images/beijing-telecom-163plus/mtr-lax-pdx.png)

*图 5：LAX 163 · AWS PDX 回程 MTR，左侧为 163Plus 家宽，右侧为普通家宽。*

两条路径连续经过第 3 跳 `218.30.53.149` 和第 4 跳 `202.97.43.109`。第 4 跳的响应丢包率分别为 68.9% 和 67.8%，到第 5 跳已分别降至 1.2% 和 0.0%。163Plus 在第 8 跳到达目标，末跳丢包率为 0.2%；普通家宽在第 11 跳到达，末跳为 13.3%。第 4 跳近七成的响应丢包未延续至后续节点，符合骨干路由器控制面 ICMP 限速的特征。真正拉开差距的是进入国内段后的表现。

### FRA Cogent · AWS SIN

[![FRA Cogent · AWS SIN MTR 逐跳对照](/assets/images/beijing-telecom-163plus/mtr-fra-cogent.png)](/assets/images/beijing-telecom-163plus/mtr-fra-cogent.png)

*图 6：FRA Cogent · AWS SIN 回程 MTR，左侧为 163Plus 家宽，右侧为普通家宽。*

起点在 AWS 新加坡。第 4–8 跳的 Cogent 主机名依次出现 `sin01 → mrs02 → par01 → fra05`，其中 `fra05` 连续出现两跳，对应新加坡经马赛、巴黎到法兰克福的方向。两侧第 4–9 跳完全相同，第 9 跳为 AS174 的 `149.11.228.55`，第 10 跳也都经过 `110.94.123.2`。到第 11 跳才出现不同的 AS4134 节点，分别为 `202.97.99.157` 与 `202.97.83.161`。这组按接入 163 前的上游标为 FRA Cogent；后段分别在第 15、17 跳到达目标。

普通家宽末跳丢包率为 **14.9%**（平均 RTT **200.4 ms**），163Plus 降至 **0.6%**（平均 RTT **211.7 ms**）。由于两条线路共用同一套 163 路由体系，新加坡流量均需绕行法兰克福接入电信；163Plus 压低了晚高峰丢包，但物理绕行带来的高基础时延依然存在。

### FRA 163 · AWS LHR

[![FRA 163 · AWS LHR MTR 逐跳对照](/assets/images/beijing-telecom-163plus/mtr-fra-lhr.png)](/assets/images/beijing-telecom-163plus/mtr-fra-lhr.png)

*图 7：FRA 163 · AWS LHR 回程 MTR，左侧为 163Plus 家宽，右侧为普通家宽。*

伦敦起点的两条路径同样在第 3 跳经过 `81.173.22.57`。与图 3 的法兰克福起点对照，四条记录在该节点重合。伦敦样本的第 4 跳分别为 `202.97.83.161` 和 `202.97.88.241`；其中 163Plus 一侧与法兰克福样本连续两跳相同。此后伦敦样本分别经 `202.97.54.53` 与 `202.97.54.65`，最终在第 9、10 跳到达目标。

### LAX Arelion

[![LAX Arelion MTR 逐跳对照](/assets/images/beijing-telecom-163plus/mtr-lax-arelion.png)](/assets/images/beijing-telecom-163plus/mtr-lax-arelion.png)

*图 8：LAX Arelion 回程 MTR，左侧为 163Plus 家宽，右侧为普通家宽。*

两侧均从 DMIT 网关出发，经 `irb-75.er01.lax.DMIT.com` 进入 Arelion 的 `twelve99.net`。第 4 跳分别为 `lax-bb2` 和 `lax-bb1`，第 5 跳又在 `lax-b22` 汇合，第 6 跳同为 `chinatelecom-ic-368151.ip.twelve99-cust.net`。交接后，163Plus 经 `202.97.93.137`，普通家宽经 `202.97.41.49`，分别在第 12、14 跳到达目标。163Plus 侧首跳响应丢包达 99.7%，但 2,221 次末跳探测的丢包率为 0.0%。

### 六组末跳对照

<div class="telecom163-table" markdown="1">

| 路径 | 线路 | Loss% | Snt | Avg / ms | StDev / ms |
|---|---|---|---|---|---|
| FRA 163 · AWS FRA | 163Plus 家宽 | 0.0% | 608 | 191.7 | 76.5 |
| FRA 163 · AWS FRA | 普通家宽 | 9.9% | 608 | 150.3 | 0.2 |
| FRA TATA | 163Plus 家宽 | 0.0% | 1631 | 161.7 | 33.4 |
| FRA TATA | 普通家宽 | 13.0% | 1634 | 167.6 | 1.1 |
| LAX 163 · AWS PDX | 163Plus 家宽 | 0.2% | 503 | 179.5 | 27.2 |
| LAX 163 · AWS PDX | 普通家宽 | 13.3% | 503 | 181.2 | 0.4 |
| FRA Cogent · AWS SIN | 163Plus 家宽 | 0.6% | 505 | 211.7 | 30.9 |
| FRA Cogent · AWS SIN | 普通家宽 | 14.9% | 504 | 200.4 | 2.1 |
| FRA 163 · AWS LHR | 163Plus 家宽 | 0.0% | 528 | 180.4 | 39.3 |
| FRA 163 · AWS LHR | 普通家宽 | 13.8% | 529 | 166.4 | 0.7 |
| LAX Arelion | 163Plus 家宽 | 0.0% | 2221 | 182.3 | 46.6 |
| LAX Arelion | 普通家宽 | 15.3% | 2220 | 167.1 | 0.3 |

</div>

以 AWS FRA 为例，两条线路各发送 608 次探测。普通家宽末跳丢包率为 9.9%，成功返回的样本平均 RTT 为 150.3 ms，StDev 仅 0.2 ms。163Plus 末跳丢包率为 0.0%，但 RTT 分布在 132.6–539.5 ms 之间，StDev 达 76.5 ms。其余五组趋势相同。六组汇总，普通家宽末跳丢包率为 **9.9%–15.3%**，StDev 为 **0.2–2.1 ms**；163Plus 有四组末跳丢包清零，其余两组为 **0.2% 和 0.6%**，六组 StDev 均升至 **27.2–76.5 ms** 范围内。

这种“高丢包、低抖动”与“低丢包、高抖动”的反差，符合两类流量在晚高峰拥塞点受到不同队列处理的特征。普通家宽若触发硬限速（Policing）或尾部丢包（Tail Drop），超限或遇到队满的探测包会被直接丢弃，不计入 RTT 统计。成功返回的探测包若未经历深队列等待，StDev 就会很低。163Plus 若获得更高的调度优先级或更深的队列缓冲（Buffer），原本会被丢弃的包便有机会等到转发。这能减少末跳丢包，也会让排队较久的响应进入 RTT 统计。各次探测的排队时延（Queuing Delay）相差越大，StDev 就越高。

## 五、iperf3：四条路径的单连接下载

<div class="telecom163-table" markdown="1">

| 路径 | 普通 / Mbps | 163Plus / Mbps | 普通 Retr | 163Plus Retr |
|---|---|---|---|---|
| LAX 163 · AWS PDX | 0.138 | 114 | 36 | 0 |
| FRA 163 · AWS FRA | 0.415 | 78.6 | 50 | 1,815 |
| LAX Arelion | 0.205 | 138 | 49 | 417 |
| FRA TATA | 61.5 | 233 | 10,228 | 41,909 |

</div>

### LAX 163：AWS PDX 起点

![AWS PDX 经 LAX 163 的逐区间发送速率与重传](/assets/images/beijing-telecom-163plus/01-iperf-lax-163.png)

*图 9：LAX 163（AWS PDX）逐秒发送速率与重传对比*

```text
【163Plus 家宽】
[  5] local 172.26.12.11 port 5201 connected to 【163Plus 家宽】 port 1523
[  5]   0.00-1.00   sec  1.38 MBytes  11.5 Mbits/sec    0    450 KBytes
[  5]   1.00-2.00   sec  12.8 MBytes   107 Mbits/sec    0   6.50 MBytes
[  5]   2.00-3.00   sec  13.9 MBytes   116 Mbits/sec    0   6.50 MBytes
[ ID] Interval           Transfer     Bitrate         Retr
[  5]   0.00-15.18  sec   206 MBytes   114 Mbits/sec    0            sender

【普通家宽】
[  5] local 172.26.12.11 port 5201 connected to 【普通家宽】 port 33360
[  5]   0.00-1.00   sec  0.00 Bytes  0.00 bits/sec   11   9.84 KBytes
[  5]   1.00-2.00   sec  0.00 Bytes  0.00 bits/sec    4   5.62 KBytes
[  5]   2.00-3.00   sec   128 KBytes  1.05 Mbits/sec    2   4.22 KBytes
[ ID] Interval           Transfer     Bitrate         Retr
[  5]   0.00-15.18  sec   256 KBytes   138 Kbits/sec   36            sender
```

普通家宽约 15 秒仅发送 256 KiB，分布在两个完整的一秒区间，每个区间 128 KiB。163Plus 在第一秒后维持 107–138 Mbps，全程零重传。两条线路平均速率分别为 **0.138 Mbps 和 114 Mbps**。从日志末列的拥塞窗口（Cwnd）看，163Plus 从第 2 秒起稳定在 6.50 MiB，普通家宽则反复重传，Cwnd 始终只有 1.41–9.84 KiB。

### FRA 163：AWS FRA 起点

![AWS FRA 经 FRA 163 的逐区间发送速率与重传](/assets/images/beijing-telecom-163plus/02-iperf-fra-163.png)

*图 10：FRA 163（AWS FRA）逐秒发送速率与重传对比*

```text
【163Plus 家宽】
[  5] local 172.26.14.138 port 5201 connected to 【163Plus 家宽】 port 1474
[  5]   7.00-8.00   sec  20.2 MBytes   170 Mbits/sec    0   3.18 MBytes
[  5]   8.00-9.00   sec  4.25 MBytes  35.7 Mbits/sec    2   1.41 KBytes
[  5]   9.00-10.00  sec  0.00 Bytes  0.00 bits/sec   37   18.3 KBytes
[  5]  10.00-11.00  sec  0.00 Bytes  0.00 bits/sec  184   56.2 KBytes
[  5]  11.00-12.00  sec  1.12 MBytes  9.44 Mbits/sec  450    132 KBytes
[  5]  12.00-13.00  sec  1.25 MBytes  10.5 Mbits/sec  634    107 KBytes
[  5]  13.00-14.00  sec  0.00 Bytes  0.00 bits/sec  453    105 KBytes
[  5]  14.00-15.00  sec  9.50 MBytes  79.7 Mbits/sec   55   2.42 MBytes
[ ID] Interval           Transfer     Bitrate         Retr
[  5]   0.00-15.15  sec   142 MBytes  78.6 Mbits/sec  1815            sender

【普通家宽】
[  5] local 172.26.14.138 port 5201 connected to 【普通家宽】 port 50696
[  5]   7.00-8.00   sec  0.00 Bytes  0.00 bits/sec    2   4.22 KBytes
[  5]   8.00-9.00   sec  0.00 Bytes  0.00 bits/sec    2   4.22 KBytes
[  5]   9.00-10.00  sec   128 KBytes  1.05 Mbits/sec    2   2.81 KBytes
[  5]  10.00-11.00  sec  0.00 Bytes  0.00 bits/sec    3   7.03 KBytes
[ ID] Interval           Transfer     Bitrate         Retr
[  5]   0.00-15.15  sec   768 KBytes   415 Kbits/sec   50            sender
```

163Plus 全程均值 **78.6 Mbps**，但传输过程出现明显断档：2–8 秒维持在 141–170 Mbps，8–9 秒降至 35.7 Mbps（Cwnd 从 3.18 MiB 骤降至 1.41 KiB），随后连续两秒发送量为 0 Bytes。12–13 秒速率为 10.5 Mbps，单秒重传 634 次；14–15 秒回升至 79.7 Mbps。普通家宽全程平均 **0.415 Mbps**。

### LAX Arelion

![LAX Arelion 的逐区间发送速率与重传](/assets/images/beijing-telecom-163plus/03-iperf-lax-arelion.png)

*图 11：LAX Arelion 逐秒发送速率与重传对比*

```text
【163Plus 家宽】
[  5] local 174.136.204.72 port 5201 connected to 【163Plus 家宽】 port 1521
[  5]   4.00-5.00   sec  16.8 MBytes   140 Mbits/sec    0   7.95 MBytes
[  5]   5.00-6.00   sec  18.1 MBytes   152 Mbits/sec  153   5.59 MBytes
[  5]   6.00-7.00   sec  19.2 MBytes   161 Mbits/sec    0   5.59 MBytes
…
[  5]  10.00-11.00  sec  16.8 MBytes   141 Mbits/sec    0   5.59 MBytes
[  5]  11.00-12.00  sec  16.4 MBytes   137 Mbits/sec  264   3.91 MBytes
[  5]  12.00-13.00  sec  19.4 MBytes   163 Mbits/sec    0   3.91 MBytes
[ ID] Interval           Transfer     Bitrate         Retr
[  5]   0.00-15.16  sec   249 MBytes   138 Mbits/sec  417            sender

【普通家宽】
[  5] local 174.136.204.72 port 5201 connected to 【普通家宽】 port 44202
[  5]   4.00-5.00   sec  0.00 Bytes  0.00 bits/sec    1   5.62 KBytes
[  5]   5.00-6.00   sec  0.00 Bytes  0.00 bits/sec    2   2.81 KBytes
[  5]   6.00-7.00   sec  0.00 Bytes  0.00 bits/sec    2   5.62 KBytes
…
[  5]  10.00-11.00  sec  0.00 Bytes  0.00 bits/sec    3   2.81 KBytes
[  5]  11.00-12.00  sec  0.00 Bytes  0.00 bits/sec    2   5.62 KBytes
[  5]  12.00-13.00  sec  0.00 Bytes  0.00 bits/sec    2   1.41 KBytes
[ ID] Interval           Transfer     Bitrate         Retr
[  5]   0.00-15.37  sec   384 KBytes   205 Kbits/sec   49            sender
```

163Plus 的 417 次重传集中在两个区间：5–6 秒有 153 次，11–12 秒有 264 次。对应发送速率仍有 152 和 137 Mbps，两个区间均未出现发送停顿。163Plus 全程平均 **138 Mbps**，普通家宽 **0.205 Mbps**。

### FRA TATA

![FRA TATA 的逐区间发送速率与重传](/assets/images/beijing-telecom-163plus/04-iperf-fra-tata.png)

*图 12：FRA TATA 逐秒发送速率与重传对比*

```text
【163Plus 家宽】
[  5] local 45.147.50.23 port 5201 connected to 【163Plus 家宽】 port 2304
[  5]   0.00-1.00   sec  2.00 MBytes  16.8 Mbits/sec    0    403 KBytes
[  5]   1.00-2.00   sec  49.6 MBytes   416 Mbits/sec    0   22.1 MBytes
[  5]   2.00-3.00   sec  20.1 MBytes   169 Mbits/sec  10973   11.6 MBytes
[  5]   3.00-4.00   sec  31.5 MBytes   264 Mbits/sec  2023   1.87 MBytes
[  5]   4.00-5.00   sec  31.5 MBytes   264 Mbits/sec  8305   19.1 MBytes
[  5]   5.00-6.00   sec  20.4 MBytes   171 Mbits/sec  8253   7.29 MBytes
[ ID] Interval           Transfer     Bitrate         Retr
[  5]   0.00-15.19  sec   422 MBytes   233 Mbits/sec  41909            sender

【普通家宽】
[  5] local 45.147.50.23 port 5201 connected to 【普通家宽】 port 58864
[  5]   0.00-1.00   sec   896 KBytes  7.33 Mbits/sec    8   78.8 KBytes
[  5]   1.00-2.00   sec   512 KBytes  4.20 Mbits/sec   28    305 KBytes
[  5]   2.00-3.00   sec  4.50 MBytes  37.7 Mbits/sec  121   1.45 MBytes
[  5]   3.00-4.00   sec  20.4 MBytes   171 Mbits/sec  559   7.42 MBytes
[  5]   4.00-5.00   sec  10.0 MBytes  83.9 Mbits/sec  1000   8.25 MBytes
[  5]   5.00-6.00   sec  10.4 MBytes  87.1 Mbits/sec  1200   8.21 MBytes
[ ID] Interval           Transfer     Bitrate         Retr
[  5]   0.00-15.80  sec   116 MBytes  61.5 Mbits/sec  10228            sender
```

普通家宽发送 **116 MiB**，平均 **61.5 Mbps**，重传 **10,228 次**；163Plus 发送 **422 MiB**，平均 **233 Mbps**，重传 **41,909 次**。163Plus 的吞吐为普通家宽的 **3.8 倍**，发送量为 **3.64 倍**，重传数为 **4.10 倍**。

按发送量折算，普通家宽约 **88 次重传/MiB**，163Plus 约 **99 次/MiB**，后者高约 13%，单位数据量的重传负担处于同一量级。两条线路均经 TATA 接入，海外互联侧是可能的共同瓶颈。在相近的重传负担下，具备国内 C–I 段保障的 163Plus 仍达到普通家宽 **3.8 倍的单流吞吐**。

## 六、总结

晚高峰四组测试中，LAX 163、LAX Arelion 和 FRA 163（AWS FRA）的普通家宽均不足 0.5 Mbps，163Plus 分别达到 **114、138 和 78.6 Mbps**；FRA TATA 则由 **61.5 Mbps** 提升至 **233 Mbps**。

综合来看，北京电信 163Plus 有效缓解了普通 163 家宽晚高峰在 C–I 段的拥塞丢包，让海外单连接 TCP 流量得以顺利撑开窗口起速。但它的作用范围仅限于国内出口段的转发调度：一方面，若海外互联侧或 PoP 节点本身容量不足，传输瓶颈与重传依然存在；另一方面，它不会改变原有的 163 路由走向（如新加坡经 Cogent 绕行法兰克福的路径开通后依然绕行），对时延敏感的场景仍取决于目标节点具体的海外接入路由。

如果你常用欧美的低价服务器，希望晚高峰从这些机器下载时快一些，又用不到 IPv6 和公网 IPv4，我觉得每月花 30 元开通 163Plus 还算划算。此外据我了解，上海电信面向家宽的 CN2 和 163Plus 都已停止新办，北京这项业务如果正好用得上，我建议趁还能办时及时上车开通。

## 参考资料与原始数据

Luminous，[《〖杂谈〗运营商链路简评&鉴别（163/169/CN2等)》](https://luotianyi.vc/4242.html)，2020-08-25。

原始数据附件：

- [六组 MTR 逐跳记录（脱敏）](/assets/images/beijing-telecom-163plus/data/MTR-脱敏完整记录.txt)
- [四组 iperf3 服务端日志（脱敏）](/assets/images/beijing-telecom-163plus/data/iperf3-脱敏原始记录.txt)
