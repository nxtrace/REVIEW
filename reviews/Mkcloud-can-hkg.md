---
layout: default
title: "🇨🇳 Mkcloud 广东-香港 IEPL 专线 广州BGP 测评"
seo_keywords: "Mkcloud, 广东香港IEPL, 广州BGP, 香港BGP"
redirect_from:
  - /reviews/Mkcloud-can-hkg.md
  - /REVIEW/reviews/Mkcloud-can-hkg.md
---

# 🇨🇳 Mkcloud 广东-香港 IEPL 专线 广州BGP 测评

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

- [**官方购买入口**](https://www.mkcloud.net/aff.php?aff=356&pid=242)

### 产品说明

> 该产品入口为腾讯广州八线 BGP，出口为香港 BGP，适合以广州 BGP 为前置接入的场景。

### 规格对照

<details markdown="1">
<summary>流量计费（共享带宽）</summary>

| 套餐 | vCPU | 内存 | 硬盘 | 峰值带宽 | 月流量 | 价格 |
|---|---:|---:|---:|---:|---:|---:|
| 2026 新春活动 | 6 核 | 6 GB | 60 GB | 888 Mbps | 2888 GB | ¥666 / 月 |
| 500GB 流量 | 1 核 | 2 GB | 20 GB | 150 Mbps | 500 GB | ¥228 / 月 |
| 1TB 流量 | 1 核 | 2 GB | 20 GB | 200 Mbps | 1 TB | ¥358 / 月 |
| 2TB 流量 | 2 核 | 4 GB | 40 GB | 300 Mbps | 2 TB | ¥568 / 月 |
| 4TB 流量 | 2 核 | 4 GB | 40 GB | 300 Mbps | 4 TB | ¥998 / 月 |
| 6TB 流量 | 4 核 | 8 GB | 60 GB | 500 Mbps | 6 TB | ¥1388 / 月 |
| 10TB 流量 | 4 核 | 8 GB | 60 GB | 500 Mbps | 10 TB | ¥2288 / 月 |

- 公共特性：入口腾讯广州八线 BGP、出口香港 BGP、独享 IPv4 x2（进+出）、端内延迟 1~2ms。

</details>

<details markdown="1">
<summary>带宽计费（独享带宽）</summary>

| 套餐 | vCPU | 内存 | 硬盘 | 独享带宽 | 月流量 | 价格 |
|---|---:|---:|---:|---:|---:|---:|
| 5M 独享 | 2 核 | 4 GB | 40 GB | 5 Mbps | 无限制 | ¥500 / 月 |
| 10M 独享 | 2 核 | 4 GB | 40 GB | 10 Mbps | 无限制 | ¥700 / 月 |
| 20M 独享 | 2 核 | 4 GB | 40 GB | 20 Mbps | 无限制 | ¥1320 / 月 |
| 50M 独享 | 4 核 | 8 GB | 60 GB | 50 Mbps | 无限制 | ¥3150 / 月 |
| 100M 独享 | 4 核 | 8 GB | 60 GB | 100 Mbps | 无限制 | ¥5800 / 月 |

- 公共特性：入口腾讯广州八线 BGP、出口香港 BGP、独享 IPv4 x2（进+出）、端内延迟 1~2ms。

</details>

## 评

- 适用场景：待补充
- 实际体验：待补充
- 性价比判断：待补充

## 测

### 路由表现

<details markdown="1">
<summary>线路概览</summary>

![radar]({{ '/assets/images/mkcloud-can-hkg/radar.png' | relative_url }})

</details>

<details markdown="1">
<summary>出口到主要公共服务的延迟测试</summary>

| 服务 | 平均延迟 |
|---|---:|
| Apple | 2.419 ms |
| Google | 2.302 ms |
| Cloudflare | 2.309 ms |
| AWS | 2.091 ms |
| GitHub | 32.012 ms |

</details>

### 实时监控

- **端内实时状态监控**：https://ping.nxtrace.org/goto/rDiiU8vDg
- **端内状态监控截图**：
  <details markdown="1">
  <summary>展开查看</summary>
  
  ![端内延迟监控截图]({{ '/assets/images/mkcloud-can-hkg/端内延迟监控截图（近七天）.png' | relative_url }})

  </details>

<details markdown="1">
<summary>阿里云各地区到入口延迟测试</summary>

| 探测点（阿里云） | 平均时间 |
|---|---:|
| 待补充 | 待补充 |

</details>

<details markdown="1">
<summary>国际网络带宽测试（IPv4）</summary>

| 服务商 | 地点 | 发送速度 | 接收速度 | 延迟 |
|---|---|---:|---:|---:|
| 待补充 | 待补充 | 待补充 | 待补充 | 待补充 |

</details>

### 单线程测速（iperf3）

<details markdown="1">
<summary>北京移动晚高峰</summary>

![北京移动晚高峰]({{ '/assets/images/mkcloud-can-hkg/北京四网单线程测速/北京移动晚高峰.png' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通晚高峰</summary>

![北京联通晚高峰]({{ '/assets/images/mkcloud-can-hkg/北京四网单线程测速/北京联通晚高峰.png' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通晚高峰</summary>

![北京网通晚高峰]({{ '/assets/images/mkcloud-can-hkg/北京四网单线程测速/北京网通晚高峰.png' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信晚高峰</summary>

![北京电信晚高峰]({{ '/assets/images/mkcloud-can-hkg/北京四网单线程测速/北京电信晚高峰.png' | relative_url }})

</details>

### 机器性能跑分

<details markdown="1">
<summary>综合性能跑分（YABS）</summary>

![综合性能跑分]({{ '/assets/images/mkcloud-can-hkg/综合性能跑分.png' | relative_url }})

</details>

### IP 解锁

<details markdown="1">
<summary>流媒体 / 平台解锁记录</summary>

![解锁情况]({{ '/assets/images/mkcloud-can-hkg/解锁情况/2026-02-17 22.39.34.png' | relative_url }})

</details>
