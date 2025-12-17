---
layout: default
title: DMIT.LAX.Pro
seo_keywords: "DMIT 洛杉矶 Pro, DMIT LAX, CN2 GIA, 美国VPS, Premium Routing"
redirect_from:
  - /reviews/dmit-lax-pro.md
  - /REVIEW/reviews/dmit-lax-pro.md
---

# DMIT.LAX.Pro

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

### 规格对照

- 硬件有 AN4 / AN5 两档，性能差异较大（见下方跑分）。
- 测试 IP：`154.17.30.96`

<details markdown="1">
<summary>LAX.AN5.Pro（Premium Routing Profile）</summary>

| 套餐 | vCPU | 内存 | SSD | 流量（双向） | 端口 | 月付 |
|---|---:|---:|---:|---:|---:|---:|
| LAX.AN5.Pro.TINY | 1 | 2 GB | 20 GB | 1 TB | 1 Gbps | $9.99 |
| LAX.AN5.Pro.POCKET | 2 | 2 GB | 40 GB | 1.5 TB | 4 Gbps | $14.90 |
| LAX.AN5.Pro.STARTER | 2 | 2 GB | 80 GB | 3 TB | 10 Gbps | $29.90 |
| LAX.AN5.Pro.MINI | 4 | 4 GB | 80 GB | 5 TB | 10 Gbps | $58.88 |
| LAX.AN5.Pro.MICRO | 4 | 4 GB | 160 GB | 7 TB | 10 Gbps | $74.99 |
| LAX.AN5.Pro.MEDIUM | 6 | 8 GB | 160 GB | 14 TB | 10 Gbps | $168.88 |
| LAX.AN5.Pro.LARGE | 8 | 16 GB | 320 GB | 25 TB | 10 Gbps | $338.88 |
| LAX.AN5.Pro.GIANT | 12 | 24 GB | 640 GB | 50 TB | 10 Gbps | $619.99 |

> 说明：套餐含 `1 IPv4` 与 `1 IPv6 /64`，DDoS Protect（Standard），超额降速（TINY/Pocket 为 4 Mbps，MINI/MICRO 为 8 Mbps，MEDIUM 及以上为 10 Mbps）。

</details>

### 购买链接

- [DMIT LAX Pro](https://www.dmit.io/aff.php?aff=3487&pid=186)

## 评

三网 CTG GIA（CN2 GIA）回程；  
电信 CTG GIA 去程；  
联通 CUG VIP（9929）去程；  
移动 CMIN2 去程；  
IPv6 双程三网优化，已是最优路由。

## 测

### 路由表现

<details markdown="1">
<summary>线路概览</summary>

**IPv4 路由图**
![ipv4-radar]({{ '/assets/images/dmit-lax-pro/4-radar.png' | relative_url }})

**IPv6 路由图**
![ipv6-radar]({{ '/assets/images/dmit-lax-pro/6-radar.png' | relative_url }})

</details>

<details markdown="1">
<summary>IPv4 去程</summary>

<div align="center">
  <img src="{{ '/assets/images/dmit-lax-pro/IPv4去程/2025-12-17 11.16.30.png' | relative_url }}" alt="IPv4 去程路由 1" width="32%" />
  <img src="{{ '/assets/images/dmit-lax-pro/IPv4去程/2025-12-17 11.16.32.png' | relative_url }}" alt="IPv4 去程路由 2" width="32%" />
  <img src="{{ '/assets/images/dmit-lax-pro/IPv4去程/2025-12-17 11.16.33.png' | relative_url }}" alt="IPv4 去程路由 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · ICMP</summary>

<div align="center">
  <img src="{{ '/assets/images/dmit-lax-pro/IPv4 回程 · ICMP/2025-12-17 11.11.18.png' | relative_url }}" alt="IPv4 回程 ICMP 1" width="32%" />
  <img src="{{ '/assets/images/dmit-lax-pro/IPv4 回程 · ICMP/2025-12-17 11.11.19.png' | relative_url }}" alt="IPv4 回程 ICMP 2" width="32%" />
  <img src="{{ '/assets/images/dmit-lax-pro/IPv4 回程 · ICMP/2025-12-17 11.11.20.png' | relative_url }}" alt="IPv4 回程 ICMP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · TCP</summary>

<div align="center">
  <img src="{{ '/assets/images/dmit-lax-pro/IPv4 回程 · TCP/2025-12-17 11.12.06.png' | relative_url }}" alt="IPv4 回程 TCP 1" width="32%" />
  <img src="{{ '/assets/images/dmit-lax-pro/IPv4 回程 · TCP/2025-12-17 11.12.07.png' | relative_url }}" alt="IPv4 回程 TCP 2" width="32%" />
  <img src="{{ '/assets/images/dmit-lax-pro/IPv4 回程 · TCP/2025-12-17 11.12.09.png' | relative_url }}" alt="IPv4 回程 TCP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv6 去程</summary>

<div align="center">
  <img src="{{ '/assets/images/dmit-lax-pro/IPv6去程/2025-12-17 11.27.19.png' | relative_url }}" alt="IPv6 去程路由 1" width="32%" />
  <img src="{{ '/assets/images/dmit-lax-pro/IPv6去程/2025-12-17 11.27.21.png' | relative_url }}" alt="IPv6 去程路由 2" width="32%" />
  <img src="{{ '/assets/images/dmit-lax-pro/IPv6去程/2025-12-17 11.27.22.png' | relative_url }}" alt="IPv6 去程路由 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv6 回程 · ICMP</summary>

<div align="center">
  <img src="{{ '/assets/images/dmit-lax-pro/IPv6 回程 · ICMP/2025-12-17 11.21.58.png' | relative_url }}" alt="IPv6 回程 ICMP 1" width="32%" />
  <img src="{{ '/assets/images/dmit-lax-pro/IPv6 回程 · ICMP/2025-12-17 11.21.59.png' | relative_url }}" alt="IPv6 回程 ICMP 2" width="32%" />
  <img src="{{ '/assets/images/dmit-lax-pro/IPv6 回程 · ICMP/2025-12-17 11.22.00.png' | relative_url }}" alt="IPv6 回程 ICMP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv6 回程 · TCP</summary>

<div align="center">
  <img src="{{ '/assets/images/dmit-lax-pro/IPv6 回程 · TCP/2025-12-17 11.22.49.png' | relative_url }}" alt="IPv6 回程 TCP 1" width="32%" />
  <img src="{{ '/assets/images/dmit-lax-pro/IPv6 回程 · TCP/2025-12-17 11.22.51.png' | relative_url }}" alt="IPv6 回程 TCP 2" width="32%" />
  <img src="{{ '/assets/images/dmit-lax-pro/IPv6 回程 · TCP/2025-12-17 11.22.52.png' | relative_url }}" alt="IPv6 回程 TCP 3" width="32%" />
</div>

</details>

### 实时监控
- **实时三网 ICMP**：<https://ping.nxtrace.org/goto/gsxD4eSHR>
- **实时三网 TCP**：<https://ping.nxtrace.org/goto/hTyhe-kHg>
- **官方 Looking Glass**：<https://lg.dmit.sh/?server=lax-pro>
- **北京三网延迟监控截图**：
  <details markdown="1">
  <summary>展开查看</summary>
  
  ![北京三网延迟监控截图]({{ '/assets/images/dmit-lax-pro/北京三网延迟监控截图（近七天）.png' | relative_url }})
  
  </details>

### 北京四网代理单线程测速

<details markdown="1">
<summary>北京移动晚高峰</summary>

![北京移动晚高峰]({{ '/assets/images/dmit-lax-pro/北京四网代理单线程测速/北京移动晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京移动白天</summary>

![北京移动白天]({{ '/assets/images/dmit-lax-pro/北京四网代理单线程测速/北京移动白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通晚高峰</summary>

![北京联通晚高峰]({{ '/assets/images/dmit-lax-pro/北京四网代理单线程测速/北京联通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通白天</summary>

![北京联通白天]({{ '/assets/images/dmit-lax-pro/北京四网代理单线程测速/北京联通白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通晚高峰</summary>

![北京网通晚高峰]({{ '/assets/images/dmit-lax-pro/北京四网代理单线程测速/北京网通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通白天</summary>

![北京网通白天]({{ '/assets/images/dmit-lax-pro/北京四网代理单线程测速/北京网通白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信晚高峰</summary>

![北京电信晚高峰]({{ '/assets/images/dmit-lax-pro/北京四网代理单线程测速/北京电信晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信白天</summary>

![北京电信白天]({{ '/assets/images/dmit-lax-pro/北京四网代理单线程测速/北京电信白天.jpg' | relative_url }})

</details>

### 机器性能跑分

<details markdown="1">
<summary>AN4 跑分</summary>

![综合性能跑分·AN4]({{ '/assets/images/dmit-lax-pro/综合性能跑分·AN4.png' | relative_url }})

</details>

<details markdown="1">
<summary>AN5 跑分</summary>

![综合性能跑分·AN5]({{ '/assets/images/dmit-lax-pro/综合性能跑分·AN5.jpg' | relative_url }})

</details>

### IP 解锁

<details markdown="1">
<summary>流媒体 / 平台解锁记录</summary>

![解锁情况 1]({{ '/assets/images/dmit-lax-pro/解锁情况/2025-12-17 10.29.21.png' | relative_url }})
![解锁情况 2]({{ '/assets/images/dmit-lax-pro/解锁情况/2025-12-17 10.29.23.png' | relative_url }})

</details>
