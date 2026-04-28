---
layout: default
title: "🇺🇸 咸鱼云 Saltyfish San Jose Premium 美国圣何塞 CN2 GIA CMIN2 VPS 测评"
seo_keywords: "圣何塞VPS, SJC, 咸鱼云, Saltyfish, CN2 GIA, CTG GIA, CMIN2, snapstack, 美国VPS"
redirect_from:
  - /reviews/saltyfish-sjc-pro.md
  - /REVIEW/reviews/saltyfish-sjc-pro.md
---

# 🇺🇸 咸鱼云 Saltyfish San Jose Premium 美国圣何塞 CN2 GIA CMIN2 VPS 测评

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

- [**官方购买入口**](https://portal.saltyfish.io/aff.php?aff=610&gid=15)

### 规格对照

> China Mainland Optimized by China Telecom CN2 GIA.

<details markdown="1">
<summary>San Jose VPS - Premium Network</summary>

| 套餐 | vCPU | 内存 | SSD | 流量 | 端口 | 月付 |
|---|---:|---:|---:|---:|---:|---:|
| sjc.p1.mini | 1 | 1 GB | 10 GB | 1000 GB | 1 Gbps | ¥47.60 |
| sjc.p1.micro | 1 | 2 GB | 15 GB | 2000 GB | 1 Gbps | ¥98.00 |
| sjc.p1.medium | 2 | 4 GB | 30 GB | 4000 GB | 1 Gbps | ¥196.00 |

</details>

## 评

咸鱼云美国圣何塞 CN2 GIA 小鸡，三网速度晚高峰都可以跑到800Mbps，  
电信/移动方向延迟低且稳定，适合电信用户选择，联通用户因跨网可能有一定的波动，需谨慎考虑。  

电信 CTG GIA (aka: CN2 GIA）回程 / CTG GIA 去程  
联通 CTG GIA 回程 / CUG VIP (aka: 9929) 去程  
移动 CMIN2 回程 / CMIN2 去程  

## 测

### 路由表现

<details markdown="1">
<summary>线路概览</summary>

**IPv4 路由图**
![ipv4-radar]({{ '/assets/images/saltyfish-sjc-pro/radar.png' | relative_url }})

</details>

<details markdown="1">
<summary>IPv4 去程</summary>

<div align="center">
  <img src="{{ '/assets/images/saltyfish-sjc-pro/IPv4去程/2025-12-25 21.05.37.png' | relative_url }}" alt="IPv4 去程路由 1" width="32%" />
  <img src="{{ '/assets/images/saltyfish-sjc-pro/IPv4去程/2025-12-25 21.05.39.png' | relative_url }}" alt="IPv4 去程路由 2" width="32%" />
  <img src="{{ '/assets/images/saltyfish-sjc-pro/IPv4去程/2025-12-25 21.05.40.png' | relative_url }}" alt="IPv4 去程路由 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · ICMP</summary>

<div align="center">
  <img src="{{ '/assets/images/saltyfish-sjc-pro/IPv4 回程 · ICMP/2026-04-28 20.10.53.png' | relative_url }}" alt="IPv4 回程 ICMP 1" width="32%" />
  <img src="{{ '/assets/images/saltyfish-sjc-pro/IPv4 回程 · ICMP/2025-12-25 20.56.14.png' | relative_url }}" alt="IPv4 回程 ICMP 2" width="32%" />
  <img src="{{ '/assets/images/saltyfish-sjc-pro/IPv4 回程 · ICMP/2025-12-25 20.56.15.png' | relative_url }}" alt="IPv4 回程 ICMP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · TCP</summary>

<div align="center">
  <img src="{{ '/assets/images/saltyfish-sjc-pro/IPv4 回程 · TCP/2026-04-28 20.12.19.png' | relative_url }}" alt="IPv4 回程 TCP 1" width="32%" />
  <img src="{{ '/assets/images/saltyfish-sjc-pro/IPv4 回程 · TCP/2025-12-25 21.01.42.png' | relative_url }}" alt="IPv4 回程 TCP 2" width="32%" />
  <img src="{{ '/assets/images/saltyfish-sjc-pro/IPv4 回程 · TCP/2025-12-25 21.01.43.png' | relative_url }}" alt="IPv4 回程 TCP 3" width="32%" />
</div>

</details>

### 实时监控
- **实时三网 ICMP**：<https://ping.nxtrace.org/goto/NmbPownHR>
- **实时三网 TCP**：<https://ping.nxtrace.org/goto/ZzuEownNg>
- **实时 MTR 监控**：<https://ping.nxtrace.org/goto/TwHr-tnvg>
- **官方 Looking Glass**：<https://lg.saltyfish.io/?router=sjc-premium>
- **北京三网延迟监控截图**：
  <details markdown="1">
  <summary>展开查看</summary>
  
  ![北京三网延迟监控截图]({{ '/assets/images/saltyfish-sjc-pro/北京三网延迟监控截图.png' | relative_url }})
  
  </details>

### 北京四网代理单线程测速

<details markdown="1">
<summary>北京移动晚高峰</summary>

![北京移动晚高峰]({{ '/assets/images/saltyfish-sjc-pro/北京四网代理单线程测速/北京移动晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京移动白天</summary>

![北京移动白天]({{ '/assets/images/saltyfish-sjc-pro/北京四网代理单线程测速/北京移动白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通晚高峰</summary>

![北京联通晚高峰]({{ '/assets/images/saltyfish-sjc-pro/北京四网代理单线程测速/北京联通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通白天</summary>

![北京联通白天]({{ '/assets/images/saltyfish-sjc-pro/北京四网代理单线程测速/北京联通白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通晚高峰</summary>

![北京网通晚高峰]({{ '/assets/images/saltyfish-sjc-pro/北京四网代理单线程测速/北京网通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通白天</summary>

![北京网通白天]({{ '/assets/images/saltyfish-sjc-pro/北京四网代理单线程测速/北京网通白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信晚高峰</summary>

![北京电信晚高峰]({{ '/assets/images/saltyfish-sjc-pro/北京四网代理单线程测速/北京电信晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信白天</summary>

![北京电信白天]({{ '/assets/images/saltyfish-sjc-pro/北京四网代理单线程测速/北京电信白天.jpg' | relative_url }})

</details>

### 机器性能跑分

<details markdown="1">
<summary>综合性能跑分（YABS·GB4）</summary>

![综合性能跑分]({{ '/assets/images/saltyfish-sjc-pro/综合性能跑分.png' | relative_url }})

</details>

### IP 解锁

<details markdown="1">
<summary>流媒体 / 平台解锁记录</summary>

![解锁情况]({{ '/assets/images/saltyfish-sjc-pro/解锁情况/2025-12-25 20.49.00.png' | relative_url }})

</details>
