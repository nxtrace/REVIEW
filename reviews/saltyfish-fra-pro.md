---
layout: default
title: "🇩🇪 咸鱼云 Saltyfish Frankfurt Premium 德国法兰克福 CN2 GIA VPS 测评"
seo_keywords: "法兰克福VPS, FRA, 咸鱼云, Saltyfish, CN2 GIA, CTG GIA, snapstack, CMIN2, 德国VPS"
redirect_from:
  - /reviews/saltyfish-fra-pro.md
  - /REVIEW/reviews/saltyfish-fra-pro.md
---

# 🇩🇪 咸鱼云 Saltyfish Frankfurt Premium 德国法兰克福 CN2 GIA VPS 测评

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

- [**官方购买入口**](https://portal.saltyfish.io/aff.php?aff=610&gid=14)

### 规格对照

> China Mainland Optimized by China Telecom CN2 GIA.

<details markdown="1">
<summary>Frankfurt VPS - Premium Network</summary>

| 套餐 | vCPU | 内存 | SSD | 流量 | 端口 | 月付 |
|---|---:|---:|---:|---:|---:|---:|
| fra.p1.mini | 1 | 1 GB | 15 GB | 1000 GB | 2.5 Gbps | ¥54.60 |
| fra.p1.micro | 1 | 2 GB | 20 GB | 2000 GB | 2.5 Gbps | ¥105.00 |
| fra.p1.medium | 2 | 4 GB | 40 GB | 4000 GB | 2.5 Gbps | ¥210.00 |

</details>

## 评

咸鱼云德国法兰克福 CN2 GIA+CMIN2 小鸡，线路优秀。  
适合电信/移动用户选择，对于北方用户晚高峰三网都可以跑500-800Mbps，  
而且目前该产品线所有机型均已升级2.5Gbps端口，算是欧洲鸡中经济实惠的选择了。  

电信 CTG GIA (aka: CN2 GIA）回程 / CTG GIA 去程  
联通 CTG GIA 回程 / CUG VIP (aka: 9929) 去程  
移动 CMIN2 回程 / CMIN2 去程

## 测

### 路由表现

<details markdown="1">
<summary>线路概览</summary>

**IPv4 路由图**
![ipv4-radar]({{ '/assets/images/saltyfish-fra-pro/radar.png' | relative_url }})

</details>

<details markdown="1">
<summary>IPv4 去程</summary>

<div align="center">
  <img src="{{ '/assets/images/saltyfish-fra-pro/IPv4去程/IMAGE 2025-12-15 14:54:21.jpg' | relative_url }}" alt="IPv4 去程路由 1" width="32%" />
  <img src="{{ '/assets/images/saltyfish-fra-pro/IPv4去程/IMAGE 2025-12-15 14:54:22.jpg' | relative_url }}" alt="IPv4 去程路由 2" width="32%" />
  <img src="{{ '/assets/images/saltyfish-fra-pro/IPv4去程/IMAGE 2025-12-15 14:54:24.jpg' | relative_url }}" alt="IPv4 去程路由 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · ICMP</summary>

<div align="center">
  <img src="{{ '/assets/images/saltyfish-fra-pro/IPv4 回程 · ICMP/IMAGE 2025-12-15 14:54:32.jpg' | relative_url }}" alt="IPv4 回程 ICMP 1" width="32%" />
  <img src="{{ '/assets/images/saltyfish-fra-pro/IPv4 回程 · ICMP/IMAGE 2025-12-15 14:54:33.jpg' | relative_url }}" alt="IPv4 回程 ICMP 2" width="32%" />
  <img src="{{ '/assets/images/saltyfish-fra-pro/IPv4 回程 · ICMP/IMAGE 2025-12-15 14:54:34.jpg' | relative_url }}" alt="IPv4 回程 ICMP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · TCP</summary>

<div align="center">
  <img src="{{ '/assets/images/saltyfish-fra-pro/IPv4 回程 · TCP/IMAGE 2025-12-15 14:54:41.jpg' | relative_url }}" alt="IPv4 回程 TCP 1" width="32%" />
  <img src="{{ '/assets/images/saltyfish-fra-pro/IPv4 回程 · TCP/IMAGE 2025-12-15 14:54:43.jpg' | relative_url }}" alt="IPv4 回程 TCP 2" width="32%" />
  <img src="{{ '/assets/images/saltyfish-fra-pro/IPv4 回程 · TCP/IMAGE 2025-12-15 14:54:44.jpg' | relative_url }}" alt="IPv4 回程 TCP 3" width="32%" />
</div>

</details>

### 实时监控
- **实时三网 ICMP**：<https://ping.nxtrace.org/goto/EUq7aUqIg>
- **实时三网 TCP**：<https://ping.nxtrace.org/goto/FOPV-83Ig>
- **官方 Looking Glass**：<https://lg.saltyfish.io/?router=fra-premium>
- **北京三网延迟监控截图**：
  <details markdown="1">
  <summary>展开查看</summary>
  
  ![北京三网延迟监控截图]({{ '/assets/images/saltyfish-fra-pro/北京三网延迟监控截图.png' | relative_url }})
  
  </details>

### 北京四网代理单线程测速

<details markdown="1">
<summary>北京移动晚高峰</summary>

![北京移动晚高峰]({{ '/assets/images/saltyfish-fra-pro/北京四网代理单线程测速/北京移动晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京移动白天</summary>

![北京移动白天]({{ '/assets/images/saltyfish-fra-pro/北京四网代理单线程测速/北京移动白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通晚高峰</summary>

![北京联通晚高峰]({{ '/assets/images/saltyfish-fra-pro/北京四网代理单线程测速/北京联通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通白天</summary>

![北京联通白天]({{ '/assets/images/saltyfish-fra-pro/北京四网代理单线程测速/北京联通白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通晚高峰</summary>

![北京网通晚高峰]({{ '/assets/images/saltyfish-fra-pro/北京四网代理单线程测速/北京网通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通白天</summary>

![北京网通白天]({{ '/assets/images/saltyfish-fra-pro/北京四网代理单线程测速/北京网通白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信晚高峰</summary>

![北京电信晚高峰]({{ '/assets/images/saltyfish-fra-pro/北京四网代理单线程测速/北京电信晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信白天</summary>

![北京电信白天]({{ '/assets/images/saltyfish-fra-pro/北京四网代理单线程测速/北京电信白天.jpg' | relative_url }})

</details>

### 机器性能跑分

<details markdown="1">
<summary>综合性能跑分（YABS·GB4）</summary>

![综合性能跑分]({{ '/assets/images/saltyfish-fra-pro/综合性能跑分.png' | relative_url }})

</details>

### IP 解锁

<details markdown="1">
<summary>流媒体 / 平台解锁记录</summary>

![解锁情况]({{ '/assets/images/saltyfish-fra-pro/解锁情况/2025-12-15 15.11.25.png' | relative_url }})

</details>
