---
layout: default
title: "🇯🇵 Mkcloud 上海-日本 IPLC 专线 上云互联优化入口（IXP）测评"
seo_keywords: "Mkcloud, 上海日本IPLC, IXP, 云厂BGP优化入口, 日本BGP"
redirect_from:
  - /reviews/Mkcloud-ix-sha-nrt.md
  - /REVIEW/reviews/Mkcloud-ix-sha-nrt.md
---

# 🇯🇵 Mkcloud 上海-日本 IPLC 专线 上云互联优化入口（IXP）测评

<div class="back-home" style="margin: 12px 0 24px;">
  <a href="{{ '/' | relative_url }}" style="display: inline-flex; align-items: center; gap: 8px; padding: 8px 12px; background: linear-gradient(135deg, #f8fafc 0%, #eef2f7 100%); border: 1px solid #e5e7eb; border-radius: 999px; color: #1f2937; text-decoration: none; font-size: 14px; font-weight: 600;">
    <span style="font-size: 16px;">←</span>
    <span>返回主页</span>
  </a>
</div>

<div class="toc-container" markdown="1">

## 目录
{: .no_toc }

* TOC
{:toc}

</div>

## 买

### 购买链接

- [**官方购买入口**](https://www.mkcloud.net/aff.php?aff=356&pid=247)

### 产品说明

> 该产品为云厂 BGP 网络优化入口，仅允许云厂 BGP 网络连入（阿里云国内全网、腾讯云国内全网、百度云国内全网、火山云华南、华为云华南等），需要云厂 BGP 网络作为前置搭配使用。

### 规格对照

<details markdown="1">
<summary>流量计费（共享带宽）</summary>

| 套餐 | vCPU | 内存 | 硬盘 | 峰值带宽 | 月流量 | 价格 |
|---|---:|---:|---:|---:|---:|---:|
| 2026 新春年付限定 | 2 核 | 4 GB | 40 GB | 666 Mbps | 2048 GB | ¥1908 / 年 |
| 2026 新春活动 | 6 核 | 6 GB | 60 GB | 1333 Mbps | 3888 GB | ¥388 / 月 |
| 1TB 流量 | 2 核 | 4 GB | 40 GB | 200 Mbps | 1 TB | ¥166 / 月 |
| 2TB 流量 | 2 核 | 4 GB | 40 GB | 300 Mbps | 2 TB | ¥268 / 月 |
| 3TB 流量 | 2 核 | 4 GB | 40 GB | 500 Mbps | 3 TB | ¥358 / 月 |
| 6TB 流量（1Gbps） | 4 核 | 8 GB | 40 GB | 1 Gbps | 6 TB | ¥688 / 月 |

- 公共特性：入口云厂优化网络通道、出口日本 BGP、独享 IPv4 x2（进+出）、端内延迟 25~28ms。
- 超量策略：2026 新春年付限定 / 2026 新春活动 / 1TB / 2TB 为超量停机；3TB 为超量不停机限速 10Mbps；6TB 为超量不停机限速 20Mbps。

</details>

<details markdown="1">
<summary>带宽计费（独享带宽）</summary>

| 套餐 | vCPU | 内存 | 硬盘 | 独享带宽 | 月流量 | 价格 |
|---|---:|---:|---:|---:|---:|---:|
| 20M 独享 | 2 核 | 4 GB | 40 GB | 20 Mbps | 无限制 | ¥1000 / 月 |
| 50M 独享 | 2 核 | 4 GB | 40 GB | 50 Mbps | 无限制 | ¥2250 / 月 |
| 100M 独享 | 2 核 | 4 GB | 40 GB | 100 Mbps | 无限制 | ¥3700 / 月 |
| 200M 独享 | 2 核 | 4 GB | 40 GB | 200 Mbps | 无限制 | ¥7000 / 月 |
| 500M 独享 | 8 核 | 8 GB | 60 GB | 500 Mbps | 无限制 | ¥17500 / 月 |
| 1G 独享 | 28 核 | 64 GB | 512 GB | 1 Gbps | 无限制 | ¥35000 / 月 |
| 2G 独享 | 28 核 | 64 GB | 512 GB | 2 Gbps | 无限制 | ¥70000 / 月 |
| 5G 独享 | 28 核 | 64 GB | 512 GB | 5 Gbps | 无限制 | ¥175000 / 月 |

- 公共特性：入口云厂优化网络通道、出口日本 BGP、独享 IPv4 x2（进+出）、端内延迟 25~28ms。
- 套餐补充：1G / 2G / 5G 套餐标注赠送志强金牌独立服务器。

</details>

## 评

- 适用场景：待补充
- 实际体验：待补充
- 性价比判断：待补充

## 测

### 路由表现

<details markdown="1">
<summary>线路概览</summary>

![radar]({{ '/assets/images/mkcloud-ix-sha-nrt/radar.png' | relative_url }})

</details>

<details markdown="1">
<summary>出口到主要公共服务的延迟测试</summary>

| 服务 | 平均延迟 |
|---|---:|
| Apple | 74.881 ms |
| Google | 25.760 ms |
| Cloudflare | 25.805 ms |
| AWS | 25.921 ms |
| GitHub | 26.606 ms |

</details>

### 实时监控

- **端内实时状态监控**：<https://ping.nxtrace.org/goto/CTYG8UDDg>
- **端内状态监控截图**：
  <details markdown="1">
  <summary>展开查看</summary>
  
  ![端内延迟监控截图]({{ '/assets/images/mkcloud-ix-sha-nrt/端内延迟监控截图（近七天）.png' | relative_url }})

  </details>

<details markdown="1">
<summary>阿里云各地区到入口延迟测试</summary>

| 探测点（阿里云） | 平均时间 |
|---|---:|
| 四川成都 | 49.533 ms |
| 内蒙古自治区呼和浩特 | 47.343 ms |
| 广东广州 | 35.499 ms |
| 内蒙古自治区乌兰察布 | 34.589 ms |
| 广东深圳 | 32.854 ms |
| 河北测试 | 31.413 ms |
| 北京北京 | 22.365 ms |
| 山东青岛 | 20.924 ms |
| 浙江杭州 | 13.769 ms |
| 上海上海 | 12.543 ms |

</details>

<details markdown="1">
<summary>国际网络带宽测试</summary>

| 服务商 | 地点 | 发送速度 | 接收速度 | 延迟 |
|---|---|---:|---:|---:|
| Clouvider | London, UK (10G) | 149 Mbits/sec | 31.5 Mbits/sec | 250 ms |
| Eranium | Amsterdam, NL (100G) | 154 Mbits/sec | 132 Mbits/sec | 252 ms |
| Uztelecom | Tashkent, UZ (10G) | 144 Mbits/sec | 25.5 Mbits/sec | 273 ms |
| Leaseweb | Singapore, SG (10G) | 155 Mbits/sec | 75.6 Mbits/sec | 142 ms |
| Clouvider | Los Angeles, CA, US (10G) | 171 Mbits/sec | 39.6 Mbits/sec | 130 ms |
| Leaseweb | NYC, NY, US (10G) | 161 Mbits/sec | 71.7 Mbits/sec | 182 ms |
| Edgoo | Sao Paulo, BR (1G) | 34.3 Mbits/sec | 19.0 Mbits/sec | 366 ms |

> 本组为 IPv6 测试数据。

</details>

### 单线程测速（iperf3）

<details markdown="1">
<summary>腾讯云广州（200M端口）</summary>

![腾讯云广州晚高峰测速]({{ '/assets/images/mkcloud-ix-sha-nrt/广州腾讯云晚高峰测速.png' | relative_url }})

</details>

<details markdown="1">
<summary>腾讯云上海（200M端口）</summary>

![腾讯云上海晚高峰测速]({{ '/assets/images/mkcloud-ix-sha-nrt/上海腾讯云晚高峰测速.png' | relative_url }})

</details>

### 机器性能跑分

<details markdown="1">
<summary>综合性能跑分（YABS）</summary>

![综合性能跑分]({{ '/assets/images/mkcloud-ix-sha-nrt/综合性能跑分.png' | relative_url }})

</details>

### IP 解锁

<details markdown="1">
<summary>流媒体 / 平台解锁记录</summary>

![解锁情况]({{ '/assets/images/mkcloud-ix-sha-nrt/解锁情况/2026-02-17 22.39.06.png' | relative_url }})

</details>
