---
layout: default
title: "🇭🇰 Mkcloud 广东-香港 IEPL 专线 上云互联优化入口（IXP）测评"
seo_keywords: "Mkcloud, 广东香港IEPL, IXP, 云厂BGP优化入口, 香港BGP"
redirect_from:
  - /reviews/mkcloud-ix-szx-hkg.md
  - /REVIEW/reviews/mkcloud-ix-szx-hkg.md
---

# 🇭🇰 Mkcloud 广东-香港 IEPL 专线 上云互联优化入口（IXP）测评

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

- **[官方购买入口](https://www.mkcloud.net/aff.php?aff=356&pid=91)**

### 产品说明

> 该产品为云厂 BGP 网络优化入口，仅允许云厂 BGP 网络连入（阿里云国内全网、腾讯云国内全网、百度云国内全网、火山云华南、华为云华南等），需要云厂 BGP 网络作为前置搭配使用。

### 规格对照

<details markdown="1">
<summary>流量计费（共享带宽）</summary>

| 套餐 | vCPU | 内存 | 硬盘 | 峰值带宽 | 月流量 | 月付 |
|---|---:|---:|---:|---:|---:|---:|
| 2TB 流量 | 2 核 | 4 GB | 40 GB | 1 Gbps | 2 TB | ¥158 |
| 4TB 流量 | 2 核 | 4 GB | 40 GB | 1 Gbps | 4 TB | ¥258 |
| 6TB 流量 | 4 核 | 8 GB | 40 GB | 2 Gbps | 6 TB | ¥378 |
| 10TB 流量 | 4 核 | 8 GB | 40 GB | 2 Gbps | 10 TB | ¥826 |
| 20TB 流量 | 4 核 | 8 GB | 40 GB | 2 Gbps | 20 TB | ¥1639 |
| 30TB 流量 | 4 核 | 8 GB | 60 GB | 3 Gbps | 30 TB | ¥2458 |
| 50TB 流量 | 8 核 | 8 GB | 60 GB | 3 Gbps | 50 TB | ¥3588 |
| 100TB 流量 | 8 核 | 16 GB | 80 GB | 5 Gbps | 100 TB | ¥7168 |
| 200TB 流量 | 8 核 | 16 GB | 80 GB | 5 Gbps | 200 TB | ¥12288 |
| 300TB 流量 | 8 核 | 16 GB | 80 GB | 5 Gbps | 300 TB | ¥18428 |

- 公共特性：超量停机、入口云厂优化网络通道、出口香港 BGP、独享 IPv4 x2（进+出）、端内延迟 1~2ms。

</details>

<details markdown="1">
<summary>带宽计费（独享带宽）</summary>

| 套餐 | vCPU | 内存 | 硬盘 | 独享带宽 | 月流量 | 月付 |
|---|---:|---:|---:|---:|---:|---:|
| 100M 独享 | 2 核 | 4 GB | 40 GB | 100 Mbps | 无限制 | ¥1600 |
| 200M 独享 | 2 核 | 4 GB | 40 GB | 200 Mbps | 无限制 | ¥3000 |
| 500M 独享 | 8 核 | 8 GB | 60 GB | 500 Mbps | 无限制 | ¥6000 |
| 1G 独享 | 28 核 | 64 GB | 512 GB | 1 Gbps | 无限制 | ¥9000 |
| 2G 独享 | 28 核 | 64 GB | 512 GB | 2 Gbps | 无限制 | ¥16000 |
| 5G 独享 | 28 核 | 64 GB | 512 GB | 5 Gbps | 无限制 | ¥35000 |

- 公共特性：入口云厂优化网络通道、出口香港 BGP、独享 IPv4 x2（进+出）、端内延迟 1~2ms。
- 套餐补充：1G / 2G / 5G 套餐标注赠送志强金牌独立服务器。

</details>

## 评

这款广东-香港上云互联优化入口（IXP）本质是“云厂前置 + 香港低时延出口”方案。入口仅在 IX 网络内宣告，需要阿里云、腾讯云等云厂网络前置，不属于家宽直连即用型产品。

从现有测试看，主流公共服务延迟基本在 2~3ms 区间，端内监控和单线程测速也比较稳定。我的测试机是 200Mbps 端口款，搭配腾讯云 200M 前置可稳定跑满端口。整体更适合云到云互联或中转落地用户；若目标是本地家宽直连，建议优先考虑非 IXP 入口版本。

## 测

### 路由表现

<details markdown="1">
<summary>线路概览</summary>

![radar]({{ '/assets/images/mkcloud-ix-szx-hkg/radar.png' | relative_url }})

</details>

<details markdown="1">
<summary>出口到主要公共服务的延迟测试</summary>

| 服务 | 平均延迟 |
|---|---:|
| Apple | 2.466 ms |
| Google | 2.417 ms |
| Cloudflare | 2.369 ms |
| AWS | 2.070 ms |
| GitHub | 31.990 ms |

</details>

### 实时监控

- **端内实时状态监控**：<https://ping.nxtrace.org/goto/mHXX18DvR>
- **端内状态监控截图**：
  <details markdown="1">
  <summary>展开查看</summary>
  
  ![端内延迟监控截图]({{ '/assets/images/mkcloud-ix-szx-hkg/端内延迟监控截图（近七天）.png' | relative_url }})

  </details>

<details markdown="1">
<summary>阿里云各地区到入口延迟测试</summary>

| 探测点（阿里云） | 平均时间 |
|---|---:|
| 内蒙古自治区呼和浩特 | 64.7176 ms |
| 河北测试 | 50.5393 ms |
| 山东青岛 | 45.3664 ms |
| 内蒙古自治区乌兰察布 | 40.1186 ms |
| 北京北京 | 38.8013 ms |
| 四川成都 | 36.4530 ms |
| 上海上海 | 35.4656 ms |
| 浙江杭州 | 30.5965 ms |
| 广东广州 | 9.8919 ms |
| 广东深圳 | 8.5284 ms |

</details>

<details markdown="1">
<summary>国际网络带宽测试（IPv4）</summary>

| 服务商 | 地点 | 发送速度 | 接收速度 | 延迟 |
|---|---|---:|---:|---:|
| Clouvider | London, UK (10G) | 470 Mbits/sec | 170 Mbits/sec | 196 ms |
| Eranium | Amsterdam, NL (100G) | 480 Mbits/sec | 334 Mbits/sec | 258 ms |
| Uztelecom | Tashkent, UZ (10G) | 489 Mbits/sec | 225 Mbits/sec | 112 ms |
| Leaseweb | Singapore, SG (10G) | 511 Mbits/sec | 381 Mbits/sec | 86.6 ms |
| Clouvider | Los Angeles, CA, US (10G) | 487 Mbits/sec | 253 Mbits/sec | 145 ms |
| Leaseweb | NYC, NY, US (10G) | 461 Mbits/sec | 267 Mbits/sec | 254 ms |
| Edgoo | Sao Paulo, BR (1G) | 380 Mbits/sec | 64.5 Mbits/sec | 334 ms |

</details>

### 腾讯云单线程测速(iperf3 到入口 IX IP)

<details markdown="1">
<summary>腾讯云广州（200M端口）</summary>

![腾讯云广州晚高峰测速]({{ '/assets/images/mkcloud-ix-szx-hkg/广州腾讯云晚高峰测速.png' | relative_url }})

</details>

<details markdown="1">
<summary>腾讯云上海（200M端口）</summary>

![腾讯云上海晚高峰测速]({{ '/assets/images/mkcloud-ix-szx-hkg/上海腾讯云晚高峰测速.png' | relative_url }})

</details>

### 机器性能跑分

<details markdown="1">
<summary>综合性能跑分（YABS）</summary>

![综合性能跑分]({{ '/assets/images/mkcloud-ix-szx-hkg/综合性能跑分.png' | relative_url }})

</details>

### IP 解锁

<details markdown="1">
<summary>流媒体 / 平台解锁记录</summary>

![解锁情况]({{ '/assets/images/mkcloud-ix-szx-hkg/解锁情况/2026-02-17 20.51.22.png' | relative_url }})

</details>
