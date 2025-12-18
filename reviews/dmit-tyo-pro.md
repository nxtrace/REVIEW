---
layout: default
title: "🇯🇵 DMIT.TYO.Pro 日本东京 CN2 VPS 测评"
seo_keywords: "DMIT 东京, DMIT 日本, DMIT, CN2, 东京VPS, 日本VPS, EPYC, JP"
redirect_from:
  - /reviews/dmit-tyo-pro.md
  - /REVIEW/reviews/dmit-tyo-pro.md
---

# 🇯🇵 DMIT.TYO.Pro 日本东京 CN2 VPS 测评

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

- [**官方购买入口**](https://www.dmit.io/aff.php?aff=3487)

### 规格对照

<details markdown="1">
<summary>TYO.AS3.Pro（Premium Routing Profile）</summary>

| 套餐 | vCPU | 内存 | SSD | 流量（双向） | 端口 | 月付 |
|---|---:|---:|---:|---:|---:|---:|
| TYO.AS3.Pro.TINY | 1 Core | 1 GB | 20 GB | 500 GB | 1 Gbps | $21.90 |
| TYO.AS3.Pro.STARTER | 1 Core | 2 GB | 40 GB | 1 TB | 1 Gbps | $39.90 |
| TYO.AS3.Pro.MINI | 2 Cores | 2 GB | 60 GB | 2 TB | 1 Gbps | $79.90 |
| TYO.AS3.Pro.MICRO | 4 Cores | 4 GB | 80 GB | 4 TB | 1 Gbps | $159.90 |
| TYO.AS3.Pro.MEDIUM | 4 Cores | 8 GB | 160 GB | 5 TB | 1 Gbps | $259.90 |
| TYO.AS3.Pro.LARGE | 8 Cores | 16 GB | 320 GB | 8 TB | 1 Gbps | $429.90 |
| TYO.AS3.Pro.GIANT | 8 Cores | 24 GB | 640 GB | 15 TB | 1 Gbps | $799.90 |

> 说明：每个套餐包含 `1 IPv4` 与 `1 IPv6 /64`，支持 DDoS Protect（Standard）与自定义 RAM/SSD。

</details>

## 评

对于电信用户算是日本无掺水 CN2 产品中性价比较高的了，商家信誉及机器稳定性也都很好，  
用电信宽带的富哥可以考虑一下这款产品，联通/移动宽带用户需关注所在地区跨网拥堵情况  
**电信用户速度还是比较稳定**的跑到 600Mbps 以上  
**移动联通用户慎重选择**  

三网 CTG GIA(aka CN2 GIA)回程  
电信 / 联通 CTG GIA 去程  
移动 CMI 去程  
IPv6 有三网优化（163 + CMI 可用性尚可）  

## 测

### 路由表现

<details markdown="1">
<summary>线路概览</summary>

**IPv4 路由图**
![ipv4-radar]({{ '/assets/images/dmit-tyo-pro/4-radar.png' | relative_url }})

**IPv6 路由图**
![ipv6-radar]({{ '/assets/images/dmit-tyo-pro/6-radar.png' | relative_url }})

</details>

<details markdown="1">
<summary>IPv4 去程</summary>

<div align="center">
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv4去程/2025-12-15 15.43.04.png' | relative_url }}" alt="IPv4 去程路由 1" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv4去程/2025-12-15 15.43.05.png' | relative_url }}" alt="IPv4 去程路由 2" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv4去程/2025-12-15 15.43.06.png' | relative_url }}" alt="IPv4 去程路由 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · ICMP</summary>

<div align="center">
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv4 回程 · ICMP/2025-12-15 15.41.00.png' | relative_url }}" alt="IPv4 回程 ICMP 1" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv4 回程 · ICMP/2025-12-15 15.41.02.png' | relative_url }}" alt="IPv4 回程 ICMP 2" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv4 回程 · ICMP/2025-12-15 15.41.04.png' | relative_url }}" alt="IPv4 回程 ICMP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · TCP</summary>

<div align="center">
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv4 回程 · TCP/2025-12-15 15.41.41.png' | relative_url }}" alt="IPv4 回程 TCP 1" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv4 回程 · TCP/2025-12-15 15.41.56.png' | relative_url }}" alt="IPv4 回程 TCP 2" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv4 回程 · TCP/2025-12-15 15.41.57.png' | relative_url }}" alt="IPv4 回程 TCP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv6 去程</summary>

<div align="center">
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv6去程/2025-12-15 15.53.39.png' | relative_url }}" alt="IPv6 去程路由 1" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv6去程/2025-12-15 15.53.41.png' | relative_url }}" alt="IPv6 去程路由 2" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv6去程/2025-12-15 15.53.43.png' | relative_url }}" alt="IPv6 去程路由 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv6 回程 · ICMP</summary>

<div align="center">
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv6 回程 · ICMP/2025-12-15 16.39.59.png' | relative_url }}" alt="IPv6 回程 ICMP 1" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv6 回程 · ICMP/2025-12-15 16.40.04.png' | relative_url }}" alt="IPv6 回程 ICMP 2" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv6 回程 · ICMP/2025-12-15 16.40.06.png' | relative_url }}" alt="IPv6 回程 ICMP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv6 回程 · TCP</summary>

<div align="center">
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv6 回程 · TCP/2025-12-15 16.40.32.png' | relative_url }}" alt="IPv6 回程 TCP 1" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv6 回程 · TCP/2025-12-15 16.40.36.png' | relative_url }}" alt="IPv6 回程 TCP 2" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv6 回程 · TCP/2025-12-15 16.40.39.png' | relative_url }}" alt="IPv6 回程 TCP 3" width="32%" />
</div>

</details>

### 实时监控
- **实时三网 ICMP**：<https://ping.nxtrace.org/goto/sOhaZeSNg>
- **实时三网 TCP**：<https://ping.nxtrace.org/goto/haLnM6IHg>
- **Looking Glass**：<https://lg.dmit.sh/?server=tyo-pro>
- **北京三网延迟监控截图**：
  <details markdown="1">
  <summary>展开查看</summary>
  
  ![北京三网延迟监控截图]({{ '/assets/images/dmit-tyo-pro/北京三网延迟监控截图.png' | relative_url }})
  
  </details>

### 北京四网代理单线程测速

<details markdown="1">
<summary>北京移动晚高峰</summary>

![北京移动晚高峰]({{ '/assets/images/dmit-tyo-pro/北京四网代理单线程测速/北京移动晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京移动白天</summary>

![北京移动白天]({{ '/assets/images/dmit-tyo-pro/北京四网代理单线程测速/北京移动白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通晚高峰</summary>

![北京联通晚高峰]({{ '/assets/images/dmit-tyo-pro/北京四网代理单线程测速/北京联通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通白天</summary>

![北京联通白天]({{ '/assets/images/dmit-tyo-pro/北京四网代理单线程测速/北京联通白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通晚高峰</summary>

![北京网通晚高峰]({{ '/assets/images/dmit-tyo-pro/北京四网代理单线程测速/北京网通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通白天</summary>

![北京网通白天]({{ '/assets/images/dmit-tyo-pro/北京四网代理单线程测速/北京网通白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信晚高峰</summary>

![北京电信晚高峰]({{ '/assets/images/dmit-tyo-pro/北京四网代理单线程测速/北京电信晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信白天</summary>

![北京电信白天]({{ '/assets/images/dmit-tyo-pro/北京四网代理单线程测速/北京电信白天.jpg' | relative_url }})

</details>

### 机器性能跑分

<details markdown="1">
<summary>综合性能跑分（YABS·GB5）</summary>

![综合性能跑分]({{ '/assets/images/dmit-tyo-pro/综合性能跑分.png' | relative_url }})

</details>

### IP 解锁

<details markdown="1">
<summary>流媒体 / 平台解锁记录</summary>

![解锁情况 1]({{ '/assets/images/dmit-tyo-pro/解锁情况/2025-12-15 15.36.38.png' | relative_url }})
![解锁情况 2]({{ '/assets/images/dmit-tyo-pro/解锁情况/2025-12-15 15.36.50.png' | relative_url }})

</details>
