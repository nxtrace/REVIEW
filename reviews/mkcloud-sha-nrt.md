---
layout: default
title: "🇯🇵 Mkcloud 上海-日本 IPLC 专线 上海电信 测评"
seo_keywords: "Mkcloud, 上海日本IPLC, 上海电信, 日本BGP"
redirect_from:
  - /reviews/Mkcloud-sha-nrt/
  - /reviews/Mkcloud-sha-nrt.md
  - /REVIEW/reviews/Mkcloud-sha-nrt.md
---

# 🇯🇵 Mkcloud 上海-日本 IPLC 专线 上海电信 测评

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

- [**官方购买入口**](https://www.mkcloud.net/aff.php?aff=356&gid=4)

### 产品说明

> 该产品入口为上海电信，出口为日本 BGP。

### 规格对照

<details markdown="1">
<summary>流量计费（共享带宽）</summary>

| 套餐 | vCPU | 内存 | 硬盘 | 峰值带宽 | 月流量 | 价格 |
|---|---:|---:|---:|---:|---:|---:|
| 500GB 流量 | 1 核 | 2 GB | 20 GB | 150 Mbps | 500 GB | ¥228 / 月 |
| 1TB 流量 | 1 核 | 2 GB | 20 GB | 200 Mbps | 1 TB | ¥358 / 月 |
| 2TB 流量 | 2 核 | 4 GB | 40 GB | 300 Mbps | 2 TB | ¥568 / 月 |
| 4TB 流量 | 2 核 | 4 GB | 40 GB | 300 Mbps | 4 TB | ¥998 / 月 |
| 6TB 流量 | 4 核 | 8 GB | 60 GB | 500 Mbps | 6 TB | ¥1388 / 月 |
| 10TB 流量 | 4 核 | 8 GB | 60 GB | 500 Mbps | 10 TB | ¥2288 / 月 |

- 公共特性：入口上海电信、出口日本 BGP、独享 IPv4 x2（进+出）、端内延迟 25~28ms。

</details>

<details markdown="1">
<summary>带宽计费（独享带宽）</summary>

| 套餐 | vCPU | 内存 | 硬盘 | 独享带宽 | 月流量 | 价格 |
|---|---:|---:|---:|---:|---:|---:|
| 5M 独享 | 2 核 | 4 GB | 40 GB | 5 Mbps | 无限制 | ¥600 / 月 |
| 10M 独享 | 2 核 | 4 GB | 40 GB | 10 Mbps | 无限制 | ¥800 / 月 |
| 20M 独享 | 2 核 | 4 GB | 40 GB | 20 Mbps | 无限制 | ¥1560 / 月 |
| 50M 独享 | 4 核 | 8 GB | 60 GB | 50 Mbps | 无限制 | ¥3500 / 月 |
| 100M 独享 | 4 核 | 8 GB | 60 GB | 100 Mbps | 无限制 | ¥6000 / 月 |

- 公共特性：入口上海电信、出口日本 BGP、独享 IPv4 x2（进+出）、端内延迟 25~28ms。

</details>

## 评

沪日 IPLC 上海电信入口这款属于可直连方案，端内时延约 25~28ms，整体延迟表现稳定，电信侧体验相对更友好。

考虑到跨网因素，联通和移动用户建议结合自身网络情况评估；如果更关注跨网 QoS 风险控制，可以考虑同线路的 IXP 入口版本。我的测试机是 150Mbps 端口款，实际可稳定在 120Mbps 左右，日常落地和中转场景可用性不错。

## 测

### 路由表现

<details markdown="1">
<summary>线路概览</summary>

![radar]({{ '/assets/images/mkcloud-sha-nrt/radar.png' | relative_url }})

</details>

<details markdown="1">
<summary>出口到主要公共服务的延迟测试</summary>

| 服务 | 平均延迟 |
|---|---:|
| Apple | 26.252 ms |
| Google | 25.597 ms |
| Cloudflare | 25.830 ms |
| AWS | 25.862 ms |
| GitHub | 26.570 ms |

</details>

### 实时监控

- **端内实时状态监控**：<https://ping.nxtrace.org/goto/04v7U8vDg>
- **端内状态监控截图**：
  <details markdown="1">
  <summary>展开查看</summary>
  
  ![端内延迟监控截图]({{ '/assets/images/mkcloud-sha-nrt/端内延迟监控截图（近七天）.png' | relative_url }})

  </details>

<details markdown="1">
<summary>三网延迟测试</summary>

| 城市 | 电信 | 联通 | 移动 |
|---|---:|---:|---:|
| 北京 | 20.868 ms | 27.839 ms | 29.171 ms |
| 上海 | 3.772 ms | 6.367 ms | 8.595 ms |
| 广州 | 29.345 ms | 29.876 ms | 36.261 ms |
| 成都 | 34.386 ms | 34.616 ms | 39.607 ms |
| 西安 | 26.069 ms | 29.052 ms | 32.599 ms |
| 杭州 | 10.200 ms | 17.023 ms | 9.344 ms |

</details>

<details markdown="1">
<summary>国际网络带宽测试</summary>

| 服务商 | 地点 | 发送速度 | 接收速度 | 延迟 |
|---|---|---:|---:|---:|
| Clouvider | London, UK (10G) | 136 Mbits/sec | 77.5 Mbits/sec | 251 ms |
| Eranium | Amsterdam, NL (100G) | 138 Mbits/sec | 121 Mbits/sec | 267 ms |
| Uztelecom | Tashkent, UZ (10G) | 1.01 Mbits/sec | 62.4 Mbits/sec | 268 ms |
| Leaseweb | Singapore, SG (10G) | 118 Mbits/sec | 131 Mbits/sec | 142 ms |
| Clouvider | Los Angeles, CA, US (10G) | 149 Mbits/sec | 136 Mbits/sec | 123 ms |
| Leaseweb | NYC, NY, US (10G) | 145 Mbits/sec | 102 Mbits/sec | 189 ms |
| Edgoo | Sao Paulo, BR (1G) | 131 Mbits/sec | 88.4 Mbits/sec | 311 ms |

</details>

### 单线程测速（iperf3）

<details markdown="1">
<summary>北京移动晚高峰</summary>

![北京移动晚高峰]({{ '/assets/images/mkcloud-sha-nrt/北京四网单线程测速/北京移动晚高峰.png' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通晚高峰</summary>

![北京联通晚高峰]({{ '/assets/images/mkcloud-sha-nrt/北京四网单线程测速/北京联通晚高峰.png' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通晚高峰</summary>

![北京网通晚高峰]({{ '/assets/images/mkcloud-sha-nrt/北京四网单线程测速/北京网通晚高峰.png' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信晚高峰</summary>

![北京电信晚高峰]({{ '/assets/images/mkcloud-sha-nrt/北京四网单线程测速/北京电信晚高峰.png' | relative_url }})

</details>

### CDN 测速

<details markdown="1">
<summary>Apple CDN</summary>

![Apple CDN 测速]({{ '/assets/images/mkcloud-sha-nrt/CDN测速/截屏2026-05-08 下午3.09.20.png' | relative_url }})

</details>

<details markdown="1">
<summary>Cloudflare CDN</summary>

![Cloudflare CDN 测速]({{ '/assets/images/mkcloud-sha-nrt/CDN测速/截屏2026-05-08 下午3.09.26.png' | relative_url }})

</details>

### 机器性能跑分

<details markdown="1">
<summary>综合性能跑分（YABS）</summary>

![综合性能跑分]({{ '/assets/images/mkcloud-sha-nrt/综合性能跑分.png' | relative_url }})

</details>

### IP 解锁

<details markdown="1">
<summary>流媒体 / 平台解锁记录</summary>

![解锁情况]({{ '/assets/images/mkcloud-sha-nrt/解锁情况/2026-02-17 22.39.51.png' | relative_url }})

</details>
