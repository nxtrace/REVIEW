---
layout: default
title: "🇸🇬 V.PS Performance Singapore 新加坡 CN2 VPS 详细测评"
seo_keywords: "V.PS Singapore Performance KVM VPS, V.PS Singapore EPYC Explorer, xtom, sa.net, Riven Cloud, CN2, 新加坡VPS, EPYC, SG"
redirect_from:
  - /reviews/xtom-singapore-epyc.md
  - /REVIEW/reviews/xtom-singapore-epyc.md
---

# 🇸🇬 V.PS Performance Singapore 新加坡 CN2 VPS 详细测评

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

### 购买信息

- [**官方购买入口**](https://vps.hosting/?affid=2152&oid=36)

### 规格对照

<details markdown="1">
<summary>xTom Singapore (Performance KVM VPS)</summary>

| 套餐 | vCPU | 内存 | NVMe | 流量（单向 In+Out） | 端口 | 月付 |
|---|---:|---:|---:|---:|---:|---:|
| Singapore EPYC Explorer | 2 Cores | 2 GB | 30 GB | 1 TB | 1 Gbps | €42.95 |
| Singapore EPYC Enhancer | 4 Cores | 4 GB | 60 GB | 2 TB | 1.25 Gbps | €84.95 |
| Singapore EPYC Enterprise | 4 Cores | 8 GB | 120 GB | 4 TB | 1.5 Gbps | €169.95 |
| Singapore EPYC Elite | 8 Cores | 16 GB | 240 GB | 8 TB | 2 Gbps | €329.95 |

</details>

## 评

市场上少见的新加坡CN2小鸡，联通方向有9929去程但是没给回程，算是电信快乐鸡吧，联通用户要看所在地区跨网拥堵情况，考虑产品价格，更推荐电信宽带的富哥购买  
**电信用户速度还是比较稳定**的跑到 600Mbps 以上  
**移动联通用户慎重选择**  

三网 CTG GIA(aka CN2 GIA) 回程  
电信 CTG GIA 去程  
联通 CUG VIP(aka 9929) 去程  
移动 CMI 去程  
另 IPv6 有三网优化但是就电信方向能用（163）  

## 测

### 路由表现

<details markdown="1">
<summary>线路概览</summary>

**IPv4 路由图**
![ipv4-radar]({{ '/assets/images/xtom-singapore-epyc/4-radar.png' | relative_url }})

**IPv6 路由图**
![ipv6-radar]({{ '/assets/images/xtom-singapore-epyc/6-radar.png' | relative_url }})

</details>

<details markdown="1">
<summary>IPv4 去程</summary>

<div align="center">
  <img src="{{ '/assets/images/xtom-singapore-epyc/IPv4去程/IMAGE 2025-12-14 17:54:34.jpg' | relative_url }}" alt="IPv4 去程路由 1" width="32%" />
  <img src="{{ '/assets/images/xtom-singapore-epyc/IPv4去程/IMAGE 2025-12-14 17:54:35.jpg' | relative_url }}" alt="IPv4 去程路由 2" width="32%" />
  <img src="{{ '/assets/images/xtom-singapore-epyc/IPv4去程/IMAGE 2025-12-14 17:54:37.jpg' | relative_url }}" alt="IPv4 去程路由 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · ICMP</summary>

<div align="center">
  <img src="{{ '/assets/images/xtom-singapore-epyc/IPv4 回程 · ICMP/IMAGE 2025-12-14 17:54:55.jpg' | relative_url }}" alt="IPv4 回程 ICMP 1" width="32%" />
  <img src="{{ '/assets/images/xtom-singapore-epyc/IPv4 回程 · ICMP/IMAGE 2025-12-14 17:54:56.jpg' | relative_url }}" alt="IPv4 回程 ICMP 2" width="32%" />
  <img src="{{ '/assets/images/xtom-singapore-epyc/IPv4 回程 · ICMP/IMAGE 2025-12-14 17:54:58.jpg' | relative_url }}" alt="IPv4 回程 ICMP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · TCP</summary>

<div align="center">
  <img src="{{ '/assets/images/xtom-singapore-epyc/IPv4 回程 · TCP/IMAGE 2025-12-14 17:54:47.jpg' | relative_url }}" alt="IPv4 回程 TCP 1" width="32%" />
  <img src="{{ '/assets/images/xtom-singapore-epyc/IPv4 回程 · TCP/IMAGE 2025-12-14 17:54:49.jpg' | relative_url }}" alt="IPv4 回程 TCP 2" width="32%" />
  <img src="{{ '/assets/images/xtom-singapore-epyc/IPv4 回程 · TCP/IMAGE 2025-12-14 17:54:50.jpg' | relative_url }}" alt="IPv4 回程 TCP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv6 去程</summary>

<div align="center">
  <img src="{{ '/assets/images/xtom-singapore-epyc/IPv6去程/IMAGE 2025-12-14 17:55:15.jpg' | relative_url }}" alt="IPv6 去程路由 1" width="32%" />
  <img src="{{ '/assets/images/xtom-singapore-epyc/IPv6去程/IMAGE 2025-12-14 17:55:17.jpg' | relative_url }}" alt="IPv6 去程路由 2" width="32%" />
  <img src="{{ '/assets/images/xtom-singapore-epyc/IPv6去程/IMAGE 2025-12-14 17:55:18.jpg' | relative_url }}" alt="IPv6 去程路由 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv6 回程 · ICMP</summary>

<div align="center">
  <img src="{{ '/assets/images/xtom-singapore-epyc/IPv6 回程 · ICMP/IMAGE 2025-12-14 17:55:28.jpg' | relative_url }}" alt="IPv6 回程 ICMP 1" width="32%" />
  <img src="{{ '/assets/images/xtom-singapore-epyc/IPv6 回程 · ICMP/IMAGE 2025-12-14 17:55:30.jpg' | relative_url }}" alt="IPv6 回程 ICMP 2" width="32%" />
  <img src="{{ '/assets/images/xtom-singapore-epyc/IPv6 回程 · ICMP/IMAGE 2025-12-14 17:55:31.jpg' | relative_url }}" alt="IPv6 回程 ICMP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv6 回程 · TCP</summary>

<div align="center">
  <img src="{{ '/assets/images/xtom-singapore-epyc/IPv6 回程 · TCP/IMAGE 2025-12-14 17:55:09.jpg' | relative_url }}" alt="IPv6 回程 TCP 1" width="32%" />
  <img src="{{ '/assets/images/xtom-singapore-epyc/IPv6 回程 · TCP/IMAGE 2025-12-14 17:55:10.jpg' | relative_url }}" alt="IPv6 回程 TCP 2" width="32%" />
  <img src="{{ '/assets/images/xtom-singapore-epyc/IPv6 回程 · TCP/IMAGE 2025-12-14 17:55:11.jpg' | relative_url }}" alt="IPv6 回程 TCP 3" width="32%" />
</div>

</details>

### 实时监控
- **实时三网 ICMP**：<https://ping.nxtrace.org/goto/yCkoicMDR>
- **实时三网 TCP**：<https://ping.nxtrace.org/goto/C_dom5MvR>
- **北京三网延迟监控截图**：
  <details markdown="1">
  <summary>展开查看</summary>
  
  ![北京三网延迟监控截图]({{ '/assets/images/xtom-singapore-epyc/北京三网延迟监控截图.png' | relative_url }})
  
  </details>

### 北京四网代理单线程测速

<details markdown="1">
<summary>北京移动晚高峰</summary>

![北京移动晚高峰]({{ '/assets/images/xtom-singapore-epyc/北京四网代理单线程测速/北京移动晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京移动白天</summary>

![北京移动白天]({{ '/assets/images/xtom-singapore-epyc/北京四网代理单线程测速/北京移动白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通晚高峰</summary>

![北京联通晚高峰]({{ '/assets/images/xtom-singapore-epyc/北京四网代理单线程测速/北京联通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通白天</summary>

![北京联通白天]({{ '/assets/images/xtom-singapore-epyc/北京四网代理单线程测速/北京联通白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通晚高峰</summary>

![北京网通晚高峰]({{ '/assets/images/xtom-singapore-epyc/北京四网代理单线程测速/北京网通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通白天</summary>

![北京网通白天]({{ '/assets/images/xtom-singapore-epyc/北京四网代理单线程测速/北京网通白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信晚高峰</summary>

![北京电信晚高峰]({{ '/assets/images/xtom-singapore-epyc/北京四网代理单线程测速/北京电信晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信白天</summary>

![北京电信白天]({{ '/assets/images/xtom-singapore-epyc/北京四网代理单线程测速/北京电信白天.jpg' | relative_url }})

</details>

### 机器性能跑分

<details markdown="1">
<summary>综合性能跑分</summary>

![综合性能跑分]({{ '/assets/images/xtom-singapore-epyc/综合性能跑分.jpg' | relative_url }})

</details>

### IP 解锁

<details markdown="1">
<summary>流媒体 / 平台解锁记录</summary>

![解锁情况 1]({{ '/assets/images/xtom-singapore-epyc/解锁情况/IMAGE 2025-12-14 17:56:52.jpg' | relative_url }})
![解锁情况 2]({{ '/assets/images/xtom-singapore-epyc/解锁情况/IMAGE 2025-12-14 17:56:53.jpg' | relative_url }})

</details>
